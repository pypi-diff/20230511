# Comparing `tmp/Geode_Explicit-3.0.4-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-3.1.0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2193659 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-May-09 15:08 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-09 15:08 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-May-09 15:08 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2155008 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    19968 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2069504 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   146432 b- defN 23-May-09 15:09 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-May-09 15:09 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2380 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/RECORD
-12 files, 4537063 bytes uncompressed, 2191759 bytes compressed:  51.7%
+Zip file size: 307393 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       89 b- defN 23-May-11 07:38 geode_explicit/__init__.py
+-rw-r--r--  2.0 unx      261 b- defN 23-May-11 07:38 geode_explicit/brep.py
+-rw-r--r--  2.0 unx      240 b- defN 23-May-11 07:38 geode_explicit/section.py
+-rwxr-xr-x  2.0 unx   155104 b- defN 23-May-11 07:38 geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   147016 b- defN 23-May-11 07:38 geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   393656 b- defN 23-May-11 07:38 geode_explicit/lib64/libGeode-Explicit_brep.so
+-rwxr-xr-x  2.0 unx    23368 b- defN 23-May-11 07:38 geode_explicit/lib64/libGeode-Explicit_common.so
+-rwxr-xr-x  2.0 unx    96960 b- defN 23-May-11 07:38 geode_explicit/lib64/libGeode-Explicit_section.so
+-rw-r--r--  2.0 unx     2314 b- defN 23-May-11 07:38 Geode_Explicit-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-May-11 07:38 Geode_Explicit-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-11 07:38 Geode_Explicit-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1154 b- defN 23-May-11 07:38 Geode_Explicit-3.1.0.dist-info/RECORD
+12 files, 820280 bytes uncompressed, 305413 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -3,35 +3,35 @@
 
 Filename: geode_explicit/brep.py
 Comment: 
 
 Filename: geode_explicit/section.py
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_brep.dll
+Filename: geode_explicit/lib64/geode_explicit_py_brep.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_common.dll
+Filename: geode_explicit/lib64/geode_explicit_py_section.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: geode_explicit/bin/Geode-Explicit_section.dll
+Filename: geode_explicit/lib64/libGeode-Explicit_brep.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_common.so
 Comment: 
 
-Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+Filename: geode_explicit/lib64/libGeode-Explicit_section.so
 Comment: 
 
-Filename: Geode_Explicit-3.0.4.dist-info/METADATA
+Filename: Geode_Explicit-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-3.0.4.dist-info/WHEEL
+Filename: Geode_Explicit-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-3.0.4.dist-info/top_level.txt
+Filename: Geode_Explicit-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-3.0.4.dist-info/RECORD
+Filename: Geode_Explicit-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/__init__.py

```diff
@@ -1,7 +1,4 @@
-## Copyright (c) 2019 - 2023 Geode-solutions
-
-import os, pathlib
-os.add_dll_directory(pathlib.Path(__file__).parent.resolve().joinpath('bin'))
-
-from .section import *
-from .brep import *
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .section import *
+from .brep import *
```

## geode_explicit/brep.py

```diff
@@ -1,12 +1,12 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import opengeode_inspector
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_brep import *
-ExplicitBRepLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import opengeode_inspector
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_brep import *
+ExplicitBRepLibrary.initialize()
```

## geode_explicit/section.py

```diff
@@ -1,11 +1,11 @@
-#
-# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
-#
-
-import opengeode
-import geode_common
-import geode_conversion
-import geode_background
-
-from .bin.geode_explicit_py_section import *
-ExplicitSectionLibrary.initialize()
+#
+# Copyright (c) 2019 - 2023 Geode-solutions. All rights reserved.
+#
+
+import opengeode
+import geode_common
+import geode_conversion
+import geode_background
+
+from .lib64.geode_explicit_py_section import *
+ExplicitSectionLibrary.initialize()
```

## Comparing `Geode_Explicit-3.0.4.dist-info/METADATA` & `Geode_Explicit-3.1.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-Metadata-Version: 2.1
-Name: Geode-Explicit
-Version: 3.0.4
-Summary: Geode-solutions OpenGeode module for building explicit models
-Home-page: https://github.com/Geode-solutions/Geode-Explicit
-Author: Geode-solutions
-Author-email: contact@geode-solutions.com
-License: Proprietary
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.1.2)
-Requires-Dist: geode-common (==25.*,>=25.0.6)
-Requires-Dist: geode-conversion (==5.*,>=5.0.4)
-Requires-Dist: opengeode-core (==14.*,>=14.0.14)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2)
-Requires-Dist: opengeode-inspector (==3.*,>=3.0.3)
-Requires-Dist: opengeode-io (==6.*,>=6.0.4)
-
-<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
-<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
-
-<p align="center">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
-  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
-  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
-  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
-  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
-  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
-</p>
-
-<p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
-  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
-  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://opengeode-slack-invite.herokuapp.com">
-    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
-  </a>
-
-Copyright (c) 2019 - 2023, Geode-solutions
-
-
+Metadata-Version: 2.1
+Name: Geode-Explicit
+Version: 3.1.0
+Summary: Geode-solutions OpenGeode module for building explicit models
+Home-page: https://github.com/Geode-solutions/Geode-Explicit
+Author: Geode-solutions
+Author-email: contact@geode-solutions.com
+License: Proprietary
+Description-Content-Type: text/markdown
+Requires-Dist: geode-background (==7.*,>=7.1.2)
+Requires-Dist: geode-common (==25.*,>=25.0.7)
+Requires-Dist: geode-conversion (==5.*,>=5.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.0.16)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2)
+Requires-Dist: opengeode-inspector (==3.*,>=3.0.3)
+Requires-Dist: opengeode-io (==6.*,>=6.0.4)
+
+<h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
+<h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
+
+<p align="center">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
+  <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
+  <img src="https://codecov.io/gh/Geode-solutions/Geode-Explicit_private/branch/master/graph/badge.svg" alt="Coverage Status">
+  <img src="https://img.shields.io/github/release/Geode-solutions/Geode-Explicit_private.svg" alt="Version">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/static/v1?label=Windows&logo=windows&logoColor=white&message=support&color=success" alt="Windows support">
+  <img src="https://img.shields.io/static/v1?label=Ubuntu&logo=Ubuntu&logoColor=white&message=support&color=success" alt="Ubuntu support">
+  <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
+</p>
+
+<p align="center">
+  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
+  <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
+  </a>
+
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 3.0.4 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 3.1.0 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.1.2)
-Requires-Dist: geode-common (==25.*,>=25.0.6) Requires-Dist: geode-conversion
-(==5.*,>=5.0.4) Requires-Dist: opengeode-core (==14.*,>=14.0.14) Requires-Dist:
-opengeode-geosciences (==7.*,>=7.0.6) Requires-Dist: opengeode-geosciencesio
+contact@geode-solutions.com License: Proprietary Description-Content-Type:
+text/markdown Requires-Dist: geode-background (==7.*,>=7.1.2) Requires-Dist:
+geode-common (==25.*,>=25.0.7) Requires-Dist: geode-conversion (==5.*,>=5.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.0.16) Requires-Dist: opengeode-
+geosciences (==7.*,>=7.0.6) Requires-Dist: opengeode-geosciencesio
 (==4.*,>=4.1.2) Requires-Dist: opengeode-inspector (==3.*,>=3.0.3) Requires-
 Dist: opengeode-io (==6.*,>=6.0.4)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
```

