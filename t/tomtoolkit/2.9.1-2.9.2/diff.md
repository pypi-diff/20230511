# Comparing `tmp/tomtoolkit-2.9.1.tar.gz` & `tmp/tomtoolkit-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomtoolkit-2.9.1.tar", last modified: Wed Sep 22 22:58:39 2021, max compression
+gzip compressed data, was "tomtoolkit-2.9.2.tar", last modified: Fri Oct 15 18:43:40 2021, max compression
```

## Comparing `tomtoolkit-2.9.1.tar` & `tomtoolkit-2.9.2.tar`

### file list

```diff
@@ -1,592 +1,592 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.921051 tomtoolkit-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.821048 tomtoolkit-2.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.821048 tomtoolkit-2.9.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      467 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.825048 tomtoolkit-2.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/workflows/run-canary-tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      599 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-09-22 22:58:39.921051 tomtoolkit-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14563 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/README-dev.md
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.825048 tomtoolkit-2.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.825048 tomtoolkit-2.9.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.825048 tomtoolkit-2.9.1/docs/_static/adding_pages_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    24195 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/adding_pages_doc/base.png
--rw-r--r--   0 runner    (1001) docker     (121)    11898 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/adding_pages_doc/quote.png
--rw-r--r--   0 runner    (1001) docker     (121)    29328 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/adding_pages_doc/targets.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.829048 tomtoolkit-2.9.1/docs/_static/architecture/
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/architecture/erd.csv
--rw-r--r--   0 runner    (1001) docker     (121)   175523 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/architecture/erd.png
--rw-r--r--   0 runner    (1001) docker     (121)   185406 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/architecture/snex2layout.png
--rw-r--r--   0 runner    (1001) docker     (121)   687018 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/architecture/standardlayout.png
--rw-r--r--   0 runner    (1001) docker     (121)   143284 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/common_interface.png
--rw-r--r--   0 runner    (1001) docker     (121)    12923 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/compare-across-forks.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.829048 tomtoolkit-2.9.1/docs/_static/create_broker_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    13431 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/create_broker_doc/example_query.png
--rw-r--r--   0 runner    (1001) docker     (121)    15136 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/create_broker_doc/populated_query_list.png
--rw-r--r--   0 runner    (1001) docker     (121)    19201 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/create_broker_doc/query_result.png
--rw-r--r--   0 runner    (1001) docker     (121)     7496 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/create_broker_doc/success_broker_list.png
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.829048 tomtoolkit-2.9.1/docs/_static/customize_observations/
--rw-r--r--   0 runner    (1001) docker     (121)    70315 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_observations/newform.png
--rw-r--r--   0 runner    (1001) docker     (121)    20414 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_observations/observebutton.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.833048 tomtoolkit-2.9.1/docs/_static/customize_templates_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    83992 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_templates_doc/sciencecat.jpg
--rw-r--r--   0 runner    (1001) docker     (121)  1494498 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_templates_doc/tomhomepagemod.png
--rw-r--r--   0 runner    (1001) docker     (121)   356188 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_templates_doc/tomhomepagenew.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.833048 tomtoolkit-2.9.1/docs/_static/customize_views_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    26510 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_views_doc/after.png
--rw-r--r--   0 runner    (1001) docker     (121)    24936 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/customize_views_doc/before.png
--rw-r--r--   0 runner    (1001) docker     (121)     7983 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/fork.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.833048 tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    28029 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/branchdeployed.png
--rw-r--r--   0 runner    (1001) docker     (121)   108744 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/githubconnected.png
--rw-r--r--   0 runner    (1001) docker     (121)    95423 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/githubintegration.png
--rw-r--r--   0 runner    (1001) docker     (121)   137196 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/herokudeploybranch.png
--rw-r--r--   0 runner    (1001) docker     (121)    17611 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/hs.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.833048 tomtoolkit-2.9.1/docs/_static/jupyterdoc/
--rw-r--r--   0 runner    (1001) docker     (121)    48422 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/jupyterdoc/newnotebook.png
--rw-r--r--   0 runner    (1001) docker     (121)    16157 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/lco.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   111347 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/logo-color.png
--rw-r--r--   0 runner    (1001) docker     (121)     8742 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/_static/observation_module/
--rw-r--r--   0 runner    (1001) docker     (121)    11680 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/observation_module/empty_form.png
--rw-r--r--   0 runner    (1001) docker     (121)    18874 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/observation_module/fields.png
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/observation_module/myfacility.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/_static/permissions_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    12506 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/permissions_doc/addgroup.png
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/permissions_doc/targetgroups.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/_static/plotting_data_doc/
--rw-r--r--   0 runner    (1001) docker     (121)    11589 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/plotting_data_doc/plot.png
--rw-r--r--   0 runner    (1001) docker     (121)     7503 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/pull-request.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/_static/target_fields_doc/
--rw-r--r--   0 runner    (1001) docker     (121)     6928 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift.png
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_display.png
--rw-r--r--   0 runner    (1001) docker     (121)     5836 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_filter.png
--rw-r--r--   0 runner    (1001) docker     (121)     3796 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_tag.png
--rw-r--r--   0 runner    (1001) docker     (121)   115656 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/target_sources.png
--rw-r--r--   0 runner    (1001) docker     (121)    13376 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/_static/zff.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/affiliated.rst
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/management_commands.rst
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/plugins.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.837048 tomtoolkit-2.9.1/docs/api/tom_alerts/
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_alerts/brokers.rst
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_alerts/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_alerts/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_alerts/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_alerts/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.841049 tomtoolkit-2.9.1/docs/api/tom_catalogs/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_catalogs/forms.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_catalogs/harvesters.rst
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_catalogs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_catalogs/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.841049 tomtoolkit-2.9.1/docs/api/tom_common/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_common/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_common/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_common/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_common/template_tags.rst
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_common/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.841049 tomtoolkit-2.9.1/docs/api/tom_dataproducts/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/api_views.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/data_processing.md
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/templatetags.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_dataproducts/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.841049 tomtoolkit-2.9.1/docs/api/tom_observations/
--rw-r--r--   0 runner    (1001) docker     (121)      450 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/facilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/templatetags.rst
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_observations/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.841049 tomtoolkit-2.9.1/docs/api/tom_targets/
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/api_views.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/templatetags.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/api/tom_targets/views.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.845049 tomtoolkit-2.9.1/docs/brokers/
--rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/brokers/create_broker.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16845 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/brokers/create_dash_broker.rst
--rw-r--r--   0 runner    (1001) docker     (121)      878 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/brokers/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.845049 tomtoolkit-2.9.1/docs/code/
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/code/automation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8701 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/code/backgroundtasks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4554 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/code/custom_code.rst
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/code/querying.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.845049 tomtoolkit-2.9.1/docs/common/
--rw-r--r--   0 runner    (1001) docker     (121)     9170 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/common/customsettings.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7953 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/common/latex_generation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/common/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/common/refactoring_roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/common/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.845049 tomtoolkit-2.9.1/docs/customization/
--rw-r--r--   0 runner    (1001) docker     (121)     8538 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/customization/adding_pages.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10612 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/customization/customize_template_tags.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5740 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/customization/customize_templates.rst
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/customization/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.845049 tomtoolkit-2.9.1/docs/deployment/
--rw-r--r--   0 runner    (1001) docker     (121)     4757 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/deployment/amazons3.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6667 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/deployment/deployment_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/deployment/deployment_tips.rst
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/deployment/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.849049 tomtoolkit-2.9.1/docs/introduction/
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/about.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3258 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4325 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/faqs.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)      866 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/support.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16261 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/tomarchitecture.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/introduction/workflow.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.849049 tomtoolkit-2.9.1/docs/managing_data/
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/managing_data/customizing_data_processing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/managing_data/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6445 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/managing_data/plotting_data.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.849049 tomtoolkit-2.9.1/docs/observing/
--rw-r--r--   0 runner    (1001) docker     (121)    12846 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/observing/customize_observations.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/observing/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11653 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/observing/observation_module.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11425 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/observing/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.849049 tomtoolkit-2.9.1/docs/targets/
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/targets/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/docs/targets/target_fields.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      531 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/manage.py
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/releasenotes.md
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-22 22:58:39.921051 tomtoolkit-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.849049 tomtoolkit-2.9.1/tom_alerts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     8938 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/brokers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11861 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/alerce.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/antares.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/fink.py
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/gaia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/lasair.py
--rw-r--r--   0 runner    (1001) docker     (121)    10143 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/mars.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/scimma.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/scout.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/brokers/tns.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/management/commands/runbrokerquery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      560 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/migrations/0002_auto_20190626_2135.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/migrations/0003_auto_20190701_2226.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/migrations/0004_auto_20210204_2300.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.813048 tomtoolkit-2.9.1/tom_alerts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/brokerquery_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/brokerquery_list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/partials/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/partials/submit_upstream_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/query_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/query_result.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/templatetags/alerts_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.853049 tomtoolkit-2.9.1/tom_alerts/tests/brokers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/brokers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22562 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_alerce.py
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_gaia.py
--rw-r--r--   0 runner    (1001) docker     (121)     3020 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_lasair.py
--rw-r--r--   0 runner    (1001) docker     (121)     7289 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_mars.py
--rw-r--r--   0 runner    (1001) docker     (121)    14340 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    12104 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_alerts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7790 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_base/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_base/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_catalogs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_catalogs/harvesters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/mpc.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/ned.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/simbad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/harvesters/tns.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_catalogs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_catalogs/templates/tom_catalogs/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/templates/tom_catalogs/query_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_catalogs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.857049 tomtoolkit-2.9.1/tom_catalogs/tests/harvesters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/tests/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/tests/harvesters/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/tests/harvesters/test_simbad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_catalogs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/api_router.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/api_views.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/hints.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      309 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_common/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_common/static/tom_common/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/static/tom_common/css/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/static/tom_common/img/
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-16.ico
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-32.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    55240 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-color-cropped.png
--rw-r--r--   0 runner    (1001) docker     (121)   111347 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-color.png
--rw-r--r--   0 runner    (1001) docker     (121)    20653 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-text.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/group_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/group_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/templates/auth/partials/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/partials/group_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/partials/user_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      306 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/user_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/auth/user_list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.861049 tomtoolkit-2.9.1/tom_common/templates/comments/
--rw-r--r--   0 runner    (1001) docker     (121)      511 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/comments/form.html
--rw-r--r--   0 runner    (1001) docker     (121)      920 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/comments/list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.865049 tomtoolkit-2.9.1/tom_common/templates/django_comments/
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/django_comments/comment_confirm_delete.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_common/templates/django_filters/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.865049 tomtoolkit-2.9.1/tom_common/templates/django_filters/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/django_filters/widgets/multiwidget.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.865049 tomtoolkit-2.9.1/tom_common/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/registration/login.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.865049 tomtoolkit-2.9.1/tom_common/templates/tom_common/
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/change_user_password.html
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/create_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/navbar_content.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.865049 tomtoolkit-2.9.1/tom_common/templates/tom_common/partials/
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templates/tom_common/partials/navbar_login.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.873050 tomtoolkit-2.9.1/tom_common/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templatetags/tom_common_extras.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/templatetags/user_extras.py
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     6693 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_common/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.873050 tomtoolkit-2.9.1/tom_dataproducts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      172 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/api_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.873050 tomtoolkit-2.9.1/tom_dataproducts/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.877050 tomtoolkit-2.9.1/tom_dataproducts/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/management/commands/downloaddata.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/management/commands/updatereduceddata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.877050 tomtoolkit-2.9.1/tom_dataproducts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0004_auto_20190626_0904.py
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0005_auto_20190704_1010.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0006_auto_20190912_2013.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0007_manual_20191016_rename_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0008_auto_20191205_1952.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0009_auto_20210204_2221.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/0010_manual_20210305_fix_spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12299 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.877050 tomtoolkit-2.9.1/tom_dataproducts/processors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/processors/data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/processors/photometry_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5786 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/processors/spectroscopy_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_dataproducts/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.877050 tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.881050 tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/img/
--rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/img/placeholder.png
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/photometry_sample.csv
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/spectrum_sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_dataproducts/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.881050 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/add_product_to_group.html
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproduct_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproduct_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)      316 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      736 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.885050 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/dataproduct_list_for_target.html
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/js9_button.html
--rw-r--r--   0 runner    (1001) docker     (121)      868 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/js9_scripts.html
--rw-r--r--   0 runner    (1001) docker     (121)      322 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/photometry_for_target.html
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/recent_photometry.html
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/saved_dataproduct_list_for_observation.html
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/spectroscopy_for_target.html
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/unsaved_dataproduct_list_for_observation.html
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/update_broker_data_button.html
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/upload_dataproduct.html
--rw-r--r--   0 runner    (1001) docker     (121)      420 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/upload_reduced_data.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.885050 tomtoolkit-2.9.1/tom_dataproducts/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10002 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/templatetags/dataproduct_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.885050 tomtoolkit-2.9.1/tom_dataproducts/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.885050 tomtoolkit-2.9.1/tom_dataproducts/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/test_data/test_lightcurve.csv
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/test_data/test_spectrum.csv
--rw-r--r--   0 runner    (1001) docker     (121)    89280 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/test_data/test_spectrum.fits
--rw-r--r--   0 runner    (1001) docker     (121)    23635 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    15116 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_dataproducts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.889050 tomtoolkit-2.9.1/tom_observations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     9788 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/api_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/cadence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.889050 tomtoolkit-2.9.1/tom_observations/cadences/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/cadences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5794 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/cadences/resume_cadence_after_failure.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/cadences/retry_failed_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.893050 tomtoolkit-2.9.1/tom_observations/facilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21607 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/gemini.py
--rw-r--r--   0 runner    (1001) docker     (121)    51072 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/lco.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/lt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/manual.py
--rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facilities/soar.py
--rw-r--r--   0 runner    (1001) docker     (121)    16760 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/facility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.893050 tomtoolkit-2.9.1/tom_observations/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.893050 tomtoolkit-2.9.1/tom_observations/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/management/commands/runcadencestrategies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/management/commands/updatestatus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.897050 tomtoolkit-2.9.1/tom_observations/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0002_auto_20190306_2343.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0003_auto_20190503_2318.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0004_observationgroup.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0005_auto_20191210_0007.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0006_observationgroup_cadence_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0007_observationstrategy.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0008_observationgroup_cadence_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0009_observationrecord_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0010_manual_create_dynamic_cadence.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0011_auto_20200917_0306.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/0012_auto_20210205_1819.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/observation_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     2632 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_observations/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_observations/static/tom_observations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.897050 tomtoolkit-2.9.1/tom_observations/static/tom_observations/css/
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/static/tom_observations/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.817048 tomtoolkit-2.9.1/tom_observations/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.897050 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/existing_observation_confirm.html
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/facility_status.html
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observation_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     3288 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observation_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationgroup_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationgroup_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationgroup_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationrecord_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationtemplate_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationtemplate_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationtemplate_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationupdate_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.901050 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/existing_observation_form.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/facility_map.html
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/facility_observation_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      919 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/facility_status.html
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observation_distribution.html
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observation_list.html
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observation_plan.html
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observation_type_tabs.html
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observationtemplate_from_record.html
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observationtemplate_run.html
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observing_buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/update_observation_id_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/update_status_button.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.901050 tomtoolkit-2.9.1/tom_observations/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12619 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/templatetags/observation_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.901050 tomtoolkit-2.9.1/tom_observations/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.905051 tomtoolkit-2.9.1/tom_observations/tests/facilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/facilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/facilities/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (121)    45989 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/facilities/test_lco.py
--rw-r--r--   0 runner    (1001) docker     (121)    11500 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/facilities/test_soar.py
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)    15234 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/test_cadence.py
--rw-r--r--   0 runner    (1001) docker     (121)    21135 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    25654 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_observations/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.905051 tomtoolkit-2.9.1/tom_setup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.905051 tomtoolkit-2.9.1/tom_setup/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.905051 tomtoolkit-2.9.1/tom_setup/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7899 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/management/commands/tom_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.821048 tomtoolkit-2.9.1/tom_setup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.905051 tomtoolkit-2.9.1/tom_setup/templates/tom_setup/
--rw-r--r--   0 runner    (1001) docker     (121)     9266 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/templates/tom_setup/settings.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)      729 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_setup/templates/tom_setup/urls.tmpl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.909051 tomtoolkit-2.9.1/tom_targets/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/api_views.py
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     4868 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7258 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)    12585 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.909051 tomtoolkit-2.9.1/tom_targets/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.909051 tomtoolkit-2.9.1/tom_targets/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/management/commands/setdefaultextras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.913051 tomtoolkit-2.9.1/tom_targets/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0002_auto_20190115_2102.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0002_auto_20190117_2248.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0003_merge_20190123_1754.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0004_auto_20190123_2010.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0005_auto_20190214_1722.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0006_auto_20190403_1659.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0007_auto_20190423_1455.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0007_auto_20190503_2318.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0007_auto_20190515_0047.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0008_merge_20190515_0914.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0008_merge_20190520_1645.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0009_auto_20190605_1656.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0010_auto_20190715_1657.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0010_merge_20190612_1227.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0011_merge_20190731_1821.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0012_target_perihdist.py
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0013_manual_20190916_multiple_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0014_auto_20190923_1827.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0015_auto_20190923_2233.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0016_auto_20191211_1707.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0017_auto_20200130_2350.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0018_auto_20200714_1832.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/0019_auto_20210811_0018.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18156 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.821048 tomtoolkit-2.9.1/tom_targets/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.913051 tomtoolkit-2.9.1/tom_targets/static/tom_targets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.913051 tomtoolkit-2.9.1/tom_targets/static/tom_targets/css/
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/static/tom_targets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/static/tom_targets/target_import.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.821048 tomtoolkit-2.9.1/tom_targets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.913051 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.917051 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/
--rw-r--r--   0 runner    (1001) docker     (121)     7864 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/aladin.html
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/moon_distance.html
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/recent_targets.html
--rw-r--r--   0 runner    (1001) docker     (121)      542 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/recently_updated_targets.html
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_data.html
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_distribution.html
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_feature.html
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_groups.html
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_plan.html
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_table.html
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_unknown_statuses.html
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/targetlist_select.html
--rw-r--r--   0 runner    (1001) docker     (121)      373 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     4615 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_grouping.html
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_import.html
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/targetlist_confirm_delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templates/tom_targets/targetlist_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.917051 tomtoolkit-2.9.1/tom_targets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9645 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/templatetags/targets_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.917051 tomtoolkit-2.9.1/tom_targets/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (121)    12114 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    42203 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4120 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    21459 2021-09-22 22:58:28.000000 tomtoolkit-2.9.1/tom_targets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 22:58:39.921051 tomtoolkit-2.9.1/tomtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-09-22 22:58:39.000000 tomtoolkit-2.9.1/tomtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19734 2021-09-22 22:58:39.000000 tomtoolkit-2.9.1/tomtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-22 22:58:39.000000 tomtoolkit-2.9.1/tomtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-09-22 22:58:39.000000 tomtoolkit-2.9.1/tomtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-09-22 22:58:39.000000 tomtoolkit-2.9.1/tomtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.741967 tomtoolkit-2.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.741967 tomtoolkit-2.9.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.741967 tomtoolkit-2.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/workflows/run-canary-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1689 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14563 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/README-dev.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3660 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.741967 tomtoolkit-2.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.745967 tomtoolkit-2.9.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.745967 tomtoolkit-2.9.2/docs/_static/adding_pages_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    24195 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/adding_pages_doc/base.png
+-rw-r--r--   0 runner    (1001) docker     (121)    11898 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/adding_pages_doc/quote.png
+-rw-r--r--   0 runner    (1001) docker     (121)    29328 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/adding_pages_doc/targets.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.745967 tomtoolkit-2.9.2/docs/_static/architecture/
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/architecture/erd.csv
+-rw-r--r--   0 runner    (1001) docker     (121)   175523 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/architecture/erd.png
+-rw-r--r--   0 runner    (1001) docker     (121)   185406 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/architecture/snex2layout.png
+-rw-r--r--   0 runner    (1001) docker     (121)   687018 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/architecture/standardlayout.png
+-rw-r--r--   0 runner    (1001) docker     (121)   143284 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/common_interface.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12923 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/compare-across-forks.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.745967 tomtoolkit-2.9.2/docs/_static/create_broker_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    13431 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/create_broker_doc/example_query.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15136 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/create_broker_doc/populated_query_list.png
+-rw-r--r--   0 runner    (1001) docker     (121)    19201 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/create_broker_doc/query_result.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7496 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/create_broker_doc/success_broker_list.png
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.745967 tomtoolkit-2.9.2/docs/_static/customize_observations/
+-rw-r--r--   0 runner    (1001) docker     (121)    70315 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_observations/newform.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20414 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_observations/observebutton.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.749967 tomtoolkit-2.9.2/docs/_static/customize_templates_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    83992 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_templates_doc/sciencecat.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)  1494498 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_templates_doc/tomhomepagemod.png
+-rw-r--r--   0 runner    (1001) docker     (121)   356188 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_templates_doc/tomhomepagenew.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.749967 tomtoolkit-2.9.2/docs/_static/customize_views_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    26510 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_views_doc/after.png
+-rw-r--r--   0 runner    (1001) docker     (121)    24936 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/customize_views_doc/before.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7983 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/fork.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.749967 tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    28029 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/branchdeployed.png
+-rw-r--r--   0 runner    (1001) docker     (121)   108744 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/githubconnected.png
+-rw-r--r--   0 runner    (1001) docker     (121)    95423 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/githubintegration.png
+-rw-r--r--   0 runner    (1001) docker     (121)   137196 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/herokudeploybranch.png
+-rw-r--r--   0 runner    (1001) docker     (121)    17611 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/hs.jpg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.749967 tomtoolkit-2.9.2/docs/_static/jupyterdoc/
+-rw-r--r--   0 runner    (1001) docker     (121)    48422 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/jupyterdoc/newnotebook.png
+-rw-r--r--   0 runner    (1001) docker     (121)    16157 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/lco.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   111347 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/logo-color.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8742 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.749967 tomtoolkit-2.9.2/docs/_static/observation_module/
+-rw-r--r--   0 runner    (1001) docker     (121)    11680 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/observation_module/empty_form.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18874 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/observation_module/fields.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4265 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/observation_module/myfacility.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/_static/permissions_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    12506 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/permissions_doc/addgroup.png
+-rw-r--r--   0 runner    (1001) docker     (121)     6367 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/permissions_doc/targetgroups.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/_static/plotting_data_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)    11589 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/plotting_data_doc/plot.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7503 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/pull-request.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/_static/target_fields_doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     6928 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3973 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_display.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5836 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_filter.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3796 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_tag.png
+-rw-r--r--   0 runner    (1001) docker     (121)   115656 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/target_sources.png
+-rw-r--r--   0 runner    (1001) docker     (121)    13376 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/_static/zff.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     1793 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/affiliated.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/management_commands.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/plugins.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/api/tom_alerts/
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_alerts/brokers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_alerts/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_alerts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_alerts/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_alerts/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/api/tom_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_catalogs/forms.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_catalogs/harvesters.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_catalogs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_catalogs/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/api/tom_common/
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_common/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_common/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_common/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_common/template_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_common/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.753967 tomtoolkit-2.9.2/docs/api/tom_dataproducts/
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/api_views.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/data_processing.md
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/templatetags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_dataproducts/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/api/tom_observations/
+-rw-r--r--   0 runner    (1001) docker     (121)      450 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/facilities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/templatetags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_observations/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/api/tom_targets/
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/api_views.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/groups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/templatetags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/api/tom_targets/views.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/brokers/
+-rw-r--r--   0 runner    (1001) docker     (121)     9124 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/brokers/create_broker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16845 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/brokers/create_dash_broker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      878 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/brokers/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (121)     8310 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/code/automation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8701 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/code/backgroundtasks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4554 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/code/custom_code.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/code/querying.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     9170 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/common/customsettings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7953 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/common/latex_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/common/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/common/refactoring_roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6228 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/common/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/customization/
+-rw-r--r--   0 runner    (1001) docker     (121)     8538 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/customization/adding_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10612 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/customization/customize_template_tags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5740 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/customization/customize_templates.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/customization/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.757967 tomtoolkit-2.9.2/docs/deployment/
+-rw-r--r--   0 runner    (1001) docker     (121)     4757 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/deployment/amazons3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6667 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/deployment/deployment_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2143 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/deployment/deployment_tips.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/deployment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4459 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/docs/introduction/
+-rw-r--r--   0 runner    (1001) docker     (121)     3015 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/about.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3258 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4325 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/faqs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2919 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2285 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/support.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16261 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/tomarchitecture.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3860 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/introduction/workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/docs/managing_data/
+-rw-r--r--   0 runner    (1001) docker     (121)     7085 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/managing_data/customizing_data_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/managing_data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6445 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/managing_data/plotting_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/docs/observing/
+-rw-r--r--   0 runner    (1001) docker     (121)    12846 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/observing/customize_observations.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/observing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11653 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/observing/observation_module.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11425 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/observing/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/docs/targets/
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/targets/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4658 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/docs/targets/target_fields.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)      531 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/manage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8910 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/releasenotes.md
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/tom_alerts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8938 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/tom_alerts/brokers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11861 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/alerce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/antares.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/fink.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5749 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3823 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/lasair.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10143 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/mars.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/scimma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2260 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/scout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6374 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/brokers/tns.py
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/tom_alerts/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/tom_alerts/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/management/commands/runbrokerquery.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.761967 tomtoolkit-2.9.2/tom_alerts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/migrations/0002_auto_20190626_2135.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/migrations/0003_auto_20190701_2226.py
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/migrations/0004_auto_20210204_2300.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.733967 tomtoolkit-2.9.2/tom_alerts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/brokerquery_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/brokerquery_list.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/partials/submit_upstream_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/query_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/query_result.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_alerts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/templatetags/alerts_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_alerts/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_alerts/tests/brokers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/brokers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22562 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_alerce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8235 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3020 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_lasair.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7289 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_mars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14340 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12104 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_alerts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_base/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7790 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_base/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_catalogs/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/mpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/ned.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/simbad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/harvesters/tns.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.733967 tomtoolkit-2.9.2/tom_catalogs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.765967 tomtoolkit-2.9.2/tom_catalogs/templates/tom_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/templates/tom_catalogs/query_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.769967 tomtoolkit-2.9.2/tom_catalogs/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.769967 tomtoolkit-2.9.2/tom_catalogs/tests/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/tests/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/tests/harvesters/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/tests/harvesters/test_simbad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1857 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_catalogs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.769967 tomtoolkit-2.9.2/tom_common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/api_router.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/hints.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.733967 tomtoolkit-2.9.2/tom_common/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.733967 tomtoolkit-2.9.2/tom_common/static/tom_common/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.769967 tomtoolkit-2.9.2/tom_common/static/tom_common/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.769967 tomtoolkit-2.9.2/tom_common/static/tom_common/img/
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-16.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)      862 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-32.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     7657 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)    55240 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-color-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (121)   111347 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-color.png
+-rw-r--r--   0 runner    (1001) docker     (121)    20653 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-text.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/group_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/group_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/auth/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/partials/group_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/partials/user_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/user_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/auth/user_list.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/comments/
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/comments/form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/comments/list.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/django_comments/
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/django_comments/comment_confirm_delete.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_common/templates/django_filters/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/django_filters/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/django_filters/widgets/multiwidget.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/registration/login.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/tom_common/
+-rw-r--r--   0 runner    (1001) docker     (121)     2552 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/change_user_password.html
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/create_user.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2416 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/navbar_content.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templates/tom_common/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)      605 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templates/tom_common/partials/navbar_login.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_common/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2671 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templatetags/tom_common_extras.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/templatetags/user_extras.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3277 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6693 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_common/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_dataproducts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3483 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1615 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.773968 tomtoolkit-2.9.2/tom_dataproducts/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/management/commands/downloaddata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/management/commands/updatereduceddata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     3529 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0004_auto_20190626_0904.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0005_auto_20190704_1010.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0006_auto_20190912_2013.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0007_manual_20191016_rename_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0008_auto_20191205_1952.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0009_auto_20210204_2221.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/0010_manual_20210305_fix_spectroscopy.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12299 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/processors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/processors/data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/processors/photometry_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5786 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/processors/spectroscopy_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4341 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_dataproducts/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/img/
+-rw-r--r--   0 runner    (1001) docker     (121)     5027 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/img/placeholder.png
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/photometry_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/spectrum_sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_dataproducts/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/add_product_to_group.html
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproduct_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3428 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproduct_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      736 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_list.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.777968 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/dataproduct_list_for_target.html
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/js9_button.html
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/js9_scripts.html
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/photometry_for_target.html
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/recent_photometry.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/saved_dataproduct_list_for_observation.html
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/spectroscopy_for_target.html
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/unsaved_dataproduct_list_for_observation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/update_broker_data_button.html
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/upload_dataproduct.html
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/upload_reduced_data.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_dataproducts/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10002 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/templatetags/dataproduct_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_dataproducts/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_dataproducts/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/test_data/test_lightcurve.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/test_data/test_spectrum.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    89280 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/test_data/test_spectrum.fits
+-rw-r--r--   0 runner    (1001) docker     (121)    23635 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15116 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_dataproducts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_observations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9788 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/cadence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_observations/cadences/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/cadences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5794 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/cadences/resume_cadence_after_failure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/cadences/retry_failed_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_observations/facilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21607 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/gemini.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51072 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/lco.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/lt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/manual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facilities/soar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16760 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/facility.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2480 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_observations/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.781968 tomtoolkit-2.9.2/tom_observations/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/management/commands/runcadencestrategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/management/commands/updatestatus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.785968 tomtoolkit-2.9.2/tom_observations/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      571 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0002_auto_20190306_2343.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0003_auto_20190503_2318.py
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0004_observationgroup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0005_auto_20191210_0007.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0006_observationgroup_cadence_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0007_observationstrategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0008_observationgroup_cadence_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0009_observationrecord_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2943 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0010_manual_create_dynamic_cadence.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0011_auto_20200917_0306.py
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/0012_auto_20210205_1819.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2067 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/observation_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2632 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_observations/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_observations/static/tom_observations/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.785968 tomtoolkit-2.9.2/tom_observations/static/tom_observations/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/static/tom_observations/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_observations/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.785968 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/existing_observation_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/facility_status.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observation_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3288 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observation_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationgroup_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationgroup_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationgroup_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3091 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationrecord_detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationtemplate_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationtemplate_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationtemplate_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationupdate_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.785968 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/existing_observation_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/facility_map.html
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/facility_observation_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/facility_status.html
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observation_distribution.html
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observation_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observation_plan.html
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observation_type_tabs.html
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observationtemplate_from_record.html
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observationtemplate_run.html
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observing_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/update_observation_id_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/update_status_button.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_observations/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12619 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/templatetags/observation_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_observations/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_observations/tests/facilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/facilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/facilities/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45989 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/facilities/test_lco.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11500 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/facilities/test_soar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2846 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15234 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7247 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/test_cadence.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21135 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4929 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5038 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25654 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1980 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_observations/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_setup/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_setup/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_setup/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7899 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/management/commands/tom_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_setup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_setup/templates/tom_setup/
+-rw-r--r--   0 runner    (1001) docker     (121)     9266 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/templates/tom_setup/settings.tmpl
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_setup/templates/tom_setup/urls.tmpl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_targets/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4164 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5105 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7258 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12585 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_targets/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.789968 tomtoolkit-2.9.2/tom_targets/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/management/commands/setdefaultextras.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.793968 tomtoolkit-2.9.2/tom_targets/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     5412 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0002_auto_20190115_2102.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0002_auto_20190117_2248.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0003_merge_20190123_1754.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0004_auto_20190123_2010.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0005_auto_20190214_1722.py
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0006_auto_20190403_1659.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0007_auto_20190423_1455.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0007_auto_20190503_2318.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0007_auto_20190515_0047.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0008_merge_20190515_0914.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0008_merge_20190520_1645.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0009_auto_20190605_1656.py
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0010_auto_20190715_1657.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0010_merge_20190612_1227.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0011_merge_20190731_1821.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0012_target_perihdist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0013_manual_20190916_multiple_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0014_auto_20190923_1827.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0015_auto_20190923_2233.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0016_auto_20191211_1707.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0017_auto_20200130_2350.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0018_auto_20200714_1832.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/0019_auto_20210811_0018.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18156 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7829 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_targets/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.793968 tomtoolkit-2.9.2/tom_targets/static/tom_targets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.793968 tomtoolkit-2.9.2/tom_targets/static/tom_targets/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/static/tom_targets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/static/tom_targets/target_import.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.737967 tomtoolkit-2.9.2/tom_targets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.793968 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/
+-rw-r--r--   0 runner    (1001) docker     (121)     7864 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/aladin.html
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/moon_distance.html
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/recent_targets.html
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/recently_updated_targets.html
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_data.html
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_distribution.html
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_feature.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_groups.html
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_plan.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1407 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_table.html
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_unknown_statuses.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/targetlist_select.html
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4615 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_grouping.html
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_import.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3207 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      349 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/targetlist_confirm_delete.html
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templates/tom_targets/targetlist_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/tom_targets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9740 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/templatetags/targets_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/tom_targets/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12114 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42203 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4120 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21459 2021-10-15 18:43:26.000000 tomtoolkit-2.9.2/tom_targets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:43:40.797968 tomtoolkit-2.9.2/tomtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2021-10-15 18:43:40.000000 tomtoolkit-2.9.2/tomtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    19734 2021-10-15 18:43:40.000000 tomtoolkit-2.9.2/tomtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 18:43:40.000000 tomtoolkit-2.9.2/tomtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-10-15 18:43:40.000000 tomtoolkit-2.9.2/tomtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-10-15 18:43:40.000000 tomtoolkit-2.9.2/tomtoolkit.egg-info/top_level.txt
```

### Comparing `tomtoolkit-2.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `tomtoolkit-2.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/.github/workflows/github-release.yml` & `tomtoolkit-2.9.2/.github/workflows/github-release.yml`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/.github/workflows/pypi-release.yml` & `tomtoolkit-2.9.2/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/.github/workflows/run-tests.yml` & `tomtoolkit-2.9.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/.gitignore` & `tomtoolkit-2.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/.readthedocs.yml` & `tomtoolkit-2.9.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/LICENSE` & `tomtoolkit-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/MANIFEST.in` & `tomtoolkit-2.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/PKG-INFO` & `tomtoolkit-2.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomtoolkit
-Version: 2.9.1
+Version: 2.9.2
 Summary: The TOM Toolkit and base modules
 Home-page: https://tomtoolkit.github.io
 Author: TOM Toolkit Project
 Author-email: dcollom@lco.global
 License: UNKNOWN
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science,fits,observatory
 Platform: UNKNOWN
```

### Comparing `tomtoolkit-2.9.1/README-dev.md` & `tomtoolkit-2.9.2/README-dev.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/README.md` & `tomtoolkit-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/Makefile` & `tomtoolkit-2.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/adding_pages_doc/base.png` & `tomtoolkit-2.9.2/docs/_static/adding_pages_doc/base.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/adding_pages_doc/quote.png` & `tomtoolkit-2.9.2/docs/_static/adding_pages_doc/quote.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/adding_pages_doc/targets.png` & `tomtoolkit-2.9.2/docs/_static/adding_pages_doc/targets.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/architecture/erd.csv` & `tomtoolkit-2.9.2/docs/_static/architecture/erd.csv`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/architecture/erd.png` & `tomtoolkit-2.9.2/docs/_static/architecture/erd.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/architecture/snex2layout.png` & `tomtoolkit-2.9.2/docs/_static/architecture/snex2layout.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/architecture/standardlayout.png` & `tomtoolkit-2.9.2/docs/_static/architecture/standardlayout.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/common_interface.png` & `tomtoolkit-2.9.2/docs/_static/common_interface.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/compare-across-forks.png` & `tomtoolkit-2.9.2/docs/_static/compare-across-forks.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/create_broker_doc/example_query.png` & `tomtoolkit-2.9.2/docs/_static/create_broker_doc/example_query.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/create_broker_doc/populated_query_list.png` & `tomtoolkit-2.9.2/docs/_static/create_broker_doc/populated_query_list.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/create_broker_doc/query_result.png` & `tomtoolkit-2.9.2/docs/_static/create_broker_doc/query_result.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/create_broker_doc/success_broker_list.png` & `tomtoolkit-2.9.2/docs/_static/create_broker_doc/success_broker_list.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_observations/newform.png` & `tomtoolkit-2.9.2/docs/_static/customize_observations/newform.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_observations/observebutton.png` & `tomtoolkit-2.9.2/docs/_static/customize_observations/observebutton.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_templates_doc/sciencecat.jpg` & `tomtoolkit-2.9.2/docs/_static/customize_templates_doc/sciencecat.jpg`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_templates_doc/tomhomepagemod.png` & `tomtoolkit-2.9.2/docs/_static/customize_templates_doc/tomhomepagemod.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_templates_doc/tomhomepagenew.png` & `tomtoolkit-2.9.2/docs/_static/customize_templates_doc/tomhomepagenew.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_views_doc/after.png` & `tomtoolkit-2.9.2/docs/_static/customize_views_doc/after.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/customize_views_doc/before.png` & `tomtoolkit-2.9.2/docs/_static/customize_views_doc/before.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/fork.png` & `tomtoolkit-2.9.2/docs/_static/fork.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/branchdeployed.png` & `tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/branchdeployed.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/githubconnected.png` & `tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/githubconnected.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/githubintegration.png` & `tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/githubintegration.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/heroku_deploy_doc/herokudeploybranch.png` & `tomtoolkit-2.9.2/docs/_static/heroku_deploy_doc/herokudeploybranch.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/hs.jpg` & `tomtoolkit-2.9.2/docs/_static/hs.jpg`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/jupyterdoc/newnotebook.png` & `tomtoolkit-2.9.2/docs/_static/jupyterdoc/newnotebook.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/lco.jpg` & `tomtoolkit-2.9.2/docs/_static/lco.jpg`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/logo-color.png` & `tomtoolkit-2.9.2/docs/_static/logo-color.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/logo.png` & `tomtoolkit-2.9.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/observation_module/empty_form.png` & `tomtoolkit-2.9.2/docs/_static/observation_module/empty_form.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/observation_module/fields.png` & `tomtoolkit-2.9.2/docs/_static/observation_module/fields.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/observation_module/myfacility.png` & `tomtoolkit-2.9.2/docs/_static/observation_module/myfacility.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/permissions_doc/addgroup.png` & `tomtoolkit-2.9.2/docs/_static/permissions_doc/addgroup.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/permissions_doc/targetgroups.png` & `tomtoolkit-2.9.2/docs/_static/permissions_doc/targetgroups.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/plotting_data_doc/plot.png` & `tomtoolkit-2.9.2/docs/_static/plotting_data_doc/plot.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/pull-request.png` & `tomtoolkit-2.9.2/docs/_static/pull-request.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift.png` & `tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_display.png` & `tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_display.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_filter.png` & `tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_filter.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/target_fields_doc/redshift_tag.png` & `tomtoolkit-2.9.2/docs/_static/target_fields_doc/redshift_tag.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/target_sources.png` & `tomtoolkit-2.9.2/docs/_static/target_sources.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/_static/zff.png` & `tomtoolkit-2.9.2/docs/_static/zff.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/affiliated.rst` & `tomtoolkit-2.9.2/docs/api/affiliated.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/management_commands.rst` & `tomtoolkit-2.9.2/docs/api/management_commands.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/plugins.md` & `tomtoolkit-2.9.2/docs/api/plugins.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/tom_alerts/brokers.rst` & `tomtoolkit-2.9.2/docs/api/tom_alerts/brokers.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/tom_catalogs/harvesters.rst` & `tomtoolkit-2.9.2/docs/api/tom_catalogs/harvesters.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/tom_dataproducts/api_views.rst` & `tomtoolkit-2.9.2/docs/api/tom_dataproducts/api_views.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/tom_dataproducts/data_processing.md` & `tomtoolkit-2.9.2/docs/api/tom_dataproducts/data_processing.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/api/tom_targets/api_views.rst` & `tomtoolkit-2.9.2/docs/api/tom_targets/api_views.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/brokers/create_broker.rst` & `tomtoolkit-2.9.2/docs/brokers/create_broker.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/brokers/create_dash_broker.rst` & `tomtoolkit-2.9.2/docs/brokers/create_dash_broker.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/brokers/index.rst` & `tomtoolkit-2.9.2/docs/brokers/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/code/automation.rst` & `tomtoolkit-2.9.2/docs/code/automation.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/code/backgroundtasks.rst` & `tomtoolkit-2.9.2/docs/code/backgroundtasks.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/code/custom_code.rst` & `tomtoolkit-2.9.2/docs/code/custom_code.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/code/index.rst` & `tomtoolkit-2.9.2/docs/code/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/code/querying.rst` & `tomtoolkit-2.9.2/docs/code/querying.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/common/customsettings.rst` & `tomtoolkit-2.9.2/docs/common/customsettings.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/common/latex_generation.rst` & `tomtoolkit-2.9.2/docs/common/latex_generation.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/common/permissions.rst` & `tomtoolkit-2.9.2/docs/common/permissions.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/common/refactoring_roadmap.rst` & `tomtoolkit-2.9.2/docs/common/refactoring_roadmap.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/common/scripts.rst` & `tomtoolkit-2.9.2/docs/common/scripts.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/conf.py` & `tomtoolkit-2.9.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'TOM Toolkit'
-copyright = '2020, David Collom and Lindy Lindstrom'
+copyright = '2021, David Collom and Lindy Lindstrom'
 author = 'David Collom, Lindy Lindstrom, Austin Riba'
 
 # The full version, including alpha/beta/rc tags
 # This has to mirror the setup.py version for PDF generation
 release = '1.1.0'
 
 # -- Django Configuration -------------------------------------------------
```

### Comparing `tomtoolkit-2.9.1/docs/customization/adding_pages.rst` & `tomtoolkit-2.9.2/docs/customization/adding_pages.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/customization/customize_template_tags.rst` & `tomtoolkit-2.9.2/docs/customization/customize_template_tags.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/customization/customize_templates.rst` & `tomtoolkit-2.9.2/docs/customization/customize_templates.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/customization/index.rst` & `tomtoolkit-2.9.2/docs/customization/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/deployment/amazons3.rst` & `tomtoolkit-2.9.2/docs/deployment/amazons3.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/deployment/deployment_heroku.rst` & `tomtoolkit-2.9.2/docs/deployment/deployment_heroku.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/deployment/deployment_tips.rst` & `tomtoolkit-2.9.2/docs/deployment/deployment_tips.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/deployment/index.rst` & `tomtoolkit-2.9.2/docs/deployment/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/index.rst` & `tomtoolkit-2.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/about.rst` & `tomtoolkit-2.9.2/docs/introduction/about.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/contributing.rst` & `tomtoolkit-2.9.2/docs/introduction/contributing.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/faqs.rst` & `tomtoolkit-2.9.2/docs/introduction/faqs.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/getting_started.rst` & `tomtoolkit-2.9.2/docs/introduction/getting_started.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/index.rst` & `tomtoolkit-2.9.2/docs/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/resources.rst` & `tomtoolkit-2.9.2/docs/introduction/resources.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/support.rst` & `tomtoolkit-2.9.2/docs/introduction/support.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/tomarchitecture.rst` & `tomtoolkit-2.9.2/docs/introduction/tomarchitecture.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/troubleshooting.rst` & `tomtoolkit-2.9.2/docs/introduction/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/introduction/workflow.rst` & `tomtoolkit-2.9.2/docs/introduction/workflow.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/make.bat` & `tomtoolkit-2.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/managing_data/customizing_data_processing.rst` & `tomtoolkit-2.9.2/docs/managing_data/customizing_data_processing.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/managing_data/plotting_data.rst` & `tomtoolkit-2.9.2/docs/managing_data/plotting_data.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/observing/customize_observations.rst` & `tomtoolkit-2.9.2/docs/observing/customize_observations.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/observing/index.rst` & `tomtoolkit-2.9.2/docs/observing/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/observing/observation_module.rst` & `tomtoolkit-2.9.2/docs/observing/observation_module.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/observing/strategies.rst` & `tomtoolkit-2.9.2/docs/observing/strategies.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/targets/index.rst` & `tomtoolkit-2.9.2/docs/targets/index.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/docs/targets/target_fields.rst` & `tomtoolkit-2.9.2/docs/targets/target_fields.rst`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/manage.py` & `tomtoolkit-2.9.2/manage.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/releasenotes.md` & `tomtoolkit-2.9.2/releasenotes.md`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/setup.py` & `tomtoolkit-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/alerts.py` & `tomtoolkit-2.9.2/tom_alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/alerce.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/alerce.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/antares.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/antares.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/fink.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/fink.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/gaia.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/gaia.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/lasair.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/lasair.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/mars.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/mars.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/scimma.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/scimma.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/scout.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/scout.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/brokers/tns.py` & `tomtoolkit-2.9.2/tom_alerts/brokers/tns.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/management/commands/runbrokerquery.py` & `tomtoolkit-2.9.2/tom_alerts/management/commands/runbrokerquery.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/migrations/0001_initial.py` & `tomtoolkit-2.9.2/tom_alerts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/migrations/0002_auto_20190626_2135.py` & `tomtoolkit-2.9.2/tom_alerts/migrations/0002_auto_20190626_2135.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/models.py` & `tomtoolkit-2.9.2/tom_alerts/models.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/brokerquery_list.html` & `tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/brokerquery_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/templates/tom_alerts/query_result.html` & `tomtoolkit-2.9.2/tom_alerts/templates/tom_alerts/query_result.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/templatetags/alerts_extras.py` & `tomtoolkit-2.9.2/tom_alerts/templatetags/alerts_extras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_alerce.py` & `tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_alerce.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_gaia.py` & `tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_gaia.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_lasair.py` & `tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_lasair.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/tests/brokers/test_mars.py` & `tomtoolkit-2.9.2/tom_alerts/tests/brokers/test_mars.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/tests/tests.py` & `tomtoolkit-2.9.2/tom_alerts/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/urls.py` & `tomtoolkit-2.9.2/tom_alerts/urls.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_alerts/views.py` & `tomtoolkit-2.9.2/tom_alerts/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_base/settings.py` & `tomtoolkit-2.9.2/tom_base/settings.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/forms.py` & `tomtoolkit-2.9.2/tom_catalogs/forms.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvester.py` & `tomtoolkit-2.9.2/tom_catalogs/harvester.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvesters/jplhorizons.py` & `tomtoolkit-2.9.2/tom_catalogs/harvesters/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvesters/mpc.py` & `tomtoolkit-2.9.2/tom_catalogs/harvesters/mpc.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvesters/ned.py` & `tomtoolkit-2.9.2/tom_catalogs/harvesters/ned.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvesters/simbad.py` & `tomtoolkit-2.9.2/tom_catalogs/harvesters/simbad.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/harvesters/tns.py` & `tomtoolkit-2.9.2/tom_catalogs/harvesters/tns.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/tests/harvesters/test_simbad.py` & `tomtoolkit-2.9.2/tom_catalogs/tests/harvesters/test_simbad.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/tests/tests.py` & `tomtoolkit-2.9.2/tom_catalogs/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_catalogs/views.py` & `tomtoolkit-2.9.2/tom_catalogs/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/api_router.py` & `tomtoolkit-2.9.2/tom_common/api_router.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/forms.py` & `tomtoolkit-2.9.2/tom_common/forms.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/hooks.py` & `tomtoolkit-2.9.2/tom_common/hooks.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/middleware.py` & `tomtoolkit-2.9.2/tom_common/middleware.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-16x16.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-32.ico` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-32.ico`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon-32x32.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/favicon.ico` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/icon.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/icon.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-color-cropped.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-color-cropped.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-color.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-color.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/static/tom_common/img/logo-text.png` & `tomtoolkit-2.9.2/tom_common/static/tom_common/img/logo-text.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/auth/partials/group_list.html` & `tomtoolkit-2.9.2/tom_common/templates/auth/partials/group_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/auth/partials/user_list.html` & `tomtoolkit-2.9.2/tom_common/templates/auth/partials/user_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/comments/list.html` & `tomtoolkit-2.9.2/tom_common/templates/comments/list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/tom_common/base.html` & `tomtoolkit-2.9.2/tom_common/templates/tom_common/base.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/tom_common/create_user.html` & `tomtoolkit-2.9.2/tom_common/templates/tom_common/create_user.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/tom_common/index.html` & `tomtoolkit-2.9.2/tom_common/templates/tom_common/index.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/tom_common/navbar_content.html` & `tomtoolkit-2.9.2/tom_common/templates/tom_common/navbar_content.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templates/tom_common/partials/navbar_login.html` & `tomtoolkit-2.9.2/tom_common/templates/tom_common/partials/navbar_login.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templatetags/tom_common_extras.py` & `tomtoolkit-2.9.2/tom_common/templatetags/tom_common_extras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/templatetags/user_extras.py` & `tomtoolkit-2.9.2/tom_common/templatetags/user_extras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/tests.py` & `tomtoolkit-2.9.2/tom_common/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/urls.py` & `tomtoolkit-2.9.2/tom_common/urls.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_common/views.py` & `tomtoolkit-2.9.2/tom_common/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/api_views.py` & `tomtoolkit-2.9.2/tom_dataproducts/api_views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/data_processor.py` & `tomtoolkit-2.9.2/tom_dataproducts/data_processor.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/filters.py` & `tomtoolkit-2.9.2/tom_dataproducts/filters.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/forms.py` & `tomtoolkit-2.9.2/tom_dataproducts/forms.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/hooks.py` & `tomtoolkit-2.9.2/tom_dataproducts/hooks.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/management/commands/downloaddata.py` & `tomtoolkit-2.9.2/tom_dataproducts/management/commands/downloaddata.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/management/commands/updatereduceddata.py` & `tomtoolkit-2.9.2/tom_dataproducts/management/commands/updatereduceddata.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0001_initial.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0004_auto_20190626_0904.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0004_auto_20190626_0904.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0005_auto_20190704_1010.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0005_auto_20190704_1010.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0007_manual_20191016_rename_type.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0007_manual_20191016_rename_type.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0008_auto_20191205_1952.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0008_auto_20191205_1952.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/migrations/0010_manual_20210305_fix_spectroscopy.py` & `tomtoolkit-2.9.2/tom_dataproducts/migrations/0010_manual_20210305_fix_spectroscopy.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/models.py` & `tomtoolkit-2.9.2/tom_dataproducts/models.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/processors/data_serializers.py` & `tomtoolkit-2.9.2/tom_dataproducts/processors/data_serializers.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/processors/photometry_processor.py` & `tomtoolkit-2.9.2/tom_dataproducts/processors/photometry_processor.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/processors/spectroscopy_processor.py` & `tomtoolkit-2.9.2/tom_dataproducts/processors/spectroscopy_processor.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/serializers.py` & `tomtoolkit-2.9.2/tom_dataproducts/serializers.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/static/tom_dataproducts/img/placeholder.png` & `tomtoolkit-2.9.2/tom_dataproducts/static/tom_dataproducts/img/placeholder.png`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproduct_list.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproduct_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_detail.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_detail.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_list.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/dataproductgroup_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/dataproduct_list_for_target.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/dataproduct_list_for_target.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/js9_scripts.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/js9_scripts.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/recent_photometry.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/recent_photometry.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/saved_dataproduct_list_for_observation.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/saved_dataproduct_list_for_observation.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/unsaved_dataproduct_list_for_observation.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/unsaved_dataproduct_list_for_observation.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templates/tom_dataproducts/partials/upload_dataproduct.html` & `tomtoolkit-2.9.2/tom_dataproducts/templates/tom_dataproducts/partials/upload_dataproduct.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/templatetags/dataproduct_extras.py` & `tomtoolkit-2.9.2/tom_dataproducts/templatetags/dataproduct_extras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/tests/test_api.py` & `tomtoolkit-2.9.2/tom_dataproducts/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/tests/test_data/test_spectrum.fits` & `tomtoolkit-2.9.2/tom_dataproducts/tests/test_data/test_spectrum.fits`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/tests/tests.py` & `tomtoolkit-2.9.2/tom_dataproducts/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/urls.py` & `tomtoolkit-2.9.2/tom_dataproducts/urls.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/utils.py` & `tomtoolkit-2.9.2/tom_dataproducts/utils.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_dataproducts/views.py` & `tomtoolkit-2.9.2/tom_dataproducts/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/admin.py` & `tomtoolkit-2.9.2/tom_observations/admin.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/api_views.py` & `tomtoolkit-2.9.2/tom_observations/api_views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/cadence.py` & `tomtoolkit-2.9.2/tom_observations/cadence.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/cadences/resume_cadence_after_failure.py` & `tomtoolkit-2.9.2/tom_observations/cadences/resume_cadence_after_failure.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/cadences/retry_failed_observations.py` & `tomtoolkit-2.9.2/tom_observations/cadences/retry_failed_observations.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facilities/gemini.py` & `tomtoolkit-2.9.2/tom_observations/facilities/gemini.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facilities/lco.py` & `tomtoolkit-2.9.2/tom_observations/facilities/lco.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facilities/lt.py` & `tomtoolkit-2.9.2/tom_observations/facilities/lt.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facilities/manual.py` & `tomtoolkit-2.9.2/tom_observations/facilities/manual.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facilities/soar.py` & `tomtoolkit-2.9.2/tom_observations/facilities/soar.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/facility.py` & `tomtoolkit-2.9.2/tom_observations/facility.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/forms.py` & `tomtoolkit-2.9.2/tom_observations/forms.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/management/commands/runcadencestrategies.py` & `tomtoolkit-2.9.2/tom_observations/management/commands/runcadencestrategies.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/management/commands/updatestatus.py` & `tomtoolkit-2.9.2/tom_observations/management/commands/updatestatus.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0001_initial.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0002_auto_20190306_2343.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0002_auto_20190306_2343.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0004_observationgroup.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0004_observationgroup.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0007_observationstrategy.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0007_observationstrategy.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0009_observationrecord_user.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0009_observationrecord_user.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0010_manual_create_dynamic_cadence.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0010_manual_create_dynamic_cadence.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0011_auto_20200917_0306.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0011_auto_20200917_0306.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/migrations/0012_auto_20210205_1819.py` & `tomtoolkit-2.9.2/tom_observations/migrations/0012_auto_20210205_1819.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/models.py` & `tomtoolkit-2.9.2/tom_observations/models.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/observation_template.py` & `tomtoolkit-2.9.2/tom_observations/observation_template.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/serializers.py` & `tomtoolkit-2.9.2/tom_observations/serializers.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observation_form.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observation_form.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observation_list.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observation_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationgroup_list.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationgroup_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationrecord_detail.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationrecord_detail.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/observationtemplate_list.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/observationtemplate_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/facility_status.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/facility_status.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templates/tom_observations/partials/observation_list.html` & `tomtoolkit-2.9.2/tom_observations/templates/tom_observations/partials/observation_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/templatetags/observation_extras.py` & `tomtoolkit-2.9.2/tom_observations/templatetags/observation_extras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/facilities/test_gemini.py` & `tomtoolkit-2.9.2/tom_observations/tests/facilities/test_gemini.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/facilities/test_lco.py` & `tomtoolkit-2.9.2/tom_observations/tests/facilities/test_lco.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/facilities/test_soar.py` & `tomtoolkit-2.9.2/tom_observations/tests/facilities/test_soar.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/factories.py` & `tomtoolkit-2.9.2/tom_observations/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/test_api.py` & `tomtoolkit-2.9.2/tom_observations/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/test_cadence.py` & `tomtoolkit-2.9.2/tom_observations/tests/test_cadence.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/tests.py` & `tomtoolkit-2.9.2/tom_observations/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/tests/utils.py` & `tomtoolkit-2.9.2/tom_observations/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/urls.py` & `tomtoolkit-2.9.2/tom_observations/urls.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/utils.py` & `tomtoolkit-2.9.2/tom_observations/utils.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/views.py` & `tomtoolkit-2.9.2/tom_observations/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_observations/widgets.py` & `tomtoolkit-2.9.2/tom_observations/widgets.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_setup/management/commands/tom_setup.py` & `tomtoolkit-2.9.2/tom_setup/management/commands/tom_setup.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_setup/templates/tom_setup/settings.tmpl` & `tomtoolkit-2.9.2/tom_setup/templates/tom_setup/settings.tmpl`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_setup/templates/tom_setup/urls.tmpl` & `tomtoolkit-2.9.2/tom_setup/templates/tom_setup/urls.tmpl`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/api_views.py` & `tomtoolkit-2.9.2/tom_targets/api_views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/filters.py` & `tomtoolkit-2.9.2/tom_targets/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,10 +108,19 @@
         if request.user.is_authenticated:
             return TargetList.objects.all()
         else:
             return TargetList.objects.none()
 
     targetlist__name = django_filters.ModelChoiceFilter(queryset=get_target_list_queryset, label="Target Grouping")
 
+    order = django_filters.OrderingFilter(
+        fields=['name', 'created', 'modified'],
+        field_labels={
+            'name': 'Name',
+            'created': 'Creation Date',
+            'modified': 'Last Update'
+        }
+    )
+
     class Meta:
         model = Target
         fields = ['type', 'name', 'key', 'value', 'cone_search', 'targetlist__name']
```

### Comparing `tomtoolkit-2.9.1/tom_targets/forms.py` & `tomtoolkit-2.9.2/tom_targets/forms.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/groups.py` & `tomtoolkit-2.9.2/tom_targets/groups.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/management/commands/setdefaultextras.py` & `tomtoolkit-2.9.2/tom_targets/management/commands/setdefaultextras.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0001_initial.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0002_auto_20190115_2102.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0002_auto_20190115_2102.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0002_auto_20190117_2248.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0002_auto_20190117_2248.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0004_auto_20190123_2010.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0004_auto_20190123_2010.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0005_auto_20190214_1722.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0005_auto_20190214_1722.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0006_auto_20190403_1659.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0006_auto_20190403_1659.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0013_manual_20190916_multiple_names.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0013_manual_20190916_multiple_names.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0014_auto_20190923_1827.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0014_auto_20190923_1827.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0015_auto_20190923_2233.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0015_auto_20190923_2233.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/migrations/0017_auto_20200130_2350.py` & `tomtoolkit-2.9.2/tom_targets/migrations/0017_auto_20200130_2350.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/models.py` & `tomtoolkit-2.9.2/tom_targets/models.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/serializers.py` & `tomtoolkit-2.9.2/tom_targets/serializers.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/aladin.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/aladin.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/recent_targets.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/recent_targets.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/recently_updated_targets.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/recently_updated_targets.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_data.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_data.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_groups.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_groups.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/target_table.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/target_table.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/partials/targetlist_select.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/partials/targetlist_select.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_detail.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_detail.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_form.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_form.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_grouping.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_grouping.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_import.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_import.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templates/tom_targets/target_list.html` & `tomtoolkit-2.9.2/tom_targets/templates/tom_targets/target_list.html`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/templatetags/targets_extras.py` & `tomtoolkit-2.9.2/tom_targets/templatetags/targets_extras.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from datetime import datetime, timedelta
 
 from astroplan import moon_illumination
 from astropy import units as u
 from astropy.coordinates import Angle, get_moon, SkyCoord
 from astropy.time import Time
-from dateutil.parser import parse
 from django import template
 from django.conf import settings
 from django.db.models import Q
 from guardian.shortcuts import get_objects_for_user
 import numpy as np
 from plotly import offline
 from plotly import graph_objs as go
@@ -80,36 +79,36 @@
     """
     groups = TargetList.objects.filter(targets=target)
     return {'target': target,
             'groups': groups}
 
 
 @register.inclusion_tag('tom_targets/partials/target_plan.html', takes_context=True)
-def target_plan(context):
+def target_plan(context, fast_render=False):
     """
     Displays form and renders plot for visibility calculation. Using this templatetag to render a plot requires that
     the context of the parent view have values for start_time, end_time, and airmass.
+
+    :param fast_render: Render the plot on page load, defaults to the next 24hrs and 2.5 airmass
+    :type fast_render: bool
     """
     request = context['request']
     plan_form = TargetVisibilityForm()
     visibility_graph = ''
-    if all(request.GET.get(x) for x in ['start_time', 'end_time']):
+    if all(request.GET.get(x) for x in ['start_time', 'end_time']) or fast_render:
         plan_form = TargetVisibilityForm({
-            'start_time': request.GET.get('start_time'),
-            'end_time': request.GET.get('end_time'),
-            'airmass': request.GET.get('airmass'),
+            'start_time': request.GET.get('start_time', datetime.utcnow()),
+            'end_time': request.GET.get('end_time', datetime.utcnow() + timedelta(days=1)),
+            'airmass': request.GET.get('airmass', 2.5),
             'target': context['object']
         })
         if plan_form.is_valid():
-            start_time = parse(request.GET['start_time'])
-            end_time = parse(request.GET['end_time'])
-            if request.GET.get('airmass'):
-                airmass_limit = float(request.GET.get('airmass'))
-            else:
-                airmass_limit = None
+            start_time = plan_form.cleaned_data['start_time']
+            end_time = plan_form.cleaned_data['end_time']
+            airmass_limit = plan_form.cleaned_data['airmass']
             visibility_data = get_sidereal_visibility(context['object'], start_time, end_time, 10, airmass_limit)
             plot_data = [
                 go.Scatter(x=data[0], y=data[1], mode='lines', name=site) for site, data in visibility_data.items()
             ]
             layout = go.Layout(yaxis=dict(autorange='reversed'))
             visibility_graph = offline.plot(
                 go.Figure(data=plot_data, layout=layout), output_type='div', show_link=False
```

### Comparing `tomtoolkit-2.9.1/tom_targets/tests/factories.py` & `tomtoolkit-2.9.2/tom_targets/tests/factories.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/tests/test_api.py` & `tomtoolkit-2.9.2/tom_targets/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/tests/tests.py` & `tomtoolkit-2.9.2/tom_targets/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/urls.py` & `tomtoolkit-2.9.2/tom_targets/urls.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/utils.py` & `tomtoolkit-2.9.2/tom_targets/utils.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/validators.py` & `tomtoolkit-2.9.2/tom_targets/validators.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tom_targets/views.py` & `tomtoolkit-2.9.2/tom_targets/views.py`

 * *Files identical despite different names*

### Comparing `tomtoolkit-2.9.1/tomtoolkit.egg-info/PKG-INFO` & `tomtoolkit-2.9.2/tomtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomtoolkit
-Version: 2.9.1
+Version: 2.9.2
 Summary: The TOM Toolkit and base modules
 Home-page: https://tomtoolkit.github.io
 Author: TOM Toolkit Project
 Author-email: dcollom@lco.global
 License: UNKNOWN
 Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science,fits,observatory
 Platform: UNKNOWN
```

### Comparing `tomtoolkit-2.9.1/tomtoolkit.egg-info/SOURCES.txt` & `tomtoolkit-2.9.2/tomtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

