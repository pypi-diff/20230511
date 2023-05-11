# Comparing `tmp/pipdeptree-2.7.0.tar.gz` & `tmp/pipdeptree-2.7.1.tar.gz`

## Comparing `pipdeptree-2.7.0.tar` & `pipdeptree-2.7.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.prettierrc.toml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/tox.ini
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/whitelist.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.github/workflows/check.yml
--rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/docs/twine-pdt.png
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/docs/v2beta-opts.org
--rw-r--r--   0        0        0    35116 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/src/pipdeptree/version.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    24204 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/LICENSE
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/README.md
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    15546 2020-02-02 00:00:00.000000 pipdeptree-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.prettierrc.toml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tox.ini
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/whitelist.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/docs/twine-pdt.png
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/docs/v2beta-opts.org
+-rw-r--r--   0        0        0    35115 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    24276 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/LICENSE
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.7.1/PKG-INFO
```

### Comparing `pipdeptree-2.7.0/.pre-commit-config.yaml` & `pipdeptree-2.7.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -17,39 +17,39 @@
       - id: pyupgrade
         args: ["--py37-plus"]
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         args: [--safe]
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.1]
+        additional_dependencies: [black==23.3]
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "0.6.1"
+    rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
         args: ["-p", "fix"]
   - repo: https://github.com/tox-dev/pyproject-fmt
     rev: "0.9.2"
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies:
-          - flake8-bugbear==23.3.12
-          - flake8-comprehensions==3.11.1
+          - flake8-bugbear==23.3.23
+          - flake8-comprehensions==3.12
           - flake8-pytest-style==1.7.2
           - flake8-spellcheck==0.28
           - flake8-unused-arguments==0.0.13
           - flake8-noqa==1.3.1
           - pep8-naming==0.13.3
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v2.7.1"
```

### Comparing `pipdeptree-2.7.0/CHANGES.md` & `pipdeptree-2.7.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.0/tox.ini` & `pipdeptree-2.7.1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
     py311
     py310
     py39
     py38
     py37
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.14
 
 [testenv]
 description = run the unit tests with pytest under {basepython}
-setenv =
-    COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
-    COVERAGE_PROCESS_START = {toxinidir}/setup.cfg
-    _COVERAGE_SRC = {envsitepackagesdir}/sphinx_argparse_cli
+package = wheel
+wheel_build_env = .pkg
 extras =
     graphviz
     test
+set_env =
+    COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
+    COVERAGE_PROCESS_START = {toxinidir}/setup.cfg
+    _COVERAGE_SRC = {envsitepackagesdir}/sphinx_argparse_cli
 commands =
     python -m pytest {tty:--color=yes} {posargs: \
       --junitxml {toxworkdir}{/}junit.{envname}.xml --cov {envsitepackagesdir}{/}pipdeptree \
       --cov {toxinidir}{/}tests --cov-fail-under=75 \
       --cov-config=pyproject.toml --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.2
+    pre-commit>=3.2.2
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:readme]
 description = check that the long description is valid
-basepython = python3.10
+base_python = python3.10
 skip_install = true
 deps =
     build[virtualenv]>=0.10
     twine>=4.0.2
 commands =
     python -m build --sdist --wheel -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:dev]
 description = generate a DEV environment
-usedevelop = true
+package = editable
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
 
 [flake8]
 max-complexity = 22
 max-line-length = 120
```

### Comparing `pipdeptree-2.7.0/.github/workflows/check.yml` & `pipdeptree-2.7.1/.github/workflows/check.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: check
 on:
   push:
+    tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
@@ -13,14 +14,15 @@
   test:
     name: test ${{ matrix.py }}
     runs-on: ubuntu-22.04
     strategy:
       fail-fast: false
       matrix:
         py:
+          - "3.12.0-alpha.7"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
     steps:
       - name: Install OS dependencies
@@ -89,12 +91,12 @@
           python-version: "3.11"
       - name: install build
         run: python -m pip install build
       - uses: actions/checkout@v3
       - name: build package
         run: python -m build --sdist --wheel . -o dist
       - name: publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.3
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           skip_existing: true
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `pipdeptree-2.7.0/docs/twine-pdt.png` & `pipdeptree-2.7.1/docs/twine-pdt.png`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.0/docs/v2beta-opts.org` & `pipdeptree-2.7.1/docs/v2beta-opts.org`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.0/src/pipdeptree/__init__.py` & `pipdeptree-2.7.1/src/pipdeptree/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,15 +882,15 @@
             "This option overrides all other options (except --json)."
         ),
     )
     parser.add_argument(
         "--mermaid",
         action="store_true",
         default=False,
-        help=("Display dependency tree as a Maermaid graph. " "This option overrides all other options."),
+        help=("Display dependency tree as a Mermaid graph. " "This option overrides all other options."),
     )
     parser.add_argument(
         "--graph-output",
         dest="output_format",
         help=(
             "Print a dependency graph in the specified output "
             "format. Available are all formats supported by "
```

### Comparing `pipdeptree-2.7.0/tests/test_pipdeptree.py` & `pipdeptree-2.7.1/tests/test_pipdeptree.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,24 +133,24 @@
 
 
 def test_package_dag_reverse():
     t1 = t.reverse()
     expected = {"a": [], "b": ["a", "f"], "c": ["a"], "d": ["b", "c"], "e": ["c", "d", "g"], "f": ["g"], "g": []}
     assert isinstance(t1, p.ReversedPackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t1))
-    assert all([isinstance(k, p.ReqPackage) for k in t1.keys()])
-    assert all([isinstance(v, p.DistPackage) for v in chain.from_iterable(t1.values())])
+    assert all(isinstance(k, p.ReqPackage) for k in t1.keys())
+    assert all(isinstance(v, p.DistPackage) for v in chain.from_iterable(t1.values()))
 
     # testing reversal of ReversedPackageDAG instance
     expected = {"a": ["b", "c"], "b": ["d"], "c": ["d", "e"], "d": ["e"], "e": [], "f": ["b"], "g": ["e", "f"]}
     t2 = t1.reverse()
     assert isinstance(t2, p.PackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t2))
-    assert all([isinstance(k, p.DistPackage) for k in t2.keys()])
-    assert all([isinstance(v, p.ReqPackage) for v in chain.from_iterable(t2.values())])
+    assert all(isinstance(k, p.DistPackage) for k in t2.keys())
+    assert all(isinstance(v, p.ReqPackage) for v in chain.from_iterable(t2.values()))
 
 
 # Tests for Package classes
 #
 # Note: For all render methods, we are only testing for frozen=False
 # as mocks with frozen=True are a lot more complicated
 
@@ -656,14 +656,16 @@
     implementation = platform.python_implementation()
     if implementation == "CPython":
         expected = {"pip", "setuptools", "wheel"}
     elif implementation == "PyPy":
         expected = {"cffi", "greenlet", "pip", "readline", "setuptools", "wheel"}
     else:
         raise ValueError(implementation)
+    if sys.version_info >= (3, 12):
+        expected -= {"setuptools", "wheel"}
     assert found == expected, out
 
     monkeypatch.setattr(sys, "argv", cmd + ["--graph-output", "something"])
     with pytest.raises(SystemExit) as context:
         p.main()
     out, err = capfd.readouterr()
     assert context.value.code == 1
```

### Comparing `pipdeptree-2.7.0/LICENSE` & `pipdeptree-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.0/README.md` & `pipdeptree-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.7.0/pyproject.toml` & `pipdeptree-2.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.13",
+  "hatchling>=1.14",
 ]
 
 [project]
 name = "pipdeptree"
 description = "Command line utility to show dependency tree of packages."
 readme = "README.md"
 keywords = [
@@ -37,16 +37,16 @@
 ]
 optional-dependencies.graphviz = [
   "graphviz>=0.20.1",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
   "diff-cover>=7.5",
-  "pip>=23.0.1",
-  "pytest>=7.2.2",
+  "pip>=23.1",
+  "pytest>=7.3.1",
   "pytest-cov>=4",
   "pytest-mock>=3.10",
   "virtualenv<21,>=20.21",
 ]
 urls.Changelog = "https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md"
 urls.Documentation = "https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree"
 urls.Homepage = "https://github.com/tox-dev/pipdeptree"
```

### Comparing `pipdeptree-2.7.0/PKG-INFO` & `pipdeptree-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.7.0
+Version: 2.7.1
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
@@ -40,18 +40,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Provides-Extra: graphviz
 Requires-Dist: graphviz>=0.20.1; extra == 'graphviz'
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: diff-cover>=7.5; extra == 'test'
-Requires-Dist: pip>=23.0.1; extra == 'test'
+Requires-Dist: pip>=23.1; extra == 'test'
 Requires-Dist: pytest-cov>=4; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
-Requires-Dist: pytest>=7.2.2; extra == 'test'
+Requires-Dist: pytest>=7.3.1; extra == 'test'
 Requires-Dist: virtualenv<21,>=20.21; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pipdeptree
 
 [![check](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tox-dev/pipdeptree/main.svg)](https://results.pre-commit.ci/latest/github/tox-dev/pipdeptree/main)
```

