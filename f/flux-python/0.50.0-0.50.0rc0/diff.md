# Comparing `tmp/flux-python-0.50.0.tar.gz` & `tmp/flux-python-0.50.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.50.0.tar", last modified: Sat May  6 06:45:39 2023, max compression
+gzip compressed data, was "flux-python-0.50.0rc0.tar", last modified: Wed May  3 05:14:03 2023, max compression
```

## Comparing `flux-python-0.50.0.tar` & `flux-python-0.50.0rc0.tar`

### file list

```diff
@@ -1,139 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.825886 flux-python-0.50.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-06 06:40:52.000000 flux-python-0.50.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-06 06:40:52.000000 flux-python-0.50.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-06 06:40:52.000000 flux-python-0.50.0/NOTICE.LLNS
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-06 06:45:39.825886 flux-python-0.50.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-06 06:40:52.000000 flux-python-0.50.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/alloc.py
--rw-r--r--   0 runner    (1001) docker     (123)    54936 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/bulksubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)    32425 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/fortune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/cli/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/constraint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/constraint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/constraint/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/core/handle.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/core/inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/core/trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/core/watchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/debugged.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/hostlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/idset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/job/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/JobID.py
--rw-r--r--   0 runner    (1001) docker     (123)    36034 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/Jobspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    26007 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/job/frobnicator/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/frobnicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/job/frobnicator/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/frobnicator/plugins/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/frobnicator/plugins/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/kvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/timeleft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.817886 flux-python-0.50.0/flux/job/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/job/validator/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/plugins/feasibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/plugins/jobspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/plugins/require-instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/plugins/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/validator/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/job/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/kvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/memoized_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/ResourceSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/ResourceSetImplementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/Rlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/resource/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/uri/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/uri/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/resolvers/jobid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/resolvers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/resolvers/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/resolvers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/uri/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/utils/parsedatetime/
--rw-r--r--   0 runner    (1001) docker     (123)   105234 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/es.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.821886 flux-python-0.50.0/flux/utils/tomli/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21649 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/_re.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/utils/tomli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-06 06:45:30.000000 flux-python-0.50.0/flux/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.825886 flux-python-0.50.0/flux_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 06:45:39.000000 flux-python-0.50.0/flux_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 06:45:39.825886 flux-python-0.50.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-05-06 06:40:52.000000 flux-python-0.50.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 06:45:39.825886 flux-python-0.50.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/_core_build.py
--rw-r--r--   0 runner    (1001) docker     (123)   133080 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_core_clean.h
--rw-r--r--   0 runner    (1001) docker     (123)    55807 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_core_preproc.h
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/_hostlist_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_hostlist_clean.h
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_hostlist_preproc.h
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/_idset_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_idset_clean.h
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_idset_preproc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/_rlist_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/_security_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_security_clean.h
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-06 06:45:31.000000 flux-python-0.50.0/src/_security_preproc.h
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/callbacks.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-05-06 06:40:52.000000 flux-python-0.50.0/src/make_clean_header.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5088 2023-05-03 00:25:02.000000 flux-python-0.50.0rc0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/Makefile.in
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/cli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/cli/_fortune.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/constraint/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constraint/parser.out
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constraint/parsetab.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/core/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/handle.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/inner.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/trampoline.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/watchers.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/debugged.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/future.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/hostlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/idset.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/importer.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/JobID.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/Jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/_wrapper.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/event.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/executor.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/frobnicator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/frobnicator.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/constraints.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/defaults.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/info.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/kill.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/stats.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/submit.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/validator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/validator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/feasibility.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/require-instance.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/schema.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/validator.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/wait.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/memoized_property.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/message.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/progress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/resource/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/ResourceSet.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/ResourceSetImplementation.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/Rlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/rpc.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/security.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/uri/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/uri/resolvers/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/jobid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/lsf.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/pid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/slurm.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/uri.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/utils/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/parsedatetime/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/context.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/parsedatetime.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/warns.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/tomli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/LICENSE
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_parser.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_re.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_types.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/py.typed
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/wrapper.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux_python.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.50.0rc0/flux_python.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12040 2023-05-03 05:08:54.000000 flux-python-0.50.0rc0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/src/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1637 2023-05-03 05:01:59.000000 flux-python-0.50.0rc0/src/_core_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   133080 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_core_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    54367 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_core_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      876 2023-05-03 05:10:48.000000 flux-python-0.50.0rc0/src/_hostlist_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4268 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_hostlist_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_hostlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      961 2023-05-03 05:10:41.000000 flux-python-0.50.0rc0/src/_idset_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_idset_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_idset_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-03 05:13:26.000000 flux-python-0.50.0rc0/src/_rlist_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21443 2023-05-03 00:05:27.000000 flux-python-0.50.0rc0/src/_rlist_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-03 00:05:27.000000 flux-python-0.50.0rc0/src/_rlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1218 2023-05-03 05:13:39.000000 flux-python-0.50.0rc0/src/_security_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_security_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_security_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/callbacks.h
+-rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/make_clean_header.py
```

### Comparing `flux-python-0.50.0/PKG-INFO` & `flux-python-0.50.0rc0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: flux-python
-Version: 0.50.0
-Summary: Python bindings for the flux resource manager API
-Home-page: https://github.com/flux-framework/flux-python
-License: UNKNOWN
-Keywords: flux,job manager,workload manager,orchestration,hpc
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-License-File: NOTICE.LLNS
-
 # Flux Python Bindings
 
 > 🐍️ You called me?
 
 Hello! You've found the flux Python bindings, an experiment to build and deploy
 Flux to Pypi without needing to store code alongside Flux. The goal of
 this experiment is to test them separately. This was originally developed
@@ -42,65 +20,50 @@
 to have an environment ready to go with Flux (and Flux Security). You can follow
 the instructions in the DevContainer to build the Flux Python bindings.
 By default, this environment installs the latest flux-core.
 If you want to build a custom version with Flux core you can do:
 
 ```bash
 rm -rf ~/flux-core
-export FLUX_VERSION=0.48.0
+export FLUX_VERSION=0.50.0
 wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
 tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
 sudo mv flux-core-${FLUX_VERSION} ~/flux-core
 rm flux-core-${FLUX_VERSION}.tar.gz
 cd ~/flux-core
 ./configure --prefix=/usr/local
 make
 sudo make install
 ```
 
-And then copy over the Python source to "flux" and build your custom wheel:
+And then build your custom wheel:
 
 ```bash
-$ rm -rf /workspaces/flux-python/flux
-$ cp -R src/bindings/python/flux /workspaces/flux-python/flux
 $ cd /workspaces/flux-python
-$ python3 setup.py sdist
+$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
 ```
 
 And if you want to upload:
 
 ```bash
 $ twine upload dist/*.tar.gz
 ```
 
 ## Install on a System
 
-Since we need to link to Flux libraries, you are advised to install flux and flux-security in the same location
-that will be discovered via the executable "flux," so typically `/usr` or `/usr/local`. You can do either:
-
-```bash
-# Find the flux version on your system
-flux --version
-
-# Install the bindings that match that version
-pip install flux-python==0.48.0
-```
-And if you are having trouble with the WCI cache, you can also wget the [file directly from pypi]()
-and install the .tar.gz directly.
+Since we need to link to Flux libraries, you generally will need to choose a version, and provide the same flags. We
+require access to the source repository, so you need to do:
 
 ```bash
 wget https://files.pythonhosted.org/packages/25/fb/02951d80e44a19db291f0e7370d4e7d82c0c1b17709a37913881f958dff7/flux-python-0.48.0rc0.tar.gz
-pip install flux-python-0.48.0rc0.tar.gz
-```
-
-If you install to a local (personal) location (e.g., `$HOME/.local`) you'll need to add this to your `PYTHONPATH`
-
-```bash
-# The directory "flux" is under the site-packages here
-export PYTHONPATH=$HOME/.local/lib/python3.7/site-packages
+tar -xzvf flux-python-0.48.0rc0.tar.git clone https://github.com/flux-framework/flux-security security
+git clone https://github.com/flux-framework/flux-core core
+tar -xzvf flux-python-0.48.0rc0.tar.gz
+cd flux-python-0.48.0rc0
+python3 setup.py install flux-python-0.48.0rc0.tar.gz --version 0.48.0rc0 --security-src $HOME/security --flux-root /usr/include/flux --security-include /usr/include/flux/security
 ```
 
 ### Building Modules
 
 We will need to build the tarball providing paths to the flux-core and flux-security
 sources. This can be improved upon to just be one path if all the dependencies
 are provided with the flux install (and we don't need the source). Note
@@ -171,9 +134,7 @@
 >         unsupported platform tag 'linux_x86_64'. 
 
 #### Release
 
 SPDX-License-Identifier: LGPL-3.0
 
 LLNL-CODE-764420
-
-
```

### Comparing `flux-python-0.50.0/flux/__init__.py` & `flux-python-0.50.0rc0/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/constants.py` & `flux-python-0.50.0rc0/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/core/handle.py` & `flux-python-0.50.0rc0/flux/core/handle.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/core/inner.py` & `flux-python-0.50.0rc0/flux/core/inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # This file is part of the Flux resource manager framework.
 # For details, see https://github.com/flux-framework.
 #
 # SPDX-License-Identifier: LGPL-3.0
 ###############################################################
 
+
 from _flux._core import ffi, lib
 from flux.wrapper import Wrapper
 
 
 class Core(Wrapper):
     """
     Generic Core wrapper, you probably do not want or need one of these.
```

### Comparing `flux-python-0.50.0/flux/core/trampoline.py` & `flux-python-0.50.0rc0/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/core/watchers.py` & `flux-python-0.50.0rc0/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/debugged.py` & `flux-python-0.50.0rc0/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/future.py` & `flux-python-0.50.0rc0/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/hostlist.py` & `flux-python-0.50.0rc0/flux/hostlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,57 +103,39 @@
 
     def __len__(self):
         return self.pimpl.count()
 
     def __getitem__(self, index):
         """Index and slice a hostlist
 
-        Works like normal Python list indexing, including slices.
-        Any iterable is also supported as long as the iterable contains
-        only integers.
-
-        Slices and iterables return a new Hostlist object.
+        Works like normal Python list indexing, including slices:
 
         >>> hl = Hostlist("foo[0-9]")
         >>> hl[0]
         'foo0'
         >>> hl[9]
         'foo9'
         >>> hl[-1]
         'foo9'
         >>> hl[8:]
-        Hostlist('foo[8-9]']
+        ['foo8', 'foo9']
         >>> hl[1:3]
-        Hostlist('foo[1-2]']
-        >>> hl[1,3]
-        Hostlist('foo[1,3]']
+        ['foo1', 'foo2']
 
         """
         if isinstance(index, numbers.Integral):
             if index < 0:
                 index = len(self) + index
             if 0 <= index < len(self):
                 # N.B. wrapper class already calls ffi.string() on result:
                 return self.pimpl.nth(index).decode("utf-8")
             raise IndexError("Hostlist index out of range")
 
         if isinstance(index, slice):
-            hl = Hostlist()
-            for n in range(len(self))[index]:
-                hl.append(self[n])
-            return hl
-
-        if isinstance(index, collections.abc.Iterable):
-            hl = Hostlist()
-            for n in index:
-                # Avoid infinite recursion by catching non-integer indices
-                if not isinstance(n, numbers.Integral):
-                    raise TypeError(f"Invalid Hostlist index '{n}'")
-                hl.append(self[n])
-            return hl
+            return [self[n] for n in range(len(self))[index]]
 
         raise TypeError("Hostlist index must be integer or slice")
 
     def __iter__(self):
         """Return a Hostlist iterator"""
         return HostlistIterator(self)
 
@@ -208,15 +190,15 @@
     def uniq(self):
         """Sort and remove duplicate hostnames from Hostlist"""
         self.pimpl.uniq()
         return self
 
     def expand(self):
         """Convert a Hostlist to a Python list"""
-        return list(self)
+        return self[:]
 
     def copy(self):
         """Copy a Hostlist object"""
         return Hostlist(handle=self.pimpl.copy())
 
 
 def decode(arg):
```

### Comparing `flux-python-0.50.0/flux/idset.py` & `flux-python-0.50.0rc0/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/importer.py` & `flux-python-0.50.0rc0/flux/importer.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,45 +12,36 @@
 import os
 import pkgutil
 import sys
 
 
 def import_plugins_pkg(ns_pkg):
     """Import all modules found in the namespace package ``ns_pkg``"""
-    result = {}
-    for finder, name, ispkg in pkgutil.iter_modules(ns_pkg.__path__):
-        try:
-            result[name] = importlib.import_module(f"{ns_pkg.__name__}.{name}")
-        except ImportError as exc:
-            raise ImportError(f"failed to import {name} plugin: {exc}")
-    return result
+    return {
+        name: importlib.import_module(f"{ns_pkg.__name__}.{name}")
+        for finder, name, ispkg in pkgutil.iter_modules(ns_pkg.__path__)
+    }
 
 
 def import_plugins(pkg_name, pluginpath=None):
     """Load plugins from a namespace package and optional additional paths
 
     A plugin in pluginpath with the same name as an existing plugin will
     take precedence
     """
     if pluginpath is not None:
         sys.path[1:1] = pluginpath
 
     try:
         #  Load 'pkg_name' as a namespace plugin
-        #
-        #  Note: importlib.import_module() will raise ModuleNotFoundError
-        #  if pkg_name points to an empty directory, but we just want to
-        #  return an empty list in this case:
-        #
         pkg = importlib.import_module(pkg_name)
+        plugins = import_plugins_pkg(pkg)
     except ModuleNotFoundError:
         return {}
 
-    plugins = import_plugins_pkg(pkg)
-
     if pluginpath is not None:
         #  Undo any added pluginpath elements.
         for path in pluginpath:
             sys.path.remove(path)
 
     return plugins
```

### Comparing `flux-python-0.50.0/flux/job/JobID.py` & `flux-python-0.50.0rc0/flux/job/JobID.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     """Class used to represent a Flux JOBID
 
     JobID is a subclass of `int`, so may be used in place of integer.
     However, a JobID may be created from any valid RFC 19 FLUID
     encoding, including:
 
      - decimal integer (no prefix)
-     - hexadecimal integer (prefix 0x)
+     - hexidecimal integer (prefix 0x)
      - dotted hex (dothex) (xxxx.xxxx.xxxx.xxxx)
      - kvs dir (dotted hex with `job.` prefix)
      - RFC19 F58: (Base58 encoding with prefix `ƒ` or `f`)
 
     A JobID object also has properties for encoding a JOBID into each
     of the above representations, e.g. jobid.f85, jobid.words, jobid.dothex...
 
@@ -75,20 +75,20 @@
     @property
     def f58(self):
         """Return RFC19 F58 representation of a JobID"""
         return self.encode("f58")
 
     @property
     def hex(self):
-        """Return 0x-prefixed hexadecimal representation of a JobID"""
+        """Return 0x-prefixed hexidecimal representation of a JobID"""
         return self.encode("hex")
 
     @property
     def dothex(self):
-        """Return dotted hexadecimal representation of a JobID"""
+        """Return dotted hexidecimal representation of a JobID"""
         return self.encode("dothex")
 
     @property
     def words(self):
         """Return words (mnemonic) representation of a JobID"""
         return self.encode("words")
```

### Comparing `flux-python-0.50.0/flux/job/Jobspec.py` & `flux-python-0.50.0rc0/flux/job/Jobspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import json
 import math
 import numbers
 import os
 
 import yaml
 from _flux._core import ffi
-from flux import hostlist, idset
 from flux.util import parse_fsd, set_treedict
 
 
 def _convert_jobspec_arg_to_string(jobspec):
     """
     Convert a jobspec argument into a string.  A valid jobspec argument is:
     - An instance of the Jobspec class
@@ -79,22 +78,14 @@
         raise TypeError(f"argument to constraint {operator} must be a sequence")
     if operator in ["and", "or", "not"]:
         for constraint in args:
             _validate_constraint(constraint)
     elif operator in ["properties"]:
         for name in args:
             _validate_property_query(name)
-    elif operator in ["hostlist"]:
-        for hosts in args:
-            hostlist.decode(hosts)
-    elif operator in ["ranks"]:
-        for ranks in args:
-            idset.decode(ranks)
-    else:
-        raise TypeError(f"unknown constraint operator '{operator}'")
 
 
 def _validate_constraint(constraints):
     """Validate RFC 31 Constraint object"""
     if not isinstance(constraints, abc.Mapping):
         raise TypeError("constraints must be a mapping")
     for operator, arg in constraints.items():
@@ -864,97 +855,92 @@
         num_slots=1,
         cores_per_slot=1,
         gpus_per_slot=None,
         num_nodes=None,
         broker_opts=None,
         exclusive=False,
     ):
-        """
-        Create a Jobspec describing a nested Flux instance controlled by
-        a script.
+        """Create a Jobspec describing a nested Flux instance controlled by a script.
 
         The nested Flux instance will execute the script with the given
-        command-line arguments after copying it and setting the executable
-        bit.  Conceptually, this differs from the `from_nest_command`,
-        which also creates a nested Flux instance, in that it a) requires
-        the initial program of the new instance to be an executable text
-        file and b) creates the initial program from a string rather than
-        using an executable existing somewhere on the filesystem.
+        command-line arguments after copying it and setting the executable bit.
+        Conceptually, this differs from the `from_nest_command`, which also creates a
+        nested Flux instance, in that it a) requires the initial program of the new
+        instance to be an executable text file and b) creates the initial program
+        from a string rather than using an executable existing somewhere on the
+        filesystem.
 
         Use setters to assign additional properties.
 
-        Args:
-            script (str): contents of the script to execute, as a string. The
-                script should have a shebang (e.g. `#!/bin/sh`) at the top.
-            jobname (str): name to use for system.job.name attribute This will
-                be the default job name reported by Flux.
-            args (iterable of `str`): arguments to pass to `script`
-            num_slots (int): number of resource slots to create. Slots are an
-                abstraction, and are only used (along with `cores_per_slot`
-                and `gpus_per_slot`) to determine the nested instance's
-                allocation size and layout.
-            cores_per_slot (int): number of cores to allocate per slot
-            gpus_per_slot (int): number of GPUs to allocate per slot
-            num_nodes (int): distribute allocated resource slots across N
-                individual nodes
-            broker_opts (iterable of `str`): options to pass to the new Flux
-                broker
+        :param script: contents of the script to execute, as a string. The
+            script should have a shebang (e.g. `#!/bin/sh`) at the top.
+        :param jobname: name to use as the argv[0] for this job.
+            This will be the default job name reported by Flux.
+            (Note the actual argv is overridden by the job shell when executed.)
+        :type jobname: str
+        :param args: arguments to pass to `script`
+        :type args: iterable of `str`
+        :param num_slots: number of resource slots to create. Slots are an abstraction,
+            and are only used (along with `cores_per_slot` and `gpus_per_slot`) to
+            determine the nested instance's allocation size and layout.
+        :param cores_per_slot: number of cores to allocate per slot
+        :param gpus_per_slot: number of GPUs to allocate per slot
+        :param num_nodes: distribute allocated resource slots across N individual nodes
+        :param broker_opts: options to pass to the new Flux broker
+        :type broker_opts: iterable of str
         """
         if not script.startswith("#!"):
             raise ValueError(f"{jobname} does not appear to start with '#!'")
         args = () if args is None else args
-        jobspec = cls.from_nest_command(
-            command=["{{tmpdir}}/script", *args],
-            num_slots=num_slots,
-            cores_per_slot=cores_per_slot,
-            gpus_per_slot=gpus_per_slot,
+        jobspec = cls.from_command(
+            command=[jobname, *args],  # argv[0] will be replaced with the script
+            num_tasks=num_slots,
+            cores_per_task=cores_per_slot,
+            gpus_per_task=gpus_per_slot,
             num_nodes=num_nodes,
-            broker_opts=broker_opts,
             exclusive=exclusive,
         )
+        jobspec.setattr_shell_option("per-resource.type", "node")
+        jobspec.setattr_shell_option("mpi", "none")
         #  Copy script contents into jobspec
         jobspec.setattr("system.batch.script", script)
-        jobspec.setattr("system.job.name", jobname)
+        if broker_opts is not None:
+            jobspec.setattr("system.batch.broker-opts", broker_opts)
         return jobspec
 
     @classmethod
     def from_nest_command(
         cls,
         command,
         num_slots=1,
         cores_per_slot=1,
         gpus_per_slot=None,
         num_nodes=None,
         broker_opts=None,
         exclusive=False,
     ):
-        """
-        Create a Jobspec describing a nested Flux instance controlled by
-        `command`.
+        """Create a Jobspec describing a nested Flux instance controlled by `command`.
 
-        Conceptually, this differs from the `from_batch_command` method
-        in that a) the initial program of the nested Flux instance can
-        be any executable on the file system, not just a text file and b)
-        the executable is not copied at submission time.
+        Conceptually, this differs from the `from_batch_command` method in that a)
+        the initial program of the nested Flux instance can be any executable
+        on the file system, not just a text file and b) the executable is not
+        copied at submission time.
 
         Use setters to assign additional properties.
 
-        Args:
-            command (iterable of `str`): initial program for the nested Flux
-            instance
-            num_slots (int): number of resource slots to create. Slots are
-                an abstraction, and are only used (along with `cores_per_slot`
-                and `gpus_per_slot`) to determine the nested instance's
-                allocation size and layout.
-            cores_per_slot (int): number of cores to allocate per slot
-            gpus_per_slot (int): number of GPUs to allocate per slot
-            num_nodes (int): distribute allocated resource slots across N
-                individual nodes
-            broker_opts (iterable of `str`): options to pass to the new Flux
-                broker
+        :param command: initial program for the nested Flux instance
+        :type command: iterable of str
+        :param num_slots: number of resource slots to create. Slots are an abstraction,
+            and are only used (along with `cores_per_slot` and `gpus_per_slot`) to
+            determine the nested instance's allocation size and layout.
+        :param cores_per_slot: number of cores to allocate per slot
+        :param gpus_per_slot: number of GPUs to allocate per slot
+        :param num_nodes: distribute allocated resource slots across N individual nodes
+        :param broker_opts: options to pass to the new Flux broker
+        :type broker_opts: iterable of str
         """
         broker_opts = () if broker_opts is None else broker_opts
         jobspec = cls.from_command(
             command=["flux", "broker", *broker_opts, *command],
             num_tasks=num_slots,
             cores_per_task=cores_per_slot,
             gpus_per_task=gpus_per_slot,
```

### Comparing `flux-python-0.50.0/flux/job/__init__.py` & `flux-python-0.50.0rc0/flux/job/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,9 +25,8 @@
     JobException,
     MAIN_EVENTS,
 )
 from flux.job.executor import (
     FluxExecutor,
     FluxExecutorFuture,
 )
-from flux.job.timeleft import timeleft
 from flux.core.inner import ffi
```

### Comparing `flux-python-0.50.0/flux/job/_wrapper.py` & `flux-python-0.50.0rc0/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/event.py` & `flux-python-0.50.0rc0/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/executor.py` & `flux-python-0.50.0rc0/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/frobnicator/frobnicator.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,55 +21,39 @@
     def __init__(self, config={}):
         self.queues = {}
         try:
             self.queues = config["queues"]
         except KeyError:
             pass
 
-    def queue_properties(self, name):
+    def queue_constraints(self, name):
         try:
             return self.queues[name]["requires"]
         except KeyError:
             return None
 
     def apply_constraints(self, jobspec):
         """Apply queue-specific constraints to jobspec"""
 
         if jobspec.queue:
             if jobspec.queue not in self.queues:
                 raise ValueError(f"Invalid queue '{jobspec.queue}' specified")
-            queue_properties = self.queue_properties(jobspec.queue)
-            if queue_properties is None:
+            queue_constraints = self.queue_constraints(jobspec.queue)
+            if queue_constraints is None:
                 return
-
-            # First try appending to existing constraints
+            prop = []
             try:
-                spec = jobspec.attributes["system"]["constraints"]["properties"]
-                for prop in queue_properties:
-                    if prop not in spec:
-                        spec.append(prop)
-                return
+                prop = jobspec.attributes["system"]["constraints"]["properties"]
             except KeyError:
-                #  No "properties" operator at top level, try combining
-                #  existing constraints with logical AND
                 pass
-            try:
-                jobspec.setattr(
-                    "system.constraints",
-                    {
-                        "and": [
-                            jobspec.attributes["system"]["constraints"],
-                            {"properties": queue_properties},
-                        ]
-                    },
-                )
-            except KeyError:
-                #  No existing "constraints" - set constraints to queue
-                #  constraints
-                jobspec.setattr("system.constraints", {"properties": queue_properties})
+
+            for value in queue_constraints:
+                if value not in prop:
+                    prop.append(value)
+            jobspec.setattr("system.constraints.properties", prop)
 
 
 class Frobnicator(FrobnicatorPlugin):
     def __init__(self, parser):
         super().__init__(parser)
 
     def configure(self, args, config):
```

### Comparing `flux-python-0.50.0/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/info.py` & `flux-python-0.50.0rc0/flux/job/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 import json
 import os
 import pwd
 import string
 import sys
 import time
 from collections import namedtuple
-from itertools import chain
 
 import flux.constants
 from flux.core.inner import raw
 from flux.job.JobID import JobID
 from flux.job.stats import JobStats
 from flux.memoized_property import memoized_property
+from flux.resource import SchedResourceList
 from flux.uri import JobURI
 
-try:
-    from flux.resource import SchedResourceList
-except ImportError:
-    SchedResourceList = None
-
 
 def statetostr(stateid, fmt="L"):
     return raw.flux_job_statetostr(stateid, fmt).decode("utf-8")
 
 
 def statetoemoji(stateid):
     statestr = raw.flux_job_statetostr(stateid, "S").decode("utf-8")
@@ -212,15 +207,15 @@
         return str(self).__format__(fmt)
 
 
 class InstanceInfo:
     def __init__(self, uri=None):
         self.initialized = False
         try:
-            if not uri or SchedResourceList is None:
+            if not uri:
                 raise ValueError
             handle = flux.Flux(str(uri))
             future = handle.rpc("sched.resource-status")
             self.stats = StatsInfo(handle).update_sync()
             self.resources = SchedResourceList(future.get())
             self.initialized = True
             return
@@ -289,30 +284,14 @@
         "ranks": "",
         "nodelist": "",
         "success": "",
         "result": "",
         "waitstatus": "",
     }
 
-    #  Other properties (used in to_dict())
-    properties = (
-        "id",
-        "t_submit",
-        "t_remaining",
-        "state",
-        "result",
-        "username",
-        "userid",
-        "urgency",
-        "runtime",
-        "status",
-        "returncode",
-        "dependencies",
-    )
-
     def __init__(self, info_resp):
         #  Set defaults, then update with job-list.list response items:
         combined_dict = self.defaults.copy()
         combined_dict.update(info_resp)
 
         #  Cast jobid to JobID
         combined_dict["id"] = JobID(combined_dict["id"])
@@ -490,60 +469,14 @@
         Return job duration if job is not running, otherwise runtime
         """
         state = str(self.state)
         if state in ["PRIORITY", "DEPEND", "SCHED"]:
             return self.duration
         return self.runtime
 
-    def to_dict(self, filtered=True):
-        """
-        Return a set of job attributes as a dict
-        By default, empty or unset values are filtered from the result,
-        so these keys will be missing. Set ``filtered=False`` to get the
-        unfiltered dict, which has these uninitialized values set to
-        an empty string or 0, key dependent.
-        """
-        result = {}
-        for attr in chain(self.defaults.keys(), self.properties):
-            val = getattr(self, attr)
-            if val is not None:
-                result[attr] = val
-
-        #  The following attributes all need special handling to
-        #  be converted to a dict:
-        result["annotations"] = self.annotations.annotationsDict
-        result["exception"] = self.exception.__dict__
-        if self.uri is not None:
-            result["uri"] = str(self.uri)
-
-        if not filtered:
-            return result
-
-        #  Now clear empty/unset values to avoid confusion:
-        #  - Remove any empty values (empty string).
-        #  - Remove any unset timestamp values (key t_*, value 0)
-        #  - Remove runtime and expiration if 0
-        def zero_remove(key):
-            return key.startswith("t_") or key in ("runtime", "expiration")
-
-        for key in list(result.keys()):
-            val = result[key]
-            if val == "" or (zero_remove(key) and val == 0):
-                del result[key]
-            if key == "exception" and not val["occurred"]:
-                result["exception"] = {"occurred": False}
-
-        #  Remove duplicate annotations.user.uri if necessary:
-        if self.uri is not None:
-            del result["annotations"]["user"]["uri"]
-            if not result["annotations"]["user"]:
-                del result["annotations"]["user"]
-
-        return result
-
 
 def job_fields_to_attrs(fields):
     # Note there is no attr for "id", it is always returned
     fields2attrs = {
         "id": (),
         "id.dec": (),
         "id.hex": (),
```

### Comparing `flux-python-0.50.0/flux/job/kill.py` & `flux-python-0.50.0rc0/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/kvs.py` & `flux-python-0.50.0rc0/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/list.py` & `flux-python-0.50.0rc0/flux/job/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ###############################################################
 import errno
 import os
 import pwd
 
 import flux.constants
 from flux.future import WaitAllFuture
-from flux.job.info import JobInfo
+from flux.job.info import JobInfo, statetostr
 from flux.rpc import RPC
 
 
 class JobListRPC(RPC):
     def get_jobs(self):
         return self.get()["jobs"]
 
@@ -108,21 +108,38 @@
     t_submit, t_depend, (and others when finished), state, name,
     ntasks, ncores, duration, nnodes, result, runtime, returncode,
     waitstatus, nodelist, and exception type, severity, and note.
     """
     payload = {"id": int(jobid), "attrs": ["all"]}
     rpc = JobListIdRPC(flux_handle, "job-list.list-id", payload)
     try:
-        jobinfo = rpc.get_jobinfo()
+        jobinfo = rpc.get()
 
     # The job does not exist!
     except FileNotFoundError:
         return None
 
-    return jobinfo.to_dict(filtered=False)
+    jobinfo = jobinfo["job"]
+
+    # User friendly string from integer
+    state = jobinfo["state"]
+    jobinfo["state"] = statetostr(state)
+
+    # Get job info to add to result
+    info = rpc.get_jobinfo()
+    jobinfo["nnodes"] = info._nnodes
+    jobinfo["result"] = info.result
+    jobinfo["returncode"] = info.returncode
+    jobinfo["runtime"] = info.runtime
+    jobinfo["priority"] = info._priority
+    jobinfo["waitstatus"] = info._waitstatus
+    jobinfo["nodelist"] = info._nodelist
+    jobinfo["nodelist"] = info._nodelist
+    jobinfo["exception"] = info._exception.__dict__
+    return jobinfo
 
 
 class JobListIdsFuture(WaitAllFuture):
     """Simulate interface of JobListRPC for listing multiple jobids"""
 
     def __init__(self):
         super(JobListIdsFuture, self).__init__()
```

### Comparing `flux-python-0.50.0/flux/job/stats.py` & `flux-python-0.50.0rc0/flux/job/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,20 +74,14 @@
 
         #  Compute some stats for convenience:
         #  pylint: disable=attribute-defined-outside-init
         self.pending = self.depend + self.priority + self.sched
         self.running = self.run + self.cleanup
         self.active = self.total - self.inactive
 
-        # This class reports the total number of unsuccessful jobs in
-        # the 'failed' attribute, not just the count of jobs that ran
-        # to completion with nonzero exit code
-        self.failed += self.timeout
-        self.failed += self.canceled
-
         if self.callback:
             self.callback(self, **self.cb_kwargs)
 
     def _query(self):
         return RPC(self.handle, "job-list.job-stats", {})
 
     def update(self, callback=None, **kwargs):
```

### Comparing `flux-python-0.50.0/flux/job/submit.py` & `flux-python-0.50.0rc0/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/validator/plugins/feasibility.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/validator/plugins/jobspec.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/validator/plugins/require-instance.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/validator/plugins/schema.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/schema.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/job/validator/validator.py` & `flux-python-0.50.0rc0/flux/job/validator/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return json.dumps(result)
 
     def push_result(self, errnum, errmsg=None):
         """Add a result from one validator to a ValidatorResult
 
         Args:
             errnum (:obj:`int`): error number (0 for success)
-            errmsg (:obj:`str`, optional): An optional error message for a
+            errmsg (:obj:`str`, optional): An optional error messsage for a
                 failed result.
         """
         if errnum > self.errnum:
             self.errnum = errnum
         if errmsg and errmsg not in self.errmsgs:
             self.errmsgs.append(errmsg)
 
@@ -87,15 +87,15 @@
             return self.jobinfo[attr]
 
 
 class ValidatorPlugin(ABC):  # pragma: no cover
     """Base class for Validator Plugins"""
 
     def __init__(self, parser):
-        """Initialize a ValidatorPlugin"""
+        """Intialize a ValidatorPlugin"""
 
     def configure(self, args):
         """Configure a ValidatorPlugin. Run after argparse.parse_args()
 
         Args:
             args (:obj:`Namespace`): The resulting Namespace after calling
             argparse.parse_args()
@@ -123,15 +123,15 @@
         raise NotImplementedError
 
 
 # pylint: disable=too-many-instance-attributes
 class JobValidator:
     """A plugin-based job validator class
 
-    JobValidator loads plugins that implement the ValidatorPlugin interface
+    JobValidator loads plugins that implenment the ValidatorPlugin interface
     from the 'flux.job.validator.plugins' namespace. Plugins may be configured
     at runtime by passing in a ``--plugins=LIST`` option
 
     """
 
     default_validators = ["jobspec"]
     plugin_namespace = "flux.job.validator.plugins"
```

### Comparing `flux-python-0.50.0/flux/job/wait.py` & `flux-python-0.50.0rc0/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/kvs.py` & `flux-python-0.50.0rc0/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/memoized_property.py` & `flux-python-0.50.0rc0/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/message.py` & `flux-python-0.50.0rc0/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/progress.py` & `flux-python-0.50.0rc0/flux/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 
 class ElapsedTime(float):
     """
     An ElapsedTime object is a floating point elapsed time in seconds
-    that comes with a convenient "dt" property that returns a
+    that comes with a convenient "dt" proerty that returns a
     datetime.timedelta object
     """
 
     @property
     # pylint: disable=invalid-name
     def dt(self):
         return datetime.timedelta(seconds=round(self))
@@ -55,15 +55,15 @@
 class Bottombar:
     """Maintain a status line at bottom of terminal using vt100 escape codes
 
     The Bottombar class implements a very simple status line which stays
     positioned at the last line of vt100 capable terminals through the
     use of vt100 escape codes.
 
-    This class will only work properly on vt100 compatible terminals, which
+    This class will only work propertly on vt100 compatible terminals, which
     includes xterm, rxvt, and gnome-terminal and their derivatives on Linux,
     as well as iTerm and Terminal on OSX, and reportedly the new Windows
     Terminal on Windows.
 
     Use of Bottombar requires that a ``formatter`` function be provided.
     The ``formatter`` will be called on each update as::
```

### Comparing `flux-python-0.50.0/flux/resource/ResourceSet.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/resource/ResourceSetImplementation.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/resource/Rlist.py` & `flux-python-0.50.0rc0/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/resource/__init__.py` & `flux-python-0.50.0rc0/flux/resource/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,7 @@
 #
 # SPDX-License-Identifier: LGPL-3.0
 ###############################################################
 
 from flux.resource.Rlist import Rlist
 from flux.resource.ResourceSet import ResourceSet
 from flux.resource.list import resource_list, SchedResourceList
-from flux.resource.status import resource_status, ResourceStatus
```

### Comparing `flux-python-0.50.0/flux/resource/list.py` & `flux-python-0.50.0rc0/flux/resource/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/rpc.py` & `flux-python-0.50.0rc0/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/security.py` & `flux-python-0.50.0rc0/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/uri/resolvers/jobid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/jobid.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """A URI resolver that attempts to fetch the remote_uri for a job"""
 
     def describe(self):
         return "Get URI for a given Flux JOBID"
 
     def _do_resolve(self, uri, flux_handle, force_local=False):
         #
-        #  Convert a possible hierarchy of jobids to a list, dropping any
+        #  Convert a possible hiearchy of jobids to a list, dropping any
         #   extraneous '/' (e.g. //id0/id1 -> [ "id0", "id1" ]
         jobids = filter_slash(PurePath(uri.path).parts)
 
         #  Pop the first jobid off the list, this id should be local:
         arg = jobids.pop(0)
         try:
             jobid = JobID(arg)
```

### Comparing `flux-python-0.50.0/flux/uri/resolvers/lsf.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/uri/resolvers/pid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/pid.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     #  (PID of broker child is likely close to broker_pid)
     pids.sort(key=lambda pid: abs(pid - broker_pid))
 
     #  Remove broker_pid since it definitely isn't a child
     pids.remove(broker_pid)
 
     #  Now iterate all processes, returning immediately when
-    #   we've found a process for which broker_pid is the parent
+    #   we've found a proces for which broker_pid is the parent
     for pid in pids:
         try:
             with open(f"/proc/{pid}/stat") as statf:
                 data = statf.read()
         except OSError:
             #  /proc/PID/stat is readable by all, but there is a chance
             #  of a TOU-TOC race here, so just ignore all errors
```

### Comparing `flux-python-0.50.0/flux/uri/resolvers/slurm.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/uri/uri.py` & `flux-python-0.50.0rc0/flux/uri/uri.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 
 class URIResolverURI(URI):
     """A URI which resolves to a JobURI
 
     A URI used with ``FluxURIResolver.resolve``.
     Includes a workaround for ``urllib.parse.urlparse`` problems parsing
-    path components with only digits.
+    path componenets with only digits.
     """
 
     def __init__(self, uri):
         #  Replace : with :FXX to allow path to be digits only
         super().__init__(uri.replace(":", ":FXX", 1))
         self.path = self.path.replace("FXX", "", 1)
 
@@ -186,15 +186,15 @@
 
         query = resolver_uri.query_dict
         if "local" in query and "remote" in query:
             raise ValueError("Only one of 'local' or 'remote' is allowed")
 
         result = JobURI(self.resolvers[scheme].resolve(resolver_uri))
 
-        #  Special case for 'local' or 'remote' query parameters:
+        #  Special case for 'local' or 'remote' query paramters:
         if "local" in query:
             result = JobURI(result.local)
         elif "remote" in query:
             result = JobURI(result.remote)
         return result
 
     def plugins(self):
```

### Comparing `flux-python-0.50.0/flux/util.py` & `flux-python-0.50.0rc0/flux/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
             opts = list(action.option_strings)
 
             #  Default optstring is `-l, --long-opt`
             optstring = ", ".join(opts)
 
             #  If only a long option is supported, then prefix with
-            #   whitespace by the width of a short option so that all
+            #   whitepsace by the width of a short option so that all
             #   long opts start in the same column:
             if len(opts) == 1 and len(opts[0]) > 2:
                 optstring = "    " + opts[0]
 
             #  We're done if no argument supported
             if action.nargs == 0:
                 return optstring
@@ -214,21 +214,15 @@
         exit_code = 0
         try:
             main_func()
         except SystemExit as ex:  # don't intercept sys.exit calls
             exit_code = ex
         except Exception as ex:  # pylint: disable=broad-except
             exit_code = 1
-            # Prefer '{strerror}: {filename}' error message over default
-            # OSError string representation which includes useless
-            # `[Error N]` prefix in output.
-            errmsg = getattr(ex, "strerror", None) or str(ex)
-            if getattr(ex, "filename", None):
-                errmsg += f": '{ex.filename}'"
-            self.logger.error(errmsg)
+            self.logger.error(str(ex))
             self.logger.debug(traceback.format_exc())
         finally:
             logging.shutdown()
             sys.exit(exit_code)
 
 
 def parse_fsd(fsd_string):
@@ -306,34 +300,29 @@
     two colons `::` before the Python format spec, e.g::
 
     >>> "{0:%b%d %R::>16}".format(UtilDatetime.now())
     '     Sep21 18:36'
     """
 
     def __format__(self, fmt):
-        # The string "::" is used to split the strftime() format from
+        # The string "::" is used to split the strftime() fromat from
         # any Python format spec:
         vals = fmt.split("::", 1)
 
         # Call strftime() to get the formatted datetime as a string
         result = self.strftime(vals[0])
 
         # If there was a format spec, apply it here:
         try:
             return f"{{0:{vals[1]}}}".format(result)
         except IndexError:
             return result
 
 
 def fsd(secs):
-    # Special case for RFC 23 "infinity"
-    # N.B. We return lower case "inf" to match Python's "math.inf".
-    if math.isinf(secs):
-        return "inf"
-
     #  Round <1ms down to 0s for now
     if secs < 1.0e-3:
         strtmp = "0s"
     elif secs < 10.0:
         strtmp = "%.03fs" % secs
     elif secs < 60.0:
         strtmp = "%.4gs" % secs
@@ -418,16 +407,15 @@
 
         denote_truncation = False
         if spec.endswith("+"):
             denote_truncation = True
             spec = spec[:-1]
 
         if spec.endswith("h"):
-            localepoch = datetime.fromtimestamp(0.0).strftime("%FT%T")
-            basecases = ("", "0s", "0.0", "0:00:00", "1970-01-01T00:00:00", localepoch)
+            basecases = ("", "0s", "0.0", "0:00:00", "1970-01-01T00:00:00")
             value = "-" if str(value) in basecases else str(value)
             spec = spec[:-1] + "s"
         retval = super().format_field(value, spec)
 
         if denote_truncation and len(retval) < len(str(value)):
             retval = retval[:-1] + "+"
 
@@ -536,54 +524,35 @@
         fmt = "".join(format_list)
         return fmt
 
     def header(self):
         formatter = self.HeaderFormatter()
         return formatter.format(self.header_format(), **self.headings)
 
-    def get_format_prepended(self, prepend, except_fields=None):
+    def get_format_prepended(self, prepend):
         """
         Return the format string, ensuring that the string in "prepend"
         is prepended to each format field
         """
-        if except_fields is None:
-            except_fields = []
         lst = []
         for (text, field, spec, conv) in self.format_list:
-            # Skip this field if it is in except_fields
-            if field in except_fields:
-                # Preserve any format "prefix" (i.e. the text):
-                lst.append(text)
-                continue
             # If field doesn't have 'prepend' then add it
             if field and not field.startswith(prepend):
                 field = prepend + field
             lst.append(self._fmt_tuple(text, field, spec, conv))
         return "".join(lst)
 
     def get_format(self, orig=False):
         """
         Return the format string
         """
         if orig:
             return self.fmt_orig
         return self.fmt
 
-    def copy(self, except_fields=None):
-        """
-        Return a copy of the current formatter, optionally with some
-        fields removed
-        """
-        cls = self.__class__
-        return cls(
-            self.get_format_prepended("", except_fields),
-            headings=self.headings,
-            prepend=self.prepend,
-        )
-
     def format(self, obj):
         """
         format object with internal format
         """
         try:
             retval = self.formatter().format(self.get_format(), obj)
         except KeyError as exc:
@@ -591,16 +560,15 @@
             raise KeyError(f"Invalid format field {exc} for {typestr}")
         return retval
 
     def filter_empty(self, items):
         """
         Check for format fields that are prefixed with `?:` (e.g. "?:{name}")
         and filter them out of the current format string if they result in an
-        empty value (as defined by the `empty` tuple defined below) for every
-        entry in `items`.
+        empty string for every entry in `items`.
         """
         #  Build a list of all format strings that have the collapsible
         #  sentinel '?:' to determine which are subject to the test for
         #  emptiness.
         #
         #  Note: we remove the leading `text` and the format `spec` because
         #  these may make even empty formatted fields non-empty. E.g. a spec
@@ -617,33 +585,32 @@
         # Return immediately if no format fields are collapsible
         if not lst:
             return self.get_format(orig=True)
 
         formatter = self.formatter()
 
         #  Iterate over all items, rebuilding lst each time to contain
-        #  only those fields that resulted in non-"empty" strings:
-        empty = ("", "0", "0s", "0.0", "0:00:00", "1970-01-01T00:00:00")
+        #  only those fields that resulted in nonzero strings:
         for item in items:
-            lst = [x for x in lst if formatter.format(x["fmt"], item) in empty]
+            lst = [x for x in lst if not formatter.format(x["fmt"], item)]
 
             #  If lst is now empty, that means all fields already returned
             #  nonzero strings, so we can break early
             if not lst:
                 break
 
         #  Remove any entries that were empty from self.format_list
-        #  (use index field of lst to remove by position in self.format_list)
+        #  (use index field of lst to remove by postition in self.format_list)
         format_list = [
             x
             for i, x in enumerate(self.format_list)
             if i not in [x["index"] for x in lst]
         ]
 
-        #  Remove "?:" from remaining entries so they disappear in output.
+        #  Remove "?:" from remaining entries so they disappear in ouput.
         for entry in format_list:
             if entry[0].endswith("?:"):
                 entry[0] = entry[0][:-2]
 
         #  Return new format string created from pruned format_list
         return "".join(self._fmt_tuple(*x) for x in format_list)
 
@@ -673,73 +640,22 @@
         formatter = cls(newfmt, headings=self.headings, prepend=self.prepend)
         if not no_header:
             print(formatter.header())
         for item in items:
             if callable(pre):
                 pre(item)
             line = formatter.format(item)
-            if not line:
-                continue
             try:
                 print(line)
             except UnicodeEncodeError:
                 print(line.encode("utf-8", errors="surrogateescape").decode())
             if callable(post):
                 post(item)
 
 
-class Deduplicator:
-    """
-    Generic helper to deduplicate a list of formatted items for objects
-    that can be aggregated.
-
-    Args:
-        formatter (OutputFormat): Formatter instance to use for deduplication
-        except_fields (list): List of fields to not consider when merging
-            like lines. These are typically fields that can be combined, such
-            as a node count, node list, ranks, etc.
-        combine (callable): A function that is used to combine matching
-            items, called as combine(existing, new).
-    """
-
-    def __init__(self, formatter, except_fields=None, combine=None):
-        self.formatter = formatter.copy(except_fields=except_fields)
-        self.combine = combine
-        self.hash = {}
-        self.items = []
-        #  Allow class to be iterable https://stackoverflow.com/a/48670014
-        self.__iter = None
-
-    def __iter__(self):
-        if self.__iter is None:
-            self.__iter = iter(self.items)
-        return self
-
-    def __next__(self):
-        try:
-            return next(self.__iter)
-        except StopIteration:  # support repeated iteration
-            self.__iter = None
-            raise
-
-    def append(self, item):
-        """
-        Append a new item to a deduplicator. Combines item with an existing
-        entry if the formatted result is identical to another entry.
-        """
-        key = self.formatter.format(item)
-        try:
-            result = self.hash[key]
-            if self.combine is not None:
-                self.combine(result, item)
-        except KeyError:
-            self.hash[key] = item
-            self.items.append(item)
-
-
 class Tree:
     """Very simple pstree-like display for the console
 
     Args:
         label: Label for this node
         prefix: Text which comes before connector and label
         combine_children: combine like children as they are added
@@ -971,35 +887,31 @@
     in that order.
 
     Config files are loaded from <name>.<ext>, where ext can be one
     of json, yaml, or toml. If multiple files exist they are processed
     in glob(3) order.
 
     Args:
-        name: config name, used as the stem of config file to load
-              this is typically the name of the tool
-        toolname (optional): actual name of the tool/utility if "name" is
-                             different.  used in environment variable lookup.
+        name: name of utility, used as the stem of config file to load
         subcommand (optional): name of subcommand. Used as name of subtable
                                in configuration to use.
         initial_dict: Set of default values (optional)
 
     """
 
     extension_handlers = {
         ".toml": tomllib.load,
         ".json": json.load,
         ".yaml": yaml.safe_load,
     }
 
     builtin_formats = {}
 
-    def __init__(self, name, toolname=None, subcommand=None, initial_dict=None):
+    def __init__(self, name, subcommand=None, initial_dict=None):
         self.name = name
-        self.toolname = toolname
         self.dict = {}
         if initial_dict:
             self.dict = copy.deepcopy(initial_dict)
         self.config = self.dict
 
         #  If not None,  use subcommand config in subtable = 'subtable'
         self.subtable = subcommand
@@ -1105,24 +1017,14 @@
     def validate(self, path, conf):
         """
         Validate config file as it is loaded before merging it with the
         configuration. This function does nothing in the base class, but
         subclasses may define it to implement higher level validation.
         """
 
-    def _default_env_name(self):
-        """
-        Get tool default environment variable (name upper case, s/-/_/g)
-        """
-        name = self.toolname if self.toolname else self.name
-        prefix = name.upper().replace("-", "_")
-        if self.subtable:
-            prefix += "_" + self.subtable.upper().replace("-", "_")
-        return prefix + "_FORMAT_DEFAULT"
-
     def get_format_string(self, format_name):
         """
         Convenience function to fetch a format string from the current
         config. Assumes the current config has been loaded and contains
         a "formats" table.
 
         Special format names:
@@ -1155,24 +1057,14 @@
                 print(f"[{self.subtable}.formats.{name}]")
             else:
                 print(f"[formats.{name}]")
             if "description" in entry:
                 print(f"description = \"{entry['description']}\"")
             print(f"format = \"{entry['format']}\"")
             sys.exit(0)
-        elif format_name == "default":
-            # Default can be overridden by environment variable
-            try:
-                format_name = os.environ[self._default_env_name()]
-                if "{" in format_name:
-                    return format_name
-            except KeyError:
-                # no environment var, fallthrough
-                pass
-
         try:
             return formats[format_name]["format"]
         except KeyError:
             raise ValueError(f"--format: No such format {format_name}")
 
     def __getattr__(self, attr):
         return self.config[attr]
```

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/context.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/tomli/LICENSE` & `flux-python-0.50.0rc0/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/tomli/_parser.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/utils/tomli/_re.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/flux/wrapper.py` & `flux-python-0.50.0rc0/flux/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 class MissingFunctionError(Exception):
     def __init__(self, name, c_name, name_list, arguments):
 
         call_stack = inspect.stack()
         caller = inspect.getframeinfo(call_stack[2][0])
 
         message = """
-A non-existent or unavailable function invocation has been detected.
+A non-existant or unavailable function invocation has been detected.
 Has this function been recently removed or renamed?
 
 Name called: {name}
 Possible C names: {name_list}
 Arguments: {arguments}
-Likely intended C invocation: {c_name}{arguments}
+Likely intended C invokation: {c_name}{arguments}
 Invocation detail: inside function {outer}
 {file}:{line}: {context}
         """.format(
             name=name,
             name_list=name_list,
             arguments=arguments,
             file=caller.filename,
```

### Comparing `flux-python-0.50.0/flux_python.egg-info/SOURCES.txt` & `flux-python-0.50.0rc0/flux_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-LICENSE
 MANIFEST.in
-NOTICE.LLNS
 README.md
 setup.py
 flux/.gitignore
-flux/Makefile.am
+flux/Makefile
+flux/Makefile.in
 flux/__init__.py
 flux/constants.py
 flux/debugged.py
 flux/future.py
 flux/hostlist.py
 flux/idset.py
 flux/importer.py
@@ -16,43 +15,34 @@
 flux/memoized_property.py
 flux/message.py
 flux/progress.py
 flux/rpc.py
 flux/security.py
 flux/util.py
 flux/wrapper.py
-flux/cli/__init__.py
-flux/cli/alloc.py
-flux/cli/base.py
-flux/cli/batch.py
-flux/cli/bulksubmit.py
-flux/cli/fortune.py
-flux/cli/run.py
-flux/cli/submit.py
-flux/constraint/__init__.py
-flux/constraint/parser.py
+flux/cli/_fortune.py
+flux/constraint/parser.out
+flux/constraint/parsetab.py
 flux/core/__init__.py
 flux/core/handle.py
 flux/core/inner.py
 flux/core/trampoline.py
 flux/core/watchers.py
 flux/job/JobID.py
 flux/job/Jobspec.py
 flux/job/__init__.py
 flux/job/_wrapper.py
-flux/job/directives.py
 flux/job/event.py
 flux/job/executor.py
 flux/job/info.py
 flux/job/kill.py
 flux/job/kvs.py
 flux/job/list.py
 flux/job/stats.py
 flux/job/submit.py
-flux/job/timeleft.py
 flux/job/wait.py
 flux/job/frobnicator/__init__.py
 flux/job/frobnicator/frobnicator.py
 flux/job/frobnicator/plugins/constraints.py
 flux/job/frobnicator/plugins/defaults.py
 flux/job/validator/__init__.py
 flux/job/validator/validator.py
@@ -61,15 +51,14 @@
 flux/job/validator/plugins/require-instance.py
 flux/job/validator/plugins/schema.py
 flux/resource/ResourceSet.py
 flux/resource/ResourceSetImplementation.py
 flux/resource/Rlist.py
 flux/resource/__init__.py
 flux/resource/list.py
-flux/resource/status.py
 flux/uri/__init__.py
 flux/uri/uri.py
 flux/uri/resolvers/jobid.py
 flux/uri/resolvers/lsf.py
 flux/uri/resolvers/pid.py
 flux/uri/resolvers/slurm.py
 flux/utils/README.md
@@ -107,12 +96,14 @@
 src/_hostlist_build.py
 src/_hostlist_clean.h
 src/_hostlist_preproc.h
 src/_idset_build.py
 src/_idset_clean.h
 src/_idset_preproc.h
 src/_rlist_build.py
+src/_rlist_clean.h
+src/_rlist_preproc.h
 src/_security_build.py
 src/_security_clean.h
 src/_security_preproc.h
 src/callbacks.h
 src/make_clean_header.py
```

### Comparing `flux-python-0.50.0/setup.py` & `flux-python-0.50.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,58 +21,55 @@
 
 from setuptools import find_packages
 from setuptools import setup as _setup
 from distutils.core import setup, Command
 
 # Metadata
 package_name = "flux-python"
-package_version = "0.50.0"
+package_version = "0.50.0-rc0"
 package_description = "Python bindings for the flux resource manager API"
 package_url = "https://github.com/flux-framework/flux-python"
-package_keywords = "flux, job manager, workload manager, orchestration, hpc"
+package_keywords = "flux, job manager, orchestration, hpc"
 
 try:
     with open("README.md") as filey:
         package_long_description = filey.read()
 except Exception:
     package_long_description = package_description
 
 # Setup variables for dependencies
 cffi_dep = "cffi>=1.1"
 
 # src/bindings/python
 root = os.path.dirname(os.path.abspath(__file__))
 source = os.path.join(root, "src")
 
-
 def find_flux():
     """
     Find flux install via the executable!
     """
-    path = shutil.which("flux")
+    path = shutil.which('flux')
     if not path:
-        sys.exit(
-            "Cannot find executable flux, which is required to be on PATH to find the install location."
-        )
+        sys.exit('Cannot find executable flux, which is required to be on PATH to find the install location.')
     # /usr/local/bin/flux --> /usr/local
     return os.path.dirname(os.path.dirname(path))
 
-
 flux_root = find_flux()
 
 # Module specific default options files. Format strings below will be populated
 # after receiving the custom varibles from the user
 options = {
     "core": {
         "header": "include/flux/core.h",
-        "additional_headers": [os.path.join(source, "callbacks.h")],
+        "additional_headers": [os.path.join(source, "callbacks.h")]
     },
     "hostlist": {
         "header": "include/flux/hostlist.h",
     },
+
     # Note that rlist is currently disabled, so this
     # set of metadata doesn't matter
     "rlist": {
         "header": "include/flux/rlist.h",
         "ignore_headers": ["czmq_containers"],
     },
     "idset": {
@@ -87,15 +84,14 @@
 
 # Global variables for build type, corresponds to
 build_types = {"core", "idset", "security", "hostlist"}
 
 # rlist.h is disabled for now, as it requires the flux-core build
 # build_types = {"core", "idset", "rlist", "security", "hostlist"}
 
-
 @contextmanager
 def workdir(dirname):
     """
     Allow a temporary working directory to run commands
     """
     original = os.getcwd()
     os.chdir(dirname)
@@ -161,14 +157,15 @@
         value = getattr(self, attr, None)
         if value:
             value = value.split(",")
         elif not value:
             value = []
         setattr(self, attr, value)
 
+
     def run(self):
         """
         Run the install
         """
         for build_type in build_types:
             cleaner = HeaderCleaner(
                 self.flux_root,
@@ -195,19 +192,15 @@
         self.preproc_output = os.path.join(source, "_%s_preproc.h" % build_type)
         self.output = os.path.join(source, "_%s_clean.h" % build_type)
 
         # Relative path to header is required
         self.header = kwargs["header"]
 
         # Update search to include defaults
-        custom_search = [
-            os.path.join(self.root, "include"),
-            os.path.join(self.root, "lib"),
-            os.path.join(self.root, "include", "flux"),
-        ]
+        custom_search = [os.path.join(self.root, "include"), os.path.join(self.root, "lib"), os.path.join(self.root, "include", "flux")]
         self.search = custom_search + [
             x.format(root=root) for x in kwargs.get("search", [])
         ]
 
         # Not required
         self.additional_headers = kwargs.get("additional_headers", [])
         self.ignore_headers = kwargs.get("ignore_headers", [])
@@ -257,22 +250,22 @@
         """
         Compile with gcc -E '-D__attribute__(...)=' etc.
         """
         gcc = shutil.which("gcc")
         if not gcc:
             sys.exit("Cannot find gcc compiler.")
         cmd = [
-            gcc,
-            "-E",
-            "-D __attribute__(...)=",
-            "-DFLUX_DEPRECATED(...)=",
-            self.output,
-            "-o",
-            self.preproc_output,
-        ]
+              gcc,
+              "-E",
+              "-D __attribute__(...)=",
+              '-DFLUX_DEPRECATED(...)=',
+              self.output,
+              "-o",
+              self.preproc_output,
+          ]
         print(" ".join(cmd))
         res = subprocess.call(cmd)
         if res != 0:
             sys.exit("Issue preprocessing header to %s" % self.preproc_output)
 
     def clean_compiler_directives(self):
         """
@@ -320,35 +313,35 @@
                     self.process_header(nf, os.path.dirname(os.path.abspath(nf)))
                 if not re.match("#\s*include", l):
                     self.mega_header += l
 
         # Flag as checked
         self.checked_heads[f] = 1
 
-
 def setup():
     """
     A wrapper to run setup. This likely isn't best practice, but is a first effort.
     """
     global flux_root
     global security_include
 
     # Always set the install root to the environment
     set_envar("FLUX_INSTALL_ROOT", flux_root)
 
     # The flux security path should be in the same root, under includes
     security_include = os.path.join(flux_root, "include", "flux", "security")
     if not os.path.exists(security_include):
-        sys.exit(f"Cannot find flux security under expected path {security_include}")
+        sys.exit(f'Cannot find flux security under expected path {security_include}')
 
-    # We only want this to run on creating the tarball or install
+    # We only want this to run on creating the tarball
     command = sys.argv[1]
-    print(f"Command is {command}")
-    prepare = PrepareFluxHeaders(flux_root)
-    prepare.run()
+    if command in ["sdist", "build", "build_ext"]:
+        # Custom setup commands, first without cffi to prepare headers
+        prepare = PrepareFluxHeaders(flux_root)
+        prepare.run()
 
     # Request to install additional modules (we always do core0
     # We also have to remove the setup.py flags that aren't known
     cffi_modules = ["src/_core_build.py:ffi"]
     for build_type in build_types:
         # We always include / require core (may not be necessary)
         if build_type == "core":
@@ -367,15 +360,15 @@
         long_description_content_type="text/markdown",
         keywords=package_keywords,
         url=package_url,
         setup_requires=[cffi_dep],
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
-        install_requires=[cffi_dep, "pyyaml"],
+        install_requires=[cffi_dep],
         extras_require={
             "dev": ["pyyaml", "jsonschema", "docutils", "black", "IPython"]
         },
         classifiers=[
             "Intended Audience :: Science/Research",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
```

### Comparing `flux-python-0.50.0/src/_core_build.py` & `flux-python-0.50.0rc0/src/_core_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_core_clean.h` & `flux-python-0.50.0rc0/src/_core_clean.h`

 * *Files 0% similar despite different names*

```diff
@@ -2147,17 +2147,17 @@
 
 /* Flux uses semantic versioning: <major>.<minor>.<patch>
  */
 
 /* The VERSION_STRING may include a "-N-hash" suffix from git describe
  * if this snapshot is not tagged.  This is not reflected in VERSION_PATCH.
  */
-#define FLUX_CORE_VERSION_STRING    "0.50.0"
+#define FLUX_CORE_VERSION_STRING    "0.48.0"
 #define FLUX_CORE_VERSION_MAJOR     0
-#define FLUX_CORE_VERSION_MINOR     50
+#define FLUX_CORE_VERSION_MINOR     48
 #define FLUX_CORE_VERSION_PATCH     0
 
 /* The version in 3 bytes, for numeric comparison.
  */
 #define FLUX_CORE_VERSION_HEX       ((FLUX_CORE_VERSION_MAJOR << 16) | \
                                      (FLUX_CORE_VERSION_MINOR << 8) | \
                                      (FLUX_CORE_VERSION_PATCH << 0))
```

### Comparing `flux-python-0.50.0/src/_hostlist_build.py` & `flux-python-0.50.0rc0/src/_hostlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_hostlist_clean.h` & `flux-python-0.50.0rc0/src/_hostlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_hostlist_preproc.h` & `flux-python-0.50.0rc0/src/_hostlist_preproc.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# 0 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
-# 0 "<built-in>"
-# 0 "<command-line>"
+# 1 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 1 "<built-in>"
+# 1 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
-# 0 "<command-line>" 2
-# 1 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
-# 20 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 1 "<command-line>" 2
+# 1 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 20 "/workspaces/flux-python/src/_hostlist_clean.h"
 struct hostlist *hostlist_create (void);
 
 void hostlist_destroy (struct hostlist *hl);
 
 
 
 
@@ -40,15 +40,15 @@
 int hostlist_append_list (struct hostlist *hl1, struct hostlist *hl2);
 
 
 
 
 
 const char * hostlist_nth (struct hostlist * hl, int n);
-# 68 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 68 "/workspaces/flux-python/src/_hostlist_clean.h"
 int hostlist_find (struct hostlist * hl, const char *hostname);
 
 
 
 
 
 
@@ -67,21 +67,21 @@
 
 void hostlist_sort (struct hostlist * hl);
 
 
 
 
 void hostlist_uniq (struct hostlist *hl);
-# 103 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 103 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_first (struct hostlist *hl);
-# 113 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 113 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_last (struct hostlist *hl);
-# 123 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 123 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_next (struct hostlist *hl);
-# 132 "/home/runner/work/flux-python/flux-python/src/_hostlist_clean.h"
+# 132 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_current (struct hostlist *hl);
 
 
 
 
 
 int hostlist_remove_current (struct hostlist *hl);
```

### Comparing `flux-python-0.50.0/src/_idset_build.py` & `flux-python-0.50.0rc0/src/_idset_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_idset_clean.h` & `flux-python-0.50.0rc0/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_rlist_build.py` & `flux-python-0.50.0rc0/src/_rlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_security_build.py` & `flux-python-0.50.0rc0/src/_security_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_security_clean.h` & `flux-python-0.50.0rc0/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/_security_preproc.h` & `flux-python-0.50.0rc0/src/_security_preproc.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# 0 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
-# 0 "<built-in>"
-# 0 "<command-line>"
+# 1 "/workspaces/flux-python/src/_security_clean.h"
+# 1 "<built-in>"
+# 1 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
-# 0 "<command-line>" 2
-# 1 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
-# 35 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
+# 1 "<command-line>" 2
+# 1 "/workspaces/flux-python/src/_security_clean.h"
+# 35 "/workspaces/flux-python/src/_security_clean.h"
 enum {
     FLUX_SECURITY_DISABLE_PATH_PARANOIA = 0x1,
     FLUX_SECURITY_FORCE_PATH_PARANOIA = 0x2,
 };
 
 typedef struct flux_security flux_security_t;
 
@@ -22,34 +22,34 @@
 
 int flux_security_configure (flux_security_t *ctx, const char *pattern);
 
 int flux_security_aux_set (flux_security_t *ctx, const char *name,
              void *data, flux_security_free_f freefun);
 
 void *flux_security_aux_get (flux_security_t *ctx, const char *name);
-# 95 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
+# 95 "/workspaces/flux-python/src/_security_clean.h"
 enum {
     FLUX_SIGN_NOVERIFY = 1,
 };
-# 106 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
+# 106 "/workspaces/flux-python/src/_security_clean.h"
 const char *flux_sign_wrap (flux_security_t *ctx,
                             const void *payload, int payloadsz,
                             const char *mech_type,
                             int flags);
 
 
 
 
 
 const char *flux_sign_wrap_as (flux_security_t *ctx,
                                int64_t userid,
                                const void *payload, int payloadsz,
                                const char *mech_type,
                                int flags);
-# 132 "/home/runner/work/flux-python/flux-python/src/_security_clean.h"
+# 132 "/workspaces/flux-python/src/_security_clean.h"
 int flux_sign_unwrap (flux_security_t *ctx, const char *input,
                       const void **payload, int *payloadsz,
                       int64_t *userid, int flags);
```

### Comparing `flux-python-0.50.0/src/callbacks.h` & `flux-python-0.50.0rc0/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.50.0/src/make_clean_header.py` & `flux-python-0.50.0rc0/src/make_clean_header.py`

 * *Files identical despite different names*

