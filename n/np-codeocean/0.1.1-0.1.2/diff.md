# Comparing `tmp/np_codeocean-0.1.1.tar.gz` & `tmp/np_codeocean-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.1.tar", last modified: Thu May  4 18:35:28 2023, max compression
+gzip compressed data, was "np_codeocean-0.1.2.tar", last modified: Wed May 10 23:19:01 2023, max compression
```

## Comparing `np_codeocean-0.1.1.tar` & `np_codeocean-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.1/README.md
--rw-r--r--   0        0        0     1826 2023-05-04 18:35:28.040014 np_codeocean-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 03:16:59.500618 np_codeocean-0.1.1/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0     5828 2023-05-04 18:26:53.946109 np_codeocean-0.1.1/src/np_codeocean/upload.py
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 np_codeocean-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.2/README.md
+-rw-r--r--   0        0        0     1834 2023-05-10 23:19:01.620657 np_codeocean-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 03:16:59.500618 np_codeocean-0.1.2/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.2/src/np_codeocean/upload.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.2/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 np_codeocean-0.1.2/PKG-INFO
```

### Comparing `np_codeocean-0.1.1/pyproject.toml` & `np_codeocean-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,22 +36,22 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
-    "np_session>=0.6.0",
-    "np_tools",
+    "np_session>=0.6.4",
+    "np_tools>=0.1.12",
     "aind-data-transfer[ephys]>=0.15",
     "cmake",
     "setuptools>=36.2.0",
     "awscli",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
```

### Comparing `np_codeocean-0.1.1/src/np_codeocean/upload.py` & `np_codeocean-0.1.2/src/np_codeocean/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import aind_data_transfer.jobs.s3_upload_job as s3_upload_job
 import np_config
 import np_logging
 import np_session
 import np_tools
 
+import np_codeocean.utils as utils 
+
 logger = np_logging.get_logger(__name__)
 
 CONFIG = np_config.fetch('/projects/np_codeocean')
 
 class CodeOceanUpload(NamedTuple):
     """Objects required for uploading a Mindscope Neuropixels session to CodeOcean.
     
@@ -38,32 +40,24 @@
 
 def create_ephys_symlinks(session: np_session.Session, dest: Path) -> None:
     """Create symlinks in `dest` pointing to raw ephys data files on np-exp, with only one
     `recording` per `Record Node` folder (the largest, if multiple found).
     
     Relative paths are preserved, so `dest` will essentially be a merge of
     _probeABC / _probeDEF folders.
+    
+    Top-level items other than `Record Node *` folders are excluded.
     """
     logger.info(f'Creating symlinks to raw ephys data files in {session.npexp_path}...')
-    ephys_subfolders = np_tools.get_raw_ephys_subfolders(session.npexp_path)
-    logger.debug(f'Found {len(ephys_subfolders)} ephys subfolders: {ephys_subfolders}')
-    for ephys_folder in ephys_subfolders:
-        superfluous_recording_dirs: tuple[pathlib.Path, ...] = tuple(
-            _.parent for _ in np_tools.get_superfluous_oebin_paths(ephys_folder)
-        )
-        logger.debug(f'Found {len(superfluous_recording_dirs)} superfluous recording dirs to exclude: {superfluous_recording_dirs}')
-        for src in ephys_folder.rglob('*'):
-            is_superfluous_path = any(_ in src.parents for _ in superfluous_recording_dirs)
-            if is_superfluous_path:
-                continue
-            if src.is_file():
-                np_tools.symlink(src, dest / src.relative_to(ephys_folder))
+    for abs_path, rel_path in np_tools.get_filtered_ephys_paths_relative_to_record_node_parents(session.npexp_path):
+        if abs_path.is_file():
+            np_tools.symlink(abs_path, dest / rel_path)
     logger.debug(f'Finished creating symlinks to raw ephys data files in {session.npexp_path}')
 
-
+         
 def create_behavior_symlinks(session: np_session.Session, dest: Path) -> None:
     """Create symlinks in `dest` pointing to files in top-level of session
     folder on np-exp, plus all files in `exp` subfolder, if present.
     """
     logger.info(f'Creating symlinks in {dest} to files in {session.npexp_path}...')
     for src in session.npexp_path.glob('*'):
         if src.is_file():
@@ -88,14 +82,15 @@
         'experiment-type': 'ecephys',
         'modality': 'ECEPHYS',
         'acq-date': f'{session.date:%Y-%m-%d}',
         'acq-time': f'{session.start:%H-%M-%S}',
         'aws-param-store-name': CONFIG['aws-param-store-name'],
     } # type: ignore
 
+
 def create_upload_job(session: np_session.Session, job: Path, ephys: Path, behavior: Path) -> None:
     logger.info(f'Creating upload job file {job} for session {session}...')
     _csv = get_ephys_upload_csv_for_session(session, ephys, behavior)
     with open(job, 'w') as f:
         w = csv.writer(f)
         w.writerow(_csv.keys())
         w.writerow(_csv.values())    
@@ -122,15 +117,16 @@
 
     create_ephys_symlinks(upload.session, upload.ephys)
     create_behavior_symlinks(upload.session, upload.behavior)
     create_upload_job(upload.session, upload.job, upload.ephys, upload.behavior)    
     return upload
 
 
-def upload_session(session: str | int | pathlib.Path | np_session.Session)-> None:
+def upload_session(session: str | int | pathlib.Path | np_session.Session) -> None:
+    utils.ensure_credentials()
     upload = create_codeocean_upload(str(session))
     np_logging.web('np_codeocean').info(f'Uploading {upload.session}')
     s3_upload_job.GenericS3UploadJobList(["--jobs-csv-file", upload.job.as_posix()]).run_job()
     np_logging.web('np_codeocean').info(f'Finished uploading {upload.session}')
     
 def main() -> None:
     upload_session(sys.argv[1])
```

### Comparing `np_codeocean-0.1.1/PKG-INFO` & `np_codeocean-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: np-codeocean
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Source, https://github.com/AllenInstitute/np_codeocean
 Project-URL: Issues, https://github.com/AllenInstitute/np_codeocean/issues
 Requires-Python: >=3.8
-Requires-Dist: np_session>=0.6.0
-Requires-Dist: np_tools
+Requires-Dist: np_session>=0.6.4
+Requires-Dist: np_tools>=0.1.12
 Requires-Dist: aind-data-transfer[ephys]>=0.15
 Requires-Dist: cmake
 Requires-Dist: setuptools>=36.2.0
 Requires-Dist: awscli
 Requires-Dist: bump>=1.3.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Provides-Extra: dev
```

