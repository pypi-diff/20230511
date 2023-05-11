# Comparing `tmp/gpt-review-0.8.1rc640.post1.tar.gz` & `tmp/gpt-review-0.8.1rc645.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.1rc640.post1.tar", last modified: Thu May 11 03:55:24 2023, max compression
+gzip compressed data, was "gpt-review-0.8.1rc645.post1.tar", last modified: Thu May 11 17:34:18 2023, max compression
```

## Comparing `gpt-review-0.8.1rc640.post1.tar` & `gpt-review-0.8.1rc645.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      336 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1851 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8500 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-11 03:55:23.621978 gpt-review-0.8.1rc640.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-11 03:55:23.621978 gpt-review-0.8.1rc640.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10321 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     3016 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5998 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5769 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3671 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     9229 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      523 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      924 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0      529 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_bugs.py
--rw-r--r--   0        0        0      524 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_coverage.py
--rw-r--r--   0        0        0     1177 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      516 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_summary.py
--rw-r--r--   0        0        0      218 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5421 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/mock.diff
--rw-r--r--   0        0        0      612 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_github.py
--rw-r--r--   0        0        0     5612 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1286 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_review.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.8.1rc640.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1851 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-11 17:34:18.674978 gpt-review-0.8.1rc645.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-11 17:34:18.674978 gpt-review-0.8.1rc645.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10321 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3016 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-11 17:34:12.606903 gpt-review-0.8.1rc645.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5769 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3671 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9229 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      924 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_bugs.py
+-rw-r--r--   0        0        0      524 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_coverage.py
+-rw-r--r--   0        0        0     1177 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      516 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_summary.py
+-rw-r--r--   0        0        0      218 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5421 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/mock.diff
+-rw-r--r--   0        0        0      612 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5612 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1286 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-11 17:34:12.610903 gpt-review-0.8.1rc645.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.8.1rc645.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.1rc640.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.1rc645.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.1rc645.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/dependabot.yml` & `gpt-review-0.8.1rc645.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/pull_request_template.md` & `gpt-review-0.8.1rc645.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.1rc645.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.1rc645.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.1rc645.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/workflows/python.yml` & `gpt-review-0.8.1rc645.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.1rc645.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.gitignore` & `gpt-review-0.8.1rc645.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/.vscode/settings.json` & `gpt-review-0.8.1rc645.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/LICENSE` & `gpt-review-0.8.1rc645.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/README.md` & `gpt-review-0.8.1rc645.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/action.yml` & `gpt-review-0.8.1rc645.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/pyproject.toml` & `gpt-review-0.8.1rc645.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.8.1"
 dynamic = ["version"]
 dependencies = [
   'azure-identity',
   'azure-keyvault-secrets',
-  'llama-index>=0.6.0,<=0.6.4',
+  'llama-index>=0.6.0,<=0.6.5',
   'httpx',
   'GitPython',
   'knack',
   'openai',
   'requests',
   'pyyaml',
   'typing_extensions; python_version <= "3.10"',
```

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_ask.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_git.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_github.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_openai.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/_review.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/constants.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/main.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_bugs.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_bugs.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_coverage.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_coverage.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_prompt.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_summary.py` & `gpt-review-0.8.1rc645.post1/src/gpt_review/prompts/_summary.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/conftest.py` & `gpt-review-0.8.1rc645.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/mock.diff` & `gpt-review-0.8.1rc645.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_git.py` & `gpt-review-0.8.1rc645.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_github.py` & `gpt-review-0.8.1rc645.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.1rc645.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_llama_index.py` & `gpt-review-0.8.1rc645.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_openai.py` & `gpt-review-0.8.1rc645.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_report.py` & `gpt-review-0.8.1rc645.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/tests/test_review.py` & `gpt-review-0.8.1rc645.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc640.post1/PKG-INFO` & `gpt-review-0.8.1rc645.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.1rc640.post1
+Version: 0.8.1rc645.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-identity
 Requires-Dist: azure-keyvault-secrets
-Requires-Dist: llama-index>=0.6.0,<=0.6.4
+Requires-Dist: llama-index>=0.6.0,<=0.6.5
 Requires-Dist: httpx
 Requires-Dist: GitPython
 Requires-Dist: knack
 Requires-Dist: openai
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: typing_extensions; python_version <= "3.10"
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.1rc640.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.1rc645.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: azure-identity Requires-Dist: azure-keyvault-
-secrets Requires-Dist: llama-index>=0.6.0,<=0.6.4 Requires-Dist: httpx
+secrets Requires-Dist: llama-index>=0.6.0,<=0.6.5 Requires-Dist: httpx
 Requires-Dist: GitPython Requires-Dist: knack Requires-Dist: openai Requires-
 Dist: requests Requires-Dist: pyyaml Requires-Dist: typing_extensions;
 python_version <= "3.10" Requires-Dist: transformers; python_version <= "3.8"
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test" Requires-Dist:
 black==23.3.0 ; extra == "test" Requires-Dist: check-manifest==0.49 ; extra ==
 "test" Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test" Requires-Dist:
 flake8-docstrings ; extra == "test" Requires-Dist: flake8-formatter_junit_xml ;
```

