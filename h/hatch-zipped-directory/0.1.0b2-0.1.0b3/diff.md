# Comparing `tmp/hatch_zipped_directory-0.1.0b2.tar.gz` & `tmp/hatch_zipped_directory-0.1.0b3.tar.gz`

## Comparing `hatch_zipped_directory-0.1.0b2.tar` & `hatch_zipped_directory-0.1.0b3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/.flake8
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/CHANGES.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/README.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/builder.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/hooks.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/metadata.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/utils.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/tests/test_builder.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/tests/test_hooks.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/tests/test_utils.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/LICENSE.txt
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/hatch_build.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/.flake8
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/CHANGES.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/README.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/__init__.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/builder.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/hooks.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/metadata.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/utils.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/tests/test_builder.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/tests/test_hooks.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/tests/test_metadata.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/tests/test_utils.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/LICENSE.txt
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/hatch_build.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 hatch_zipped_directory-0.1.0b3/PKG-INFO
```

### Comparing `hatch_zipped_directory-0.1.0b2/README.md` & `hatch_zipped_directory-0.1.0b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # hatch-zipped-directory
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-zipped-directory.svg)](https://pypi.org/project/hatch-zipped-directory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-zipped-directory.svg)](https://pypi.org/project/hatch-zipped-directory)
 [![Tests](https://github.com/dairiki/hatch-zipped-directory/actions/workflows/tests.yml/badge.svg)](https://github.com/dairiki/hatch-zipped-directory/actions/workflows/tests.yml)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhautvz4zffrt8jawcpl)](https://trackgit.com)
 
 -----
 
 This is a [Hatch](https://hatch.pypa.io/latest/) plugin that provides
 a custom builder to support building zip archives for quasi-manual
 installation into various foreign package installation systems.
 (Specifically, I use this for packaging
```

### Comparing `hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/builder.py` & `hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 from typing import Any
 from typing import Callable
 from typing import Iterable
 from typing import Iterator
 from zipfile import ZIP_DEFLATED
 from zipfile import ZipFile
 
+from hatchling.builders.config import BuilderConfig
 from hatchling.builders.plugin.interface import BuilderInterface
 from hatchling.builders.plugin.interface import IncludedFile
 from hatchling.builders.utils import normalize_relative_path
+from hatchling.metadata.spec import DEFAULT_METADATA_VERSION
+from hatchling.metadata.spec import get_core_metadata_constructors
 
-from .metadata import json_metadata_2_1
+from .metadata import metadata_to_json
 from .utils import atomic_write
 
 __all__ = ["ZippedDirectoryBuilder"]
 
 
 class ZipArchive:
     def __init__(self, zipfd: ZipFile, root_path: str):
@@ -39,17 +42,42 @@
     @contextmanager
     def open(cls, dst: str | os.PathLike[str], root_path: str) -> Iterator[ZipArchive]:
         with atomic_write(dst) as fp:
             with ZipFile(fp, "w", compression=ZIP_DEFLATED) as zipfd:
                 yield cls(zipfd, root_path)
 
 
+class ZippedDirectoryBuilderConfig(BuilderConfig):
+    @property
+    def core_metadata_constructor(self):
+        core_metadata_version = self.target_config.get(
+            "core-metadata-version", DEFAULT_METADATA_VERSION
+        )
+        if not isinstance(core_metadata_version, str):
+            raise TypeError(
+                f"Field `tool.hatch.build.targets.{self.plugin_name}."
+                "core-metadata-version` must be a string"
+            )
+        constructors = get_core_metadata_constructors()
+        if core_metadata_version not in constructors:
+            raise ValueError(
+                f"Unknown metadata version `{core_metadata_version}` for field "
+                f"`tool.hatch.build.targets.{self.plugin_name}.core-metadata-version`. "
+                f'Available: {", ".join(sorted(constructors))}'
+            )
+        return constructors[core_metadata_version]
+
+
 class ZippedDirectoryBuilder(BuilderInterface):
     PLUGIN_NAME = "zipped-directory"
 
+    @classmethod
+    def get_config_class(cls):
+        return ZippedDirectoryBuilderConfig
+
     def get_version_api(self) -> dict[str, Callable[..., str]]:
         return {"standard": self.build_standard}
 
     def clean(self, directory: str, versions: Iterable[str]) -> None:
         for filename in os.listdir(directory):
             if filename.endswith(".zip"):
                 os.remove(os.path.join(directory, filename))
@@ -59,18 +87,19 @@
         target = Path(directory, f"{project_name}-{self.metadata.version}.zip")
 
         install_name: str = build_data["install_name"]
 
         with ZipArchive.open(target, install_name) as archive:
             for included_file in self.recurse_included_files():
                 archive.add_file(included_file)
-            archive.write_file(
-                "METADATA.json",
-                json.dumps(json_metadata_2_1(self.metadata), indent=2),
+
+            json_metadata = metadata_to_json(
+                self.config.core_metadata_constructor(self.metadata)
             )
+            archive.write_file("METADATA.json", json.dumps(json_metadata, indent=2))
         return os.fspath(target)
 
     def get_default_build_data(self) -> dict[str, Any]:
         build_data: dict[str, Any] = super().get_default_build_data()
 
         extra_files = []
         if self.metadata.core.readme_path:
```

### Comparing `hatch_zipped_directory-0.1.0b2/hatch_zipped_directory/utils.py` & `hatch_zipped_directory-0.1.0b3/hatch_zipped_directory/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_zipped_directory-0.1.0b2/tests/test_builder.py` & `hatch_zipped_directory-0.1.0b3/tests/test_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import re
 from pathlib import Path
 from zipfile import ZipFile
 
 import pytest
 from hatchling.builders.plugin.interface import IncludedFile
 from hatchling.metadata.core import ProjectMetadata
 
@@ -123,14 +124,32 @@
 
 
 @pytest.fixture
 def builder(project_root, project_metadata):
     return ZippedDirectoryBuilder(project_root, metadata=project_metadata)
 
 
+@pytest.mark.parametrize("target_config", [{"core-metadata-version": "2.2"}])
+def test_config_core_metadata_constructor(builder):
+    metadata = builder.config.core_metadata_constructor(builder.metadata)
+    assert re.search(r"(?im)^Metadata-Version: 2.2$", metadata)
+
+
+@pytest.mark.parametrize("target_config", [{"core-metadata-version": None}])
+def test_config_core_metadata_constructor_type_error(builder):
+    with pytest.raises(TypeError, match="must be a string"):
+        builder.config.core_metadata_constructor(builder.metadata)
+
+
+@pytest.mark.parametrize("target_config", [{"core-metadata-version": "42.203"}])
+def test_config_core_metadata_constructor_value_error(builder):
+    with pytest.raises(ValueError, match="(?i)unknown metadata version"):
+        builder.config.core_metadata_constructor(builder.metadata)
+
+
 def test_ZippedDirectoryBuilder_clean(builder, tmp_path):
     dist_path = tmp_path / "dist"
     dist_path.mkdir()
     dist_path.joinpath("foo.whl").touch()
     dist_path.joinpath("bar.zip").touch()
 
     builder.clean(os.fspath(dist_path), ["standard"])
```

### Comparing `hatch_zipped_directory-0.1.0b2/tests/test_utils.py` & `hatch_zipped_directory-0.1.0b3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_zipped_directory-0.1.0b2/LICENSE.txt` & `hatch_zipped_directory-0.1.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_zipped_directory-0.1.0b2/hatch_build.py` & `hatch_zipped_directory-0.1.0b3/hatch_build.py`

 * *Files identical despite different names*

### Comparing `hatch_zipped_directory-0.1.0b2/pyproject.toml` & `hatch_zipped_directory-0.1.0b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -55,15 +55,21 @@
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 full = [
     "pip freeze | paste -sd , -",
-    "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=hatch_zipped_directory --cov=tests",
+    """pytest \
+        --cov-fail-under=100 \
+        --cov-report=term-missing \
+        --cov-config=pyproject.toml \
+        --cov=hatch_zipped_directory \
+        --cov=tests
+    """,
 ]
 
 [tool.hatch.envs.dev]
 extra-dependencies = [
   "flake8",
   "flake8-bugbear",
   "mypy",
```

### Comparing `hatch_zipped_directory-0.1.0b2/PKG-INFO` & `hatch_zipped_directory-0.1.0b3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-zipped-directory
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: A custom builder to build zipped directories
 Project-URL: Homepage, https://github.com/dairiki/hatch-zipped-directory
 Author-email: Jeff Dairiki <dairiki@dairiki.org>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: hatch,packaging
 Classifier: Development Status :: 4 - Beta
@@ -26,14 +26,15 @@
 Description-Content-Type: text/markdown
 
 # hatch-zipped-directory
 
 [![PyPI - Version](https://img.shields.io/pypi/v/hatch-zipped-directory.svg)](https://pypi.org/project/hatch-zipped-directory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hatch-zipped-directory.svg)](https://pypi.org/project/hatch-zipped-directory)
 [![Tests](https://github.com/dairiki/hatch-zipped-directory/actions/workflows/tests.yml/badge.svg)](https://github.com/dairiki/hatch-zipped-directory/actions/workflows/tests.yml)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhautvz4zffrt8jawcpl)](https://trackgit.com)
 
 -----
 
 This is a [Hatch](https://hatch.pypa.io/latest/) plugin that provides
 a custom builder to support building zip archives for quasi-manual
 installation into various foreign package installation systems.
 (Specifically, I use this for packaging
@@ -127,14 +128,30 @@
 
 `hatch-zipped-directory` is distributed under the terms of the
 [MIT](https://spdx.org/licenses/MIT.html) license.
 
 
 ## Changes
 
+### 0.1.0b3 (2023-05-10)
+
+#### Features
+
+- Refactor JSON metadata code. Now we use `hatchling` to generate
+  conventionall RFC 822-formatted distribution metadata, then convert
+  that to JSON, explicitly following the steps outline in [PEP
+  566](https://peps.python.org/pep-0566/#json-compatible-metadata).
+  Among other things, this allows configuration of the
+  *Metadata-Version* by setting
+  `tool.hatch.build.targets.zipped-directory.core-metadata-version`.
+
+#### Tests
+
+- We now have 100% test coverage.
+
 ### 0.1.0b2 (2023-01-10)
 
 #### Features
 
 - The prefixing of file names under a top-level directory in the zip
   archive can now be disabled by setting `install-name = ""`.
   Thank you @gwerbin([#1][])
```

