# Comparing `tmp/testgear-cli-0.1.2.tar.gz` & `tmp/testgear-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-cli-0.1.2.tar", last modified: Wed Apr  5 09:47:43 2023, max compression
+gzip compressed data, was "testgear-cli-0.1.3.tar", last modified: Fri May 26 08:30:33 2023, max compression
```

## Comparing `testgear-cli-0.1.2.tar` & `testgear-cli-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:43.357010 testgear-cli-0.1.2/
--rw-rw-rw-   0        0        0       53 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/.flake8
--rw-rw-rw-   0        0        0      785 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/.gitignore
--rw-rw-rw-   0        0        0    11558 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      776 2023-04-05 09:47:43.357010 testgear-cli-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/README.md
--rw-rw-rw-   0        0        0       62 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/main.py
--rw-rw-rw-   0        0        0      241 2023-04-05 09:40:07.000000 testgear-cli-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 09:47:43.357010 testgear-cli-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-05 09:47:05.000000 testgear-cli-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:43.310176 testgear-cli-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:43.341376 testgear-cli-0.1.2/src/testgear_cli/
--rw-rw-rw-   0        0        0        0 2023-01-19 09:06:35.000000 testgear-cli-0.1.2/src/testgear_cli/__init__.py
--rw-rw-rw-   0        0        0     1083 2023-04-05 09:41:55.000000 testgear-cli-0.1.2/src/testgear_cli/__main__.py
--rw-rw-rw-   0        0        0     4339 2023-04-05 09:43:14.000000 testgear-cli-0.1.2/src/testgear_cli/apiclient.py
--rw-rw-rw-   0        0        0     4129 2023-04-05 09:47:05.000000 testgear-cli-0.1.2/src/testgear_cli/args_parser.py
--rw-rw-rw-   0        0        0     5352 2023-04-05 09:47:05.000000 testgear-cli-0.1.2/src/testgear_cli/configurator.py
--rw-rw-rw-   0        0        0     1237 2023-04-05 09:43:14.000000 testgear-cli-0.1.2/src/testgear_cli/converter.py
--rw-rw-rw-   0        0        0     1763 2023-04-05 09:43:14.000000 testgear-cli-0.1.2/src/testgear_cli/importer.py
--rw-rw-rw-   0        0        0      485 2023-01-19 09:06:35.000000 testgear-cli-0.1.2/src/testgear_cli/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:43.357010 testgear-cli-0.1.2/src/testgear_cli/models/
--rw-rw-rw-   0        0        0        0 2023-01-19 09:06:35.000000 testgear-cli-0.1.2/src/testgear_cli/models/__init__.py
--rw-rw-rw-   0        0        0      344 2023-04-05 09:47:05.000000 testgear-cli-0.1.2/src/testgear_cli/models/config.py
--rw-rw-rw-   0        0        0      158 2023-01-19 09:06:35.000000 testgear-cli-0.1.2/src/testgear_cli/models/mode.py
--rw-rw-rw-   0        0        0      119 2023-01-19 09:06:35.000000 testgear-cli-0.1.2/src/testgear_cli/models/status.py
--rw-rw-rw-   0        0        0     1373 2023-04-05 09:42:44.000000 testgear-cli-0.1.2/src/testgear_cli/models/testcase.py
--rw-rw-rw-   0        0        0      117 2023-04-05 06:35:06.000000 testgear-cli-0.1.2/src/testgear_cli/models/testrun.py
--rw-rw-rw-   0        0        0     2806 2023-04-05 09:47:05.000000 testgear-cli-0.1.2/src/testgear_cli/parser.py
--rw-rw-rw-   0        0        0     1791 2023-04-05 09:43:14.000000 testgear-cli-0.1.2/src/testgear_cli/service.py
-drwxrwxrwx   0        0        0        0 2023-04-05 09:47:43.357010 testgear-cli-0.1.2/src/testgear_cli.egg-info/
--rw-rw-rw-   0        0        0      776 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-05 09:47:42.000000 testgear-cli-0.1.2/src/testgear_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:33.627783 testgear-cli-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/src/testgear_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/src/testgear_cli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/models/testrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-26 08:30:22.000000 testgear-cli-0.1.3/src/testgear_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:30:33.631783 testgear-cli-0.1.3/src/testgear_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 08:30:33.000000 testgear-cli-0.1.3/src/testgear_cli.egg-info/top_level.txt
```

### Comparing `testgear-cli-0.1.2/LICENSE` & `testgear-cli-0.1.3/LICENSE`

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

### Comparing `testgear-cli-0.1.2/src/testgear_cli/args_parser.py` & `testgear-cli-0.1.3/src/testgear_cli/args_parser.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import argparse
-
-from testgear_cli.models.config import Config
-from testgear_cli.models.mode import Mode
-
-
-class ArgsParser:
-    """Class representing a arguments parser"""
-
-    def __init__(self):
-        self.__init_parser()
-        self.__add_args()
-
-    def __init_parser(self):
-        self.parser = argparse.ArgumentParser(
-            prog="testgear",
-            usage="%(prog)s [options]",
-            description="""This tool is the command line wrapper of Test Gear
-                     allowing you to upload the test results in real time to Test Gear""",
-        )
-
-    def parse_args(self):
-        """Function parses commandline arguments and returns config."""
-        args = self.parser.parse_args()
-        return Config(
-            Mode(args.mode),
-            args.url,
-            args.token,
-            args.project_id,
-            args.configuration_id,
-            args.testrun_id,
-            args.testrun_name,
-            args.separator,
-            args.namespace,
-            args.results,
-            args.debug,
-            args.output,
-        )
-
-    def __add_args(self):
-        self.parser.add_argument(
-            "-m",
-            "--mode",
-            action="store",
-            choices=["import", "create", "finish", "upload"],
-            default="import",
-            dest="mode",
-            help="Set CLI mode",
-        )
-        self.parser.add_argument(
-            "-u",
-            "--url",
-            action="store",
-            default=None,
-            dest="url",
-            metavar="https://demo.test-gear.io",
-            help="Set url address of the Test Gear instance",
-        )
-        self.parser.add_argument(
-            "-t",
-            "--token",
-            action="store",
-            dest="token",
-            metavar="T2lKd2pLZGI4WHRhaVZUejNl",
-            help="Set API token",
-        )
-        self.parser.add_argument(
-            "-pi",
-            "--project-id",
-            action="store",
-            dest="project_id",
-            metavar="5236eb3f-7c05-46f9-a609-dc0278896464",
-            help="Set project id",
-        )
-        self.parser.add_argument(
-            "-ci",
-            "--configuration-id",
-            action="store",
-            dest="configuration_id",
-            metavar="15dbb164-c1aa-4cbf-830c-8c01ae14f4fb",
-            help="Set configuration id",
-        )
-        self.parser.add_argument(
-            "-ti",
-            "--testrun-id",
-            action="store",
-            dest="testrun_id",
-            metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
-            help="Set test run id",
-        )
-        self.parser.add_argument(
-            "-tn",
-            "--testrun-name",
-            action="store",
-            dest="testrun_name",
-            metavar="TestRun01",
-            help="Set test run name",
-        )
-        self.parser.add_argument(
-            "-s",
-            "--separator",
-            action="store",
-            dest="separator",
-            metavar=".",
-            help="Separate the classname value in the results into namespace and classname",
-        )
-        self.parser.add_argument(
-            "-ns",
-            "--namespace",
-            action="store",
-            dest="namespace",
-            metavar="NameSpace01",
-            help="Set namespace",
-        )
-        self.parser.add_argument(
-            "-r",
-            "--results",
-            action="store",
-            dest="results",
-            metavar="DIR",
-            default=None,
-            help="Set directory with results file",
-        )
-        self.parser.add_argument(
-            "-d",
-            "--debug",
-            action="store_true",
-            dest="debug",
-            help="Set debug logs",
-        )
-        self.parser.add_argument(
-            "-o",
-            "--output",
-            action="store",
-            dest="output",
-            metavar="FILE",
-            default=None,
-            help="Set file path for output",
-        )
+import argparse
+
+from testgear_cli.models.config import Config
+from testgear_cli.models.mode import Mode
+
+
+class ArgsParser:
+    """Class representing a arguments parser"""
+
+    def __init__(self):
+        self.__init_parser()
+        self.__add_args()
+
+    def __init_parser(self):
+        self.parser = argparse.ArgumentParser(
+            prog="testgear",
+            usage="%(prog)s [options]",
+            description="""This tool is the command line wrapper of Test Gear
+                     allowing you to upload the test results in real time to Test Gear""",
+        )
+
+    def parse_args(self):
+        """Function parses commandline arguments and returns config."""
+        args = self.parser.parse_args()
+        return Config(
+            Mode(args.mode),
+            args.url,
+            args.token,
+            args.project_id,
+            args.configuration_id,
+            args.testrun_id,
+            args.testrun_name,
+            args.separator,
+            args.namespace,
+            args.results,
+            args.debug,
+            args.output,
+        )
+
+    def __add_args(self):
+        self.parser.add_argument(
+            "-m",
+            "--mode",
+            action="store",
+            choices=["import", "create", "finish", "upload"],
+            default="import",
+            dest="mode",
+            help="Set CLI mode",
+        )
+        self.parser.add_argument(
+            "-u",
+            "--url",
+            action="store",
+            default=None,
+            dest="url",
+            metavar="https://demo.test-gear.io",
+            help="Set url address of the Test Gear instance",
+        )
+        self.parser.add_argument(
+            "-t",
+            "--token",
+            action="store",
+            dest="token",
+            metavar="T2lKd2pLZGI4WHRhaVZUejNl",
+            help="Set API token",
+        )
+        self.parser.add_argument(
+            "-pi",
+            "--project-id",
+            action="store",
+            dest="project_id",
+            metavar="5236eb3f-7c05-46f9-a609-dc0278896464",
+            help="Set project id",
+        )
+        self.parser.add_argument(
+            "-ci",
+            "--configuration-id",
+            action="store",
+            dest="configuration_id",
+            metavar="15dbb164-c1aa-4cbf-830c-8c01ae14f4fb",
+            help="Set configuration id",
+        )
+        self.parser.add_argument(
+            "-ti",
+            "--testrun-id",
+            action="store",
+            dest="testrun_id",
+            metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
+            help="Set test run id",
+        )
+        self.parser.add_argument(
+            "-tn",
+            "--testrun-name",
+            action="store",
+            dest="testrun_name",
+            metavar="TestRun01",
+            help="Set test run name",
+        )
+        self.parser.add_argument(
+            "-s",
+            "--separator",
+            action="store",
+            dest="separator",
+            metavar=".",
+            help="Separate the classname value in the results into namespace and classname",
+        )
+        self.parser.add_argument(
+            "-ns",
+            "--namespace",
+            action="store",
+            dest="namespace",
+            metavar="NameSpace01",
+            help="Set namespace",
+        )
+        self.parser.add_argument(
+            "-r",
+            "--results",
+            action="store",
+            dest="results",
+            metavar="DIR",
+            default=None,
+            help="Set directory with results file",
+        )
+        self.parser.add_argument(
+            "-d",
+            "--debug",
+            action="store_true",
+            dest="debug",
+            help="Set debug logs",
+        )
+        self.parser.add_argument(
+            "-o",
+            "--output",
+            action="store",
+            dest="output",
+            metavar="FILE",
+            default=None,
+            help="Set file path for output",
+        )
```

### Comparing `testgear-cli-0.1.2/src/testgear_cli/service.py` & `testgear-cli-0.1.3/src/testgear_cli/service.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import logging
-from testgear_cli.parser import Parser
-
-from testgear_cli.apiclient import ApiClient
-from testgear_cli.configurator import Configurator
-from testgear_cli.importer import Importer
-
-
-class Service:
-    def __init__(
-        self,
-        config: Configurator,
-        api_client: ApiClient,
-        parser: Parser,
-        importer: Importer,
-    ):
-        self.__config = config
-        self.__api_client = api_client
-        self.__parser = parser
-        self.__importer = importer
-
-    def import_results(self):
-        self.__upload_results()
-        self.finished_testrun()
-
-    def upload_results(self):
-        self.__upload_results()
-
-    def create_testrun(self):
-        test_run_id = self.__create_test_run()
-        with open(self.__config.get_output(), "w") as text_file:
-            text_file.write(test_run_id)
-
-    def finished_testrun(self):
-        self.__api_client.complete_test_run(self.__config.get_testrun_id())
-
-    def __create_test_run(self):
-        return self.__api_client.create_test_run(
-            self.__config.get_project_id(), self.__config.get_testrun_name()
-        )
-
-    def __upload_results(self):
-        logging.info("Collecting log files ...")
-
-        results = self.__parser.read_file()
-
-        if self.__config.get_testrun_id() is None:
-            test_run_id = self.__create_test_run()
-            self.__config.set_testrun_id(test_run_id)
-        else:
-            test_run = self.__api_client.get_test_run(self.__config.get_testrun_id())
-            self.__config.set_project_id(test_run.project_id)
-
-        logging.info("Sending test results to Test Gear ...")
-
-        self.__importer.send_results(results)
-
-        logging.info("Successfully sent test results")
+import logging
+from testgear_cli.parser import Parser
+
+from testgear_cli.apiclient import ApiClient
+from testgear_cli.configurator import Configurator
+from testgear_cli.importer import Importer
+
+
+class Service:
+    def __init__(
+        self,
+        config: Configurator,
+        api_client: ApiClient,
+        parser: Parser,
+        importer: Importer,
+    ):
+        self.__config = config
+        self.__api_client = api_client
+        self.__parser = parser
+        self.__importer = importer
+
+    def import_results(self):
+        self.__upload_results()
+        self.finished_testrun()
+
+    def upload_results(self):
+        self.__upload_results()
+
+    def create_testrun(self):
+        test_run_id = self.__create_test_run()
+        with open(self.__config.get_output(), "w") as text_file:
+            text_file.write(test_run_id)
+
+    def finished_testrun(self):
+        self.__api_client.complete_test_run(self.__config.get_testrun_id())
+
+    def __create_test_run(self):
+        return self.__api_client.create_test_run(
+            self.__config.get_project_id(), self.__config.get_testrun_name()
+        )
+
+    def __upload_results(self):
+        logging.info("Collecting log files ...")
+
+        results = self.__parser.read_file()
+
+        if self.__config.get_testrun_id() is None:
+            test_run_id = self.__create_test_run()
+            self.__config.set_testrun_id(test_run_id)
+        else:
+            test_run = self.__api_client.get_test_run(self.__config.get_testrun_id())
+            self.__config.set_project_id(test_run.project_id)
+
+        logging.info("Sending test results to Test Gear ...")
+
+        self.__importer.send_results(results)
+
+        logging.info("Successfully sent test results")
```

### Comparing `testgear-cli-0.1.2/src/testgear_cli.egg-info/SOURCES.txt` & `testgear-cli-0.1.3/src/testgear_cli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-.flake8
-.gitignore
 LICENSE
 README.md
-main.py
-requirements.txt
 setup.py
 src/testgear_cli/__init__.py
 src/testgear_cli/__main__.py
 src/testgear_cli/apiclient.py
 src/testgear_cli/args_parser.py
 src/testgear_cli/configurator.py
 src/testgear_cli/converter.py
```

