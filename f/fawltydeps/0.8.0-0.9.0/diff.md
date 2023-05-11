# Comparing `tmp/fawltydeps-0.8.0.tar.gz` & `tmp/fawltydeps-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fawltydeps-0.8.0.tar", max compression
+gzip compressed data, was "fawltydeps-0.9.0.tar", max compression
```

## Comparing `fawltydeps-0.8.0.tar` & `fawltydeps-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1070 2023-03-21 06:52:38.586890 fawltydeps-0.8.0/LICENSE
--rw-r--r--   0        0        0    22624 2023-03-28 07:18:11.271132 fawltydeps-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-03-21 06:52:38.598950 fawltydeps-0.8.0/fawltydeps/__init__.py
--rw-r--r--   0        0        0     2237 2023-03-21 06:52:38.598950 fawltydeps-0.8.0/fawltydeps/check.py
--rw-r--r--   0        0        0     9308 2023-03-30 15:55:48.647437 fawltydeps-0.8.0/fawltydeps/cli_parser.py
--rw-r--r--   0        0        0    14944 2023-03-24 15:10:22.126937 fawltydeps-0.8.0/fawltydeps/extract_declared_dependencies.py
--rw-r--r--   0        0        0     8269 2023-03-22 13:13:09.590519 fawltydeps-0.8.0/fawltydeps/extract_imports.py
--rw-r--r--   0        0        0     4091 2023-03-21 06:52:38.598950 fawltydeps-0.8.0/fawltydeps/limited_eval.py
--rw-r--r--   0        0        0    12040 2023-03-30 15:55:48.647437 fawltydeps-0.8.0/fawltydeps/main.py
--rw-r--r--   0        0        0    13534 2023-03-30 08:08:19.412505 fawltydeps-0.8.0/fawltydeps/packages.py
--rw-r--r--   0        0        0     9350 2023-03-30 15:55:48.647437 fawltydeps-0.8.0/fawltydeps/settings.py
--rw-r--r--   0        0        0     5963 2023-03-21 16:59:15.610015 fawltydeps-0.8.0/fawltydeps/types.py
--rw-r--r--   0        0        0     1855 2023-03-29 12:36:58.021386 fawltydeps-0.8.0/fawltydeps/utils.py
--rw-r--r--   0        0        0     3959 2023-03-30 16:09:38.902639 fawltydeps-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    24224 1970-01-01 00:00:00.000000 fawltydeps-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-12-09 14:32:49.005231 fawltydeps-0.9.0/LICENSE
+-rw-r--r--   0        0        0    23816 2023-04-13 13:25:24.827813 fawltydeps-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-09 14:32:49.005231 fawltydeps-0.9.0/fawltydeps/__init__.py
+-rw-r--r--   0        0        0      961 2023-02-17 18:22:16.209652 fawltydeps-0.9.0/fawltydeps/backports.py
+-rw-r--r--   0        0        0     2237 2023-03-21 12:00:35.682847 fawltydeps-0.9.0/fawltydeps/check.py
+-rw-r--r--   0        0        0     9545 2023-04-13 13:25:24.827813 fawltydeps-0.9.0/fawltydeps/cli_parser.py
+-rw-r--r--   0        0        0    14944 2023-04-13 13:25:11.026816 fawltydeps-0.9.0/fawltydeps/extract_declared_dependencies.py
+-rw-r--r--   0        0        0     8269 2023-04-13 13:25:11.027816 fawltydeps-0.9.0/fawltydeps/extract_imports.py
+-rw-r--r--   0        0        0     4091 2023-03-21 12:00:35.682847 fawltydeps-0.9.0/fawltydeps/limited_eval.py
+-rw-r--r--   0        0        0    10972 2023-04-13 13:25:24.827813 fawltydeps-0.9.0/fawltydeps/main.py
+-rw-r--r--   0        0        0    17234 2023-04-13 13:25:24.828813 fawltydeps-0.9.0/fawltydeps/packages.py
+-rw-r--r--   0        0        0    10675 2023-04-13 13:25:24.828813 fawltydeps-0.9.0/fawltydeps/settings.py
+-rw-r--r--   0        0        0     5963 2023-04-13 13:26:41.147800 fawltydeps-0.9.0/fawltydeps/types.py
+-rw-r--r--   0        0        0     3090 2023-04-13 13:25:24.828813 fawltydeps-0.9.0/fawltydeps/utils.py
+-rw-r--r--   0        0        0     3959 2023-04-13 13:57:52.755906 fawltydeps-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    25498 1970-01-01 00:00:00.000000 fawltydeps-0.9.0/setup.py
+-rw-r--r--   0        0        0    25414 1970-01-01 00:00:00.000000 fawltydeps-0.9.0/PKG-INFO
```

### Comparing `fawltydeps-0.8.0/LICENSE` & `fawltydeps-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fawltydeps-0.8.0/README.md` & `fawltydeps-0.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,27 +36,27 @@
   For example, you have `numpy` listed in your `requirements.txt`, but you never actually `import numpy`.
   Pragmatically, this means that project installation may consume more space than needed and will be more likely to break with future software releases; in short, these are costs paid for no benefit.
 
 ## Installation
 
 The library is distributed with PyPI, so simply:
 
-```
+```sh
 pip install fawltydeps
 ```
 
 or any other way to install Python packages from PyPI should be enough to make it available in your environment.
 
 Consider adding `fawltydeps` to your development dependencies, to help you catch undeclared and unused dependencies in your projects.
 
 ## Usage
 
 To check the project in the current directory run:
 
-```
+```sh
 fawltydeps
 ```
 
 This will find imports in all the Python code under the current directory,
 extract dependencies declared by your project, and then report
 [_undeclared_ and _unused_ dependencies](#key-concepts).
 
@@ -76,24 +76,24 @@
 ### Where to find code and dependency declarations
 
 By default, FawltyDeps will look for Python code (`*.py` and `*.ipynb`) and
 dependency declarations (see list of supported files below) under the current
 directory. If you want FawltyDeps to look elsewhere, you can pass a different
 directory (aka `basepath`) as a positional argument:
 
-```
+```sh
 fawltydeps my_project/
 ```
 
 If you want to separately declare the source of the code and the source of the
 dependencies, you may use the `--code` and `--deps` options documented in the
 next section. In short, giving the `basepath` positional argument is equivalent
 to passing both the `--code` and the `--deps` options, like this:
 
-```
+```sh
 fawltydeps --code my_project/ --deps my_project/
 ```
 
 #### Where to find Python code
 
 The `--code` option tells FawltyDeps where to find the Python code to parse for
 `import` statements. You can pass any number of these:
@@ -103,15 +103,15 @@
 - `-`: Passing a single dash (`--code=-`) tells FawltyDeps to read Python code
   from stdin.
 
 If no `--code` option is passed, FawltyDeps will find all Python code under the
 `basepath`, if given, or the current directory (i.e. same as `--code=.`).
 To include both code from stdin (`import foo`) and a file path (`file.py`), use:
 
-```
+```sh
 echo "import foo" | fawltydeps --list-imports --code - file.py
 ```
 
 #### Where to find declared dependencies
 
 The `--deps` option tells FawltyDeps where to look for your project's declared
 dependencies. A number of file formats are supported:
@@ -128,55 +128,94 @@
 be searched, parsing all of the supported files (see the above list) found
 within. You would typically want to pass individual files, if you want to
 be explicit about where to find the declared dependencies.
 
 If no `--deps` option is passed, FawltyDeps will look for the above files under
 the `basepath`, if given, or the current directory (i.e. same as `--deps .`).
 
-### Resolving dependencies via your Python environment
+### Resolving dependencies
 
 When FawltyDeps looks for undeclared and unused dependencies, it needs to match
 `import` statements in your code with corresponding package dependencies
 declared in your project configuration.
 
-To solve this, FawltyDeps looks at the packages installed in your _current
+To solve this, FawltyDeps adopts several strategies: mapping provided by the user,
+identity mapping, and most powerful of all - using your python environment.
+
+#### Python environment mapping
+
+FawltyDeps looks at the packages installed in your _current
 Python environment_ and what import names each of them provide in order to
 correctly match your dependencies against your imports.
 
 The _current Python environment_ in this case is the environment in which
 FawltyDeps itself is installed. This works well when you, for example,
 `pip install fawltydeps` into the same virtualenv as your project dependencies.
 
 If you instead want FawltyDeps to look into a _different_ Python environment for
 mapping dependencies to import names, you can use the `--pyenv` option,
 for example:
 
-```
+```sh
 fawltydeps --code my_package/ --deps pyproject.toml --pyenv .venv/
 ```
 
 This will tell FawltyDeps:
 
 - to look for `import` statements in the `my_package/` directory,
 - to parse dependencies from `pyprojects.toml`, and
 - to use the Python environment at `.venv/` to map dependency names in
   `pyproject.toml` into import names used in your code under `my_package/`
 
+#### Identity mapping
+
 When FawltyDeps is unable to find an installed package that corresponds to a
 declared dependency, FawltyDeps will fall back to an "identity mapping", where
 it _assumes_ that the dependency provides a single import of the same name,
 i.e. it will expect that when you depend on `some_package`, then that should
 correspond to `import some_package` statements in your code.
 
 This fallback assumption is not always correct, but it allows FawltyDeps to
 produce results (albeit sometimes inaccurate) when the current Python
 environment does not contain all of your declared dependencies. Please see
 FAQ below about [why FawltyDeps must run in the same Python environment as your
 project dependencies](#why-must-fawltydeps-run-in-the-same-python-environment-as-my-project-dependencies).
 
+#### User-defined mapping
+
+You may define your mapping by providing a toml file with package to imports mapping,
+`my_mapping.toml`:
+
+```toml
+my-package = ["mpkg"]
+scikit-learn = ["sklearn"]
+multiple-modules = ["module1", "module2"]
+```
+
+To use your mapping, run:
+
+```sh
+fawltydeps --custom-mapping-file my_mapping.toml
+```
+
+FawltyDeps will parse `my_mapping.toml` file and use extracted mapping for matching dependencies to imports.
+
+You may also place the custom mapping in the `pyproject.toml` file of your project, inside a `[tool.fawltydeps.custom_mapping]` section, like this:
+
+```toml
+[tool.fawltydeps.custom_mapping]
+my-package = ["mpkg"]
+scikit-learn = ["sklearn"]
+multiple-modules = ["module1", "module2"]
+```
+
+Caution when using your mapping is advised. The user-defined mapping takes precedence over all other resolving strategies.
+If the mapping file has some stale mapping entries, they will not be resolved by
+Python environment resolver (which in general is the most accurate).
+
 ### Ignoring irrelevant results
 
 There may be `import` statements in your code that should not be considered an
 undeclared dependency. This might happen if you for example do a conditional
 `import` with a `try: ... except ImportError: ...` block (or similar).
 FawltyDeps is not able to recognize whether these dependencies should have been
 declared or not, but you can ask for them to be ignored with the
@@ -381,15 +420,15 @@
 ## FAQ
 
 ### I run `fawltydeps` and get some undeclared dependencies. What can I do with it?
 
 You can run a detailed report to see the exact location (file and line number), in which
 the undeclared dependencies were imported:
 
-```
+```sh
 fawltydeps --detailed
 ```
 
 and debug each occurrence. Typically an undeclared dependency can be fixed in a couple of ways:
 
 - A true undeclared dependency is fixed by _declaring_ it, e.g. adding it to your `pyproject.toml` or similar.
 - If you disagree with FawltyDeps' classification, you can always use `--ignore-undeclared` to silence the error. If you're sure this dependency should not have been reported by FawltyDeps, you may consider filing a bug report.
@@ -397,40 +436,40 @@
 ### How not to display tools like `black` and `pylint` in _unused dependencies_?
 
 By default, all packages declared as dependencies by your project are included
 in the FawltyDeps analysis, even if they only contain tools that were not meant
 to be `import`ed, but rather meant to be run by, say, in a pre-commit hook or a
 CI script. In such cases you may use either:
 
-```
+```sh
 fawltydeps --ignore-unused black pylint
 ```
 
 or add an equivalent directive to the FawltyDeps configuration in your
 `pyproject.toml` (see below).
 
 ### How can I store my `fawltydeps` command line options in a configuration file?
 
 You can run:
 
-```
+```sh
 fawltydeps --generate-toml-config
 ```
 
 to generate a `[tool.fawltydeps]` section with the current configuration that
 you can then directly copy into your `pyproject.toml`. Options that have their
 default value are commented in this output, so you have quickly see where your
 settings differ from the FawltyDeps defaults.
 
 This also works together with other command line options, so for example in the
 previous question, you could add `--generate-toml-config` to the command line
 (i.e. run `fawltydeps --ignore-unused black pylint --generate-toml-config`),
 to get this:
 
-```
+```toml
 [tool.fawltydeps]
 # Default options are commented...
 ignore_unused = ["black", "pylint"]
 ```
 
 ### How to use FawltyDeps in a monorepo?
 
@@ -440,26 +479,26 @@
 The produced report may be overwhelming and at the same time not granular enough.
 
 Instead, you should run FawltyDeps for each package separately.
 This collects dependencies and import statements for one package at a time.
 
 Having:
 
-```.
+```sh
 ├ lib1
 | ├ pyproject.toml
 | ├ ....
 ├ lib2
 | ├ pyproject.toml
 | ├ ....
 ```
 
 run for each `libX`:
 
-```
+```sh
 fawltydeps libX
 ```
 
 ### Why must FawltyDeps run in the same Python environment as my project dependencies?
 
 As explained above in the section on [resolving dependencies via your Python
 environment](#resolving-dependencies-via-your-python-environment), the core
```

### Comparing `fawltydeps-0.8.0/fawltydeps/check.py` & `fawltydeps-0.9.0/fawltydeps/check.py`

 * *Files identical despite different names*

### Comparing `fawltydeps-0.8.0/fawltydeps/cli_parser.py` & `fawltydeps-0.9.0/fawltydeps/cli_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,22 @@
         metavar="PYENV_DIR",
         help=(
             "Where to find a Python environment that has the project dependencies"
             " installed, defaults to the Python environment where FawltyDeps is"
             " installed."
         ),
     )
+    parser.add_argument(
+        "--custom-mapping-file",
+        type=Path,
+        metavar="FILE_PATH",
+        help=(
+            "Path to toml file containing mapping of dependencies to imports defined by the user."
+        ),
+    )
 
 
 def populate_parser_configuration(parser: argparse._ActionsContainer) -> None:
     """Add configuration Settings members to the command-line parser.
 
     Only `config-file` may specify default values.
     Verbosity-related options do not correspond directly to a Settings member,
```

### Comparing `fawltydeps-0.8.0/fawltydeps/extract_declared_dependencies.py` & `fawltydeps-0.9.0/fawltydeps/extract_declared_dependencies.py`

 * *Files identical despite different names*

### Comparing `fawltydeps-0.8.0/fawltydeps/extract_imports.py` & `fawltydeps-0.9.0/fawltydeps/extract_imports.py`

 * *Files identical despite different names*

### Comparing `fawltydeps-0.8.0/fawltydeps/limited_eval.py` & `fawltydeps-0.9.0/fawltydeps/limited_eval.py`

 * *Files identical despite different names*

### Comparing `fawltydeps-0.8.0/fawltydeps/main.py` & `fawltydeps-0.9.0/fawltydeps/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 minimal computation involved in setting the install_requires and extras_require
 arguments.
 """
 
 import json
 import logging
 import sys
-from functools import partial, wraps
+from functools import partial
 from operator import attrgetter
-from typing import Callable, Dict, List, Optional, TextIO, TypeVar
+from typing import Dict, List, Optional, TextIO
 
 from pydantic.json import custom_pydantic_encoder  # pylint: disable=no-name-in-module
 
 from fawltydeps import extract_imports
 from fawltydeps.check import calculate_undeclared, calculate_unused
 from fawltydeps.cli_parser import build_parser
 from fawltydeps.extract_declared_dependencies import extract_declared_dependencies
@@ -28,54 +28,22 @@
 from fawltydeps.types import (
     DeclaredDependency,
     ParsedImport,
     UndeclaredDependency,
     UnparseablePathException,
     UnusedDependency,
 )
-from fawltydeps.utils import version
+from fawltydeps.utils import calculated_once, version
 
 logger = logging.getLogger(__name__)
 
 VERBOSE_PROMPT = "For a more verbose report re-run with the `--detailed` option."
 UNUSED_DEPS_OUTPUT_PREFIX = "These dependencies appear to be unused (i.e. not imported)"
 
 
-Instance = TypeVar("Instance")
-T = TypeVar("T")
-
-
-def calculated_once(method: Callable[[Instance], T]) -> Callable[[Instance], T]:
-    """Emulate functools.cached_property for our simple use case.
-
-    functools.cached_property does not exist in Python v3.7, so we emulate the
-    simple things we need here:
-
-    Each method that uses this decorator will store its return value in an
-    instance attribute whose name is the method name prefixed with underscore.
-    The first time the property is referenced, the method will be called, its
-    return value stored in the corresponding instance attribute, and also
-    returned to the caller. All subsequent references (as long as the stored
-    value it not None) will return the instance attribute value directly,
-    without calling the method.
-    """
-
-    @wraps(method)
-    def wrapper(self: Instance) -> T:
-        cached_attr = f"_{method.__name__}"
-        cached_value: Optional[T] = getattr(self, cached_attr, None)
-        if cached_value is not None:
-            return cached_value
-        calculated: T = method(self)
-        setattr(self, cached_attr, calculated)
-        return calculated
-
-    return wrapper
-
-
 class Analysis:  # pylint: disable=too-many-instance-attributes
     """Result from FawltyDeps analysis, to be presented to the user."""
 
     def __init__(self, settings: Settings, stdin: Optional[TextIO] = None):
         self.settings = settings
         self.stdin = stdin
         self.version = version()
@@ -110,14 +78,16 @@
 
     @property
     @calculated_once
     def resolved_deps(self) -> Dict[str, Package]:
         """The resolved mapping of dependency names to provided import names."""
         return resolve_dependencies(
             (dep.name for dep in self.declared_deps),
+            custom_mapping_file=self.settings.custom_mapping_file,
+            custom_mapping=self.settings.custom_mapping,
             pyenv_path=self.settings.pyenv,
             install_deps=self.settings.install_deps,
         )
 
     @property
     @calculated_once
     def undeclared_deps(self) -> List[UndeclaredDependency]:
@@ -256,15 +226,15 @@
         analysis.is_enabled(Action.REPORT_UNDECLARED),
         analysis.is_enabled(Action.REPORT_UNUSED),
     )
 
     if analysis.settings.output_format == OutputFormat.JSON:
         analysis.print_json(stdout)
     elif analysis.settings.output_format == OutputFormat.HUMAN_DETAILED:
-        analysis.print_human_readable(sys.stdout, details=True)
+        analysis.print_human_readable(stdout, details=True)
         if exit_code == 0 and success_message:
             print(f"\n{success_message}", file=stdout)
     elif analysis.settings.output_format == OutputFormat.HUMAN_SUMMARY:
         analysis.print_human_readable(stdout, details=False)
         if exit_code == 0 and success_message:
             print(f"\n{success_message}", file=stdout)
         else:
```

### Comparing `fawltydeps-0.8.0/fawltydeps/packages.py` & `fawltydeps-0.9.0/fawltydeps/packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,24 +20,32 @@
 from importlib_metadata import (
     DistributionFinder,
     MetadataPathFinder,
     _top_level_declared,
     _top_level_inferred,
 )
 
-from fawltydeps.utils import hide_dataclass_fields
+from fawltydeps.types import CustomMapping, UnparseablePathException
+from fawltydeps.utils import calculated_once, hide_dataclass_fields
+
+if sys.version_info >= (3, 11):
+    import tomllib  # pylint: disable=no-member
+else:
+    import tomli as tomllib
+
 
 logger = logging.getLogger(__name__)
 
 
 class DependenciesMapping(str, Enum):
     """Types of dependency and imports mapping"""
 
     IDENTITY = "identity"
     LOCAL_ENV = "local_env"
+    USER_DEFINED = "user_defined"
 
 
 @dataclass
 class Package:
     """Encapsulate an installable Python package.
 
     This encapsulates the mapping between a package name (i.e. something you can
@@ -99,14 +107,91 @@
 
         Return an empty dict if this PackageResolver is unable to resolve any
         of the given packages.
         """
         raise NotImplementedError
 
 
+class UserDefinedMapping(BasePackageResolver):
+    """Use user-defined mapping loaded from a toml file"""
+
+    def __init__(
+        self,
+        mapping_path: Optional[Path] = None,
+        custom_mapping: Optional[CustomMapping] = None,
+    ) -> None:
+        self.mapping_path = mapping_path
+        if self.mapping_path and not self.mapping_path.is_file():
+            raise UnparseablePathException(
+                ctx="Given mapping path is not a file.", path=self.mapping_path
+            )
+        self.custom_mapping = custom_mapping
+        # We enumerate packages declared in the mapping _once_ and cache the result here:
+        self._packages: Optional[Dict[str, Package]] = None
+
+    @property
+    @calculated_once
+    def packages(self) -> Dict[str, Package]:
+        """Gather a custom mapping given by a user.
+
+        Mapping may come from two sources:
+        * _mapping_path_ which is a file in a given path, which is parsed to a ditionary
+        * _custom_mapping_ which is a dictionary of package to imports mapping.
+
+        This enumerates the available packages  _once_, and caches the result for
+        the remainder of this object's life in _packages.
+        """
+        custom_mapping_from_file: Dict[str, List[str]] = {}
+
+        if self.mapping_path is not None:
+            logger.debug(f"Loading user-defined mapping from {self.mapping_path}")
+            with open(self.mapping_path, "rb") as mapping_file:
+                custom_mapping_from_file = tomllib.load(mapping_file)
+
+        mapping = {
+            Package.normalize_name(name): Package(
+                name,
+                {DependenciesMapping.USER_DEFINED: set(imports)},
+            )
+            for name, imports in custom_mapping_from_file.items()
+        }
+
+        if self.custom_mapping is not None:
+            logger.debug("Applying user-defined mapping from settings.")
+
+            for name, imports in self.custom_mapping.items():
+                normalised_name = Package.normalize_name(name)
+                if normalised_name in mapping:
+                    logger.info(
+                        "Mapping for %s already found in %s. Import names "
+                        "from the configuration file are appended to ones "
+                        "found in the mapping file.",
+                        normalised_name,
+                        self.mapping_path,
+                    )
+                    mapping[normalised_name].add_import_names(
+                        *imports, mapping=DependenciesMapping.USER_DEFINED
+                    )
+                else:
+                    mapping[normalised_name] = Package(
+                        name,
+                        {DependenciesMapping.USER_DEFINED: set(imports)},
+                    )
+
+        return mapping
+
+    def lookup_packages(self, package_names: Set[str]) -> Dict[str, Package]:
+        """Convert package names to locally available Package objects."""
+        return {
+            name: self.packages[Package.normalize_name(name)]
+            for name in package_names
+            if Package.normalize_name(name) in self.packages
+        }
+
+
 class LocalPackageResolver(BasePackageResolver):
     """Lookup imports exposed by packages installed in a Python environment."""
 
     def __init__(self, pyenv_path: Optional[Path] = None) -> None:
         """Lookup packages installed in the given virtualenv.
 
         Default to the current python environment if `pyenv_path` is not given
@@ -265,14 +350,16 @@
     def lookup_packages(self, package_names: Set[str]) -> Dict[str, Package]:
         """Convert package names into Package objects w/the same import name."""
         return {name: self.lookup_package(name) for name in package_names}
 
 
 def resolve_dependencies(
     dep_names: Iterable[str],
+    custom_mapping_file: Optional[Path] = None,
+    custom_mapping: Optional[CustomMapping] = None,
     pyenv_path: Optional[Path] = None,
     install_deps: bool = False,
 ) -> Dict[str, Package]:
     """Associate dependencies with corresponding Package objects.
 
     Use LocalPackageResolver to find Package objects for each of the given
     dependencies inside the virtualenv given by 'pyenv_path'. When 'pyenv_path'
@@ -283,15 +370,23 @@
     """
     deps = set(dep_names)  # consume the iterable once
 
     # This defines the "stack" of resolvers that we will use to convert
     # dependencies into provided import names. We call .lookup_package() on
     # each resolver in order until one of them returns a Package object. At
     # that point we are happy, and don't consult any of the later resolvers.
-    resolvers: List[BasePackageResolver] = [LocalPackageResolver(pyenv_path)]
+    resolvers: List[BasePackageResolver] = []
+    if custom_mapping_file or custom_mapping:
+        resolvers.append(
+            UserDefinedMapping(
+                mapping_path=custom_mapping_file, custom_mapping=custom_mapping
+            )
+        )
+
+    resolvers.append(LocalPackageResolver(pyenv_path))
     if install_deps:
         resolvers += [TemporaryPipInstallResolver()]
     # Identity mapping being at the bottom of the resolvers stack ensures that
     # _all_ deps are matched. TODO: If we make the identity mapping optional,
     # we must remember to properly handle/signal unresolved dependencies.
     resolvers += [IdentityMapping()]
```

### Comparing `fawltydeps-0.8.0/fawltydeps/settings.py` & `fawltydeps-0.9.0/fawltydeps/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import total_ordering
 from pathlib import Path
 from typing import ClassVar, List, Optional, Set, TextIO, Tuple, Type, Union
 
 from pydantic import BaseSettings
 from pydantic.env_settings import SettingsSourceCallable  # pylint: disable=E0611
 
-from fawltydeps.types import PathOrSpecial, TomlData
+from fawltydeps.types import CustomMapping, PathOrSpecial, TomlData
 
 if sys.version_info >= (3, 11):
     import tomllib  # pylint: disable=no-member
 else:
     import tomli as tomllib
 
 logger = logging.getLogger(__name__)
@@ -118,14 +118,16 @@
     """
 
     actions: Set[Action] = {Action.REPORT_UNDECLARED, Action.REPORT_UNUSED}
     output_format: OutputFormat = OutputFormat.HUMAN_SUMMARY
     code: Set[PathOrSpecial] = {Path(".")}
     deps: Set[Path] = {Path(".")}
     pyenv: Optional[Path] = None
+    custom_mapping_file: Optional[Path] = None
+    custom_mapping: Optional[CustomMapping] = None
     ignore_undeclared: Set[str] = set()
     ignore_unused: Set[str] = set()
     deps_parser_choice: Optional[ParserChoice] = None
     install_deps: bool = False
     verbosity: int = 0
 
     # Class vars: these can not be overridden in the same way as above, only by
@@ -230,16 +232,47 @@
             name: getattr(settings, name) == default
             for name, default in defaults.items()
         }
     except AttributeError:
         logger.critical(f"Sanity check failed: {settings!r} is missing a field!")
         raise
 
-    lines = [
-        "# Copy this TOML section into your pyproject.toml to configure FawltyDeps",
-        "# (default values are commented)",
-        "[tool.fawltydeps]",
-    ] + [
-        f"{'# ' if has_default_value[name] else ''}{name} = {value!r}"
-        for name, value in simple_settings.items()
-    ]
+    dictionary_options = {"custom_mapping"}
+
+    def _option_to_toml(name, value) -> str:  # type: ignore
+        """Serialize options to toml configuration entries
+
+        Options that are of dictionary type must be given a section entry.
+        Assumption: dictionaries options are not nested.
+        """
+        comment_char = "# " if has_default_value[name] else ""
+        if name in dictionary_options:
+            toml_option = f"{comment_char}[tool.fawltydeps.{name}]"
+            if value is not None:
+                toml_option += "".join(
+                    [f"\n{comment_char}{k} = {v!r}" for k, v in value.items()]
+                )
+        else:
+            toml_option = f"{comment_char}{name} = {value!r}"
+        return toml_option
+
+    lines = (
+        [
+            "# Copy this TOML section into your pyproject.toml to configure FawltyDeps",
+            "# (default values are commented)",
+            "[tool.fawltydeps]",
+        ]
+        + [
+            _option_to_toml(name, value)
+            for name, value in simple_settings.items()
+            # First handle non-dictionary options, as we don't want them to end
+            # up inside the config section resulting from a dictionary option.
+            if name not in dictionary_options
+        ]
+        + [
+            _option_to_toml(name, value)
+            for name, value in simple_settings.items()
+            # Export dictionary options as separate TOML  config sections
+            if name in dictionary_options
+        ]
+    )
     print("\n".join(lines), file=out)
```

### Comparing `fawltydeps-0.8.0/fawltydeps/types.py` & `fawltydeps-0.9.0/fawltydeps/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from typing import Literal  # pylint: disable=no-member
 else:
     from typing_extensions import Literal
 
 SpecialPath = Literal["<stdin>"]
 PathOrSpecial = Union[SpecialPath, Path]
 TomlData = Dict[str, Any]  # type: ignore
+CustomMapping = Dict[str, List[str]]
 
 
 class UnparseablePathException(Exception):
     """Exception type when alleged path (deps or code) can't be parsed"""
 
     def __init__(self, ctx: str, path: Path):
         self.msg = f"{ctx}: {path}"
@@ -31,20 +32,20 @@
     """Reference to a source location, e.g. a file, a line within a file, etc.
 
     This is deliberately kept flexible, and the intention is for instances to
     be associated with data that originates from some input file (or even
     something read from a non-file like stdin), and carry as much or as little
     information as is appropriate about the _source_ of the associated data.
 
-    Examples include:
-     - Referring to a specific line (+ column?) in a file of Python source code
-     - Referring to a line number in anonymous Python code read from stdin
-     - Referring to a file of dependency information (e.g. pyproject.toml),
-       where a specific line number is not available (for any reason)
-     - Referring to a specific cell in a Jupyter notebook.
+    Examples include referring to:
+     - a specific line (+ column?) in a file of Python source code,
+     - a line number in anonymous Python code read from stdin,
+     - a file of dependency information (e.g. pyproject.toml) where a specific
+       line number is not available (for any reason),
+     - a specific cell in a Jupyter notebook.
 
     Instances have a string representation that reflect the level of detail
     provided, and they are sortable.
     """
 
     path: PathOrSpecial
     cellno: Optional[int] = None
```

### Comparing `fawltydeps-0.8.0/pyproject.toml` & `fawltydeps-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fawltydeps"
-version = "0.8.0"
+version = "0.9.0"
 description = "Find undeclared and unused 3rd-party dependencies in your Python project."
 authors = [
     "Maria Knorps <maria.knorps@tweag.io>",
     "Nour El Mawass <nour.elmawass@tweag.io>",
     "Johan Herland <johan.herland@tweag.io>",
     "Vince Reuter <vince.reuter@tweag.io>",
 ]
```

### Comparing `fawltydeps-0.8.0/PKG-INFO` & `fawltydeps-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fawltydeps
-Version: 0.8.0
+Version: 0.9.0
 Summary: Find undeclared and unused 3rd-party dependencies in your Python project.
 Home-page: https://github.com/tweag/FawltyDeps
 License: MIT
 Author: Maria Knorps
 Author-email: maria.knorps@tweag.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,16 +25,16 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: importlib_metadata (>=6.0.0,<7.0.0)
 Requires-Dist: isort (>=5.10,<5.12.0)
 Requires-Dist: pip-requirements-parser (>=32.0.1,<33.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0); python_version < "3.8"
 Project-URL: Repository, https://github.com/tweag/FawltyDeps
 Description-Content-Type: text/markdown
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/fawltydeps.svg)](https://pypi.org/project/fawltydeps/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/fawltydeps.svg)](https://pypi.org/project/fawltydeps/) ![Build](https://img.shields.io/github/actions/workflow/status/tweag/fawltydeps/ci.yaml) [![Licence](https://img.shields.io/pypi/l/fawltydeps.svg)](https://pypi.org/project/fawltydeps/) [![Code of conduct](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 
 # FawltyDeps
 
@@ -72,27 +72,27 @@
   For example, you have `numpy` listed in your `requirements.txt`, but you never actually `import numpy`.
   Pragmatically, this means that project installation may consume more space than needed and will be more likely to break with future software releases; in short, these are costs paid for no benefit.
 
 ## Installation
 
 The library is distributed with PyPI, so simply:
 
-```
+```sh
 pip install fawltydeps
 ```
 
 or any other way to install Python packages from PyPI should be enough to make it available in your environment.
 
 Consider adding `fawltydeps` to your development dependencies, to help you catch undeclared and unused dependencies in your projects.
 
 ## Usage
 
 To check the project in the current directory run:
 
-```
+```sh
 fawltydeps
 ```
 
 This will find imports in all the Python code under the current directory,
 extract dependencies declared by your project, and then report
 [_undeclared_ and _unused_ dependencies](#key-concepts).
 
@@ -112,24 +112,24 @@
 ### Where to find code and dependency declarations
 
 By default, FawltyDeps will look for Python code (`*.py` and `*.ipynb`) and
 dependency declarations (see list of supported files below) under the current
 directory. If you want FawltyDeps to look elsewhere, you can pass a different
 directory (aka `basepath`) as a positional argument:
 
-```
+```sh
 fawltydeps my_project/
 ```
 
 If you want to separately declare the source of the code and the source of the
 dependencies, you may use the `--code` and `--deps` options documented in the
 next section. In short, giving the `basepath` positional argument is equivalent
 to passing both the `--code` and the `--deps` options, like this:
 
-```
+```sh
 fawltydeps --code my_project/ --deps my_project/
 ```
 
 #### Where to find Python code
 
 The `--code` option tells FawltyDeps where to find the Python code to parse for
 `import` statements. You can pass any number of these:
@@ -139,15 +139,15 @@
 - `-`: Passing a single dash (`--code=-`) tells FawltyDeps to read Python code
   from stdin.
 
 If no `--code` option is passed, FawltyDeps will find all Python code under the
 `basepath`, if given, or the current directory (i.e. same as `--code=.`).
 To include both code from stdin (`import foo`) and a file path (`file.py`), use:
 
-```
+```sh
 echo "import foo" | fawltydeps --list-imports --code - file.py
 ```
 
 #### Where to find declared dependencies
 
 The `--deps` option tells FawltyDeps where to look for your project's declared
 dependencies. A number of file formats are supported:
@@ -164,55 +164,94 @@
 be searched, parsing all of the supported files (see the above list) found
 within. You would typically want to pass individual files, if you want to
 be explicit about where to find the declared dependencies.
 
 If no `--deps` option is passed, FawltyDeps will look for the above files under
 the `basepath`, if given, or the current directory (i.e. same as `--deps .`).
 
-### Resolving dependencies via your Python environment
+### Resolving dependencies
 
 When FawltyDeps looks for undeclared and unused dependencies, it needs to match
 `import` statements in your code with corresponding package dependencies
 declared in your project configuration.
 
-To solve this, FawltyDeps looks at the packages installed in your _current
+To solve this, FawltyDeps adopts several strategies: mapping provided by the user,
+identity mapping, and most powerful of all - using your python environment.
+
+#### Python environment mapping
+
+FawltyDeps looks at the packages installed in your _current
 Python environment_ and what import names each of them provide in order to
 correctly match your dependencies against your imports.
 
 The _current Python environment_ in this case is the environment in which
 FawltyDeps itself is installed. This works well when you, for example,
 `pip install fawltydeps` into the same virtualenv as your project dependencies.
 
 If you instead want FawltyDeps to look into a _different_ Python environment for
 mapping dependencies to import names, you can use the `--pyenv` option,
 for example:
 
-```
+```sh
 fawltydeps --code my_package/ --deps pyproject.toml --pyenv .venv/
 ```
 
 This will tell FawltyDeps:
 
 - to look for `import` statements in the `my_package/` directory,
 - to parse dependencies from `pyprojects.toml`, and
 - to use the Python environment at `.venv/` to map dependency names in
   `pyproject.toml` into import names used in your code under `my_package/`
 
+#### Identity mapping
+
 When FawltyDeps is unable to find an installed package that corresponds to a
 declared dependency, FawltyDeps will fall back to an "identity mapping", where
 it _assumes_ that the dependency provides a single import of the same name,
 i.e. it will expect that when you depend on `some_package`, then that should
 correspond to `import some_package` statements in your code.
 
 This fallback assumption is not always correct, but it allows FawltyDeps to
 produce results (albeit sometimes inaccurate) when the current Python
 environment does not contain all of your declared dependencies. Please see
 FAQ below about [why FawltyDeps must run in the same Python environment as your
 project dependencies](#why-must-fawltydeps-run-in-the-same-python-environment-as-my-project-dependencies).
 
+#### User-defined mapping
+
+You may define your mapping by providing a toml file with package to imports mapping,
+`my_mapping.toml`:
+
+```toml
+my-package = ["mpkg"]
+scikit-learn = ["sklearn"]
+multiple-modules = ["module1", "module2"]
+```
+
+To use your mapping, run:
+
+```sh
+fawltydeps --custom-mapping-file my_mapping.toml
+```
+
+FawltyDeps will parse `my_mapping.toml` file and use extracted mapping for matching dependencies to imports.
+
+You may also place the custom mapping in the `pyproject.toml` file of your project, inside a `[tool.fawltydeps.custom_mapping]` section, like this:
+
+```toml
+[tool.fawltydeps.custom_mapping]
+my-package = ["mpkg"]
+scikit-learn = ["sklearn"]
+multiple-modules = ["module1", "module2"]
+```
+
+Caution when using your mapping is advised. The user-defined mapping takes precedence over all other resolving strategies.
+If the mapping file has some stale mapping entries, they will not be resolved by
+Python environment resolver (which in general is the most accurate).
+
 ### Ignoring irrelevant results
 
 There may be `import` statements in your code that should not be considered an
 undeclared dependency. This might happen if you for example do a conditional
 `import` with a `try: ... except ImportError: ...` block (or similar).
 FawltyDeps is not able to recognize whether these dependencies should have been
 declared or not, but you can ask for them to be ignored with the
@@ -417,15 +456,15 @@
 ## FAQ
 
 ### I run `fawltydeps` and get some undeclared dependencies. What can I do with it?
 
 You can run a detailed report to see the exact location (file and line number), in which
 the undeclared dependencies were imported:
 
-```
+```sh
 fawltydeps --detailed
 ```
 
 and debug each occurrence. Typically an undeclared dependency can be fixed in a couple of ways:
 
 - A true undeclared dependency is fixed by _declaring_ it, e.g. adding it to your `pyproject.toml` or similar.
 - If you disagree with FawltyDeps' classification, you can always use `--ignore-undeclared` to silence the error. If you're sure this dependency should not have been reported by FawltyDeps, you may consider filing a bug report.
@@ -433,40 +472,40 @@
 ### How not to display tools like `black` and `pylint` in _unused dependencies_?
 
 By default, all packages declared as dependencies by your project are included
 in the FawltyDeps analysis, even if they only contain tools that were not meant
 to be `import`ed, but rather meant to be run by, say, in a pre-commit hook or a
 CI script. In such cases you may use either:
 
-```
+```sh
 fawltydeps --ignore-unused black pylint
 ```
 
 or add an equivalent directive to the FawltyDeps configuration in your
 `pyproject.toml` (see below).
 
 ### How can I store my `fawltydeps` command line options in a configuration file?
 
 You can run:
 
-```
+```sh
 fawltydeps --generate-toml-config
 ```
 
 to generate a `[tool.fawltydeps]` section with the current configuration that
 you can then directly copy into your `pyproject.toml`. Options that have their
 default value are commented in this output, so you have quickly see where your
 settings differ from the FawltyDeps defaults.
 
 This also works together with other command line options, so for example in the
 previous question, you could add `--generate-toml-config` to the command line
 (i.e. run `fawltydeps --ignore-unused black pylint --generate-toml-config`),
 to get this:
 
-```
+```toml
 [tool.fawltydeps]
 # Default options are commented...
 ignore_unused = ["black", "pylint"]
 ```
 
 ### How to use FawltyDeps in a monorepo?
 
@@ -476,26 +515,26 @@
 The produced report may be overwhelming and at the same time not granular enough.
 
 Instead, you should run FawltyDeps for each package separately.
 This collects dependencies and import statements for one package at a time.
 
 Having:
 
-```.
+```sh
 ├ lib1
 | ├ pyproject.toml
 | ├ ....
 ├ lib2
 | ├ pyproject.toml
 | ├ ....
 ```
 
 run for each `libX`:
 
-```
+```sh
 fawltydeps libX
 ```
 
 ### Why must FawltyDeps run in the same Python environment as my project dependencies?
 
 As explained above in the section on [resolving dependencies via your Python
 environment](#resolving-dependencies-via-your-python-environment), the core
```

