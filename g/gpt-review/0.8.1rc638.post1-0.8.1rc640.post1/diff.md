# Comparing `tmp/gpt-review-0.8.1rc638.post1.tar.gz` & `tmp/gpt-review-0.8.1rc640.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.1rc638.post1.tar", last modified: Thu May 11 01:28:35 2023, max compression
+gzip compressed data, was "gpt-review-0.8.1rc640.post1.tar", last modified: Thu May 11 03:55:24 2023, max compression
```

## Comparing `gpt-review-0.8.1rc638.post1.tar` & `gpt-review-0.8.1rc640.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      336 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4200 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1851 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8500 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-11 01:28:34.960528 gpt-review-0.8.1rc638.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-11 01:28:34.964528 gpt-review-0.8.1rc638.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     8772 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     2772 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5788 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5769 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3671 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8994 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      523 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-11 01:28:28.636481 gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0      529 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_bugs.py
--rw-r--r--   0        0        0      524 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_coverage.py
--rw-r--r--   0        0        0     1177 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      516 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_summary.py
--rw-r--r--   0        0        0      218 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     5421 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/mock.diff
--rw-r--r--   0        0        0      612 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_git.py
--rw-r--r--   0        0        0     1443 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_github.py
--rw-r--r--   0        0        0     5612 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1286 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_report.py
--rw-r--r--   0        0        0      797 2023-05-11 01:28:28.640481 gpt-review-0.8.1rc638.post1/tests/test_review.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.8.1rc638.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4200 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1851 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8500 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-11 03:55:23.621978 gpt-review-0.8.1rc640.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-11 03:55:23.621978 gpt-review-0.8.1rc640.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0    10321 2023-05-11 03:55:15.902016 gpt-review-0.8.1rc640.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     3016 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5998 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5769 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3671 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9229 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      924 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_bugs.py
+-rw-r--r--   0        0        0      524 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_coverage.py
+-rw-r--r--   0        0        0     1177 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      516 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_summary.py
+-rw-r--r--   0        0        0      218 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5421 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/mock.diff
+-rw-r--r--   0        0        0      612 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5612 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1286 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-11 03:55:15.906016 gpt-review-0.8.1rc640.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 gpt-review-0.8.1rc640.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.1rc638.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.1rc640.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.1rc640.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/dependabot.yml` & `gpt-review-0.8.1rc640.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/pull_request_template.md` & `gpt-review-0.8.1rc640.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.1rc640.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.1rc640.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.1rc640.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/workflows/python.yml` & `gpt-review-0.8.1rc640.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.1rc640.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.gitignore` & `gpt-review-0.8.1rc640.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/.vscode/settings.json` & `gpt-review-0.8.1rc640.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/LICENSE` & `gpt-review-0.8.1rc640.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/README.md` & `gpt-review-0.8.1rc640.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/action.yml` & `gpt-review-0.8.1rc640.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/pyproject.toml` & `gpt-review-0.8.1rc640.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_ask.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_ask.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,15 +72,38 @@
     large: bool = False,
     directory: Optional[str] = None,
     required_exts: Optional[List[str]] = None,
     hidden: bool = False,
     recursive: bool = False,
     repository: Optional[str] = None,
 ) -> Dict[str, str]:
-    """Ask GPT a question."""
+    """Ask GPT a question.
+
+    Args:
+        question (List[str]): The question to ask GPT.
+        max_tokens (int, optional): The maximum number of tokens to generate. Defaults to C.MAX_TOKENS_DEFAULT.
+        temperature (float, optional): Controls randomness. Defaults to C.TEMPERATURE_DEFAULT.
+        top_p (float, optional): Controls diversity via nucleus sampling. Defaults to C.TOP_P_DEFAULT.
+        frequency_penalty (float, optional): How much to penalize new tokens based on their existing frequency in the
+            text so far. Defaults to C.FREQUENCY_PENALTY_DEFAULT.
+        presence_penalty (float, optional): How much to penalize new tokens based on whether they appear in the text so
+            far. Defaults to C.PRESENCE_PENALTY_DEFAULT.
+        files (Optional[List[str]], optional): The files to search. Defaults to None.
+        messages ([type], optional): [description]. Defaults to None.
+        fast (bool, optional): Use the fast model. Defaults to False.
+        large (bool, optional): Use the large model. Defaults to False.
+        directory (Optional[str], optional): The directory to search. Defaults to None.
+        required_exts (Optional[List[str]], optional): The required file extensions. Defaults to None.
+        hidden (bool, optional): Include hidden files. Defaults to False.
+        recursive (bool, optional): Recursively search the directory. Defaults to False.
+        repository (Optional[str], optional): The repository to search. Defaults to None.
+
+    Returns:
+            Dict[str, str]: The response from GPT.
+    """
     _load_azure_openai_context()
 
     prompt = " ".join(question)
 
     if files or directory or repository:
         response = _query_index(
             prompt,
```

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_git.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_git.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,15 +58,23 @@
     diff = _diff()
     logging.debug("Diff: %s", diff)
 
     return _request_goal(diff, goal, fast=not gpt4, large=large)
 
 
 def _commit(gpt4: bool = False, large: bool = False) -> Dict[str, str]:
-    """Run git commit with a commit message generated by GPT."""
+    """Run git commit with a commit message generated by GPT.
+
+    Args:
+        gpt4 (bool, optional): Whether to use gpt-4. Defaults to False.
+        large (bool, optional): Whether to use gpt-4-32k. Defaults to False.
+
+    Returns:
+        response (Dict[str, str]): The response from git commit.
+    """
     message = _commit_message(gpt4=gpt4, large=large)
     logging.debug("Commit Message: %s", message)
     repo = Repo.init(_find_git_dir())
     commit = repo.git.commit(message=message)
     return {"response": commit}
```

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_github.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_github.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,24 @@
             return {"response": "PR posted"}
 
         logging.warning("No PR to post too")
         return {"response": "No PR to post too"}
 
 
 def _github_review(repository=None, pull_request=None, access_token=None) -> Dict[str, str]:
-    """Review GitHub PR with Open AI, and post response as a comment."""
+    """Review GitHub PR with Open AI, and post response as a comment.
+
+    Args:
+        repository (str): The repo of the PR.
+        pull_request (str): The PR number.
+        access_token (str): The GitHub access token.
+
+    Returns:
+        Dict[str, str]: The response.
+    """
     diff = _GitHubClient.get_pr_diff(repository, pull_request, access_token)
     _GitHubClient.post_pr_summary(diff)
     return {"response": "Review posted as a comment."}
 
 
 class GitHubCommandGroup(GPTCommandGroup):
     """Ask Command Group."""
```

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_openai.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/_review.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/_review.py`

 * *Files 5% similar despite different names*

```diff
@@ -241,15 +241,23 @@
 
     summary += _summarize_risk(git_diff)
 
     return summary
 
 
 def _review(diff: str = ".diff", config: str = "config.summary.yml") -> Dict[str, str]:
-    """Review a git diff from file"""
+    """Review a git diff from file
+
+    Args:
+        diff (str, optional): The diff to review. Defaults to ".diff".
+        config (str, optional): The config to use. Defaults to "config.summary.yml".
+
+    Returns:
+        Dict[str, str]: The response from GPT-4.
+    """
 
     # If config is a file, use it
 
     with open(diff, "r", encoding="utf8") as file:
         diff_contents = file.read()
 
         if os.path.isfile(config):
```

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/constants.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/main.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     return f"""
 type: {help_type}
 short-summary: {short_summary}
 """
 
 
 helps[""] = _help_text("group", "Easily interact with GPT APIs.")
+helps["ask"] = _help_text("group", "Use GPT to ask questions.")
 helps["git"] = _help_text("group", "Use GPT enchanced git commands.")
+helps["git commit"] = _help_text("command", "Run git commit with a commit message generated by GPT.")
 helps["github"] = _help_text("group", "Use GPT with GitHub Repositories.")
+helps["github review"] = _help_text("command", "Review GitHub PR with Open AI, and post response as a comment.")
 helps["review"] = _help_text("group", "Use GPT to perform customized reviews.")
+helps["review diff"] = _help_text("command", "Review a git diff from file.")
 
 
 exit_code = cli()
 sys.exit(exit_code)
```

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_bugs.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_bugs.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_coverage.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_coverage.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_prompt.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/src/gpt_review/prompts/_summary.py` & `gpt-review-0.8.1rc640.post1/src/gpt_review/prompts/_summary.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/conftest.py` & `gpt-review-0.8.1rc640.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/mock.diff` & `gpt-review-0.8.1rc640.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_git.py` & `gpt-review-0.8.1rc640.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_github.py` & `gpt-review-0.8.1rc640.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.1rc640.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_llama_index.py` & `gpt-review-0.8.1rc640.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_openai.py` & `gpt-review-0.8.1rc640.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_report.py` & `gpt-review-0.8.1rc640.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/tests/test_review.py` & `gpt-review-0.8.1rc640.post1/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.1rc638.post1/PKG-INFO` & `gpt-review-0.8.1rc640.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.1rc638.post1
+Version: 0.8.1rc640.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.1rc638.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.1rc640.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

