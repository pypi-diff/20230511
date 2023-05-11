# Comparing `tmp/pyalpa-0.8.0.tar.gz` & `tmp/pyalpa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.8.0.tar", max compression
+gzip compressed data, was "pyalpa-0.9.0.tar", max compression
```

## Comparing `pyalpa-0.8.0.tar` & `pyalpa-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-04-12 21:05:18.616059 pyalpa-0.8.0/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-12 21:05:18.616059 pyalpa-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/__init__.py
--rw-r--r--   0        0        0      732 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1249 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/base.py
--rw-r--r--   0        0        0     6243 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/cli/local_repo.py
--rw-r--r--   0        0        0      227 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/__init__.py
--rw-r--r--   0        0        0     1264 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/alpa_local.py
--rw-r--r--   0        0        0     2184 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/alpa_repo.py
--rw-r--r--   0        0        0     1157 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/base.py
--rw-r--r--   0        0        0     2759 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/metadata.py
--rw-r--r--   0        0        0     2790 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/config/packit.py
--rw-r--r--   0        0        0     1233 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/constants.py
--rw-r--r--   0        0        0      158 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/exceptions.py
--rw-r--r--   0        0        0     4021 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/gh.py
--rw-r--r--   0        0        0     2463 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/git.py
--rw-r--r--   0        0        0     1447 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/messages.py
--rw-r--r--   0        0        0        0 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/__init__.py
--rw-r--r--   0        0        0    11699 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/base.py
--rw-r--r--   0        0        0     4536 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/branch.py
--rw-r--r--   0        0        0     1661 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/repository/subdirectory.py
--rw-r--r--   0        0        0     3879 2023-04-12 21:05:18.616059 pyalpa-0.8.0/alpa/upstream_integration.py
--rw-r--r--   0        0        0      846 2023-04-12 21:05:18.616059 pyalpa-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 pyalpa-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-11 20:59:18.638701 pyalpa-0.9.0/LICENSE
+-rw-r--r--   0        0        0      683 2023-05-11 20:59:18.638701 pyalpa-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1203 2023-05-11 20:59:18.638701 pyalpa-0.9.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6810 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      160 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1264 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2649 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/base.py
+-rw-r--r--   0        0        0     3344 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/config/metadata.py
+-rw-r--r--   0        0        0     1233 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     4055 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/gh.py
+-rw-r--r--   0        0        0     2735 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/git.py
+-rw-r--r--   0        0        0     1553 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/messages.py
+-rw-r--r--   0        0        0     2956 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/packit.py
+-rw-r--r--   0        0        0      298 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    12145 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/base.py
+-rw-r--r--   0        0        0     5810 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1666 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-05-11 20:59:18.642701 pyalpa-0.9.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      846 2023-05-11 20:59:18.646701 pyalpa-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 pyalpa-0.9.0/PKG-INFO
```

### Comparing `pyalpa-0.8.0/LICENSE` & `pyalpa-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/alpa/cli/alpa_repo.py` & `pyalpa-0.9.0/alpa/cli/alpa_repo.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/alpa/cli/base.py` & `pyalpa-0.9.0/alpa/cli/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from alpa.cli.local_repo import (
     show_history,
     switch,
     commit,
     pull,
     push,
     list_,
-    genspec,
     add,
     get_pkg_archive,
     mockbuild,
     create_packit_config,
 )
 from alpa.repository.branch import AlpaRepoBranch
 
@@ -41,15 +40,14 @@
 
 entry_point.add_command(show_history)
 entry_point.add_command(switch)
 entry_point.add_command(commit)
 entry_point.add_command(pull)
 entry_point.add_command(push)
 entry_point.add_command(list_)
-entry_point.add_command(genspec)
 entry_point.add_command(add)
 entry_point.add_command(get_pkg_archive)
 entry_point.add_command(mockbuild)
 entry_point.add_command(create_packit_config)
 
 
 if __name__ == "__main__":
```

### Comparing `pyalpa-0.8.0/alpa/cli/local_repo.py` & `pyalpa-0.9.0/alpa/cli/local_repo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 These commands need to create LocalRepo -> no GH token required
 """
+import os
+import subprocess
 from os import getcwd
 from pathlib import Path
+from shutil import which
 
 import click
-from click import ClickException, Choice
-from specfile import Specfile
+from click import ClickException
 
-from alpa.config import MetadataConfig, PackitConfig
+from alpa.config import MetadataConfig
 from alpa.repository.branch import LocalRepoBranch, AlpaRepoBranch
-from alpa.upstream_integration import UpstreamIntegration
+
+from alpa.messages import NO_PRE_COMMIT
 
 pkg_name = click.argument("name", type=str)
 
 
 @click.command("show-history")
 @click.option(
     "-o",
@@ -61,43 +64,57 @@
 @click.command("add")
 @click.argument("to_add", type=str, required=True)
 def add(to_add: str) -> None:
     """Add files to git history. Basically calls `git add <input>`"""
     LocalRepoBranch(Path(getcwd())).add(to_add)
 
 
+def _skip_pre_commit_checks_for_non_rpm_os() -> None:
+    process = subprocess.run(
+        ["rpm", "--help"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+    )
+    if process.returncode != 0:
+        # no special pre-commit hooks for non-RPM OS :/
+        disabled_checks = ["source0-uses-version-macro", "check-packit-file"]
+        click.secho(
+            "Warning! You don't have RPM based OS, these checks are "
+            f"disabled: {disabled_checks}",
+            fg="yellow",
+        )
+        os.environ["SKIP"] = ",".join(disabled_checks)
+
+
 @click.command("push")
 @click.option(
     "-p",
     "--pull-request",
     is_flag=True,
     show_default=True,
     default=False,
     help="This will create pull request on GitHub for you.",
 )
-def push(pull_request: bool) -> None:
+@click.option("-n", "--no-verify", is_flag=True, help="Do not run pre-commit")
+def push(pull_request: bool, no_verify: bool) -> None:
     """Pushes your commited changes to the Alpa repo so you can make PR"""
+    if not no_verify:
+        if which("pre-commit") is None:
+            click.secho(NO_PRE_COMMIT, fg="red", err=True)
+            return
+
+        _skip_pre_commit_checks_for_non_rpm_os()
+        ret = subprocess.run(["pre-commit", "run", "--all-files"])
+        if ret.returncode != 0:
+            # pre-commit already gives info about fail
+            return
+
     repo_path = Path(getcwd())
     local_repo = LocalRepoBranch(repo_path)
-
-    packit_conf = PackitConfig(local_repo.package)
-    if not packit_conf.packit_config_file_exists():
-        packit_conf.create_packit_config()
-        local_repo.git_cmd(["add", ".packit.yaml"])
-        local_repo.git_cmd(
-            [
-                "commit",
-                '-m "alpa: automatically add .packit.yaml config to the package"',
-            ]
-        )
-
     local_repo.push(local_repo.branch)
 
     if not pull_request:
-        local_repo.git_cmd(["branch", "-d", local_repo.feat_branch])
         return
 
     alpa = AlpaRepoBranch(repo_path)
     pr = alpa.gh_repo.create_pr(
         title=f"[alpa-cli] Create update of package {local_repo.package}",
         body=(
             "This PR was created automatically via alpa-cli for "
@@ -120,33 +137,34 @@
 @click.option("-p", "--pattern", type=str, default="", help="Optional pattern to match")
 def list_(pattern: str) -> None:
     """List all packages or packages matching regex"""
     for pkg in LocalRepoBranch(Path(getcwd())).get_packages(pattern):
         click.echo(pkg)
 
 
-@click.command("genspec")
-@click.option(
-    "--lang",
-    type=Choice(["python", "java"], case_sensitive=False),
-    required=True,
-    help="Choose the programming language for which the generator is designed",
-)
-@click.option(
-    "-t",
-    "--test",
-    default=False,
-    help=(
-        "Send package with generated spec file to "
-        "packit to test whether build will succeed."
-    ),
-)
-def genspec(lang: str, test: bool) -> None:
-    """This command uses some existing spec file generators for you"""
-    raise NotImplementedError("Not implemented yet (1.0 goal)")
+# TODO: please implement me
+# @click.command("genspec")
+# @click.option(
+#     "--lang",
+#     type=Choice(["python", "java"], case_sensitive=False),
+#     required=True,
+#     help="Choose the programming language for which the generator is designed",
+# )
+# @click.option(
+#     "-t",
+#     "--test",
+#     default=False,
+#     help=(
+#         "Send package with generated spec file to "
+#         "packit to test whether build will succeed."
+#     ),
+# )
+# def genspec(lang: str, test: bool) -> None:
+#     """This command uses some existing spec file generators for you"""
+#     raise NotImplementedError("Not implemented yet (1.0 goal)")
 
 
 @click.command("create-packit-config")
 @click.option(
     "--override",
     is_flag=True,
     show_default=True,
@@ -157,45 +175,44 @@
     """Creates packit config based on metadata.yaml file in package"""
     if not LocalRepoBranch(Path(getcwd())).create_packit_config(override):
         raise ClickException(
             "Packit file already exists. To override it use --override flag."
         )
 
 
-def _get_chroots_to_build(meta: MetadataConfig, distros: list[str]) -> list[str]:
-    chroots = []
-    for arch in meta.arch:
-        for distro in distros:
-            chroots.append(f"{distro}-{arch}")
-    return chroots
-
-
 @click.command("mockbuild")
 @click.option(
     "--chroot",
     type=str,
     default="",
     help="Override chroots specified in metadata.yaml by one specific chroot",
 )
 def mockbuild(chroot: str) -> None:
     """
     Uses mock tool to build package. WARNING: works only on rpm-based systems.
 
     Builds for all chroots specified in metadata.yaml. Can be overriden by --chroot
      option which does build against one specified chroot.
     """
-    meta = MetadataConfig.get_config()
-    distros = [chroot] if chroot else list(meta.targets)
-    chroots = _get_chroots_to_build(meta, distros)
+    from alpa.upstream_integration import UpstreamIntegration
+
+    if chroot:
+        chroots = [chroot]
+    else:
+        chroots = MetadataConfig.get_config().chroots
+
     UpstreamIntegration(Path(getcwd())).mockbuild(chroots)
 
 
 @click.command("get-pkg-archive")
 def get_pkg_archive() -> None:
-    """Gets archive from package config"""
+    """Gets archive from package config. WARNING: works only on rpm-based systems."""
+    from specfile import Specfile
+    from alpa.upstream_integration import UpstreamIntegration
+
     specfile_path = None
     cwd = Path(getcwd())
     for file in cwd.iterdir():
         if str(file).endswith(".spec"):
             specfile_path = file
 
     if specfile_path is None:
```

### Comparing `pyalpa-0.8.0/alpa/config/alpa_local.py` & `pyalpa-0.9.0/alpa/config/alpa_local.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/alpa/config/alpa_repo.py` & `pyalpa-0.9.0/alpa/config/alpa_repo.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,30 +23,46 @@
 class AlpaRepoConfig(Config):
     def __init__(
         self,
         repo_type: AlpaRepoType,
         copr_owner: str,
         copr_repo: str,
         allow_foreign_contributing: bool = False,
+        targets: Optional[set[str]] = None,
+        arch: Optional[set[str]] = None,
     ) -> None:
         self.repo_type = repo_type
         self.copr_owner = copr_owner
         self.copr_repo = copr_repo
+
+        # optional parameters
         self.allow_foreign_contributing = allow_foreign_contributing
+        self.targets = targets
+        self.arch = arch
 
     @classmethod
     def _config_from_dict(cls, d: dict) -> "AlpaRepoConfig":
         for mandatory_key in ["repo_type", "copr_owner", "copr_repo"]:
             cls._check_for_mandatory_key(d, mandatory_key, "alpa.yaml")
 
+        targets = d.get("targets")
+        if targets is not None:
+            targets = set(targets)
+
+        arch = d.get("arch")
+        if arch is not None:
+            arch = set(arch)
+
         return AlpaRepoConfig(
             repo_type=AlpaRepoType[d["repo_type"]],
             copr_owner=d["copr_owner"],
             copr_repo=d["copr_repo"],
             allow_foreign_contributing=d.get("allow_foreign_contributing", False),
+            targets=targets,
+            arch=arch,
         )
 
     @classmethod
     def _load_alpa_config(cls, pwd: Path) -> Optional["AlpaRepoConfig"]:
         config_file_path = cls.get_config_file_path(pwd, ALPA_CONFIG_FILE_NAMES)
         if config_file_path is None:
             return None
@@ -60,12 +76,14 @@
             ["git", "rev-parse", "--show-toplevel"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         if process.returncode != 0:
             raise AlpaConfException(process.stderr)
 
-        alpa_config = cls._load_alpa_config(Path(process.stdout.decode().strip()))
+        alpa_config = cls._load_alpa_config(
+            Path("/home/jkyjovsk/Documents/git/github/alpa/test-branch-repo")
+        )
         if alpa_config is None:
             raise FileNotFoundError("No alpa config file in git root found")
 
         return alpa_config
```

### Comparing `pyalpa-0.8.0/alpa/config/base.py` & `pyalpa-0.9.0/alpa/config/base.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/alpa/config/packit.py` & `pyalpa-0.9.0/alpa/packit.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,59 +10,64 @@
 from yaml import dump
 
 from alpa.config import AlpaRepoConfig, MetadataConfig
 
 from alpa.constants import PACKIT_CONFIG_NAMES
 
 
-class PackitConfig:
+class Packit:
     def __init__(self, package_name: str) -> None:
         self.package_name = package_name
         self.working_dir = Path(getcwd())
         self.metadata = MetadataConfig.get_config(self.working_dir)
         self.alpa_repo_config = AlpaRepoConfig.get_config()
 
     def get_packit_config(self) -> dict:
+        targets_with_arch = []
+        for arch in self.metadata.arch:
+            for target in self.metadata.targets:
+                targets_with_arch.append(f"{target}-{arch}")
+
         jobs = [
             {
                 "job": "copr_build",
                 "trigger": "pull_request",
-                "targets": list(self.metadata.targets),
+                "targets": targets_with_arch,
                 "owner": self.alpa_repo_config.copr_owner,
                 "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
             },
             {
                 "job": "copr_build",
                 "trigger": "commit",
                 "branch": self.package_name,
-                "targets": list(self.metadata.targets),
+                "targets": targets_with_arch,
                 "owner": self.alpa_repo_config.copr_owner,
                 "project": self.alpa_repo_config.copr_repo,
             },
         ]
 
         if self.metadata.autoupdate is not None:
             autoupdate_dict = {
                 "job": "copr_build",
                 "trigger": "commit",
                 "branch": f"__alpa_autoupdate_{self.package_name}",
-                "targets": list(self.metadata.targets),
+                "targets": targets_with_arch,
                 "owner": self.alpa_repo_config.copr_owner,
                 "project": f"{self.alpa_repo_config.copr_repo}-pull-requests",
             }
             jobs.append(autoupdate_dict)
 
         return {
             "specfile_path": f"{self.package_name}.spec",
             "srpm_build_deps": ["pip"],
             "actions": {
                 "create-archive": [
                     "pip install pyalpa",
                     'bash -c "alpa get-pkg-archive"',
-                    f'bash -c "ls -1 ./{self.package_name}-*.tar.gz"',
+                    'bash -c "ls -1 ./*.tar.gz"',
                 ],
             },
             "jobs": jobs,
         }
 
     def packit_config_file_exists(self) -> bool:
         for packit_config_name in PACKIT_CONFIG_NAMES:
@@ -70,13 +75,13 @@
                 file.name for file in self.working_dir.iterdir() if file.is_file()
             ]
             if packit_config_name in files_in_dir:
                 return True
 
         return False
 
-    def create_packit_config(self) -> None:
-        if self.packit_config_file_exists():
+    def create_packit_config(self, override: bool = False) -> None:
+        if not override and self.packit_config_file_exists():
             raise FileExistsError("Packit configuration file already exists")
 
         with open(".packit.yaml", "w") as packit_yaml:
             packit_yaml.write(dump(self.get_packit_config(), sort_keys=False))
```

### Comparing `pyalpa-0.8.0/alpa/constants.py` & `pyalpa-0.9.0/alpa/constants.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/alpa/gh.py` & `pyalpa-0.9.0/alpa/gh.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,19 @@
         self._repo = api.get_repo(f"{namespace}/{repo_name}")
 
     @property
     def clone_url(self) -> str:
         if self.has_write_access(self._api.get_user().login):
             return self._repo.ssh_url
 
-        click.echo(
+        click.secho(
             RETURNING_CLONE_URL_MSG.format(
                 user=self._api.get_user().login, repo=self._repo.full_name
-            )
+            ),
+            fg="bright_yellow",
         )
         return self._repo.clone_url
 
     @property
     def upstream_clone_url(self) -> Optional[str]:
         upstream = self.get_upstream()
         if upstream is None:
```

### Comparing `pyalpa-0.8.0/alpa/git.py` & `pyalpa-0.9.0/alpa/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,29 @@
 
 @dataclass
 class GitCmdResult:
     stdout: str
     stderr: str
     retval: int
 
+    @property
+    def stderr_and_stdout(self) -> str:
+        result = ""
+        if self.stdout:
+            result += self.stdout
+
+        if not self.stderr:
+            return result
+
+        if result:
+            result += "\n"
+
+        result += self.stderr
+        return result
+
 
 class GitCMD:
     def __init__(self, cwd: str) -> None:
         self.git_root = cwd
         output = self.git_cmd(["rev-parse", "--show-toplevel"])
         if "not a git repository" in output.stderr:
             raise FileNotFoundError(output.stderr)
@@ -36,16 +51,16 @@
             context = cwd
 
         logger.debug(
             f"Running git cmd: $ git {' '.join(arguments)}; in context {context}"
         )
         process = subprocess.run(
             ["git"] + arguments,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
             cwd=context,
         )
         stdout = process.stdout.decode()
         stderr = process.stderr.decode()
         logger.debug(
             f"git cmd results: stdout: {stdout}; stderr: {stderr}; "
             f"retval: {process.returncode}"
```

### Comparing `pyalpa-0.8.0/alpa/messages.py` & `pyalpa-0.9.0/alpa/messages.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,7 +36,11 @@
     "back to its predefined state."
 )
 
 RETURNING_CLONE_URL_MSG = (
     "User {user} does not have access to {repo} repository. "
     "Using https url for cloning instead of ssh url."
 )
+
+NO_PRE_COMMIT = (
+    "pre-commit is not installed! Please install " "it via `pip install pre-commit`"
+)
```

### Comparing `pyalpa-0.8.0/alpa/repository/base.py` & `pyalpa-0.9.0/alpa/repository/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path
 from typing import Optional, Iterable
 from urllib.parse import urlparse
 
 from click import UsageError, ClickException
 import click
 
+from alpa.packit import Packit
 from alpa.constants import (
     ALPA_FEAT_BRANCH,
     ALPA_FEAT_BRANCH_PREFIX,
     ORIGIN_NAME,
     UPSTREAM_NAME,
 )
 from alpa.gh import GithubAPI, GithubRepo
@@ -47,15 +48,15 @@
         logger.debug(f"Remote name for this repository is set to {self.remote_name}")
 
         # lazy properties
         self._namespace: Optional[str] = None
         self._repo_name: Optional[str] = None
 
     @abstractmethod
-    def get_packages(self, regex: str) -> list[str]:
+    def get_packages(self, regex: str = "") -> list[str]:
         pass
 
     @abstractmethod
     def switch_to_package(self, package: str) -> None:
         pass
 
     @abstractmethod
@@ -233,37 +234,49 @@
         logger.debug(f"Branch {branch} does not exist in {branches}")
         return False
 
     def get_history_of_branch(self, branch: str, params: list[str]) -> str:
         return self.git_cmd(["log", "--decorate", "--graph"] + params + [branch]).stdout
 
     def commit(self, message: str, pre_commit: bool) -> bool:
-        if pre_commit:
-            ret = subprocess.run(["pre-commit", "run", "--all-files"])
-            if ret.returncode != 0:
-                return False
+        packit_conf = Packit(self.package)
+        if not packit_conf.packit_config_file_exists():
+            packit_conf.create_packit_config()
+            self.git_cmd(["add", ".packit.yaml"])
+            self.git_cmd(
+                [
+                    "commit",
+                    "-m",
+                    "alpa: automatically add .packit.yaml config to the package",
+                    ".packit.yaml",
+                ]
+            )
 
         self._ensure_feature_branch()
         if message:
             self.git_cmd(["commit", "-m", message])
         else:
             self.git_cmd(["commit"])
 
         return True
 
     def add(self, to_add: str) -> None:
         self._ensure_feature_branch()
-        self.git_cmd(["add", to_add])
+        self.git_cmd(["add"] + to_add.split())
 
     def pull(self, branch: str) -> None:
-        click.echo(self.git_cmd(["pull", self.remote_name, branch]).stdout)
+        click.echo(self.git_cmd(["pull", self.remote_name, branch]).stderr_and_stdout)
 
-    def push(self, branch: str) -> None:
+    def push(self, branch: str, force: bool = False) -> None:
         # you always want to push to origin, even from a fork
-        click.echo(self.git_cmd(["push", ORIGIN_NAME, branch]).stdout)
+        cmd = ["push", ORIGIN_NAME, branch]
+        if force:
+            cmd.append("--force")
+
+        click.echo(self.git_cmd(cmd).stderr_and_stdout)
 
     @staticmethod
     def _parse_reponame_from_url(url: str) -> str:
         without_git_suffix = url.removesuffix(".git")
         if without_git_suffix.startswith("https://") or without_git_suffix.startswith(
             "http://"
         ):
```

### Comparing `pyalpa-0.8.0/alpa/repository/branch.py` & `pyalpa-0.9.0/alpa/repository/branch.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 import re
 from typing import Optional, Type
 
 from click import ClickException
 import click
 
-from alpa.config import PackitConfig
+from alpa.packit import Packit
 from alpa.constants import (
     ALPA_FEAT_BRANCH_PREFIX,
     MAIN_BRANCH,
     PackageRequest,
     DeleteRequest,
     REQUEST_LABEL,
 )
@@ -30,71 +30,108 @@
     @property
     def package(self) -> str:
         return self.branch.removeprefix(ALPA_FEAT_BRANCH_PREFIX)
 
     def get_history_of_package(self, package: str) -> str:
         raise NotImplementedError("Please implement me!")
 
-    def get_packages(self, regex: str) -> list[str]:
+    def get_packages(self, regex: str = "") -> list[str]:
         refs_without_main = filter(
             lambda ref: ref != "main", self.get_remote_branches(self.remote_name)
         )
         relevant_refs = self._get_relevant_remote_refs(refs_without_main)
 
         if regex == "":
             return list(relevant_refs)
 
         pattern = re.compile(regex)
         return [ref for ref in relevant_refs if pattern.match(ref)]
 
     def switch_to_package(self, package: str) -> None:
         if self.is_dirty():
-            click.echo(
+            click.secho(
                 "Repo is dirty, please commit your changes before switching to"
-                f" another package.\n {self.get_status_output()}"
+                f" another package.\n {self.get_status_output()}",
+                fg="red",
+                err=True,
             )
             return None
 
         feat_branch = self.get_feat_branch_of_package(package)
         if self.branch_exists(feat_branch) and not self.is_branch_merged(feat_branch):
             branch_to_switch = feat_branch
         else:
             branch_to_switch = package
             if self.branch_exists(feat_branch):
                 self.git_cmd(["branch", "-D", feat_branch])
 
         result = self.git_cmd(["switch", branch_to_switch])
         if result.retval == 0:
-            click.echo(result.stdout.replace("branch", "package"))
-        else:
-            click.echo(f"Switching to the package {package} for the first time")
-            click.echo(
-                self.git_cmd(["fetch", self.remote_name, branch_to_switch]).stdout
-            )
-            click.echo(
-                self.git_cmd(["switch", branch_to_switch]).stdout.replace(
-                    "branch", "package"
-                )
+            click.echo(result.stderr_and_stdout.replace("branch", "package"))
+            return
+
+        process = self.git_cmd(["fetch", self.remote_name, branch_to_switch])
+        if process.retval != 0:
+            click.secho(f"Package {package} doesn't exist!", fg="red", err=True)
+            return
+
+        click.echo(f"Switching to the package {package} for the first time")
+        click.echo(
+            self.git_cmd(["switch", branch_to_switch]).stderr_and_stdout.replace(
+                "branch", "package"
             )
+        )
 
     def _ensure_feature_branch(self) -> None:
         if self.branch != self.package:
             return None
 
         click.echo("Switching to feature branch")
         self.git_cmd(["switch", "-c", self.feat_branch])
 
     def create_packit_config(self, override: bool) -> bool:
-        packit_conf = PackitConfig(self.package)
+        packit_conf = Packit(self.package)
         if packit_conf.packit_config_file_exists() and not override:
             return False
 
-        packit_conf.create_packit_config()
+        packit_conf.create_packit_config(override)
         return True
 
+    def _rebase_needed(self) -> bool:
+        self.git_cmd(["fetch", self.remote_name])
+        last_package_commit = self.git_cmd(["rev-parse", self.branch]).stdout
+        last_remote_main_commit = self.git_cmd(
+            ["rev-parse", f"{self.remote_name}/{MAIN_BRANCH}"]
+        ).stdout
+        return (
+            last_package_commit != last_remote_main_commit
+            and self.git_cmd(
+                [
+                    "merge-base",
+                    "--is-ancestor",
+                    last_remote_main_commit,
+                    last_package_commit,
+                ]
+            ).retval
+            != 0
+        )
+
+    def push(self, branch: str, force: bool = False) -> None:
+        if self._rebase_needed():
+            rebase_from = f"{self.remote_name}/{MAIN_BRANCH}"
+            click.secho(
+                "Warning! Main branch has new updates! Rebasing your package "
+                "with main branch...\n"
+                f"git rebase {rebase_from}",
+                fg="yellow",
+            )
+            self.git_cmd(["rebase", rebase_from])
+
+        super().push(branch, force=True)
+
 
 class AlpaRepoBranch(AlpaRepo, LocalRepoBranch):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path, gh_api)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
```

### Comparing `pyalpa-0.8.0/alpa/repository/subdirectory.py` & `pyalpa-0.9.0/alpa/repository/subdirectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def _ensure_feature_branch(self) -> None:
         raise NotImplementedError("Please implement me.")
 
     def get_history_of_package(self, package: str) -> str:
         raise NotImplementedError("Please implement me.")
 
-    def get_packages(self, regex: str) -> list[str]:
+    def get_packages(self, regex: str = "") -> list[str]:
         raise NotImplementedError("Please implement me.")
 
     def switch_to_package(self, package: str) -> None:
         raise NotImplementedError("Please implement me.")
 
 
 class AlpaRepoSubdirectory(AlpaRepo, LocalRepoSubdirectory):
```

### Comparing `pyalpa-0.8.0/alpa/upstream_integration.py` & `pyalpa-0.9.0/alpa/upstream_integration.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.8.0/pyproject.toml` & `pyalpa-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.8.0"
+version = "0.9.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
```

