# Comparing `tmp/jupyter_scheduler-1.3.1.tar.gz` & `tmp/jupyter_scheduler-1.3.2.tar.gz`

## Comparing `jupyter_scheduler-1.3.1.tar` & `jupyter_scheduler-1.3.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.eslintrc.js
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.prettierrc
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.stylelintrc
--rw-r--r--   0        0        0    29618 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/babel.config.js
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/conftest.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jest.config.js
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/tsconfig.json
--rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/yarn.lock
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/binder/environment.yml
--rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/binder/postBuild
--rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/dev/seed.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/dev/templates/1.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/dev/templates/2.ipynb
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/dev/templates/3.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/Makefile
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/conf.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/make.bat
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/requirements.txt
--rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/_static/jupyter_logo.png
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/contributors/index.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/developers/index.md
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/operators/index.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/index.md
--rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/actions_definition_details.png
--rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/actions_job_details.png
--rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/actions_list.png
--rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/create_job_form.png
--rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/create_job_from_filebrowser.png
--rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/create_job_from_notebook.png
--rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/custom_schedule.png
--rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/download_button.png
--rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/downloaded_files.png
--rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/headers.png
--rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/item_name.png
--rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/launcher.png
--rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/docs/users/images/run_on_schedule.png
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter-config/nb-config/jupyter_scheduler.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter-config/server-config/jupyter_scheduler.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/_version.py
--rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/environments.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/exceptions.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/executors.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/extension.py
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/handlers.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/job_files_manager.py
--rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/models.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/orm.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/parameterize.py
--rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/scheduler.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/task_runner.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/utils.py
--rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/package.json
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
--rw-r--r--   0        0        0   347355 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/177.adf946fcd5474bd5f35d.js
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
--rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
--rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
--rw-r--r--   0        0        0   121683 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/470.43bf62b4a180bfef098d.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/470.43bf62b4a180bfef098d.js.LICENSE.txt
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
--rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
--rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
--rw-r--r--   0        0        0    80399 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/810.adad3f61633c8610a1c5.js
--rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
--rw-r--r--   0        0        0    10078 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/remoteEntry.ee24a1789f8c03da85c8.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/mocks.py
--rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_job_files_manager.py
--rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/schema/plugin.json
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/advanced-options.tsx
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/context.ts
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/handler.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/hooks.ts
--rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/index.tsx
--rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/model.ts
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/notebook-jobs-panel.tsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/size.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/svg.d.ts
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/theme-provider.ts
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/tokens.ts
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/__tests__/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/box.tsx
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/button-bar.tsx
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/button.tsx
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/cluster.tsx
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/collapsible-panel.tsx
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/compute-type-picker.tsx
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/confirm-buttons.tsx
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/confirm-dialog-buttons.tsx
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/create-schedule-options.tsx
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/environment-picker.tsx
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/error-boundary.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/heading.tsx
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/icon-buttons.tsx
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/icons.ts
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/input-file-snapshot.tsx
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/job-definition-row.tsx
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/job-file-link.tsx
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/job-row.tsx
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/labeled-value.tsx
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/output-format-picker.tsx
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/parameters-picker.tsx
--rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/schedule-inputs.tsx
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/stack.tsx
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/advanced-table/advanced-table-header.tsx
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/advanced-table/advanced-table.tsx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/components/advanced-table/index.tsx
--rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/create-job-from-definition.tsx
--rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/create-job.tsx
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/edit-job-definition.tsx
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/list-jobs.tsx
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/detail-view/detail-view.tsx
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/detail-view/index.tsx
--rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/detail-view/job-definition.tsx
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/mainviews/detail-view/job-detail.tsx
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/util/errors.tsx
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/src/util/job-name-validation.tsx
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/base.css
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/box.css
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/button.css
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/cluster.css
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/collapsible-panel.css
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/edit-job-definitions.css
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/heading.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/index.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/labeled-value.css
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/stack.css
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/variables.css
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/icons/calendar-add-on.svg
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/icons/calendar-month.svg
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/style/icons/event-note.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/ui-tests/tests/jupyter_scheduler.spec.ts
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/LICENSE
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/README.md
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.eslintrc.js
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.prettierrc
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.stylelintrc
+-rw-r--r--   0        0        0    31582 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/MANIFEST.in
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/babel.config.js
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/conftest.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jest.config.js
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/tsconfig.json
+-rw-r--r--   0        0        0   473708 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/yarn.lock
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/binder/environment.yml
+-rwxr-xr-x   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/binder/postBuild
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/seed.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/1.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/2.ipynb
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/dev/templates/3.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/Makefile
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/conf.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/make.bat
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/requirements.txt
+-rw-r--r--   0        0        0    26997 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/_static/jupyter_logo.png
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/contributors/index.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/developers/index.md
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/operators/index.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/index.md
+-rw-r--r--   0        0        0    91253 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_definition_details.png
+-rw-r--r--   0        0        0    72256 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_job_details.png
+-rw-r--r--   0        0        0    23784 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/actions_list.png
+-rw-r--r--   0        0        0   102590 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_form.png
+-rw-r--r--   0        0        0   130914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_from_filebrowser.png
+-rw-r--r--   0        0        0    28924 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/create_job_from_notebook.png
+-rw-r--r--   0        0        0    74875 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/custom_schedule.png
+-rw-r--r--   0        0        0    39322 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/download_button.png
+-rw-r--r--   0        0        0    45498 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/downloaded_files.png
+-rw-r--r--   0        0        0    67024 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/headers.png
+-rw-r--r--   0        0        0    58085 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/item_name.png
+-rw-r--r--   0        0        0    92104 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/launcher.png
+-rw-r--r--   0        0        0    56679 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/docs/users/images/run_on_schedule.png
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter-config/nb-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter-config/server-config/jupyter_scheduler.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/_version.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/environments.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/exceptions.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/executors.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/extension.py
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/handlers.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/job_files_manager.py
+-rw-r--r--   0        0        0     8541 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/models.py
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/orm.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/parameterize.py
+-rw-r--r--   0        0        0    30914 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/scheduler.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/task_runner.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/utils.py
+-rw-r--r--   0        0        0     4715 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/package.json
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/122.b4ab1a65371e7c0f8bdd.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js
+-rw-r--r--   0        0        0   347357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js
+-rw-r--r--   0        0        0    11074 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js
+-rw-r--r--   0        0        0    19234 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js
+-rw-r--r--   0        0        0   121687 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js.LICENSE.txt
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js.LICENSE.txt
+-rw-r--r--   0        0        0   210890 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js.LICENSE.txt
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js
+-rw-r--r--   0        0        0    80399 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/810.a39d1a3a560985b29e1f.js
+-rw-r--r--   0        0        0    25917 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js
+-rw-r--r--   0        0        0    10078 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/remoteEntry.a26c2ca760e8eddba3c9.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/mocks.py
+-rw-r--r--   0        0        0    27273 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_job_files_manager.py
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.html
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/schema/plugin.json
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/advanced-options.tsx
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/context.ts
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/handler.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/hooks.ts
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/index.tsx
+-rw-r--r--   0        0        0    13031 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/model.ts
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/notebook-jobs-panel.tsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/size.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/svg.d.ts
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/theme-provider.ts
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/tokens.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/__tests__/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/box.tsx
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/button-bar.tsx
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/button.tsx
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/cluster.tsx
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/collapsible-panel.tsx
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/compute-type-picker.tsx
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/confirm-buttons.tsx
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/confirm-dialog-buttons.tsx
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/create-schedule-options.tsx
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/environment-picker.tsx
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/error-boundary.tsx
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/heading.tsx
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/icon-buttons.tsx
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/icons.ts
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/input-file-snapshot.tsx
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-definition-row.tsx
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-file-link.tsx
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/job-row.tsx
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/labeled-value.tsx
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/output-format-picker.tsx
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/parameters-picker.tsx
+-rw-r--r--   0        0        0    16376 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/schedule-inputs.tsx
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/stack.tsx
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table-header.tsx
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table.tsx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/components/advanced-table/index.tsx
+-rw-r--r--   0        0        0     8298 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/create-job-from-definition.tsx
+-rw-r--r--   0        0        0    19783 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/create-job.tsx
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/edit-job-definition.tsx
+-rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/list-jobs.tsx
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/detail-view.tsx
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/index.tsx
+-rw-r--r--   0        0        0     7010 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-definition.tsx
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-detail.tsx
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/util/errors.tsx
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/src/util/job-name-validation.tsx
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/base.css
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/box.css
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/button.css
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/cluster.css
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/collapsible-panel.css
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/edit-job-definitions.css
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/heading.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/index.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/labeled-value.css
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/stack.css
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/variables.css
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/calendar-add-on.svg
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/calendar-month.svg
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/style/icons/event-note.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/ui-tests/tests/jupyter_scheduler.spec.ts
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/README.md
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 jupyter_scheduler-1.3.2/PKG-INFO
```

### Comparing `jupyter_scheduler-1.3.1/.eslintrc.js` & `jupyter_scheduler-1.3.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/.pre-commit-config.yaml` & `jupyter_scheduler-1.3.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,27 @@
       - id: check-yaml
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
         args: ["--profile", "black"]
         files: \.py$
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
@@ -42,15 +42,15 @@
             "flake8-bugbear==20.1.4",
             "flake8-logging-format==0.6.0",
             "flake8-implicit-str-concat==0.2.0",
           ]
         stages: [manual]
 
   - repo: https://github.com/sirosen/check-jsonschema
-    rev: 0.21.0
+    rev: 0.23.0
     hooks:
       - id: check-jsonschema
         name: "Check GitHub Workflows"
         files: ^\.github/workflows/
         types: [yaml]
         args: ["--schemafile", "https://json.schemastore.org/github-workflow"]
         stages: [manual]
```

### Comparing `jupyter_scheduler-1.3.1/.stylelintrc` & `jupyter_scheduler-1.3.2/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/CHANGELOG.md` & `jupyter_scheduler-1.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,49 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.3.2
+
+([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.1...6e4081a273b6da508942d3fe0b4a8ee75f2eade3))
+
+### Bugs fixed
+
+- Fixed encoding while reading notebook in some platforms [#354](https://github.com/jupyter-server/jupyter-scheduler/pull/354) ([@3coins](https://github.com/3coins))
+
+### Maintenance and upkeep improvements
+
+- Bump webpack from 5.74.0 to 5.76.1 [#360](https://github.com/jupyter-server/jupyter-scheduler/pull/360) ([@dependabot](https://github.com/dependabot))
+- Bump json5 from 1.0.1 to 1.0.2 [#359](https://github.com/jupyter-server/jupyter-scheduler/pull/359) ([@dependabot](https://github.com/dependabot))
+- Bump loader-utils from 1.4.0 to 1.4.2 [#357](https://github.com/jupyter-server/jupyter-scheduler/pull/357) ([@dependabot](https://github.com/dependabot))
+- Bump http-cache-semantics from 4.1.0 to 4.1.1 [#358](https://github.com/jupyter-server/jupyter-scheduler/pull/358) ([@dependabot](https://github.com/dependabot))
+- Bump decode-uri-component from 0.2.0 to 0.2.2 [#356](https://github.com/jupyter-server/jupyter-scheduler/pull/356) ([@dependabot](https://github.com/dependabot))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-02-27&to=2023-05-11&type=c))
+
+[@3coins](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3A3coins+updated%3A2023-02-27..2023-05-11&type=Issues) | [@dependabot](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Adependabot+updated%3A2023-02-27..2023-05-11&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Agithub-actions+updated%3A2023-02-27..2023-05-11&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3Apre-commit-ci+updated%3A2023-02-27..2023-05-11&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.3.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.3.0...e36032d3331200b4f21261bdc50e8d733e66b2bc))
 
 ### Bugs fixed
 
 - Fixed issue with extension always deactivating [#347](https://github.com/jupyter-server/jupyter-scheduler/pull/347) ([@3coins](https://github.com/3coins))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyter-scheduler/graphs/contributors?from=2023-02-24&to=2023-02-27&type=c))
 
 [@3coins](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyter-scheduler+involves%3A3coins+updated%3A2023-02-24..2023-02-27&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.3.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyter-scheduler/compare/v1.2.0...e7c0c1b12f3a0debb9cd30b1ddc6d6b7ddfd800e))
 
 ### Enhancements made
 
 - bump binder node version [#343](https://github.com/jupyter-server/jupyter-scheduler/pull/343) ([@dlqqq](https://github.com/dlqqq))
```

### Comparing `jupyter_scheduler-1.3.1/MANIFEST.in` & `jupyter_scheduler-1.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/conftest.py` & `jupyter_scheduler-1.3.2/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jest.config.js` & `jupyter_scheduler-1.3.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/package.json` & `jupyter_scheduler-1.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.2'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `jupyter_scheduler-1.3.1/tsconfig.json` & `jupyter_scheduler-1.3.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/yarn.lock` & `jupyter_scheduler-1.3.2/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4229,17 +4229,17 @@
 
 decimal.js@^10.2.1:
   version "10.4.0"
   resolved "https://registry.yarnpkg.com/decimal.js/-/decimal.js-10.4.0.tgz#97a7448873b01e92e5ff9117d89a7bca8e63e0fe"
   integrity sha512-Nv6ENEzyPQ6AItkGwLE2PGKinZZ9g59vSh2BeH6NqPu0OTKZ5ruJsVqh/orbAnqXc9pBbgXAIrc2EyaCj8NpGg==
 
 decode-uri-component@^0.2.0:
-  version "0.2.0"
-  resolved "https://registry.yarnpkg.com/decode-uri-component/-/decode-uri-component-0.2.0.tgz#eb3913333458775cb84cd1a1fae062106bb87545"
-  integrity sha512-hjf+xovcEn31w/EUYdTXQh/8smFL/dzYjohQGEIgjyNavaJfBY2p5F527Bo1VPATxv0VYTUC2bOcXvqFwk78Og==
+  version "0.2.2"
+  resolved "https://registry.yarnpkg.com/decode-uri-component/-/decode-uri-component-0.2.2.tgz#e69dbe25d37941171dd540e024c444cd5188e1e9"
+  integrity sha512-FqUYQ+8o158GyGTrMFJms9qh3CqTKvAqgqsTnkLI8sKu0028orqBhxNMFkFen0zGyg6epACD32pjVk58ngIErQ==
 
 decompress-response@^3.3.0:
   version "3.3.0"
   resolved "https://registry.yarnpkg.com/decompress-response/-/decompress-response-3.3.0.tgz#80a4dd323748384bfa248083622aedec982adff3"
   integrity sha512-BzRPQuY1ip+qDonAOz42gRm/pg9F768C+npV/4JOsxRC2sq+Rlk+Q4ZCAsOhnIaMrgarILY+RMUIvMmmX1qAEA==
   dependencies:
     mimic-response "^1.0.0"
@@ -5640,17 +5640,17 @@
   dependencies:
     domelementtype "^2.0.1"
     domhandler "^4.0.0"
     domutils "^2.5.2"
     entities "^2.0.0"
 
 http-cache-semantics@^4.0.0:
-  version "4.1.0"
-  resolved "https://registry.yarnpkg.com/http-cache-semantics/-/http-cache-semantics-4.1.0.tgz#49e91c5cbf36c9b94bcfcd71c23d5249ec74e390"
-  integrity sha512-carPklcUh7ROWRK7Cv27RPtdhYhUsela/ue5/jKzjegVvXDqM2ILE9Q2BGn9JZJh1g87cp56su/FgQSzcWS8cQ==
+  version "4.1.1"
+  resolved "https://registry.yarnpkg.com/http-cache-semantics/-/http-cache-semantics-4.1.1.tgz#abe02fcb2985460bf0323be664436ec3476a6d5a"
+  integrity sha512-er295DKPVsV82j5kw1Gjt+ADA/XYHsajl82cGNQG2eyoPkvgUhX+nDIyelzhIWbbsXP39EHcI6l5tYs2FYqYXQ==
 
 http-errors@2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/http-errors/-/http-errors-2.0.0.tgz#b7774a1486ef73cf7667ac9ae0858c012c57b9d3"
   integrity sha512-FtwrG/euBzaEjYeRqOgly7G0qviiXoJWnvEH2Z1plBdXgbyjv34pHTSb9zoeHMyDy33+DWy5Wt9Wo+TURtOYSQ==
   dependencies:
     depd "2.0.0"
@@ -6703,22 +6703,22 @@
 
 json-to-html@~0.1.2:
   version "0.1.2"
   resolved "https://registry.yarnpkg.com/json-to-html/-/json-to-html-0.1.2.tgz#7a095ae4a34b33534aad0970ca4b7417b2c11ee3"
   integrity sha512-gwezGNdnxPnp+7m5aVFq080KGjURyLqLAMmoRlkfnapQYluxQX18Hu+MOPYOtPaipYSB1bawQem5cmvRo/aAMA==
 
 json5@2.x, json5@^2.1.1, json5@^2.1.2, json5@^2.2.1:
-  version "2.2.1"
-  resolved "https://registry.yarnpkg.com/json5/-/json5-2.2.1.tgz#655d50ed1e6f95ad1a3caababd2b0efda10b395c"
-  integrity sha512-1hqLFMSrGHRHxav9q9gNjJ5EXznIxGVO09xQRrwplcS8qs28pZ8s8hupZAmqDwZUmVZ2Qb2jnyPOWcDH8m8dlA==
+  version "2.2.3"
+  resolved "https://registry.yarnpkg.com/json5/-/json5-2.2.3.tgz#78cd6f1a19bdc12b73db5ad0c61efd66c1e29283"
+  integrity sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==
 
 json5@^1.0.1:
-  version "1.0.1"
-  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.1.tgz#779fb0018604fa854eacbf6252180d83543e3dbe"
-  integrity sha512-aKS4WQjPenRxiQsC93MNfjx+nbF4PAdYzmd/1JIj8HYzqfbu86beTuNgXDzPknWk0n0uARlyewZo4s++ES36Ow==
+  version "1.0.2"
+  resolved "https://registry.yarnpkg.com/json5/-/json5-1.0.2.tgz#63d98d60f21b313b77c4d6da18bfa69d80e1d593"
+  integrity sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==
   dependencies:
     minimist "^1.2.0"
 
 jsonfile@^6.0.1:
   version "6.1.0"
   resolved "https://registry.yarnpkg.com/jsonfile/-/jsonfile-6.1.0.tgz#bc55b2634793c679ec6403094eb13698a6ec0aae"
   integrity sha512-5dgndWOriYSm5cnYaJNhalLNDKOqFwyDB/rr1E9ZsGciGvKPs8R2xYGCacuf3z6K1YKDz182fd+fY3cn3pMqXQ==
@@ -6968,26 +6968,26 @@
 
 loader-runner@^4.2.0:
   version "4.3.0"
   resolved "https://registry.yarnpkg.com/loader-runner/-/loader-runner-4.3.0.tgz#c1b4a163b99f614830353b16755e7149ac2314e1"
   integrity sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==
 
 loader-utils@^1.0.0, loader-utils@^1.1.0:
-  version "1.4.0"
-  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-1.4.0.tgz#c579b5e34cb34b1a74edc6c1fb36bfa371d5a613"
-  integrity sha512-qH0WSMBtn/oHuwjy/NucEgbx5dbxxnxup9s4PVXJUDHZBQY+s0NWA9rJf53RBnQZxfch7euUui7hpoAPvALZdA==
+  version "1.4.2"
+  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-1.4.2.tgz#29a957f3a63973883eb684f10ffd3d151fec01a3"
+  integrity sha512-I5d00Pd/jwMD2QCduo657+YM/6L3KZu++pmX9VFncxaxvHcru9jx1lBaFft+r4Mt2jK0Yhp41XlRAihzPxHNCg==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^1.0.1"
 
 loader-utils@^2.0.0, loader-utils@~2.0.0:
-  version "2.0.2"
-  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-2.0.2.tgz#d6e3b4fb81870721ae4e0868ab11dd638368c129"
-  integrity sha512-TM57VeHptv569d/GKh6TAYdzKblwDNiumOdkFnejjD0XwTH87K90w3O7AiJRqdQoXygvi1VQTJTLGhJl7WqA7A==
+  version "2.0.4"
+  resolved "https://registry.yarnpkg.com/loader-utils/-/loader-utils-2.0.4.tgz#8b5cb38b5c34a9a018ee1fc0e6a066d1dfcc528c"
+  integrity sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==
   dependencies:
     big.js "^5.2.2"
     emojis-list "^3.0.0"
     json5 "^2.1.2"
 
 locate-path@^5.0.0:
   version "5.0.0"
@@ -10089,17 +10089,17 @@
 
 webpack-sources@^3.2.3:
   version "3.2.3"
   resolved "https://registry.yarnpkg.com/webpack-sources/-/webpack-sources-3.2.3.tgz#2d4daab8451fd4b240cc27055ff6a0c2ccea0cde"
   integrity sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==
 
 webpack@^5.41.1:
-  version "5.74.0"
-  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.74.0.tgz#02a5dac19a17e0bb47093f2be67c695102a55980"
-  integrity sha512-A2InDwnhhGN4LYctJj6M1JEaGL7Luj6LOmyBHjcI8529cm5p6VXiTIW2sn6ffvEAKmveLzvu4jrihwXtPojlAA==
+  version "5.76.1"
+  resolved "https://registry.yarnpkg.com/webpack/-/webpack-5.76.1.tgz#7773de017e988bccb0f13c7d75ec245f377d295c"
+  integrity sha512-4+YIK4Abzv8172/SGqObnUjaIHjLEuUasz9EwQj/9xmPPkYJy2Mh03Q/lJfSD3YLzbxy5FeTq5Uw0323Oh6SJQ==
   dependencies:
     "@types/eslint-scope" "^3.7.3"
     "@types/estree" "^0.0.51"
     "@webassemblyjs/ast" "1.11.1"
     "@webassemblyjs/wasm-edit" "1.11.1"
     "@webassemblyjs/wasm-parser" "1.11.1"
     acorn "^8.7.1"
```

### Comparing `jupyter_scheduler-1.3.1/binder/postBuild` & `jupyter_scheduler-1.3.2/binder/postBuild`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/dev/seed.py` & `jupyter_scheduler-1.3.2/dev/seed.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/dev/templates/1.ipynb` & `jupyter_scheduler-1.3.2/dev/templates/1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/dev/templates/2.ipynb` & `jupyter_scheduler-1.3.2/dev/templates/2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/dev/templates/3.ipynb` & `jupyter_scheduler-1.3.2/dev/templates/3.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/Makefile` & `jupyter_scheduler-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/conf.py` & `jupyter_scheduler-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/make.bat` & `jupyter_scheduler-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/_static/jupyter_logo.png` & `jupyter_scheduler-1.3.2/docs/_static/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/contributors/index.md` & `jupyter_scheduler-1.3.2/docs/contributors/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/developers/index.md` & `jupyter_scheduler-1.3.2/docs/developers/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/operators/index.md` & `jupyter_scheduler-1.3.2/docs/operators/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/index.md` & `jupyter_scheduler-1.3.2/docs/users/index.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/actions_definition_details.png` & `jupyter_scheduler-1.3.2/docs/users/images/actions_definition_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/actions_job_details.png` & `jupyter_scheduler-1.3.2/docs/users/images/actions_job_details.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/actions_list.png` & `jupyter_scheduler-1.3.2/docs/users/images/actions_list.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/create_job_form.png` & `jupyter_scheduler-1.3.2/docs/users/images/create_job_form.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/create_job_from_filebrowser.png` & `jupyter_scheduler-1.3.2/docs/users/images/create_job_from_filebrowser.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/create_job_from_notebook.png` & `jupyter_scheduler-1.3.2/docs/users/images/create_job_from_notebook.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/custom_schedule.png` & `jupyter_scheduler-1.3.2/docs/users/images/custom_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/download_button.png` & `jupyter_scheduler-1.3.2/docs/users/images/download_button.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/downloaded_files.png` & `jupyter_scheduler-1.3.2/docs/users/images/downloaded_files.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/headers.png` & `jupyter_scheduler-1.3.2/docs/users/images/headers.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/item_name.png` & `jupyter_scheduler-1.3.2/docs/users/images/item_name.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/launcher.png` & `jupyter_scheduler-1.3.2/docs/users/images/launcher.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/docs/users/images/run_on_schedule.png` & `jupyter_scheduler-1.3.2/docs/users/images/run_on_schedule.png`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/environments.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/exceptions.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/executors.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import nbconvert
 import nbformat
 from nbconvert.preprocessors import CellExecutionError, ExecutePreprocessor
 
 from jupyter_scheduler.models import DescribeJob, JobFeature, Status
 from jupyter_scheduler.orm import Job, create_session
 from jupyter_scheduler.parameterize import add_parameters
-from jupyter_scheduler.utils import get_utc_timestamp, resolve_path
+from jupyter_scheduler.utils import get_utc_timestamp
 
 
 class ExecutionManager(ABC):
     """Base execution manager.
     Clients are expected to override this class
     to provide concrete implementations of the
     execution manager. At the minimum, subclasses
@@ -119,15 +119,15 @@
 
 class DefaultExecutionManager(ExecutionManager):
     """Default execution manager that executes notebooks"""
 
     def execute(self):
         job = self.model
 
-        with open(self.staging_paths["input"]) as f:
+        with open(self.staging_paths["input"], encoding="utf-8") as f:
             nb = nbformat.read(f, as_version=4)
 
         if job.parameters:
             nb = add_parameters(nb, job.parameters)
 
         ep = ExecutePreprocessor(
             kernel_name=nb.metadata.kernelspec["name"],
@@ -159,15 +159,15 @@
             JobFeature.min_retry_interval_millis: False,
             JobFeature.output_filename_template: False,
             JobFeature.stop_job: True,
             JobFeature.delete_job: True,
         }
 
     def validate(cls, input_path: str) -> bool:
-        with open(input_path) as f:
+        with open(input_path, encoding="utf-8") as f:
             nb = nbformat.read(f, as_version=4)
             try:
                 nb.metadata.kernelspec["name"]
             except:
                 return False
             else:
                 return True
@@ -182,15 +182,15 @@
     Should be used along with :class:`~jupyter_scheduler.scheduler.ArchiveDownloadingScheduler`
     as the `scheduler_class` during jupyter server start.
     """
 
     def execute(self):
         job = self.model
 
-        with open(self.staging_paths["input"]) as f:
+        with open(self.staging_paths["input"], encoding="utf-8") as f:
             nb = nbformat.read(f, as_version=4)
 
         if job.parameters:
             nb = add_parameters(nb, job.parameters)
 
         ep = ExecutePreprocessor(
             kernel_name=nb.metadata.kernelspec["name"],
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/extension.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/handlers.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/job_files_manager.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/models.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/orm.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/orm.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/parameterize.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/parameterize.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/scheduler.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/task_runner.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/task_runner.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/utils.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/package.json` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a26c2ca760e8eddba3c9.js'}}",*

 * * "'version'": "'1.3.2'"}*

```diff
@@ -72,15 +72,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ee24a1789f8c03da85c8.js",
+            "load": "static/remoteEntry.a26c2ca760e8eddba3c9.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_scheduler"
                 },
@@ -141,9 +141,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.3.2'"}*

```diff
@@ -136,9 +136,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/schemas/@jupyterlab/scheduler/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/171.7e2184d69fabf35a20de.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/177.adf946fcd5474bd5f35d.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/177.57d0a2a23069220f5e7d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9516,15 +9516,15 @@
                         }), r ? (0, ve.jsx)(vc, {
                             ownerState: d,
                             className: p.actionIcon,
                             children: r
                         }) : null]
                     }))
                 }));
-            var Zc = o(74);
+            var Zc = o(6866);
 
             function xc(e) {
                 return (0, me.Z)("MuiInputAdornment", e)
             }
             const yc = (0, fe.Z)("MuiInputAdornment", ["root", "filled", "standard", "outlined", "positionStart", "positionEnd", "disablePointerEvents", "hiddenLabel", "sizeSmall"]);
             var wc;
             const Sc = ["children", "className", "component", "disablePointerEvents", "disableTypography", "position", "variant"],
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/275.62f1e9da62039893b2cb.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/282.28fe0d7276919a94dd69.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/378.4f60560ffdb6fb1ca62d.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/458.d59c5307102faf5c19a8.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/470.43bf62b4a180bfef098d.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/470.add1a31599b9c294ee16.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 470.43bf62b4a180bfef098d.js.LICENSE.txt */
+/*! For license information please see 470.add1a31599b9c294ee16.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_jupyterlab_scheduler = self.webpackChunk_jupyterlab_scheduler || []).push([
     [470], {
         8999: (e, t, n) => {
             function o(e, t) {
                 return o = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                     return e.__proto__ = t, e
@@ -1883,15 +1883,15 @@
             var o = n(4867);
 
             function r(e) {
                 return (0, o.Z)("MuiIconButton", e)
             }
             const a = (0, n(1588).Z)("MuiIconButton", ["root", "disabled", "colorInherit", "colorPrimary", "colorSecondary", "edgeStart", "edgeEnd", "sizeSmall", "sizeMedium", "sizeLarge"])
         },
-        74: (e, t, n) => {
+        6866: (e, t, n) => {
             n.d(t, {
                 Z: () => v
             });
             var o = n(9756),
                 r = n(2122),
                 a = n(6271),
                 i = n(4780),
@@ -4296,15 +4296,15 @@
                         children: ye
                     }))]
                 })
             }));
             var C, M, T = n(6594),
                 I = n(9711),
                 O = n(9700),
-                N = n(74),
+                N = n(6866),
                 $ = n(9481),
                 A = n(7530),
                 F = n(8884);
             const j = ["autoWidth", "children", "classes", "className", "defaultOpen", "displayEmpty", "IconComponent", "id", "input", "inputProps", "label", "labelId", "MenuProps", "multiple", "native", "onClose", "onOpen", "open", "renderValue", "SelectDisplayProps", "variant"],
                 L = {
                     name: "MuiSelect",
                     overridesResolver: (e, t) => t.root,
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/506.91939c8c6d49c197dab0.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/613.17512dda5aad1f2a390f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/687.fad750aa8d73847aa14f.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/747.c67d17d558ca77e2d691.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/810.adad3f61633c8610a1c5.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/810.a39d1a3a560985b29e1f.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5,32 +5,32 @@
             n.r(t), n.d(t, {
                 CommandIDs: () => mt,
                 JobsView: () => E,
                 NotebookJobsPanelId: () => ut,
                 Scheduler: () => st,
                 default: () => bt
             });
-            var o = n(6866),
-                a = n(5510),
-                l = n(3535),
-                r = n(1279),
-                i = n(5767),
-                s = n(1258),
-                c = n(5442),
+            var o = n(5687),
+                a = n(3033),
+                l = n(7280),
+                r = n(1467),
+                i = n(1123),
+                s = n(8820),
+                c = n(3169),
                 d = n(6271),
                 m = n.n(d),
                 u = n(296);
 
             function h(e) {
                 let t = "jp-jobs-Cluster";
                 return t += ` justify-content-${e.justifyContent||"flex-start"}`, t += ` align-items-${e.alignItems||"center"}`, t += ` gap-${e.gap||1}`, m().createElement("div", {
                     className: t
                 }, e.children)
             }
-            var p = n(6591);
+            var p = n(2502);
             const b = {
                 lineHeight: 0
             };
 
             function v(e) {
                 return m().createElement(u.IconButton, {
                     "aria-label": "delete",
@@ -287,15 +287,15 @@
                     name: "jupyterlab-scheduler:calendar-month",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 18 18" height="16px" width="16px">\n  <path fill="#0097A7" d="M10 12q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 12 10 12Zm-3.25 0q-.312 0-.531-.219Q6 11.562 6 11.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 12 6.75 12Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM10 15q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q10.312 15 10 15Zm-3.25 0q-.312 0-.531-.219Q6 14.562 6 14.25q0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531Q7.062 15 6.75 15Zm6.5 0q-.312 0-.531-.219-.219-.219-.219-.531 0-.312.219-.531.219-.219.531-.219.312 0 .531.219.219.219.219.531 0 .312-.219.531-.219.219-.531.219ZM4.5 18q-.625 0-1.062-.448Q3 17.104 3 16.5v-11q0-.604.438-1.052Q3.875 4 4.5 4H6V2h1.5v2h5V2H14v2h1.5q.625 0 1.062.448Q17 4.896 17 5.5v11q0 .604-.438 1.052Q16.125 18 15.5 18Zm0-1.5h11V9h-11v7.5Z"/>\n</svg>\n'
                 }),
                 x = new p.LabIcon({
                     name: "jupyterlab-scheduler:event-note",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" height="48" width="48">\n  <path fill="#0097A7" d="M14 27v-3h20v3Zm0 9v-3h13.95v3Zm-5 8q-1.2 0-2.1-.9Q6 42.2 6 41V10q0-1.2.9-2.1Q7.8 7 9 7h3.25V4h3.25v3h17V4h3.25v3H39q1.2 0 2.1.9.9.9.9 2.1v31q0 1.2-.9 2.1-.9.9-2.1.9Zm0-3h30V19.5H9V41Z"/>\n</svg>\n'
                 });
-            var I, F = n(4886);
+            var I, F = n(8142);
             class O {
                 constructor(e) {
                     this.serverSettings = e.serverSettings || s.ServerConnection.makeSettings()
                 }
                 serializeToQueryString(e) {
                     return "?" + Object.keys(e).map((t => {
                         if ("sort_by" === t) {
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/871.cd06f2a4174d6795c435.js`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/remoteEntry.ee24a1789f8c03da85c8.js` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/remoteEntry.a26c2ca760e8eddba3c9.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -45,49 +45,49 @@
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         122: "b4ab1a65371e7c0f8bdd",
         171: "7e2184d69fabf35a20de",
-        177: "adf946fcd5474bd5f35d",
+        177: "57d0a2a23069220f5e7d",
         211: "965ff0ba094d7e4fdd24",
         222: "db4a16544c517f58fd84",
         271: "785d67d6f2d304bfbb8c",
         275: "62f1e9da62039893b2cb",
         282: "28fe0d7276919a94dd69",
         378: "4f60560ffdb6fb1ca62d",
         458: "d59c5307102faf5c19a8",
-        470: "43bf62b4a180bfef098d",
+        470: "add1a31599b9c294ee16",
         506: "91939c8c6d49c197dab0",
         613: "17512dda5aad1f2a390f",
         687: "fad750aa8d73847aa14f",
         747: "c67d17d558ca77e2d691",
         799: "1008956a5a660d3a40dc",
-        810: "adad3f61633c8610a1c5",
+        810: "a39d1a3a560985b29e1f",
         871: "cd06f2a4174d6795c435",
         948: "e8dc554b871d1bd3bef5"
     } [e] + ".js?v=" + {
         122: "b4ab1a65371e7c0f8bdd",
         171: "7e2184d69fabf35a20de",
-        177: "adf946fcd5474bd5f35d",
+        177: "57d0a2a23069220f5e7d",
         211: "965ff0ba094d7e4fdd24",
         222: "db4a16544c517f58fd84",
         271: "785d67d6f2d304bfbb8c",
         275: "62f1e9da62039893b2cb",
         282: "28fe0d7276919a94dd69",
         378: "4f60560ffdb6fb1ca62d",
         458: "d59c5307102faf5c19a8",
-        470: "43bf62b4a180bfef098d",
+        470: "add1a31599b9c294ee16",
         506: "91939c8c6d49c197dab0",
         613: "17512dda5aad1f2a390f",
         687: "fad750aa8d73847aa14f",
         747: "c67d17d558ca77e2d691",
         799: "1008956a5a660d3a40dc",
-        810: "adad3f61633c8610a1c5",
+        810: "a39d1a3a560985b29e1f",
         871: "cd06f2a4174d6795c435",
         948: "e8dc554b871d1bd3bef5"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -141,15 +141,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : d > l.from)) && (n[r] = {
                             get: t,
                             from: d,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.1", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@emotion/react", "11.10.4", (() => Promise.all([P.e(275), P.e(506), P.e(271), P.e(171)]).then((() => () => P(5506))))), l("@emotion/styled", "11.10.4", (() => Promise.all([P.e(378), P.e(271), P.e(211), P.e(799), P.e(122)]).then((() => () => P(4378))))), l("@jupyterlab/scheduler", "1.3.2", (() => Promise.all([P.e(687), P.e(470), P.e(271), P.e(222), P.e(948), P.e(810)]).then((() => () => P(1810))))), l("@mui/material", "5.10.6", (() => Promise.all([P.e(687), P.e(177), P.e(470), P.e(271), P.e(222), P.e(948)]).then((() => () => P(4177))))), l("@mui/system", "5.10.6", (() => Promise.all([P.e(275), P.e(687), P.e(871), P.e(271), P.e(211), P.e(222)]).then((() => () => P(1871))))), l("cronstrue", "2.12.0", (() => P.e(458).then((() => () => P(2458))))), l("tzdata", "1.0.33", (() => P.e(613).then((() => () => P(8613)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -256,34 +256,34 @@
         6271: () => h("default", "react", [1, 17, 0, 1]),
         2148: () => m("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([P.e(275), P.e(506), P.e(282)]).then((() => () => P(5506))))),
         8800: () => m("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([P.e(378), P.e(211), P.e(799)]).then((() => () => P(4378))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         7313: () => m("default", "@mui/system", [1, 5, 10, 6], (() => Promise.all([P.e(275), P.e(871), P.e(211)]).then((() => () => P(1871))))),
         296: () => m("default", "@mui/material", [1, 5, 10, 6], (() => P.e(177).then((() => () => P(4177))))),
         763: () => m("default", "tzdata", [1, 1, 0, 33], (() => P.e(613).then((() => () => P(8613))))),
-        1258: () => h("default", "@jupyterlab/services", [1, 6, 6, 1]),
-        1279: () => h("default", "@jupyterlab/launcher", [1, 3, 6, 1]),
+        1123: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        1467: () => h("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
         1526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
         1840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
         2344: () => m("default", "cronstrue", [1, 2, 12, 0], (() => P.e(458).then((() => () => P(2458))))),
-        3535: () => h("default", "@jupyterlab/filebrowser", [1, 3, 6, 1]),
-        4886: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 1]),
-        5442: () => h("default", "@jupyterlab/translation", [1, 3, 6, 1]),
-        5510: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 1]),
-        5767: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 1]),
-        6591: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 1]),
-        6866: () => h("default", "@jupyterlab/application", [1, 3, 6, 1]),
+        2502: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
+        3033: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        3169: () => h("default", "@jupyterlab/translation", [1, 3, 6, 3]),
+        5687: () => h("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        7280: () => h("default", "@jupyterlab/filebrowser", [1, 3, 6, 3]),
+        8142: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        8820: () => h("default", "@jupyterlab/services", [1, 6, 6, 3]),
         5211: () => p("default", "@emotion/react", (() => Promise.all([P.e(275), P.e(506), P.e(282)]).then((() => () => P(5506))))),
         799: () => m("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([P.e(275), P.e(506)]).then((() => () => P(5506)))))
     }, g = {
         211: [5211],
         222: [2148, 8800],
         271: [6271],
         799: [799],
-        810: [296, 763, 1258, 1279, 1526, 1840, 2344, 3535, 4886, 5442, 5510, 5767, 6591, 6866],
+        810: [296, 763, 1123, 1467, 1526, 1840, 2344, 2502, 3033, 3169, 5687, 7280, 8142, 8820],
         948: [4456, 7313]
     }, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
```

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/labextension/static/third-party-licenses.json` & `jupyter_scheduler-1.3.2/jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/mocks.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_handlers.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_job_files_manager.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_job_files_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_scheduler.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/utils.py` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld-1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-1/helloworld.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz` & `jupyter_scheduler-1.3.2/jupyter_scheduler/tests/test_staging_dir/job-2/helloworld.tar.gz`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/schema/plugin.json` & `jupyter_scheduler-1.3.2/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/advanced-options.tsx` & `jupyter_scheduler-1.3.2/src/advanced-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/handler.ts` & `jupyter_scheduler-1.3.2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/index.tsx` & `jupyter_scheduler-1.3.2/src/index.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/model.ts` & `jupyter_scheduler-1.3.2/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/notebook-jobs-panel.tsx` & `jupyter_scheduler-1.3.2/src/notebook-jobs-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/theme-provider.ts` & `jupyter_scheduler-1.3.2/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/tokens.ts` & `jupyter_scheduler-1.3.2/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/cluster.tsx` & `jupyter_scheduler-1.3.2/src/components/cluster.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/collapsible-panel.tsx` & `jupyter_scheduler-1.3.2/src/components/collapsible-panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/compute-type-picker.tsx` & `jupyter_scheduler-1.3.2/src/components/compute-type-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/confirm-buttons.tsx` & `jupyter_scheduler-1.3.2/src/components/confirm-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/confirm-dialog-buttons.tsx` & `jupyter_scheduler-1.3.2/src/components/confirm-dialog-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/create-schedule-options.tsx` & `jupyter_scheduler-1.3.2/src/components/create-schedule-options.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/environment-picker.tsx` & `jupyter_scheduler-1.3.2/src/components/environment-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/error-boundary.tsx` & `jupyter_scheduler-1.3.2/src/components/error-boundary.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/heading.tsx` & `jupyter_scheduler-1.3.2/src/components/heading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/icon-buttons.tsx` & `jupyter_scheduler-1.3.2/src/components/icon-buttons.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/icons.ts` & `jupyter_scheduler-1.3.2/src/components/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/input-file-snapshot.tsx` & `jupyter_scheduler-1.3.2/src/components/input-file-snapshot.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/job-definition-row.tsx` & `jupyter_scheduler-1.3.2/src/components/job-definition-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/job-file-link.tsx` & `jupyter_scheduler-1.3.2/src/components/job-file-link.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/job-row.tsx` & `jupyter_scheduler-1.3.2/src/components/job-row.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/labeled-value.tsx` & `jupyter_scheduler-1.3.2/src/components/labeled-value.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/output-format-picker.tsx` & `jupyter_scheduler-1.3.2/src/components/output-format-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/parameters-picker.tsx` & `jupyter_scheduler-1.3.2/src/components/parameters-picker.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/schedule-inputs.tsx` & `jupyter_scheduler-1.3.2/src/components/schedule-inputs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/advanced-table/advanced-table-header.tsx` & `jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table-header.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/components/advanced-table/advanced-table.tsx` & `jupyter_scheduler-1.3.2/src/components/advanced-table/advanced-table.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/create-job-from-definition.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/create-job-from-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/create-job.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/create-job.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/edit-job-definition.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/edit-job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/list-jobs.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/list-jobs.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/detail-view/detail-view.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/detail-view/detail-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/detail-view/job-definition.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-definition.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/mainviews/detail-view/job-detail.tsx` & `jupyter_scheduler-1.3.2/src/mainviews/detail-view/job-detail.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/util/errors.tsx` & `jupyter_scheduler-1.3.2/src/util/errors.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/src/util/job-name-validation.tsx` & `jupyter_scheduler-1.3.2/src/util/job-name-validation.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/base.css` & `jupyter_scheduler-1.3.2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/button.css` & `jupyter_scheduler-1.3.2/style/button.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/cluster.css` & `jupyter_scheduler-1.3.2/style/cluster.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/stack.css` & `jupyter_scheduler-1.3.2/style/stack.css`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/icons/calendar-add-on.svg` & `jupyter_scheduler-1.3.2/style/icons/calendar-add-on.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/style/icons/calendar-month.svg` & `jupyter_scheduler-1.3.2/style/icons/calendar-month.svg`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/ui-tests/README.md` & `jupyter_scheduler-1.3.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/ui-tests/jupyter_server_test_config.py` & `jupyter_scheduler-1.3.2/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/.gitignore` & `jupyter_scheduler-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/LICENSE` & `jupyter_scheduler-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/README.md` & `jupyter_scheduler-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_scheduler-1.3.1/pyproject.toml` & `jupyter_scheduler-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.3.1", "jupyterlab~=3.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter_scheduler"
-version = "1.3.1"
+version = "1.3.2"
 description = "A JupyterLab extension for running notebook jobs"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 authors = [
     { name = "Project Jupyter" },
 ]
@@ -89,15 +89,15 @@
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
 build_dir = "jupyter_scheduler/labextension"
 
 [tool.tbump.version]
-current = "1.3.1"
+current = "1.3.2"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [[tool.tbump.file]]
 src = "pyproject.toml"
 version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\""
 
 [[tool.tbump.file]]
```

### Comparing `jupyter_scheduler-1.3.1/PKG-INFO` & `jupyter_scheduler-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_scheduler
-Version: 1.3.1
+Version: 1.3.2
 Summary: A JupyterLab extension for running notebook jobs
 Project-URL: Homepage, https://github.com/jupyter-server/jupyter-scheduler
 Author: Project Jupyter
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Project Jupyter
         All rights reserved.
```

