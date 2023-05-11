# Comparing `tmp/cruft-2.8.0.tar.gz` & `tmp/cruft-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cruft-2.8.0.tar", max compression
+gzip compressed data, was "cruft-2.9.0.tar", max compression
```

## Comparing `cruft-2.8.0.tar` & `cruft-2.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1089 2020-08-12 06:54:44.417132 cruft-2.8.0/LICENSE
--rw-r--r--   0        0        0     8474 2021-02-22 00:18:39.399787 cruft-2.8.0/README.md
--rw-r--r--   0        0        0      380 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/__init__.py
--rw-r--r--   0        0        0       52 2020-08-12 06:54:44.417132 cruft-2.8.0/cruft/__main__.py
--rw-r--r--   0        0        0     8458 2021-03-09 23:24:17.889925 cruft-2.8.0/cruft/_cli.py
--rw-r--r--   0        0        0      239 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/_commands/__init__.py
--rw-r--r--   0        0        0     1247 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/_commands/check.py
--rw-r--r--   0        0        0     2200 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/_commands/create.py
--rw-r--r--   0        0        0     3379 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/_commands/diff.py
--rw-r--r--   0        0        0     2217 2021-02-22 00:18:39.399787 cruft-2.8.0/cruft/_commands/link.py
--rw-r--r--   0        0        0     9037 2021-03-09 23:24:17.889925 cruft-2.8.0/cruft/_commands/update.py
--rw-r--r--   0        0        0      528 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/_commands/utils/__init__.py
--rw-r--r--   0        0        0     3600 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/_commands/utils/cookiecutter.py
--rw-r--r--   0        0        0     1259 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/_commands/utils/cruft.py
--rw-r--r--   0        0        0     1757 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/_commands/utils/diff.py
--rw-r--r--   0        0        0     4262 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/_commands/utils/generate.py
--rw-r--r--   0        0        0      853 2020-08-12 06:54:44.421131 cruft-2.8.0/cruft/_logo.py
--rw-r--r--   0        0        0       22 2021-03-09 23:27:14.891131 cruft-2.8.0/cruft/_version.py
--rw-r--r--   0        0        0     1815 2021-02-22 00:18:39.403787 cruft-2.8.0/cruft/exceptions.py
--rw-r--r--   0        0        0     1395 2021-03-09 23:26:52.634983 cruft-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     9703 2021-03-09 23:30:17.479079 cruft-2.8.0/setup.py
--rw-r--r--   0        0        0     9464 2021-03-09 23:30:17.479706 cruft-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2020-08-12 06:54:44.417132 cruft-2.9.0/LICENSE
+-rw-r--r--   0        0        0     8696 2021-06-30 20:12:02.524582 cruft-2.9.0/README.md
+-rw-r--r--   0        0        0      380 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/__init__.py
+-rw-r--r--   0        0        0       52 2020-08-12 06:54:44.417132 cruft-2.9.0/cruft/__main__.py
+-rw-r--r--   0        0        0     8458 2021-03-09 23:24:17.889925 cruft-2.9.0/cruft/_cli.py
+-rw-r--r--   0        0        0      239 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/_commands/__init__.py
+-rw-r--r--   0        0        0     1247 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/_commands/check.py
+-rw-r--r--   0        0        0     2200 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/_commands/create.py
+-rw-r--r--   0        0        0     3379 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/_commands/diff.py
+-rw-r--r--   0        0        0     2217 2021-02-22 00:18:39.399787 cruft-2.9.0/cruft/_commands/link.py
+-rw-r--r--   0        0        0     9037 2021-03-09 23:24:17.889925 cruft-2.9.0/cruft/_commands/update.py
+-rw-r--r--   0        0        0      528 2021-02-22 00:18:39.403787 cruft-2.9.0/cruft/_commands/utils/__init__.py
+-rw-r--r--   0        0        0     3600 2021-02-22 00:18:39.403787 cruft-2.9.0/cruft/_commands/utils/cookiecutter.py
+-rw-r--r--   0        0        0     1259 2021-02-22 00:18:39.403787 cruft-2.9.0/cruft/_commands/utils/cruft.py
+-rw-r--r--   0        0        0     1899 2021-06-30 20:12:02.524582 cruft-2.9.0/cruft/_commands/utils/diff.py
+-rw-r--r--   0        0        0     4544 2021-06-30 20:12:02.524582 cruft-2.9.0/cruft/_commands/utils/generate.py
+-rw-r--r--   0        0        0      853 2020-08-12 06:54:44.421131 cruft-2.9.0/cruft/_logo.py
+-rw-r--r--   0        0        0       22 2021-06-30 20:16:38.585554 cruft-2.9.0/cruft/_version.py
+-rw-r--r--   0        0        0     2205 2021-06-30 20:12:02.524582 cruft-2.9.0/cruft/exceptions.py
+-rw-r--r--   0        0        0     1389 2021-06-30 20:16:32.885534 cruft-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9935 2021-06-30 20:27:13.102132 cruft-2.9.0/setup.py
+-rw-r--r--   0        0        0     9686 2021-06-30 20:27:13.103008 cruft-2.9.0/PKG-INFO
```

### Comparing `cruft-2.8.0/LICENSE` & `cruft-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/README.md` & `cruft-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,24 @@
             ...
         }
 
     Or, if you have toml installed, you can add skip files directly to a `tool.cruft` section of your `pyproject.toml` file:
 
         [tool.cruft]
         skip = ["cruft/__init__.py", "tests"]
+    
+    Note that it is possible to use glob patterns for selecting the files to skip:
+        {
+            "skip": [
+                "**/__init__.py",
+                "tests/*"
+            ],
+            ...
+        }
+
 
 
 ## Checking a Project
 
 Checking to see if a project is missing a template update is as easy as running `cruft check`. If the project is out-of-date an error and exit code 1 will be returned.
 `cruft check` can be added to CI pipelines to ensure projects don't unintentionally drift.
```

### Comparing `cruft-2.8.0/cruft/_cli.py` & `cruft-2.9.0/cruft/_cli.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/check.py` & `cruft-2.9.0/cruft/_commands/check.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/create.py` & `cruft-2.9.0/cruft/_commands/create.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/diff.py` & `cruft-2.9.0/cruft/_commands/diff.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/link.py` & `cruft-2.9.0/cruft/_commands/link.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/update.py` & `cruft-2.9.0/cruft/_commands/update.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/utils/__init__.py` & `cruft-2.9.0/cruft/_commands/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/utils/cookiecutter.py` & `cruft-2.9.0/cruft/_commands/utils/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/utils/cruft.py` & `cruft-2.9.0/cruft/_commands/utils/cruft.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/_commands/utils/diff.py` & `cruft-2.9.0/cruft/_commands/utils/diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from pathlib import Path
 from subprocess import PIPE, run  # nosec
 from typing import List
 
+from cruft import exceptions
+
 
 def _git_diff(*args: str) -> List[str]:
     return ["git", "-c", "diff.noprefix=", "diff", "--no-index", "--relative", *args]
 
 
 def get_diff(repo0: Path, repo1: Path) -> str:
     """Compute the raw diff between two repositories."""
-    diff = run(
-        _git_diff("--no-ext-diff", "--no-color", str(repo0), str(repo1)),
-        cwd=str(repo0),
-        stdout=PIPE,
-        stderr=PIPE,
-    ).stdout.decode()
-
+    try:
+        diff = run(
+            _git_diff("--no-ext-diff", "--no-color", str(repo0), str(repo1)),
+            cwd=str(repo0),
+            stdout=PIPE,
+            stderr=PIPE,
+        ).stdout.decode()
+    except UnicodeDecodeError:
+        raise exceptions.ChangesetUnicodeError()
     # By default, git diff --no-index will output full paths like so:
     # --- a/tmp/tmpmp34g21y/remote/.coveragerc
     # +++ b/tmp/tmpmp34g21y/local/.coveragerc
     # We don't want this as we may need to apply the diff later on.
     # Note that diff headers contain repo0 and repo1 with both "a" and "b"
     # prefixes: headers for new files have a/repo1, headers for deleted files
     # have b/repo0.
```

### Comparing `cruft-2.8.0/cruft/_commands/utils/generate.py` & `cruft-2.9.0/cruft/_commands/utils/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 from pathlib import Path
 from shutil import move, rmtree
 from tempfile import TemporaryDirectory
-from typing import Optional, Set
+from typing import Optional, Set, Union
+from warnings import warn
 
 from cookiecutter.generate import generate_files
 from git import Repo
 
 from .cookiecutter import CookiecutterContext, generate_cookiecutter_context
 from .cruft import CruftState
 
 try:
-    import toml  # type: ignore
+    import toml
 except ImportError:  # pragma: no cover
     toml = None  # type: ignore
 
 
 def cookiecutter_template(
     output_dir: Path,
     repo: Repo,
@@ -94,28 +95,33 @@
 
 
 def _get_skip_paths(cruft_state: CruftState, pyproject_file: Path) -> Set[Path]:
     skip_cruft = cruft_state.get("skip", [])
     if toml and pyproject_file.is_file():
         pyproject_cruft = toml.loads(pyproject_file.read_text()).get("tool", {}).get("cruft", {})
         skip_cruft.extend(pyproject_cruft.get("skip", []))
+    elif pyproject_file.is_file():
+        warn(
+            "pyproject.toml is present in repo, but `toml` package is not installed. "
+            "Cruft configuration may be ignored."
+        )
     return set(map(Path, skip_cruft))
 
 
 def _get_deleted_files(template_dir: Path, project_dir: Path):
     cwd = Path.cwd()
     os.chdir(template_dir)
     template_paths = set(Path(".").glob("**/*"))
     os.chdir(cwd)
     os.chdir(project_dir)
     deleted_paths = set(filter(lambda path: not path.exists(), template_paths))
     os.chdir(cwd)
     return deleted_paths
 
 
-def _remove_paths(root: Path, paths_to_remove: Set[Path]):
+def _remove_paths(root: Path, paths_to_remove: Union[Set[Path], Set[str]]):
     for path_to_remove in paths_to_remove:
-        path = root / path_to_remove
-        if path.is_dir():
-            rmtree(path)
-        elif path.is_file():
-            path.unlink()
+        for path in root.glob(str(path_to_remove)):
+            if path.is_file() or path.is_symlink():
+                path.unlink()
+            elif path.is_dir():
+                rmtree(path)
```

### Comparing `cruft-2.8.0/cruft/_logo.py` & `cruft-2.9.0/cruft/_logo.py`

 * *Files identical despite different names*

### Comparing `cruft-2.8.0/cruft/exceptions.py` & `cruft-2.9.0/cruft/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,7 +43,19 @@
     """Raised when an invalid cookiecutter repository is provided."""
 
     def __init__(self, cookiecutter_repo: str, details: str = ""):
         self.cookiecutter_repo = cookiecutter_repo
         super().__init__(
             f"Unable to initialize the cookiecutter using {cookiecutter_repo}! {details.strip()}"
         )
+
+
+class ChangesetUnicodeError(CruftError):
+    """Raised when `cruft update` is unable to generate the change"""
+
+    def __init__(self):
+        super().__init__(
+            (
+                "Unable to interpret changes between current project and cookiecutter template as "
+                "unicode. Typically a result of hidden binary files in project folder."
+            )
+        )
```

### Comparing `cruft-2.8.0/pyproject.toml` & `cruft-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 name = "cruft"
-version = "2.8.0"
+version = "2.9.0"
 description = "Allows you to maintain all the necessary cruft for packaging and building projects separate from the code you intentionally write. Built on-top of CookieCutter."
 authors = ["Timothy Crosley <timothy.crosley@gmail.com>", "Sambhav Kothari <sambhavs.email@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 cookiecutter = "^1.6"
 gitpython = "^3.0"
 toml = { version = "^0.10", optional = true }
-typer = "^0.3.1"
+typer = "^0.3.2"
 click = "^7.1.2"
 examples = {version = "^1.0.2", optional = true}
 
 [tool.poetry.extras]
 pyproject = ["toml"]
 examples = ["examples"]
 
 [tool.poetry.dev-dependencies]
 vulture = "^1.0"
 bandit = "^1.6"
 safety = "^1.8"
 isort = "^5.3"
 flake8-bugbear = "^19.8"
-black = {version = "^18.3-alpha.0", allow-prereleases = true}
-mypy = "^0.730.0"
+black = {version = "^20.8b1", allow-prereleases = true}
+mypy = "^0.812.0"
 ipython = "^7.7"
 pytest = "^5.0"
 pytest-cov = "^2.7"
 pep8-naming = "^0.8.2"
-portray = "^1.3.0"
+portray = "^1.6.0"
 examples = "^1.0.2"
 pytest-xdist = "^1.34.0"
 pytest-mock = "^3.3.1"
 
 [tool.poetry.scripts]
 cruft = "cruft._cli:app"
```

### Comparing `cruft-2.8.0/setup.py` & `cruft-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=7.1.2,<8.0.0',
  'cookiecutter>=1.6,<2.0',
  'gitpython>=3.0,<4.0',
- 'typer>=0.3.1,<0.4.0']
+ 'typer>=0.3.2,<0.4.0']
 
 extras_require = \
 {'examples': ['examples>=1.0.2,<2.0.0'], 'pyproject': ['toml>=0.10,<0.11']}
 
 entry_points = \
 {'console_scripts': ['cruft = cruft._cli:app']}
 
 setup_kwargs = {
     'name': 'cruft',
-    'version': '2.8.0',
+    'version': '2.9.0',
     'description': 'Allows you to maintain all the necessary cruft for packaging and building projects separate from the code you intentionally write. Built on-top of CookieCutter.',
-    'long_description': '[![cruft - Fight Back Against the Boilerplate Monster!](https://raw.github.com/cruft/cruft/master/art/logo_large.png)](https://cruft.github.io/cruft/)\n_________________\n\n[![PyPI version](https://badge.fury.io/py/cruft.svg)](http://badge.fury.io/py/cruft)\n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/cruft.svg)](https://anaconda.org/conda-forge/cruft)\n[![Build Status](https://github.com/cruft/cruft/workflows/Run%20tests/badge.svg)](https://github.com/cruft/cruft/actions?query=workflow%3A%22Run+tests%22+branch%3Amaster)\n[![codecov](https://codecov.io/gh/cruft/cruft/branch/master/graph/badge.svg)](https://codecov.io/gh/cruft/cruft)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)\n[![Join the chat at https://gitter.im/cruft/community](https://badges.gitter.im/cruft/community.svg)](https://gitter.im/cruft/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/pypi/cruft/)\n[![Downloads](https://pepy.tech/badge/cruft)](https://pepy.tech/project/cruft)\n\n#### Trending Contributors\n\n[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/0)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/0)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/1)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/1)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/2)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/2)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/3)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/3)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/4)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/4)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/5)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/5)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/6)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/6)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/7)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/7)\n_________________\n\n[Read Latest Documentation](https://cruft.github.io/cruft/) - [Browse GitHub Code Repository](https://github.com/cruft/cruft/)\n_________________\n\n**cruft** allows you to maintain all the necessary boilerplate for packaging and building projects separate from the code you intentionally write.\nFully compatible with existing [Cookiecutter](https://github.com/cookiecutter/cookiecutter) templates.\n\nCreating new projects from templates using cruft is easy:\n\n![Example Usage New Project](https://raw.githubusercontent.com/cruft/cruft/master/art/example.gif)\n\nAnd, so is updating them as the template changes overtime:\n\n![Example Usage New Project](https://raw.githubusercontent.com/cruft/cruft/master/art/example_update.gif)\n\nMany project template utilities exist that automate the copying and pasting of code to create new projects. This *seems* great! However, once created, most leave you with that copy-and-pasted code to manage through the life of your project.\n\ncruft is different. It automates the creation of new projects like the others, but then it also helps you to manage the boilerplate through the life of the project. cruft makes sure your code stays in-sync with the template it came from for you.\n\n## Key Features:\n\n* **Cookiecutter Compatible**: cruft utilizes [Cookiecutter](https://github.com/cookiecutter/cookiecutter) as its template expansion engine. Meaning it retains full compatibility with all existing [Cookiecutter](https://github.com/cookiecutter/cookiecutter) templates.\n* **Template Validation**: cruft can quickly validate whether or not a project is using the latest version of a template using `cruft check`. This check can easily be added to CI pipelines to ensure your projects stay in-sync.\n* **Automatic Template Updates**: cruft automates the process of updating code to match the latest version of a template, making it easy to utilize template improvements across many projects.\n\n## Installation:\n\nTo get started - install `cruft` using a Python package manager:\n\n`pip3 install cruft`\n\nOR\n\n`poetry add cruft`\n\nOR\n\n`pipenv install cruft`\n\n\n## Creating a New Project:\n\nTo create a new project using cruft run `cruft create PROJECT_URL` from the command line.\n\nFor example:\n\n        cruft create https://github.com/timothycrosley/cookiecutter-python/\n\ncruft will then ask you any necessary questions to create your new project. It will use your answers to expand the provided template, and then return the directory it placed the expanded project.\nBehind the scenes, cruft uses [Cookiecutter](https://github.com/cookiecutter/cookiecutter) to do the project expansion. The only difference in the resulting output is a `.cruft.json` file that\ncontains the git hash of the template used as well as the parameters specified.\n\n## Updating a Project\n\nTo update an existing project, that was created using cruft, run `cruft update` in the root of the project.\nIf there are any updates, cruft will have you review them before applying. If you accept the changes cruft will apply them to your project\nand update the `.cruft.json` file for you.\n\n!!! tip\n    Sometimes certain files just aren\'t good fits for updating. Such as test cases or `__init__` files. You can tell cruft to always skip updating these files on a project by project basis by added them\n    to a skip section within your .cruft.json file:\n\n        {\n            "template": "https://github.com/timothycrosley/cookiecutter-python",\n            "commit": "8a65a360d51250221193ed0ec5ed292e72b32b0b",\n            "skip": [\n                "cruft/__init__.py",\n                "tests"\n            ],\n            ...\n        }\n\n    Or, if you have toml installed, you can add skip files directly to a `tool.cruft` section of your `pyproject.toml` file:\n\n        [tool.cruft]\n        skip = ["cruft/__init__.py", "tests"]\n\n\n## Checking a Project\n\nChecking to see if a project is missing a template update is as easy as running `cruft check`. If the project is out-of-date an error and exit code 1 will be returned.\n`cruft check` can be added to CI pipelines to ensure projects don\'t unintentionally drift.\n\n\n## Linking an Existing Project\n\nHave an existing project that you created from a template in the past using Cookiecutter directly? You can link it to the template that was used to create it using: `cruft link TEMPLATE_REPOSITORY`.\n\nFor example:\n\n        cruft link https://github.com/timothycrosley/cookiecutter-python/\n\nYou can then specify the last commit of the template the project has been updated to be consistent with, or accept the default of using the latest commit from the template.\n\n## Compute the diff\n\nWith time, your boilerplate may end up being very different from the actual cookiecutter template. Cruft allows you to quickly see what changed in your local project compared to the template. It is as easy as running `cruft diff`. If any local file differs from the template, the diff will appear in your terminal in a similar fashion to `git diff`.\n\nThe `cruft diff` command optionally accepts an `--exit-code` flag that will make cruft exit with a non-0 code should any diff is found. You can combine this flag with the `skip` section of your `.cruft.json` to make stricter CI checks that ensures any improvement to the template is always submitted upstream.\n\n## Why Create cruft?\n\nSince I first saw videos of [quickly](https://www.youtube.com/watch?v=9EctXzH2dss) being used to automate Ubuntu application creation, I\'ve had a love/hate relationship with these kinds of tools.\nI\'ve used them for many projects and certainly seen them lead to productivity improvements. However, I\'ve always felt like they were a double-edged sword. Sure, they would automate away the copying and pasting many would do to create projects. However, by doing so,\nthey encouraged more code to be copied and pasted! Then, over time, you could easily be left with hundreds of projects that contained copy-and-pasted code with no way to easy way to update them. I created cruft to be a tool that recognized that balance between project creation and maintenance and provided mechanisms to keep built projects up-to-date.\n\nI hope you too find `cruft` useful!\n\n~Timothy Crosley\n',
+    'long_description': '[![cruft - Fight Back Against the Boilerplate Monster!](https://raw.github.com/cruft/cruft/master/art/logo_large.png)](https://cruft.github.io/cruft/)\n_________________\n\n[![PyPI version](https://badge.fury.io/py/cruft.svg)](http://badge.fury.io/py/cruft)\n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/cruft.svg)](https://anaconda.org/conda-forge/cruft)\n[![Build Status](https://github.com/cruft/cruft/workflows/Run%20tests/badge.svg)](https://github.com/cruft/cruft/actions?query=workflow%3A%22Run+tests%22+branch%3Amaster)\n[![codecov](https://codecov.io/gh/cruft/cruft/branch/master/graph/badge.svg)](https://codecov.io/gh/cruft/cruft)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://timothycrosley.github.io/isort/)\n[![Join the chat at https://gitter.im/cruft/community](https://badges.gitter.im/cruft/community.svg)](https://gitter.im/cruft/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.python.org/pypi/cruft/)\n[![Downloads](https://pepy.tech/badge/cruft)](https://pepy.tech/project/cruft)\n\n#### Trending Contributors\n\n[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/0)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/0)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/1)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/1)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/2)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/2)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/3)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/3)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/4)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/4)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/5)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/5)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/6)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/6)[![](https://sourcerer.io/fame/samj1912/cruft/cruft/images/7)](https://sourcerer.io/fame/samj1912/cruft/cruft/links/7)\n_________________\n\n[Read Latest Documentation](https://cruft.github.io/cruft/) - [Browse GitHub Code Repository](https://github.com/cruft/cruft/)\n_________________\n\n**cruft** allows you to maintain all the necessary boilerplate for packaging and building projects separate from the code you intentionally write.\nFully compatible with existing [Cookiecutter](https://github.com/cookiecutter/cookiecutter) templates.\n\nCreating new projects from templates using cruft is easy:\n\n![Example Usage New Project](https://raw.githubusercontent.com/cruft/cruft/master/art/example.gif)\n\nAnd, so is updating them as the template changes overtime:\n\n![Example Usage New Project](https://raw.githubusercontent.com/cruft/cruft/master/art/example_update.gif)\n\nMany project template utilities exist that automate the copying and pasting of code to create new projects. This *seems* great! However, once created, most leave you with that copy-and-pasted code to manage through the life of your project.\n\ncruft is different. It automates the creation of new projects like the others, but then it also helps you to manage the boilerplate through the life of the project. cruft makes sure your code stays in-sync with the template it came from for you.\n\n## Key Features:\n\n* **Cookiecutter Compatible**: cruft utilizes [Cookiecutter](https://github.com/cookiecutter/cookiecutter) as its template expansion engine. Meaning it retains full compatibility with all existing [Cookiecutter](https://github.com/cookiecutter/cookiecutter) templates.\n* **Template Validation**: cruft can quickly validate whether or not a project is using the latest version of a template using `cruft check`. This check can easily be added to CI pipelines to ensure your projects stay in-sync.\n* **Automatic Template Updates**: cruft automates the process of updating code to match the latest version of a template, making it easy to utilize template improvements across many projects.\n\n## Installation:\n\nTo get started - install `cruft` using a Python package manager:\n\n`pip3 install cruft`\n\nOR\n\n`poetry add cruft`\n\nOR\n\n`pipenv install cruft`\n\n\n## Creating a New Project:\n\nTo create a new project using cruft run `cruft create PROJECT_URL` from the command line.\n\nFor example:\n\n        cruft create https://github.com/timothycrosley/cookiecutter-python/\n\ncruft will then ask you any necessary questions to create your new project. It will use your answers to expand the provided template, and then return the directory it placed the expanded project.\nBehind the scenes, cruft uses [Cookiecutter](https://github.com/cookiecutter/cookiecutter) to do the project expansion. The only difference in the resulting output is a `.cruft.json` file that\ncontains the git hash of the template used as well as the parameters specified.\n\n## Updating a Project\n\nTo update an existing project, that was created using cruft, run `cruft update` in the root of the project.\nIf there are any updates, cruft will have you review them before applying. If you accept the changes cruft will apply them to your project\nand update the `.cruft.json` file for you.\n\n!!! tip\n    Sometimes certain files just aren\'t good fits for updating. Such as test cases or `__init__` files. You can tell cruft to always skip updating these files on a project by project basis by added them\n    to a skip section within your .cruft.json file:\n\n        {\n            "template": "https://github.com/timothycrosley/cookiecutter-python",\n            "commit": "8a65a360d51250221193ed0ec5ed292e72b32b0b",\n            "skip": [\n                "cruft/__init__.py",\n                "tests"\n            ],\n            ...\n        }\n\n    Or, if you have toml installed, you can add skip files directly to a `tool.cruft` section of your `pyproject.toml` file:\n\n        [tool.cruft]\n        skip = ["cruft/__init__.py", "tests"]\n    \n    Note that it is possible to use glob patterns for selecting the files to skip:\n        {\n            "skip": [\n                "**/__init__.py",\n                "tests/*"\n            ],\n            ...\n        }\n\n\n\n## Checking a Project\n\nChecking to see if a project is missing a template update is as easy as running `cruft check`. If the project is out-of-date an error and exit code 1 will be returned.\n`cruft check` can be added to CI pipelines to ensure projects don\'t unintentionally drift.\n\n\n## Linking an Existing Project\n\nHave an existing project that you created from a template in the past using Cookiecutter directly? You can link it to the template that was used to create it using: `cruft link TEMPLATE_REPOSITORY`.\n\nFor example:\n\n        cruft link https://github.com/timothycrosley/cookiecutter-python/\n\nYou can then specify the last commit of the template the project has been updated to be consistent with, or accept the default of using the latest commit from the template.\n\n## Compute the diff\n\nWith time, your boilerplate may end up being very different from the actual cookiecutter template. Cruft allows you to quickly see what changed in your local project compared to the template. It is as easy as running `cruft diff`. If any local file differs from the template, the diff will appear in your terminal in a similar fashion to `git diff`.\n\nThe `cruft diff` command optionally accepts an `--exit-code` flag that will make cruft exit with a non-0 code should any diff is found. You can combine this flag with the `skip` section of your `.cruft.json` to make stricter CI checks that ensures any improvement to the template is always submitted upstream.\n\n## Why Create cruft?\n\nSince I first saw videos of [quickly](https://www.youtube.com/watch?v=9EctXzH2dss) being used to automate Ubuntu application creation, I\'ve had a love/hate relationship with these kinds of tools.\nI\'ve used them for many projects and certainly seen them lead to productivity improvements. However, I\'ve always felt like they were a double-edged sword. Sure, they would automate away the copying and pasting many would do to create projects. However, by doing so,\nthey encouraged more code to be copied and pasted! Then, over time, you could easily be left with hundreds of projects that contained copy-and-pasted code with no way to easy way to update them. I created cruft to be a tool that recognized that balance between project creation and maintenance and provided mechanisms to keep built projects up-to-date.\n\nI hope you too find `cruft` useful!\n\n~Timothy Crosley\n',
     'author': 'Timothy Crosley',
     'author_email': 'timothy.crosley@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cruft-2.8.0/PKG-INFO` & `cruft-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cruft
-Version: 2.8.0
+Version: 2.9.0
 Summary: Allows you to maintain all the necessary cruft for packaging and building projects separate from the code you intentionally write. Built on-top of CookieCutter.
 License: MIT
 Author: Timothy Crosley
 Author-email: timothy.crosley@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: examples
 Provides-Extra: pyproject
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cookiecutter (>=1.6,<2.0)
 Requires-Dist: examples (>=1.0.2,<2.0.0); extra == "examples"
 Requires-Dist: gitpython (>=3.0,<4.0)
 Requires-Dist: toml (>=0.10,<0.11); extra == "pyproject"
-Requires-Dist: typer (>=0.3.1,<0.4.0)
+Requires-Dist: typer (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 [![cruft - Fight Back Against the Boilerplate Monster!](https://raw.github.com/cruft/cruft/master/art/logo_large.png)](https://cruft.github.io/cruft/)
 _________________
 
 [![PyPI version](https://badge.fury.io/py/cruft.svg)](http://badge.fury.io/py/cruft)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/cruft.svg)](https://anaconda.org/conda-forge/cruft)
@@ -111,14 +111,24 @@
             ...
         }
 
     Or, if you have toml installed, you can add skip files directly to a `tool.cruft` section of your `pyproject.toml` file:
 
         [tool.cruft]
         skip = ["cruft/__init__.py", "tests"]
+    
+    Note that it is possible to use glob patterns for selecting the files to skip:
+        {
+            "skip": [
+                "**/__init__.py",
+                "tests/*"
+            ],
+            ...
+        }
+
 
 
 ## Checking a Project
 
 Checking to see if a project is missing a template update is as easy as running `cruft check`. If the project is out-of-date an error and exit code 1 will be returned.
 `cruft check` can be added to CI pipelines to ensure projects don't unintentionally drift.
```

