# Comparing `tmp/wikimapper-0.1.6.tar.gz` & `tmp/wikimapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimapper-0.1.6.tar", last modified: Thu Apr 21 08:41:04 2022, max compression
+gzip compressed data, was "wikimapper-0.2.0.tar", last modified: Thu May 11 17:54:58 2023, max compression
```

## Comparing `wikimapper-0.1.6.tar` & `wikimapper-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 08:41:04.567485 wikimapper-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-04-21 08:40:51.000000 wikimapper-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-04-21 08:40:51.000000 wikimapper-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11835 2022-04-21 08:41:04.567485 wikimapper-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8435 2022-04-21 08:40:51.000000 wikimapper-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-21 08:41:04.567485 wikimapper-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4358 2022-04-21 08:40:51.000000 wikimapper-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 08:41:04.567485 wikimapper-0.1.6/wikimapper/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7890 2022-04-21 08:40:51.000000 wikimapper-0.1.6/wikimapper/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-21 08:41:04.567485 wikimapper-0.1.6/wikimapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11835 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-21 08:41:04.000000 wikimapper-0.1.6/wikimapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 17:54:58.026540 wikimapper-0.2.0/
+-rw-rw-rw-   0        0        0    11558 2022-04-21 08:01:16.000000 wikimapper-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-04-21 08:01:16.000000 wikimapper-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11149 2023-05-11 17:54:58.026540 wikimapper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9749 2023-05-11 17:54:45.000000 wikimapper-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-11 17:54:58.027540 wikimapper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4514 2022-04-21 08:37:18.000000 wikimapper-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:54:58.007540 wikimapper-0.2.0/tests/
+-rw-rw-rw-   0        0        0      559 2022-04-21 08:01:16.000000 wikimapper-0.2.0/tests/test_download.py
+-rw-rw-rw-   0        0        0     5129 2023-05-11 17:50:21.000000 wikimapper-0.2.0/tests/test_mapper.py
+-rw-rw-rw-   0        0        0      597 2022-04-21 08:37:18.000000 wikimapper-0.2.0/tests/test_processor.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:54:58.011540 wikimapper-0.2.0/wikimapper/
+-rw-rw-rw-   0        0        0      141 2022-04-21 08:01:16.000000 wikimapper-0.2.0/wikimapper/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-11 17:51:18.000000 wikimapper-0.2.0/wikimapper/__version__.py
+-rw-rw-rw-   0        0        0     5304 2022-04-21 08:37:18.000000 wikimapper-0.2.0/wikimapper/cli.py
+-rw-rw-rw-   0        0        0     2034 2022-04-21 08:37:18.000000 wikimapper-0.2.0/wikimapper/download.py
+-rw-rw-rw-   0        0        0     5728 2023-05-11 17:50:21.000000 wikimapper-0.2.0/wikimapper/mapper.py
+-rw-rw-rw-   0        0        0     8137 2023-01-21 21:49:27.000000 wikimapper-0.2.0/wikimapper/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-11 17:54:58.025541 wikimapper-0.2.0/wikimapper.egg-info/
+-rw-rw-rw-   0        0        0    11149 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-11 17:54:57.000000 wikimapper-0.2.0/wikimapper.egg-info/top_level.txt
```

### Comparing `wikimapper-0.1.6/LICENSE` & `wikimapper-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `wikimapper-0.1.6/PKG-INFO` & `wikimapper-0.2.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,285 +1,294 @@
-Metadata-Version: 2.1
-Name: wikimapper
-Version: 0.1.6
-Summary: Mapping Wikidata and Wikipedia entities to each other
-Home-page: https://github.com/jcklie/wikimapper
-Author: Jan-Christoph Klie
-Author-email: git@mrklie.com
-License: Apache License 2.0
-Project-URL: Bug Tracker, https://github.com/jcklie/wikimapper/issues
-Project-URL: Documentation, https://github.com/jcklie/wikimapper
-Project-URL: Source Code, https://github.com/jcklie/wikimapper
-Description: 
-        wikimapper
-        ==========
-        
-        .. image:: https://travis-ci.org/jcklie/wikimapper.svg?branch=master
-          :target: https://travis-ci.org/jcklie/wikimapper
-        
-        .. image:: https://codecov.io/gh/jcklie/wikimapper/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/jcklie/wikimapper
-        
-        .. image:: https://img.shields.io/pypi/l/wikimapper.svg
-          :alt: PyPI - License
-          :target: https://pypi.org/project/wikimapper/
-        
-        .. image:: https://img.shields.io/pypi/pyversions/wikimapper.svg
-          :alt: PyPI - Python Version
-          :target: https://pypi.org/project/wikimapper/
-        
-        .. image:: https://img.shields.io/pypi/v/wikimapper.svg
-          :alt: PyPI
-          :target: https://pypi.org/project/wikimapper/
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-          :target: https://github.com/ambv/black  
-        
-        This small Python library helps you to map Wikipedia page titles (e.g. `Manatee
-        <https://en.wikipedia.org/wiki/Manatee>`_ to `Q42797 <https://www.wikidata.org/wiki/Q42797>`_)
-        and vice versa. This is done by creating an index of these mappings from a Wikipedia SQL dump.
-        Precomputed indices can be found under `Precomputed indices`_. Redirects are taken into account.
-        
-        Installation
-        ------------
-        
-        This package can be installed via ``pip``, the Python package manager.
-        
-        .. code:: bash
-        
-            pip install wikimapper
-        
-        If all you want is just mapping, then you can also just download ``wikimapper/mapper.py`` and
-        add it to your project. It does not have any external dependencies.
-        
-        Usage
-        -----
-        
-        Using the mapping functionality requires a precomputed index. It is created from Wikipedia
-        SQL dumps (see `Create your own index`_) or can be downloaded for certain languages
-        (see `Precomputed indices`_). For the following to work, it is assumed that an index either
-        has been created or downloaded. Using the command line for batch mapping is not recommended,
-        as it requires repeated opening and closing the database, leading to a speed penalty.
-        
-        Map Wikipedia page title to Wikidata id
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from wikimapper import WikiMapper
-        
-            mapper = WikiMapper("index_enwiki-latest.db")
-            wikidata_id = mapper.title_to_id("Python_(programming_language)")
-            print(wikidata_id) # Q28865
-        
-        or from the command line via
-        
-        .. code:: bash
-        
-            $ wikimapper title2id index_enwiki-latest.db Germany
-            Q183
-        
-        Map Wikipedia URL to Wikidata id
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from wikimapper import WikiMapper
-        
-            mapper = WikiMapper("index_enwiki-latest.db")
-            wikidata_id = mapper.url_to_id("https://en.wikipedia.org/wiki/Python_(programming_language)")
-            print(wikidata_id) # Q28865
-        
-        or from the command line via
-        
-        .. code:: bash
-        
-            $ wikimapper url2id index_enwiki-latest.db https://en.wikipedia.org/wiki/Germany
-            Q183
-        
-        It is not checked whether the URL origins from the same Wiki as the index you created!
-        
-        Map Wikidata id to Wikipedia page title
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: python
-        
-            from wikimapper import WikiMapper
-        
-            mapper = WikiMapper("index_enwiki-latest.db")
-            titles = mapper.id_to_titles("Q183")
-            print(titles) # Germany, Deutschland, ...
-        
-        or from the command line via
-        
-        .. code:: bash
-        
-            $ wikimapper id2titles data/index_enwiki-latest.db Q183
-            Germany
-            Bundesrepublik_Deutschland
-            Land_der_Dichter_und_Denker
-            Jerman
-            ...
-        
-        Mapping id to title can lead to more than one result, as some pages in Wikipedia are
-        redirects, all linking to the same Wikidata item.
-        
-        Create your own index
-        ~~~~~~~~~~~~~~~~~~~~~
-        
-        While some indices are precomupted, it is sometimes useful to create your own. The
-        following section describes the steps need. Regarding creation speed: The index creation
-        code works, but is not optimized. It takes around 10 minutes on my Notebook (T480s)
-        to create it for English Wikipedia if the data is already downloaded.
-        
-        **1. Download the data**
-        
-        The easiest way is to use the command line tool that ships with this package. It
-        can be e.g. invoked by
-        
-        .. code:: bash
-        
-            $ wikimapper download enwiki-latest --dir data
-        
-        Use ``wikimapper download --help`` for a full description of the tool.
-        
-        The abbreviation for the Wiki of your choice can be found on `Wikipedia
-        <https://en.wikipedia.org/wiki/List_of_Wikipedias>`_. Available SQL dumps can be
-        e.g. found on `Wikimedia <https://dumps.wikimedia.org/>`_, you need to suffix
-        the Wiki name, e.g. ``https://dumps.wikimedia.org/dewiki/`` for the German one.
-        If possible, use a different mirror than the default in order to spread the resource usage.
-        
-        **2. Create the index**
-        
-        The next step is to create an index from the downloaded dump. The easiest way is to use
-        the command line tool that ships with this package. It can be e.g. invoked by
-        
-        .. code:: bash
-        
-            $ wikimapper create enwiki-latest --dumpdir data --target data/index_enwiki-latest.db
-        
-        This creates an index for the previously downloaded dump and saves it in ``data/index_enwiki-latest.db``.
-        Use ``wikimapper create --help`` for a full description of the tool.
-        
-        Precomputed indices
-        -------------------
-        
-        .. _precomputed:
-        
-        Several precomputed indices can be found `here <https://public.ukp.informatik.tu-darmstadt.de/wikimapper/>`_ .
-        
-        Command line interface
-        ----------------------
-        
-        This package comes with a command line interface that is automatically available
-        when installing via ``pip``. It can be invoked by ``wikimapper`` from the command
-        line.
-        
-        ::
-        
-            $ wikimapper
-        
-            usage: wikimapper [-h] [--version]
-                              {download,create,title2id,url2id,id2titles} ...
-        
-            Map Wikipedia page titles to Wikidata IDs and vice versa.
-        
-            positional arguments:
-              {download,create,title2id,url2id,id2titles}
-                                    sub-command help
-                download            Download Wikipedia dumps for creating a custom index.
-                create              Use a previously downloaded Wikipedia dump to create a
-                                    custom index.
-                title2id            Map a Wikipedia title to a Wikidata ID.
-                url2id              Map a Wikipedia URL to a Wikidata ID.
-                id2titles           Map a Wikidata ID to one or more Wikipedia titles.
-        
-            optional arguments:
-              -h, --help            show this help message and exit
-              --version             show program's version number and exit
-        
-        See ``wikimapper ${sub-command} --help`` for more information.
-        
-        Development
-        -----------
-        
-        The required dependencies are managed by **pip**. A virtual environment
-        containing all needed packages for development and production can be
-        created and activated by
-        
-        ::
-        
-            virtualenv venv --python=python3 --no-site-packages
-            source venv/bin/activate
-            pip install -e ".[test, dev, doc]"
-        
-        The tests can be run in the current environment by invoking
-        
-        ::
-        
-            make test
-        
-        or in a clean environment via
-        
-        ::
-        
-            tox
-        
-        FAQ
-        ---
-        
-        How does the parsing of the dump work?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        `jamesmishra <https://github.com/jamesmishra/mysqldump-to-csv>`__ has noticed that
-        SQL dumps from Wikipedia almost look like CSV. He provides some basic functions
-        to parse insert statements into tuples. We then use the Wikipedia SQL page
-        dump to get the mapping between title and internal id, page props to get
-        the Wikidata ID for a title and then the redirect dump in order to fill
-        titles that are only redirects and do not have an entry in the page props table.
-        
-        Why do you not use the Wikidata SPARQL endpoint for that?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        It is possible to query the official Wikidata SPARQL endpoint to do the mapping:
-        
-        .. code:: sparql
-        
-            prefix schema: <http://schema.org/>
-            SELECT * WHERE {
-              <https://en.wikipedia.org/wiki/Manatee> schema:about ?item .
-            }
-        
-        This has several issues: First, it uses the network, which is slow. Second, I try to use
-        that endpoint as infrequent as possible to save their resources (my use case is to map
-        data sets that have easily tens of thousands of entries). Third, I had coverage issues due
-        to redirects in Wikipedia not being resolved (around ~20% of the time for some older data sets).
-        So I created this package to do the mapping offline instead.
-        
-        Acknowledgements
-        ----------------
-        
-        I am very thankful for `jamesmishra <https://github.com/jamesmishra>`__  to provide
-        `mysqldump-to-csv <https://github.com/jamesmishra/mysqldump-to-csv>`__ . Also,
-        `mbugert <https://github.com/mbugert>`__ helped me tremendously understanding
-        Wikipedia dumps and giving me the idea on how to map.
-        
-Keywords: wikidata wikipedia wiki kb knowledge-base
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.5.0
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: doc
+wikimapper
+==========
+
+.. image:: https://img.shields.io/pypi/l/wikimapper.svg
+  :alt: PyPI - License
+  :target: https://pypi.org/project/wikimapper/
+
+.. image:: https://img.shields.io/pypi/pyversions/wikimapper.svg
+  :alt: PyPI - Python Version
+  :target: https://pypi.org/project/wikimapper/
+
+.. image:: https://img.shields.io/pypi/v/wikimapper.svg
+  :alt: PyPI
+  :target: https://pypi.org/project/wikimapper/
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+  :target: https://github.com/ambv/black  
+
+This small Python library helps you to map Wikipedia page titles (e.g. `Manatee
+<https://en.wikipedia.org/wiki/Manatee>`_ to `Q42797 <https://www.wikidata.org/wiki/Q42797>`_)
+and vice versa. This is done by creating an index of these mappings from a Wikipedia SQL dump.
+Precomputed indices can be found under `Precomputed indices`_. Redirects are taken into account.
+
+Installation
+------------
+
+This package can be installed via ``pip``, the Python package manager.
+
+.. code:: bash
+
+    pip install wikimapper
+
+If all you want is just mapping, then you can also just download ``wikimapper/mapper.py`` and
+add it to your project. It does not have any external dependencies.
+
+Usage
+-----
+
+Using the mapping functionality requires a precomputed index. It is created from Wikipedia
+SQL dumps (see `Create your own index`_) or can be downloaded for certain languages
+(see `Precomputed indices`_). For the following to work, it is assumed that an index either
+has been created or downloaded. Using the command line for batch mapping is not recommended,
+as it requires repeated opening and closing the database, leading to a speed penalty.
+
+Map Wikipedia page title to Wikidata id
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    wikidata_id = mapper.title_to_id("Python_(programming_language)")
+    print(wikidata_id) # Q28865
+
+or from the command line via
+
+.. code:: bash
+
+    $ wikimapper title2id index_enwiki-latest.db Germany
+    Q183
+
+Map Wikipedia URL to Wikidata id
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    wikidata_id = mapper.url_to_id("https://en.wikipedia.org/wiki/Python_(programming_language)")
+    print(wikidata_id) # Q28865
+
+or from the command line via
+
+.. code:: bash
+
+    $ wikimapper url2id index_enwiki-latest.db https://en.wikipedia.org/wiki/Germany
+    Q183
+
+It is not checked whether the URL origins from the same Wiki as the index you created!
+
+Map Wikidata id to Wikipedia page title
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    titles = mapper.id_to_titles("Q183")
+    print(titles) # Germany, Deutschland, ...
+
+or from the command line via
+
+.. code:: bash
+
+    $ wikimapper id2titles data/index_enwiki-latest.db Q183
+    Germany
+    Bundesrepublik_Deutschland
+    Land_der_Dichter_und_Denker
+    Jerman
+    ...
+
+Mapping id to title can lead to more than one result, as some pages in Wikipedia are
+redirects, all linking to the same Wikidata item.
+
+Map Wikipedia id to Wikidata id
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    wikidata_id = mapper.wikipedia_id_to_id(3342)
+    print(wikidata_id)  # Q183
+
+
+Map Wikidata id to Wikipedia id
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    wikipedia_ids = mapper.id_to_wikipedia_ids("Q183")
+    print(wikipedia_ids)  # [3342, 10590, 11833, 11840, ...]
+
+Mapping Wikidata id to Wikipedia id can lead to more than one result, as some pages in Wikipedia are
+redirects, all linking to the same Wikidata item.
+
+Map Wikipedia id to Wikipedia page title
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    page_title = mapper.wikipedia_id_to_title(3342)
+    print(page_title)  # Bundesrepublik_Deutschland
+
+Map Wikipedia page title to Wikipedia id
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from wikimapper import WikiMapper
+
+    mapper = WikiMapper("index_enwiki-latest.db")
+    wikipedia_id = mapper.title_to_wikipedia_id("Germany")
+    print(wikipedia_id)  # 11867
+
+Create your own index
+~~~~~~~~~~~~~~~~~~~~~
+
+While some indices are precomupted, it is sometimes useful to create your own. The
+following section describes the steps need. Regarding creation speed: The index creation
+code works, but is not optimized. It takes around 10 minutes on my Notebook (T480s)
+to create it for English Wikipedia if the data is already downloaded.
+
+**1. Download the data**
+
+The easiest way is to use the command line tool that ships with this package. It
+can be e.g. invoked by
+
+.. code:: bash
+
+    $ wikimapper download enwiki-latest --dir data
+
+Use ``wikimapper download --help`` for a full description of the tool.
+
+The abbreviation for the Wiki of your choice can be found on `Wikipedia
+<https://en.wikipedia.org/wiki/List_of_Wikipedias>`_. Available SQL dumps can be
+e.g. found on `Wikimedia <https://dumps.wikimedia.org/>`_, you need to suffix
+the Wiki name, e.g. ``https://dumps.wikimedia.org/dewiki/`` for the German one.
+If possible, use a different mirror than the default in order to spread the resource usage.
+
+**2. Create the index**
+
+The next step is to create an index from the downloaded dump. The easiest way is to use
+the command line tool that ships with this package. It can be e.g. invoked by
+
+.. code:: bash
+
+    $ wikimapper create enwiki-latest --dumpdir data --target data/index_enwiki-latest.db
+
+This creates an index for the previously downloaded dump and saves it in ``data/index_enwiki-latest.db``.
+Use ``wikimapper create --help`` for a full description of the tool.
+
+Precomputed indices
+-------------------
+
+.. _precomputed:
+
+Several precomputed indices can be found `here <https://public.ukp.informatik.tu-darmstadt.de/wikimapper/>`_ .
+
+Command line interface
+----------------------
+
+This package comes with a command line interface that is automatically available
+when installing via ``pip``. It can be invoked by ``wikimapper`` from the command
+line.
+
+::
+
+    $ wikimapper
+
+    usage: wikimapper [-h] [--version]
+                      {download,create,title2id,url2id,id2titles} ...
+
+    Map Wikipedia page titles to Wikidata IDs and vice versa.
+
+    positional arguments:
+      {download,create,title2id,url2id,id2titles}
+                            sub-command help
+        download            Download Wikipedia dumps for creating a custom index.
+        create              Use a previously downloaded Wikipedia dump to create a
+                            custom index.
+        title2id            Map a Wikipedia title to a Wikidata ID.
+        url2id              Map a Wikipedia URL to a Wikidata ID.
+        id2titles           Map a Wikidata ID to one or more Wikipedia titles.
+
+    optional arguments:
+      -h, --help            show this help message and exit
+      --version             show program's version number and exit
+
+See ``wikimapper ${sub-command} --help`` for more information.
+
+Development
+-----------
+
+The required dependencies are managed by **pip**. A virtual environment
+containing all needed packages for development and production can be
+created and activated by
+
+::
+
+    virtualenv venv --python=python3 --no-site-packages
+    source venv/bin/activate
+    pip install -e ".[test, dev, doc]"
+
+The tests can be run in the current environment by invoking
+
+::
+
+    make test
+
+or in a clean environment via
+
+::
+
+    tox
+
+FAQ
+---
+
+How does the parsing of the dump work?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+`jamesmishra <https://github.com/jamesmishra/mysqldump-to-csv>`__ has noticed that
+SQL dumps from Wikipedia almost look like CSV. He provides some basic functions
+to parse insert statements into tuples. We then use the Wikipedia SQL page
+dump to get the mapping between title and internal id, page props to get
+the Wikidata ID for a title and then the redirect dump in order to fill
+titles that are only redirects and do not have an entry in the page props table.
+
+Why do you not use the Wikidata SPARQL endpoint for that?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+It is possible to query the official Wikidata SPARQL endpoint to do the mapping:
+
+.. code:: sparql
+
+    prefix schema: <http://schema.org/>
+    SELECT * WHERE {
+      <https://en.wikipedia.org/wiki/Manatee> schema:about ?item .
+    }
+
+This has several issues: First, it uses the network, which is slow. Second, I try to use
+that endpoint as infrequent as possible to save their resources (my use case is to map
+data sets that have easily tens of thousands of entries). Third, I had coverage issues due
+to redirects in Wikipedia not being resolved (around ~20% of the time for some older data sets).
+So I created this package to do the mapping offline instead.
+
+Acknowledgements
+----------------
+
+I am very thankful for `jamesmishra <https://github.com/jamesmishra>`__  to provide
+`mysqldump-to-csv <https://github.com/jamesmishra/mysqldump-to-csv>`__ . Also,
+`mbugert <https://github.com/mbugert>`__ helped me tremendously understanding
+Wikipedia dumps and giving me the idea on how to map.
```

### Comparing `wikimapper-0.1.6/setup.py` & `wikimapper-0.2.0/setup.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-# !/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the "upload" functionality of this file, you must:
-#   $ pip install twine
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import setup, Command, find_packages
-
-# Package meta-data.
-NAME = "wikimapper"
-DESCRIPTION = "Mapping Wikidata and Wikipedia entities to each other"
-HOMEPAGE = "https://github.com/jcklie/wikimapper"
-EMAIL = "git@mrklie.com"
-AUTHOR = "Jan-Christoph Klie"
-REQUIRES_PYTHON = ">=3.5.0"
-
-install_requires=[]
-
-test_dependencies = [
-    "pytest",
-]
-
-dev_dependencies = [
-    "black",
-    "isort",
-    "twine",
-    "pygments",
-    "wheel"
-]
-
-doc_dependencies = []
-
-extras = {
-    "test" : test_dependencies,
-    "dev": dev_dependencies,
-    "doc": doc_dependencies
-}
-
-# The rest you shouldn"t have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if "README.rst" is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, "README.rst"), encoding="utf-8") as f:
-        long_description = "\n" + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package"s __version__.py module as a dictionary.
-about = {}
-with open(os.path.join(here, "wikimapper", "__version__.py")) as f:
-    exec(f.read(), about)
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = "Build and publish the package."
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status("Removing previous builds…")
-            rmtree(os.path.join(here, "dist"))
-        except OSError:
-            pass
-
-        self.status("Building Source and Wheel (universal) distribution…")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
-
-        self.status("Uploading the package to PyPI via Twine…")
-        os.system("twine upload dist/*")
-
-        self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
-        os.system("git push --tags")
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about["__version__"],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/x-rst",
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=HOMEPAGE,
-    packages=find_packages(exclude="tests"),
-    keywords="wikidata wikipedia wiki kb knowledge-base",
-
-    project_urls={
-        "Bug Tracker": "https://github.com/jcklie/wikimapper/issues",
-        "Documentation": "https://github.com/jcklie/wikimapper",
-        "Source Code": "https://github.com/jcklie/wikimapper",
-    },
-
-    install_requires=install_requires,
-    test_suite="tests",
-
-    tests_require=test_dependencies,
-    extras_require=extras,
-
-    include_package_data=True,
-    license="Apache License 2.0",
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Scientific/Engineering :: Human Machine Interfaces",
-        "Topic :: Scientific/Engineering :: Information Analysis",
-        "Topic :: Text Processing :: Linguistic",
-    ],
-
-    # $ setup.py publish support.
-    cmdclass={
-        "upload": UploadCommand,
-    },
-
-    entry_points={
-        'console_scripts': ['wikimapper=wikimapper.cli:main'],
-    }
-)
+# !/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the "upload" functionality of this file, you must:
+#   $ pip install twine
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import setup, Command, find_packages
+
+# Package meta-data.
+NAME = "wikimapper"
+DESCRIPTION = "Mapping Wikidata and Wikipedia entities to each other"
+HOMEPAGE = "https://github.com/jcklie/wikimapper"
+EMAIL = "git@mrklie.com"
+AUTHOR = "Jan-Christoph Klie"
+REQUIRES_PYTHON = ">=3.5.0"
+
+install_requires=[]
+
+test_dependencies = [
+    "pytest",
+]
+
+dev_dependencies = [
+    "black",
+    "isort",
+    "twine",
+    "pygments",
+    "wheel"
+]
+
+doc_dependencies = []
+
+extras = {
+    "test" : test_dependencies,
+    "dev": dev_dependencies,
+    "doc": doc_dependencies
+}
+
+# The rest you shouldn"t have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if "README.rst" is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, "README.rst"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package"s __version__.py module as a dictionary.
+about = {}
+with open(os.path.join(here, "wikimapper", "__version__.py")) as f:
+    exec(f.read(), about)
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = "Build and publish the package."
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print("\033[1m{0}\033[0m".format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
+        except OSError:
+            pass
+
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about["__version__"],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=HOMEPAGE,
+    packages=find_packages(exclude="tests"),
+    keywords="wikidata wikipedia wiki kb knowledge-base",
+
+    project_urls={
+        "Bug Tracker": "https://github.com/jcklie/wikimapper/issues",
+        "Documentation": "https://github.com/jcklie/wikimapper",
+        "Source Code": "https://github.com/jcklie/wikimapper",
+    },
+
+    install_requires=install_requires,
+    test_suite="tests",
+
+    tests_require=test_dependencies,
+    extras_require=extras,
+
+    include_package_data=True,
+    license="Apache License 2.0",
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Wiki",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Scientific/Engineering :: Human Machine Interfaces",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Text Processing :: Linguistic",
+    ],
+
+    # $ setup.py publish support.
+    cmdclass={
+        "upload": UploadCommand,
+    },
+
+    entry_points={
+        'console_scripts': ['wikimapper=wikimapper.cli:main'],
+    }
+)
```

### Comparing `wikimapper-0.1.6/wikimapper/download.py` & `wikimapper-0.2.0/wikimapper/download.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import logging
-import os
-import shutil
-import sys
-import urllib.parse
-import urllib.request
-
-_logger = logging.getLogger(__name__)
-
-
-def _report_hook(count: int, block_size: int, total_size: int):
-    percent = min(int(count * block_size * 100 / total_size), 100)
-    sys.stdout.write("\r%2d%%" % percent)
-
-
-def _download_file(url: str, target: str, overwrite: bool):
-    """Downloads the content identified by `url` and saves it in `target`."""
-    if os.path.exists(target) and not overwrite:
-        _logger.info("[%s] already exists, skipping downloading [%s]!", target, url)
-        return
-
-    _logger.info("Downloading [%s] to [%s]", url, target)
-
-    local_name, _ = urllib.request.urlretrieve(url, reporthook=_report_hook)
-    sys.stdout.write("\r")
-    shutil.move(local_name, target)
-
-
-def download_wikidumps(
-    dumpname: str, path: str, mirror: str = "https://dumps.wikimedia.org/", overwrite: bool = False
-):
-    """Downloads pages, page props and redirect SQL dumps for the dump
-    specified by `dumpname` to the folder `path`. If `overwrite` is true,
-    then it is downloaded again even if the files already exist.
-
-    Args:
-        dumpname (str): The name of the dump, e.g. `enwiki-latest` or `barwiki-20190420`.
-        path (str): Path to the folder where the dumps should be downloaded to.
-        mirror (str): The Wikipedia mirror to download from. Defaults to `https://dumps.wikimedia.org/`.
-        overwrite (bool): If true, then overwrite existing files, else, do not download again. Defaults to `False`.
-
-    """
-    os.makedirs(path, exist_ok=True)
-
-    wiki_name, date = dumpname.split("-")
-
-    url = urllib.parse.urljoin(mirror, wiki_name) + "/" + date + "/"
-
-    pages_dump = dumpname + "-page.sql.gz"
-    page_props_dump = dumpname + "-page_props.sql.gz"
-    redirects_dump = dumpname + "-redirect.sql.gz"
-
-    for dump in [pages_dump, page_props_dump, redirects_dump]:
-        _download_file(url + dump, os.path.join(path, dump), overwrite)
+import logging
+import os
+import shutil
+import sys
+import urllib.parse
+import urllib.request
+
+_logger = logging.getLogger(__name__)
+
+
+def _report_hook(count: int, block_size: int, total_size: int):
+    percent = min(int(count * block_size * 100 / total_size), 100)
+    sys.stdout.write("\r%2d%%" % percent)
+
+
+def _download_file(url: str, target: str, overwrite: bool):
+    """Downloads the content identified by `url` and saves it in `target`."""
+    if os.path.exists(target) and not overwrite:
+        _logger.info("[%s] already exists, skipping downloading [%s]!", target, url)
+        return
+
+    _logger.info("Downloading [%s] to [%s]", url, target)
+
+    local_name, _ = urllib.request.urlretrieve(url, reporthook=_report_hook)
+    sys.stdout.write("\r")
+    shutil.move(local_name, target)
+
+
+def download_wikidumps(
+    dumpname: str, path: str, mirror: str = "https://dumps.wikimedia.org/", overwrite: bool = False
+):
+    """Downloads pages, page props and redirect SQL dumps for the dump
+    specified by `dumpname` to the folder `path`. If `overwrite` is true,
+    then it is downloaded again even if the files already exist.
+
+    Args:
+        dumpname (str): The name of the dump, e.g. `enwiki-latest` or `barwiki-20190420`.
+        path (str): Path to the folder where the dumps should be downloaded to.
+        mirror (str): The Wikipedia mirror to download from. Defaults to `https://dumps.wikimedia.org/`.
+        overwrite (bool): If true, then overwrite existing files, else, do not download again. Defaults to `False`.
+
+    """
+    os.makedirs(path, exist_ok=True)
+
+    wiki_name, date = dumpname.split("-")
+
+    url = urllib.parse.urljoin(mirror, wiki_name) + "/" + date + "/"
+
+    pages_dump = dumpname + "-page.sql.gz"
+    page_props_dump = dumpname + "-page_props.sql.gz"
+    redirects_dump = dumpname + "-redirect.sql.gz"
+
+    for dump in [pages_dump, page_props_dump, redirects_dump]:
+        _download_file(url + dump, os.path.join(path, dump), overwrite)
```

### Comparing `wikimapper-0.1.6/wikimapper/processor.py` & `wikimapper-0.2.0/wikimapper/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,229 +1,230 @@
-""" Uses a Wikipedia dump to construct a mapping between Wikidata and Wikipedia.
-    Credit: Uses parts of https://github.com/jamesmishra/mysqldump-to-csv
-"""
-
-import csv
-import ctypes as ct
-import gzip
-import logging
-import os
-import sqlite3
-
-_logger = logging.getLogger(__name__)
-
-
-def _is_insert(line):
-    """
-    Returns true if the line begins a SQL insert statement.
-    """
-    return line.startswith("INSERT INTO")
-
-
-def _get_values(line):
-    """
-    Returns the portion of an INSERT statement containing values
-    """
-    return line[line.find("` VALUES ") + 9 :]
-
-
-def _values_sanity_check(values):
-    """
-    Ensures that values from the INSERT statement meet basic checks.
-    """
-    assert values
-    assert values[0] == "("
-    # Assertions have not been raised
-    return True
-
-
-def _parse_values(values):
-    """
-    Given a file handle and the raw values from a MySQL INSERT
-    statement, write the equivalent CSV to the file
-    """
-    latest_row = []
-
-    reader = csv.reader(
-        [values], delimiter=",", doublequote=False, escapechar="\\", quotechar="'", strict=True
-    )
-
-    for reader_row in reader:
-        for column in reader_row:
-            # If our current string is empty...
-            if len(column) == 0 or column == "NULL":
-                latest_row.append(chr(0))
-                continue
-            # If our string starts with an open paren
-            if column[0] == "(":
-                # Assume that this column does not begin
-                # a new row.
-                new_row = False
-                # If we've been filling out a row
-                if len(latest_row) > 0:
-                    # Check if the previous entry ended in
-                    # a close paren. If so, the row we've
-                    # been filling out has been COMPLETED
-                    # as:
-                    #    1) the previous entry ended in a )
-                    #    2) the current entry starts with a (
-                    if latest_row[-1][-1] == ")":
-                        # Remove the close paren.
-                        latest_row[-1] = latest_row[-1][:-1]
-                        new_row = True
-                # If we've found a new row, write it out
-                # and begin our new one
-                if new_row:
-                    yield latest_row
-                    latest_row = []
-                # If we're beginning a new row, eliminate the
-                # opening parentheses.
-                if len(latest_row) == 0:
-                    column = column[1:]
-            # Add our column to the row we're working on.
-            latest_row.append(column)
-        # At the end of an INSERT statement, we'll
-        # have the semicolon.
-        # Make sure to remove the semicolon and
-        # the close paren.
-        if latest_row[-1][-2:] == ");":
-            latest_row[-1] = latest_row[-1][:-2]
-            yield latest_row
-
-
-def create_index(dumpname: str, path_to_dumps: str, path_to_db: str = None) -> str:
-    """Creates an index mapping Wikipedia page titles to Wikidata IDs and vice versa.
-    This requires a previously downloaded dump `dumpname` in `path_to_dumps`.
-
-    Args:
-        dumpname(str): Name of the Wikipedia SQL  dump that should be used for creating an index.
-        path_to_dumps(str): Folder in which the dump has been downloaded to.
-        path_to_db(str): Path where the index will be saved to. Defaults to `index_${dump_name}.db`.
-
-    Returns:
-        str: The path to the created database.
-
-    """
-    if path_to_db is None:
-        path_to_db = "index_{0}.db".format(dumpname)
-
-    _logger.info("Creating index for [%s] in [%s]", dumpname, path_to_db)
-
-    wiki_name, date = dumpname.split("-")
-
-    pages_dump = os.path.join(path_to_dumps, dumpname + "-page.sql.gz")
-    page_props_dump = os.path.join(path_to_dumps, dumpname + "-page_props.sql.gz")
-    redirects_dump = os.path.join(path_to_dumps, dumpname + "-redirect.sql.gz")
-
-    # https://stackoverflow.com/a/54517228
-    csv.field_size_limit(int(ct.c_ulong(-1).value // 2))
-
-    # (Re)Create the database file
-    try:
-        os.remove(path_to_db)
-    except FileNotFoundError:
-        pass
-
-    conn = sqlite3.connect(path_to_db, isolation_level="EXCLUSIVE")
-
-    with conn:
-        conn.execute(
-            """CREATE TABLE mapping (
-            wikipedia_id int PRIMARY KEY ,
-            wikipedia_title text,
-            wikidata_id text)"""
-        )
-
-    c = conn.cursor()
-
-    # Parse the Wikipedia page dump; extract page id and page title from the sql
-    # https://www.mediawiki.org/wiki/Manual:Page_table
-    _logger.info("Parsing pages dump")
-    with gzip.open(pages_dump, "rt", encoding="utf-8", newline="\n") as f:
-        for line in f:
-            # Look for an INSERT statement and parse it.
-            if not _is_insert(line):
-                continue
-
-            values = _get_values(line)
-
-            for v in _parse_values(values):
-                # Filter the namespace; only use real articles
-                # https://www.mediawiki.org/wiki/Manual:Namespace
-                if v[1] == "0":
-                    c.execute(
-                        "INSERT INTO mapping (wikipedia_id, wikipedia_title) VALUES (?, ?)",
-                        (v[0], v[2]),
-                    )
-
-    conn.commit()
-
-    # We create this index here as all titles have been inserted now.
-    # Doing it earlier would recreate the index on every title insert.
-    _logger.info("Creating database index on 'wikipedia_title'")
-    conn.execute("""CREATE UNIQUE INDEX idx_wikipedia_title ON mapping(wikipedia_title);""")
-    conn.commit()
-
-    # Parse the Wikipedia page property dump; extract page id and Wikidata id from the sql
-    # https://www.mediawiki.org/wiki/Manual:Page_props_table/en
-    _logger.info("Parsing page properties dump")
-    with gzip.open(page_props_dump, "r") as f:
-        for line in f:
-            line = line.decode("utf-8", "ignore")
-
-            # Look for an INSERT statement and parse it.
-            if not _is_insert(line):
-                continue
-
-            values = _get_values(line)
-            for v in _parse_values(values):
-                # The page property table contains many properties, we only care about the Wikidata id
-                if v[1] == "wikibase_item":
-                    c.execute(
-                        "UPDATE mapping SET wikidata_id = ? WHERE wikipedia_id = ?", (v[2], v[0])
-                    )
-    conn.commit()
-
-    # Parse the Wikipedia redirect dump; fill in missing Wikidata ids
-    # https://www.mediawiki.org/wiki/Manual:Redirect_table
-    _logger.info("Parsing redirects dump")
-    with gzip.open(redirects_dump, "rt", encoding="utf-8", newline="\n") as f:
-        for line in f:
-            # Look for an INSERT statement and parse it.
-            if not _is_insert(line):
-                continue
-
-            values = _get_values(line)
-
-            for v in _parse_values(values):
-                source_wikipedia_id = v[0]
-                target_title = v[2]
-                namespace = v[1]
-
-                # We only care about main articles
-                if namespace != "0":
-                    continue
-
-                c.execute(
-                    "SELECT wikidata_id FROM mapping WHERE wikipedia_title = ?", (target_title,)
-                )
-                result = c.fetchone()
-
-                if result is None or result[0] is None:
-                    continue
-
-                wikidata_id = result[0]
-                c.execute(
-                    "UPDATE mapping SET wikidata_id = ? WHERE wikipedia_id = ?",
-                    (wikidata_id, source_wikipedia_id),
-                )
-
-    conn.commit()
-
-    _logger.info("Creating database index on 'wikidata_id'")
-    conn.execute("""CREATE INDEX idx_wikidata_id ON mapping(wikidata_id);""")
-    conn.commit()
-
-    c.close()
-    conn.close()
-
-    return path_to_db
+""" Uses a Wikipedia dump to construct a mapping between Wikidata and Wikipedia.
+    Credit: Uses parts of https://github.com/jamesmishra/mysqldump-to-csv
+"""
+
+import csv
+import ctypes as ct
+import gzip
+import logging
+import os
+import sqlite3
+
+_logger = logging.getLogger(__name__)
+
+
+def _is_insert(line):
+    """
+    Returns true if the line begins a SQL insert statement.
+    """
+    return line.startswith("INSERT INTO")
+
+
+def _get_values(line):
+    """
+    Returns the portion of an INSERT statement containing values
+    """
+    return line[line.find("` VALUES ") + 9 :]
+
+
+def _values_sanity_check(values):
+    """
+    Ensures that values from the INSERT statement meet basic checks.
+    """
+    assert values
+    assert values[0] == "("
+    # Assertions have not been raised
+    return True
+
+
+def _parse_values(values):
+    """
+    Given a file handle and the raw values from a MySQL INSERT
+    statement, write the equivalent CSV to the file
+    """
+    latest_row = []
+
+    reader = csv.reader(
+        [values], delimiter=",", doublequote=False, escapechar="\\", quotechar="'", strict=True
+    )
+
+    for reader_row in reader:
+        for column in reader_row:
+            # If our current string is empty...
+            if len(column) == 0 or column == "NULL":
+                latest_row.append(chr(0))
+                continue
+            # If our string starts with an open paren
+            if column[0] == "(":
+                # Assume that this column does not begin
+                # a new row.
+                new_row = False
+                # If we've been filling out a row
+                if len(latest_row) > 0:
+                    # Check if the previous entry ended in
+                    # a close paren. If so, the row we've
+                    # been filling out has been COMPLETED
+                    # as:
+                    #    1) the previous entry ended in a )
+                    #    2) the current entry starts with a (
+                    if latest_row[-1][-1] == ")":
+                        # Remove the close paren.
+                        latest_row[-1] = latest_row[-1][:-1]
+                        new_row = True
+                # If we've found a new row, write it out
+                # and begin our new one
+                if new_row:
+                    yield latest_row
+                    latest_row = []
+                # If we're beginning a new row, eliminate the
+                # opening parentheses.
+                if len(latest_row) == 0:
+                    column = column[1:]
+            # Add our column to the row we're working on.
+            latest_row.append(column)
+        # At the end of an INSERT statement, we'll
+        # have the semicolon.
+        # Make sure to remove the semicolon and
+        # the close paren.
+        if latest_row[-1][-2:] == ");":
+            latest_row[-1] = latest_row[-1][:-2]
+            yield latest_row
+
+
+def create_index(dumpname: str, path_to_dumps: str, path_to_db: str = None) -> str:
+    """Creates an index mapping Wikipedia page titles to Wikidata IDs and vice versa.
+    This requires a previously downloaded dump `dumpname` in `path_to_dumps`.
+
+    Args:
+        dumpname(str): Name of the Wikipedia SQL  dump that should be used for creating an index.
+        path_to_dumps(str): Folder in which the dump has been downloaded to.
+        path_to_db(str): Path where the index will be saved to. Defaults to `index_${dump_name}.db`.
+
+    Returns:
+        str: The path to the created database.
+
+    """
+    if path_to_db is None:
+        path_to_db = "index_{0}.db".format(dumpname)
+
+    _logger.info("Creating index for [%s] in [%s]", dumpname, path_to_db)
+
+    wiki_name, date = dumpname.split("-")
+
+    pages_dump = os.path.join(path_to_dumps, dumpname + "-page.sql.gz")
+    page_props_dump = os.path.join(path_to_dumps, dumpname + "-page_props.sql.gz")
+    redirects_dump = os.path.join(path_to_dumps, dumpname + "-redirect.sql.gz")
+
+    # https://stackoverflow.com/a/54517228
+    csv.field_size_limit(int(ct.c_ulong(-1).value // 2))
+
+    # (Re)Create the database file
+    try:
+        os.remove(path_to_db)
+    except FileNotFoundError:
+        pass
+
+    conn = sqlite3.connect(path_to_db, isolation_level="EXCLUSIVE")
+
+    with conn:
+        conn.execute(
+            """CREATE TABLE mapping (
+            wikipedia_id int PRIMARY KEY ,
+            wikipedia_title text,
+            wikidata_id text)"""
+        )
+
+    c = conn.cursor()
+
+    # Parse the Wikipedia page dump; extract page id and page title from the sql
+    # https://www.mediawiki.org/wiki/Manual:Page_table
+    _logger.info("Parsing pages dump")
+    with gzip.open(pages_dump, "rt", encoding="utf-8", newline="\n") as f:
+        for line in f:
+            # Look for an INSERT statement and parse it.
+            if not _is_insert(line):
+                continue
+
+            values = _get_values(line)
+
+            for v in _parse_values(values):
+                # Filter the namespace; only use real articles
+                # https://www.mediawiki.org/wiki/Manual:Namespace
+                if v[1] == "0":
+                    c.execute(
+                        "INSERT INTO mapping (wikipedia_id, wikipedia_title) VALUES (?, ?)",
+                        (v[0], v[2]),
+                    )
+
+    conn.commit()
+
+    # We create this index here as all titles have been inserted now.
+    # Doing it earlier would recreate the index on every title insert.
+    _logger.info("Creating database index on 'wikipedia_title'")
+    conn.execute("""CREATE UNIQUE INDEX idx_wikipedia_title ON mapping(wikipedia_title);""")
+    conn.commit()
+
+    # Parse the Wikipedia page property dump; extract page id and Wikidata id from the sql
+    # https://www.mediawiki.org/wiki/Manual:Page_props_table/en
+    _logger.info("Parsing page properties dump")
+    with gzip.open(page_props_dump, "r") as f:
+        for line in f:
+            line = line.decode("utf-8", "ignore")
+
+            # Look for an INSERT statement and parse it.
+            if not _is_insert(line):
+                continue
+
+            values = _get_values(line)
+            for v in _parse_values(values):
+                # The page property table contains many properties, we only care about the Wikidata id
+                if v[1] == "wikibase_item":
+                    c.execute(
+                        "UPDATE mapping SET wikidata_id = ? WHERE wikipedia_id = ?", (v[2], v[0])
+                    )
+    conn.commit()
+
+    # Parse the Wikipedia redirect dump; fill in missing Wikidata ids
+    # https://www.mediawiki.org/wiki/Manual:Redirect_table
+    _logger.info("Parsing redirects dump")
+    with gzip.open(redirects_dump, "r") as f:
+        for line in f:
+            line = line.decode("utf-8", "ignore")
+            # Look for an INSERT statement and parse it.
+            if not _is_insert(line):
+                continue
+
+            values = _get_values(line)
+
+            for v in _parse_values(values):
+                source_wikipedia_id = v[0]
+                target_title = v[2]
+                namespace = v[1]
+
+                # We only care about main articles
+                if namespace != "0":
+                    continue
+
+                c.execute(
+                    "SELECT wikidata_id FROM mapping WHERE wikipedia_title = ?", (target_title,)
+                )
+                result = c.fetchone()
+
+                if result is None or result[0] is None:
+                    continue
+
+                wikidata_id = result[0]
+                c.execute(
+                    "UPDATE mapping SET wikidata_id = ? WHERE wikipedia_id = ?",
+                    (wikidata_id, source_wikipedia_id),
+                )
+
+    conn.commit()
+
+    _logger.info("Creating database index on 'wikidata_id'")
+    conn.execute("""CREATE INDEX idx_wikidata_id ON mapping(wikidata_id);""")
+    conn.commit()
+
+    c.close()
+    conn.close()
+
+    return path_to_db
```

