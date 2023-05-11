# Comparing `tmp/copernicus_marine_client-0.5.1.tar.gz` & `tmp/copernicus_marine_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.5.1.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.6.0.tar", max compression
```

## Comparing `copernicus_marine_client-0.5.1.tar` & `copernicus_marine_client-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.192830 copernicus_marine_client-0.5.1/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.5.1/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    10868 2023-04-14 09:01:19.325083 copernicus_marine_client-0.5.1/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     3978 2023-04-14 09:01:19.328098 copernicus_marine_client-0.5.1/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3282 2023-04-14 06:39:18.368218 copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4874 2023-04-14 09:01:19.330085 copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0     9147 2023-04-14 09:02:50.587339 copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     7548 2023-04-14 09:01:19.334097 copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     3780 2023-04-14 09:01:19.336102 copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0     1037 2023-04-14 09:21:58.037403 copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0      755 2023-04-14 09:22:07.034647 copernicus_marine_client-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11857 2023-04-14 09:01:19.321085 copernicus_marine_client-0.5.1/README.md
--rw-r--r--   0        0        0    12988 1970-01-01 00:00:00.000000 copernicus_marine_client-0.5.1/setup.py
--rw-r--r--   0        0        0    12251 1970-01-01 00:00:00.000000 copernicus_marine_client-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-05-11 11:12:41.197210 copernicus_marine_client-0.6.0/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.6.0/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22193 2023-05-11 11:12:41.200332 copernicus_marine_client-0.6.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6005 2023-05-11 11:12:41.205333 copernicus_marine_client-0.6.0/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3282 2023-05-04 11:59:08.729763 copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     6673 2023-05-11 11:12:41.209333 copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    12050 2023-05-11 11:22:11.351346 copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     7691 2023-05-10 15:49:41.108051 copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     3778 2023-05-11 11:12:41.216676 copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     1037 2023-05-11 11:12:41.220681 copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     7123 2023-05-10 15:49:41.112053 copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     9729 2023-05-11 11:12:41.223836 copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0      819 2023-05-11 11:15:07.692550 copernicus_marine_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12440 2023-05-11 11:25:30.456436 copernicus_marine_client-0.6.0/README.md
+-rw-r--r--   0        0        0    13628 1970-01-01 00:00:00.000000 copernicus_marine_client-0.6.0/setup.py
+-rw-r--r--   0        0        0    12927 1970-01-01 00:00:00.000000 copernicus_marine_client-0.6.0/PKG-INFO
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from dataclasses import dataclass
 from datetime import datetime
 from json import load
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 
 @dataclass
 class SubsetRequest:
-    dataset_url: str = ""
-    dataset_id: str = ""
+    dataset_url: Optional[str] = None
+    dataset_id: Optional[str] = None
     output_directory: str = ""
     assume_yes: bool = False
     dry_run: bool = False
     variables: Optional[List[str]] = None
     minimal_longitude: Optional[float] = None
     maximal_longitude: Optional[float] = None
     minimal_latitude: Optional[float] = None
@@ -19,16 +19,25 @@
     minimal_depth: Optional[float] = None
     maximal_depth: Optional[float] = None
     start_datetime: Optional[datetime] = None
     end_datetime: Optional[datetime] = None
     output_filename: Optional[str] = None
     force_protocol: Optional[str] = None
 
-    def get_subset_request_dict(self) -> Dict:
-        return self.__dict__
+    def update(self, new_dict: dict):
+        """Method to update values in SubsetRequest object.
+        Skips "None" values
+        """
+        for key, value in new_dict.items():
+            if value is None or (
+                isinstance(value, (list, tuple)) and len(value) < 1
+            ):
+                pass
+            else:
+                self.__dict__.update({key: value})
 
     def enforce_types(self):
         def datetime_parser(string: str):
             for fmt in [
                 "%Y",
                 "%Y-%m-%d",
                 "%Y-%m-%dT%H:%M:%S",
@@ -70,26 +79,78 @@
     json_file = open(filepath)
     subset_request = SubsetRequest()
     subset_request.__dict__.update(load(json_file))
     subset_request.enforce_types()
     return subset_request
 
 
+def convert_motu_api_request_to_structure(
+    motu_api_request: str,
+) -> SubsetRequest:
+    prefix = "python -m motuclient "
+    string = motu_api_request.replace(prefix, "").replace("'", "")
+    arguments = [
+        substr.strip() for substr in string.split("--")[1:]
+    ]  # for subsubstr in substr.split(" ", maxsplit=1)]
+    arg_value_tuples = [
+        tuple(substr.split(" ", maxsplit=1)) for substr in arguments
+    ]
+    motu_api_request_dict: Dict[str, Any] = {}
+    for arg, value in arg_value_tuples:
+        if arg == "variable":
+            # special case for variable, since it can have multiple values
+            motu_api_request_dict.setdefault(arg, []).append(value)
+        else:
+            motu_api_request_dict[arg] = value
+    subset_request = SubsetRequest(
+        output_directory=".",
+        assume_yes=False,
+        dry_run=False,
+        output_filename=None,
+        force_protocol=None,
+    )
+    conversion_dict = {
+        "product-id": "dataset_id",
+        "latitude-min": "minimal_latitude",
+        "latitude-max": "maximal_latitude",
+        "longitude-min": "minimal_longitude",
+        "longitude-max": "maximal_longitude",
+        "depth-min": "minimal_depth",
+        "depth-max": "maximal_depth",
+        "date-min": "start_datetime",
+        "date-max": "end_datetime",
+        "variable": "variables",
+    }
+    for key, value in motu_api_request_dict.items():
+        if key in conversion_dict.keys():
+            subset_request.__dict__.update({conversion_dict[key]: value})
+    subset_request.enforce_types()
+    return subset_request
+
+
 @dataclass
 class NativeRequest:
-    dataset_url: str = ""
-    dataset_id: str = ""
+    dataset_url: Optional[str] = None
+    dataset_id: Optional[str] = None
     no_directories: bool = False
     show_outputnames: bool = False
     output_directory: str = "."
     assume_yes: bool = False
     dry_run: bool = False
+    force_protocol: Optional[str] = None
 
-    def get_native_request_dict(self) -> Dict:
-        return self.__dict__
+    def update(self, new_dict: dict):
+        """Method to update values in NativeRequest object.
+        Skips "None" values
+        """
+        for key, value in new_dict.items():
+            if value is None:
+                pass
+            else:
+                self.__dict__.update({key: value})
 
     def enforce_types(self):
         type_enforced_dict = {}
         for key, value in self.__dict__.items():
             if key in [
                 "no_directories",
                 "show_outputnames",
@@ -105,18 +166,7 @@
 
 def native_request_from_file(filepath) -> NativeRequest:
     json_file = open(filepath)
     native_request = NativeRequest()
     native_request.__dict__.update(load(json_file))
     native_request.enforce_types()
     return native_request
-
-
-if __name__ == "__main__":
-    sr = subset_request_from_file(
-        "tests/resources/example_subset_request.json"
-    )
-    print(sr)
-    nr = native_request_from_file(
-        "tests/resources/example_native_request.json"
-    )
-    print(nr)
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import click
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     FTP_KEY,
+    S3NATIVE_KEY,
     get_protocol_from_url,
     get_protocol_url_from_id,
 )
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
     native_request_from_file,
 )
 from copernicus_marine_client.download_functions.download_ftp import (
     download_ftp,
 )
+from copernicus_marine_client.download_functions.download_s3native import (
+    download_s3native,
+)
 
-PROTOCOL_KEYS_ORDER = [FTP_KEY]
+PROTOCOL_KEYS_ORDER = {"s3native": S3NATIVE_KEY, "ftp": FTP_KEY}
 
 
 @click.group()
 def cli_group_native() -> None:
     pass
 
 
@@ -77,88 +81,115 @@
     + " output files before download.",
     default=False,
 )
 @click.option(
     "--output-directory",
     "-o",
     type=click.Path(),
-    required=True,
     help="The destination directory for the downloaded files."
     + " Default is the current directory",
-    default=".",
 )
 @click.option(
     "--assume-yes",
     is_flag=True,
     default=False,
     help="Whether to ask for confirmation before download, after header display. "
     "If 'True', skips confirmation.",
 )
 @click.option(
+    "--force-protocol",
+    type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
+    help="Force download through one of the available protocols",
+)
+@click.option(
     "--dry-run",
     is_flag=True,
     default=False,
     help="Flag to specify NOT to send the request to external server. "
     "Returns the request instead",
 )
 @click.option(
     "--request-file",
     type=click.Path(),
     help="Option to pass a file containg CLI arguments. "
-    "The file MUST follow the structure of dataclass 'SubsetRequest'. "
-    "ANY PARAMETER SPECIFIED ASIDE FROM FILE WILL NOT "
-    "BE TAKEN INTO CONSIDERATION FOR THE REQUEST IF FILE "
-    "IS SPECIFIED.",
+    "The file MUST follow the structure of dataclass 'NativeRequest'. ",
 )
 def native(
     dataset_url: str,
     dataset_id: str,
     login: str,
     password: str,
     no_directories: bool,
     show_outputnames: bool,
     output_directory: str,
     assume_yes: bool,
     request_file: str,
-    dry_run: bool = False,
+    force_protocol: str,
+    dry_run: bool,
 ):
+    native_request = NativeRequest()
     if request_file:
         native_request = native_request_from_file(request_file)
-    else:
-        native_request = NativeRequest(
-            dataset_url=dataset_url,
-            dataset_id=dataset_id,
-            no_directories=no_directories,
-            show_outputnames=show_outputnames,
-            output_directory=output_directory,
-            assume_yes=assume_yes,
-            dry_run=dry_run,
-        )
+    request_update_dict = {
+        "dataset_url": dataset_url,
+        "dataset_id": dataset_id,
+        "output_directory": output_directory,
+        "force_protocol": force_protocol,
+    }
+    native_request.update(request_update_dict)
+    # Specific treatment for default values:
+    # In order to not overload arguments with default values
+    if no_directories:
+        native_request.no_directories = no_directories
+    if show_outputnames:
+        native_request.show_outputnames = show_outputnames
+    if assume_yes:
+        native_request.assume_yes = assume_yes
+    if force_protocol:
+        native_request.force_protocol = force_protocol
+    if dry_run:
+        native_request.dry_run = dry_run
+
     native_function(
         login,
         password,
         native_request,
     )
 
 
 def native_function(
     login: str,
     password: str,
     native_request: NativeRequest,
 ):
+    if native_request.force_protocol:
+        click.echo(
+            f"You forced selection of protocol: {native_request.force_protocol}"
+        )
+    possible_protocols = (
+        list(PROTOCOL_KEYS_ORDER.values())
+        if not native_request.force_protocol
+        else [PROTOCOL_KEYS_ORDER[native_request.force_protocol]]
+    )
+    print(possible_protocols)
     if not native_request.dataset_url:
         if not native_request.dataset_id:
             raise SyntaxError(
                 "Must specify at least one of 'dataset_url' or 'dataset_id'"
             )
         protocol, native_request.dataset_url = get_protocol_url_from_id(
-            native_request.dataset_id, PROTOCOL_KEYS_ORDER
+            native_request.dataset_id, possible_protocols
         )
     else:
         protocol = get_protocol_from_url(native_request.dataset_url)
+        if protocol != native_request.force_protocol:
+            raise ValueError(
+                f"Forced protocol {native_request.force_protocol} does not match "
+                f"user-specified url {native_request.dataset_url}"
+            )
     if protocol == FTP_KEY:
         if native_request.dry_run:
             print(
                 "download_ftp("
                 + ", ".join(
                     [
                         f"{login}",
@@ -172,9 +203,30 @@
 
         download_summary = download_ftp(
             login,
             password,
             native_request,
         )
         click.echo(download_summary)
+    elif protocol == S3NATIVE_KEY:
+        if native_request.dry_run:
+            print(
+                "download_s3native("
+                + ", ".join(
+                    [
+                        f"{login}",
+                        "HIDING_PASSWORD",
+                        f"{native_request}",
+                    ]
+                )
+                + ")"
+            )
+            return
+
+        download_summary = download_s3native(
+            login,
+            password,
+            native_request,
+        )
+        click.echo(download_summary)
     else:
         raise TypeError(f"Protocol type not handled: {protocol}")
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,74 @@
 from datetime import datetime
 from typing import List, Optional
 
 import click
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
+    GEOCHUNKED_KEY,
     MOTU_KEY,
     OPENDAP_KEY,
+    TIMECHUNKED_KEY,
     get_dataset_url_from_id,
     get_protocol_from_url,
     parse_catalogue,
 )
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
+    convert_motu_api_request_to_structure,
     subset_request_from_file,
 )
 from copernicus_marine_client.download_functions.download_motu import (
     download_motu,
 )
 from copernicus_marine_client.download_functions.download_opendap import (
     download_opendap,
 )
+from copernicus_marine_client.download_functions.download_zarr import (
+    download_zarr,
+    get_optimized_chunking,
+)
 
-PROTOCOL_KEYS_ORDER = {"opendap": OPENDAP_KEY, "motu": MOTU_KEY}
+PROTOCOL_KEYS_ORDER = {
+    "zarr": (TIMECHUNKED_KEY, GEOCHUNKED_KEY),
+    "zarr-map": TIMECHUNKED_KEY,
+    "zarr-timeserie": GEOCHUNKED_KEY,
+    "opendap": OPENDAP_KEY,
+    "motu": MOTU_KEY,
+}
 
 
 @click.group()
 def cli_group_subset() -> None:
     pass
 
 
 @cli_group_subset.command(
     "subset",
-    help="""Downloads subsets of datasets as NetCDF files.
+    help=(
+        """Downloads subsets of datasets as NetCDF files or Zarr stores.
     Either one of 'dataset-id' or 'dataset-url' is required
     (can be found via the 'copernicus-marine describe' command).
+    The arguments value passed individually through the CLI take precedence
+    over the values from the "motu-api-request" option, which takes precedence
+    over the ones from the "request-file" option
 
 Example:
 
   copernicus-marine subset
 --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
 --variable analysed_sst --variable sea_ice_fraction
 --start-datetime 2021-01-01 --end-datetime 2021-01-02
 --minimal-longitude 0.0 --maximal-longitude 0.1
 --minimal-latitude 0.0 --maximal-latitude 0.1
 
   copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst
   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
-""",
+"""
+    ),
 )
 @click.option(
     "--dataset-url",
     "-u",
     type=str,
     help="The full dataset URL",
 )
@@ -78,45 +96,45 @@
     help="Specify dataset variables",
     multiple=True,
 )
 @click.option(
     "--minimal-longitude",
     "-x",
     type=click.FloatRange(min=-180, max=180),
-    help="Minimal longitude for the subset",
+    help="Minimal longitude for the subset. Requires a float within this range:",
 )
 @click.option(
     "--maximal-longitude",
     "-X",
     type=click.FloatRange(min=-180, max=180),
-    help="Maximal longitude for the subset",
+    help="Maximal longitude for the subset. Requires a float within this range:",
 )
 @click.option(
     "--minimal-latitude",
     "-y",
     type=click.FloatRange(min=-90, max=90),
-    help="Minimal latitude for the subset",
+    help="Minimal latitude for the subset. Requires a float within this range:",
 )
 @click.option(
     "--maximal-latitude",
     "-Y",
     type=click.FloatRange(min=-90, max=90),
-    help="Maximal latitude for the subset",
+    help="Maximal latitude for the subset. Requires a float within this range:",
 )
 @click.option(
     "--minimal-depth",
     "-z",
     type=click.FloatRange(min=0),
-    help="Minimal depth for the subset",
+    help="Minimal depth for the subset. Requires a float within this range:",
 )
 @click.option(
     "--maximal-depth",
     "-Z",
     type=click.FloatRange(min=0),
-    help="Maximal depth for the subset",
+    help="Maximal depth for the subset. Requires a float within this range:",
 )
 @click.option(
     "--start-datetime",
     "-t",
     type=click.DateTime(
         ["%Y", "%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
     ),
@@ -130,29 +148,28 @@
     ),
     help="The end datetime of the temporal subset",
 )
 @click.option(
     "--output-directory",
     "-o",
     type=click.Path(),
-    required=True,
     help="The destination folder for the downloaded files."
     + " Default is the current directory",
-    default="",
 )
 @click.option(
     "--output-filename",
     "-f",
     type=click.Path(),
     help="Concatenate the downloaded data in the given file name"
-    + " (under the output path)",
+    + " (under the output directory)",
 )
 @click.option(
     "--assume-yes",
     is_flag=True,
+    default=False,
     help="Flag to skip confirmation before download",
 )
 @click.option(
     "--force-protocol",
     type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
@@ -163,18 +180,24 @@
     help="Flag to specify NOT to send the request to external server. "
     "Returns the request instead",
 )
 @click.option(
     "--request-file",
     type=click.Path(),
     help="Option to pass a filename corresponding to a file containg CLI arguments. "
-    "The file MUST follow the structure of dataclass 'SubsetRequest'. "
-    "ANY PARAMETER SPECIFIED ASIDE FROM FILE WILL NOT "
-    "BE TAKEN INTO CONSIDERATION FOR THE REQUEST IF FILE "
-    "IS SPECIFIED.",
+    "The file MUST follow the structure of dataclass 'SubsetRequest'. ",
+)
+@click.option(
+    "--motu-api-request",
+    type=str,
+    help=(
+        "Option to pass a complete MOTU api request as a string. "
+        'Caution, user has to replace double quotes " with single '
+        "quotes ' in the request"
+    ),
 )
 def subset(
     dataset_url: str,
     dataset_id: str,
     login: str,
     password: str,
     variables: Optional[List[str]],
@@ -185,66 +208,83 @@
     minimal_depth: Optional[float],
     maximal_depth: Optional[float],
     start_datetime: Optional[datetime],
     end_datetime: Optional[datetime],
     output_filename: Optional[str],
     force_protocol: Optional[str],
     request_file: Optional[str],
-    output_directory: str = "",
+    output_directory: str,
+    motu_api_request: Optional[str],
     assume_yes: bool = False,
     dry_run: bool = False,
 ):
+    subset_request = SubsetRequest()
     if request_file:
         subset_request = subset_request_from_file(request_file)
-    else:
-        subset_request = SubsetRequest(
-            dataset_url=dataset_url,
-            dataset_id=dataset_id,
-            variables=variables,
-            minimal_longitude=minimal_longitude,
-            maximal_longitude=maximal_longitude,
-            minimal_latitude=minimal_latitude,
-            maximal_latitude=maximal_latitude,
-            minimal_depth=minimal_depth,
-            maximal_depth=maximal_depth,
-            start_datetime=start_datetime,
-            end_datetime=end_datetime,
-            output_directory=output_directory,
-            output_filename=output_filename,
-            assume_yes=assume_yes,
-            force_protocol=force_protocol,
-            dry_run=dry_run,
+    if motu_api_request:
+        motu_api_subset_request = convert_motu_api_request_to_structure(
+            motu_api_request
         )
+        subset_request.update(motu_api_subset_request.__dict__)
+    request_update_dict = {
+        "dataset_url": dataset_url,
+        "dataset_id": dataset_id,
+        "variables": variables,
+        "minimal_longitude": minimal_longitude,
+        "maximal_longitude": maximal_longitude,
+        "minimal_latitude": minimal_latitude,
+        "maximal_latitude": maximal_latitude,
+        "minimal_depth": minimal_depth,
+        "maximal_depth": maximal_depth,
+        "start_datetime": start_datetime,
+        "end_datetime": end_datetime,
+        "output_directory": output_directory,
+        "output_filename": output_filename,
+        "force_protocol": force_protocol,
+    }
+    subset_request.update(request_update_dict)
+    # Specific treatment for default values:
+    # In order to not overload arguments with default values
+    if assume_yes:
+        subset_request.assume_yes = assume_yes
+    if dry_run:
+        subset_request.dry_run = dry_run
     subset_function(
         login,
         password,
         subset_request,
     )
 
 
 def subset_function(
     login: str,
     password: str,
     subset_request: SubsetRequest,
 ):
+    def _flatten(x):
+        if isinstance(x, (tuple, list)):
+            return [a for i in x for a in _flatten(i)]
+        else:
+            return [x]
+
+    catalogue = parse_catalogue()
     possible_protocols = (
-        PROTOCOL_KEYS_ORDER.values()
+        [p for p in list(PROTOCOL_KEYS_ORDER.values()) if isinstance(p, str)]
         if not subset_request.force_protocol
-        else [PROTOCOL_KEYS_ORDER[subset_request.force_protocol]]
+        else _flatten(PROTOCOL_KEYS_ORDER[subset_request.force_protocol])
     )
     if subset_request.force_protocol:
         click.echo(
             f"You forced selection of protocol: {subset_request.force_protocol}"
         )
     if not subset_request.dataset_url:
         if not subset_request.dataset_id:
             raise SyntaxError(
                 "Must specify at least one of 'dataset_url' or 'dataset_id'"
             )
-        catalogue = parse_catalogue()
         protocol_keys_iterator = iter(possible_protocols)
         while not subset_request.dataset_url:
             try:
                 protocol = next(protocol_keys_iterator)
             except StopIteration:
                 raise KeyError(
                     f"Dataset {subset_request.dataset_id} does "
@@ -252,20 +292,61 @@
                     f"for subset function. Available protocols: {possible_protocols}"
                 )
             subset_request.dataset_url = get_dataset_url_from_id(
                 catalogue, subset_request.dataset_id, protocol
             )
     else:
         protocol = get_protocol_from_url(subset_request.dataset_url)
-        catalogue = None
     if (
         subset_request.force_protocol
-        and protocol != subset_request.force_protocol
+        and protocol != PROTOCOL_KEYS_ORDER[subset_request.force_protocol]
     ):
         raise AttributeError("Dataset url does not match forced protocol!")
+    elif protocol in [TIMECHUNKED_KEY, GEOCHUNKED_KEY]:
+        # Check if both timechunked and geochunked data are available
+        url_timechunked, url_geochunked = (
+            map(
+                get_dataset_url_from_id,
+                [catalogue] * 2,
+                [subset_request.dataset_id] * 2,
+                [TIMECHUNKED_KEY, GEOCHUNKED_KEY],
+            )
+            if subset_request.dataset_id
+            else (None, None)
+        )
+        if (
+            url_timechunked
+            and url_geochunked
+            and (subset_request.force_protocol in [None, "zarr"])
+        ):
+            subset_request.dataset_url = (
+                url_timechunked
+                if get_optimized_chunking(subset_request)
+                else url_geochunked
+            )
+        click.echo("download through S3+Zarr")
+        if subset_request.dry_run:
+            print(
+                "download_zarr("
+                + ", ".join(
+                    [
+                        f"{login}",
+                        "HIDING_PASSWORD",
+                        f"{subset_request}",
+                    ]
+                )
+                + ")"
+            )
+            return
+        download_zarr(
+            login,
+            password,
+            subset_request,
+        )
+
     elif protocol == OPENDAP_KEY:
         click.echo("download through OPeNDAP")
         if subset_request.dry_run:
             print(
                 "download_opendap("
                 + ", ".join(
                     [
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from ftplib import FTP
 from multiprocessing.pool import ThreadPool
 from typing import Any, Tuple
 
 import click
 from numpy import append, arange
+from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
 )
 
 # /////////////////////////////
 # ---Using ftplib
@@ -17,32 +18,27 @@
 
 def download_ftp(
     login: str,
     password: str,
     native_request: NativeRequest,
 ) -> str:
     message, host, filenames_in = download_header(
-        [native_request.dataset_url], login, password
+        [str(native_request.dataset_url)], login, password
     )
     filenames_out = create_filenames_out(
         filenames_in,
         native_request.output_directory,
         native_request.no_directories,
     )
     click.echo(message)
     if native_request.show_outputnames:
         click.echo("Output filenames:")
         [click.echo(filename_out) for filename_out in filenames_out]
     if not native_request.assume_yes:
         click.confirm("Do you want to continue?", abort=True)
-    filenames_out = create_filenames_out(
-        filenames_in,
-        native_request.output_directory,
-        native_request.no_directories,
-    )
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
     groups_in_files = [
@@ -99,18 +95,16 @@
             ),
         )
         flattened_results = [r for res in results for r in res]
         total_size += sum([int(res[1]) for res in flattened_results])
         for result in flattened_results[:20]:
             message += str(result[0])
             message += f" - {format_file_size(float(result[1]))}\n"
-            if len(flattened_results) > 20:
-                message += (
-                    f"Printed 20 out of {len(flattened_results)} files\n"
-                )
+        if len(flattened_results) > 20:
+            message += f"Printed 20 out of {len(flattened_results)} files\n"
     message += (
         f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
     )
     return (message, host, filenames)
 
 
 def get_filenames_recursively(
@@ -151,15 +145,26 @@
 ) -> str:
     def _ftp_file_download(ftp, file_in, file_out):
         """
         Download ONE file and return a string of the result
         """
         os.makedirs(os.path.dirname(file_out), exist_ok=True)
         with open(file_out, "wb") as fp:
-            res = ftp.retrbinary("RETR " + file_in, fp.write)
+            size = ftp.size(file_in)
+            with tqdm(
+                total=size,
+                unit_scale=True,
+                desc=file_in.split("/")[-1],
+            ) as pbar:
+
+                def callback(data):
+                    pbar.update(len(data))
+                    fp.write(data)
+
+                res = ftp.retrbinary(f"RETR {file_in}", callback)
             if not res.startswith("226 Transfer complete"):
                 print(f"Download {file_in}failed")
                 if os.path.isfile(file_out):
                     os.remove(file_out)
                 summary_string = f"Could not download {file_in}!\n"
             else:
                 summary_string = f"File {file_out} created\n"
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_motu.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,13 @@
         options_list.extend(
             [
                 flat
                 for var in subset_request.variables
                 for flat in ["--variable", var]
             ]
         )
-
     run(
         [
             "motuclient",
         ]
         + options_list
     )
```

### Comparing `copernicus_marine_client-0.5.1/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.6.0/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.5.1/pyproject.toml` & `copernicus_marine_client-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.5.1"
+version = "0.6.0"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
@@ -12,14 +12,18 @@
 click = ">=8.0.4"
 numpy = ">=1.0"
 requests = ">=2.27.1"
 opendap-downloader = ">0.8.0"
 setuptools = ">=62.0.0"
 motuclient = "1.8.4"
 cachier = ">=2.0.2"
+pystac = ">=1.7.2"
+xarray = ">=2023.3.0"
+tqdm = ">=4.65.0"
+
 
 [tool.poetry.dev-dependencies]
 pre-commit = "2.20.0"
 types-requests = "2.27.11"
 
 [tool.poetry.scripts]
 copernicus-marine = 'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface'
```

### Comparing `copernicus_marine_client-0.5.1/README.md` & `copernicus_marine_client-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -88,26 +88,29 @@
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Login:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
+File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
 
 Check out the help:
 
 ```
 > copernicus-marine subset --help
 
 Usage: copernicus-marine subset [OPTIONS]
 
-  Downloads subsets of datasets as NetCDF files.     Either one of 'dataset-
+  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of 'dataset-
   id' or 'dataset-url' is required     (can be found via the 'copernicus-
-  marine describe' command).
+  marine describe' command).     The arguments value passed individually
+  through the CLI take precedence     over the values from the "motu-api-
+  request" option, which takes precedence     over the ones from the "request-
+  file" option
 
   Example:
 
     copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
     --variable analysed_sst --variable sea_ice_fraction --start-datetime
     2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
     longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
@@ -119,51 +122,53 @@
 Options:
   -u, --dataset-url TEXT          The full dataset URL
   -i, --dataset-id TEXT           The dataset id
   --login TEXT
   --password TEXT
   -v, --variable TEXT             Specify dataset variables
   -x, --minimal-longitude FLOAT RANGE
-                                  Minimal longitude for the subset
-                                  [-180<=x<=180]
+                                  Minimal longitude for the subset. Requires a
+                                  float whithin this range:  [-180<=x<=180]
   -X, --maximal-longitude FLOAT RANGE
-                                  Maximal longitude for the subset
-                                  [-180<=x<=180]
+                                  Maximal longitude for the subset. Requires a
+                                  float whithin this range:  [-180<=x<=180]
   -y, --minimal-latitude FLOAT RANGE
-                                  Minimal latitude for the subset
-                                  [-90<=x<=90]
+                                  Minimal latitude for the subset. Requires a
+                                  float whithin this range:  [-90<=x<=90]
   -Y, --maximal-latitude FLOAT RANGE
-                                  Maximal latitude for the subset
-                                  [-90<=x<=90]
+                                  Maximal latitude for the subset. Requires a
+                                  float whithin this range:  [-90<=x<=90]
   -z, --minimal-depth FLOAT RANGE
-                                  Minimal depth for the subset  [x>=0]
+                                  Minimal depth for the subset. Requires a
+                                  float whithin this range:  [x>=0]
   -Z, --maximal-depth FLOAT RANGE
-                                  Maximal depth for the subset  [x>=0]
+                                  Maximal depth for the subset. Requires a
+                                  float whithin this range:  [x>=0]
   -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
                                   The start datetime of the temporal subset
   -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
                                   The end datetime of the temporal subset
   -o, --output-directory PATH     The destination folder for the downloaded
                                   files. Default is the current directory
-                                  [required]
   -f, --output-filename PATH      Concatenate the downloaded data in the given
-                                  file name (under the output path)
+                                  file name (under the output directory)
   --assume-yes                    Flag to skip confirmation before download
-  --force-protocol [opendap|motu]
+  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
                                   Force download through one of the available
                                   protocols
   --dry-run                       Flag to specify NOT to send the request to
                                   external server. Returns the request instead
   --request-file PATH             Option to pass a filename corresponding to a
                                   file containg CLI arguments. The file MUST
                                   follow the structure of dataclass
-                                  'SubsetRequest'. ANY PARAMETER SPECIFIED
-                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO
-                                  CONSIDERATION FOR THE REQUEST IF FILE IS
-                                  SPECIFIED.
+                                  'SubsetRequest'.
+  --motu-api-request TEXT         Option to pass a complete MOTU api request
+                                  as a string. Caution, user has to replace
+                                  double quotes " with single quotes ' in the
+                                  request
   --help                          Show this message and exit.
 ```
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
```

### Comparing `copernicus_marine_client-0.5.1/setup.py` & `copernicus_marine_client-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 install_requires = \
 ['cachier>=2.0.2',
  'click>=8.0.4',
  'motuclient==1.8.4',
  'numpy>=1.0',
  'opendap-downloader>0.8.0',
  'owslib>=0.27.2',
+ 'pystac>=1.7.2',
  'requests>=2.27.1',
- 'setuptools>=62.0.0']
+ 'setuptools>=62.0.0',
+ 'tqdm>=4.65.0',
+ 'xarray>=2023.3.0']
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.5.1',
+    'version': '0.6.0',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files.     Either one of \'dataset-\n  id\' or \'dataset-url\' is required     (can be found via the \'copernicus-\n  marine describe\' command).\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X\n    0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset\n                                  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset\n                                  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset\n                                  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset\n                                  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n                                  [required]\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output path)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'. ANY PARAMETER SPECIFIED\n                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO\n                                  CONSIDERATION FOR THE REQUEST IF FILE IS\n                                  SPECIFIED.\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of \'dataset-\n  id\' or \'dataset-url\' is required     (can be found via the \'copernicus-\n  marine describe\' command).     The arguments value passed individually\n  through the CLI take precedence     over the values from the "motu-api-\n  request" option, which takes precedence     over the ones from the "request-\n  file" option\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X\n    0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset. Requires a\n                                  float whithin this range:  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset. Requires a\n                                  float whithin this range:  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset. Requires a\n                                  float whithin this range:  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output directory)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'.\n  --motu-api-request TEXT         Option to pass a complete MOTU api request\n                                  as a string. Caution, user has to replace\n                                  double quotes " with single quotes \' in the\n                                  request\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `copernicus_marine_client-0.5.1/PKG-INFO` & `copernicus_marine_client-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.5.1
+Version: 0.6.0
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachier (>=2.0.2)
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: motuclient (==1.8.4)
 Requires-Dist: numpy (>=1.0)
 Requires-Dist: opendap-downloader (>0.8.0)
 Requires-Dist: owslib (>=0.27.2)
+Requires-Dist: pystac (>=1.7.2)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: setuptools (>=62.0.0)
+Requires-Dist: tqdm (>=4.65.0)
+Requires-Dist: xarray (>=2023.3.0)
 Description-Content-Type: text/markdown
 
 # Copernicus Marine Service client
 
 A library to facilitate the access of Copernicus Marine Service products and datasets.
 
 ## Introduction
@@ -109,26 +112,29 @@
 > copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Login:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
+File downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
 
 Check out the help:
 
 ```
 > copernicus-marine subset --help
 
 Usage: copernicus-marine subset [OPTIONS]
 
-  Downloads subsets of datasets as NetCDF files.     Either one of 'dataset-
+  Downloads subsets of datasets as NetCDF files or Zarr store.     Either one of 'dataset-
   id' or 'dataset-url' is required     (can be found via the 'copernicus-
-  marine describe' command).
+  marine describe' command).     The arguments value passed individually
+  through the CLI take precedence     over the values from the "motu-api-
+  request" option, which takes precedence     over the ones from the "request-
+  file" option
 
   Example:
 
     copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
     --variable analysed_sst --variable sea_ice_fraction --start-datetime
     2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
     longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
@@ -140,51 +146,53 @@
 Options:
   -u, --dataset-url TEXT          The full dataset URL
   -i, --dataset-id TEXT           The dataset id
   --login TEXT
   --password TEXT
   -v, --variable TEXT             Specify dataset variables
   -x, --minimal-longitude FLOAT RANGE
-                                  Minimal longitude for the subset
-                                  [-180<=x<=180]
+                                  Minimal longitude for the subset. Requires a
+                                  float whithin this range:  [-180<=x<=180]
   -X, --maximal-longitude FLOAT RANGE
-                                  Maximal longitude for the subset
-                                  [-180<=x<=180]
+                                  Maximal longitude for the subset. Requires a
+                                  float whithin this range:  [-180<=x<=180]
   -y, --minimal-latitude FLOAT RANGE
-                                  Minimal latitude for the subset
-                                  [-90<=x<=90]
+                                  Minimal latitude for the subset. Requires a
+                                  float whithin this range:  [-90<=x<=90]
   -Y, --maximal-latitude FLOAT RANGE
-                                  Maximal latitude for the subset
-                                  [-90<=x<=90]
+                                  Maximal latitude for the subset. Requires a
+                                  float whithin this range:  [-90<=x<=90]
   -z, --minimal-depth FLOAT RANGE
-                                  Minimal depth for the subset  [x>=0]
+                                  Minimal depth for the subset. Requires a
+                                  float whithin this range:  [x>=0]
   -Z, --maximal-depth FLOAT RANGE
-                                  Maximal depth for the subset  [x>=0]
+                                  Maximal depth for the subset. Requires a
+                                  float whithin this range:  [x>=0]
   -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
                                   The start datetime of the temporal subset
   -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
                                   The end datetime of the temporal subset
   -o, --output-directory PATH     The destination folder for the downloaded
                                   files. Default is the current directory
-                                  [required]
   -f, --output-filename PATH      Concatenate the downloaded data in the given
-                                  file name (under the output path)
+                                  file name (under the output directory)
   --assume-yes                    Flag to skip confirmation before download
-  --force-protocol [opendap|motu]
+  --force-protocol [zarr|zarr-map|zarr-timeserie|opendap|motu]
                                   Force download through one of the available
                                   protocols
   --dry-run                       Flag to specify NOT to send the request to
                                   external server. Returns the request instead
   --request-file PATH             Option to pass a filename corresponding to a
                                   file containg CLI arguments. The file MUST
                                   follow the structure of dataclass
-                                  'SubsetRequest'. ANY PARAMETER SPECIFIED
-                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO
-                                  CONSIDERATION FOR THE REQUEST IF FILE IS
-                                  SPECIFIED.
+                                  'SubsetRequest'.
+  --motu-api-request TEXT         Option to pass a complete MOTU api request
+                                  as a string. Caution, user has to replace
+                                  double quotes " with single quotes ' in the
+                                  request
   --help                          Show this message and exit.
 ```
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
```

