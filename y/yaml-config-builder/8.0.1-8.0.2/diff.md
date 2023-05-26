# Comparing `tmp/yaml_config_builder-8.0.1.tar.gz` & `tmp/yaml_config_builder-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml_config_builder-8.0.1.tar", max compression
+gzip compressed data, was "yaml_config_builder-8.0.2.tar", max compression
```

## Comparing `yaml_config_builder-8.0.1.tar` & `yaml_config_builder-8.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    12061 2023-05-09 06:24:29.607523 yaml_config_builder-8.0.1/LICENSE
--rw-r--r--   0        0        0      950 2023-05-09 06:24:29.607523 yaml_config_builder-8.0.1/README.md
--rw-r--r--   0        0        0     2832 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/pyproject.toml
--rw-r--r--   0        0        0      338 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/__init__.py
--rw-r--r--   0        0        0    17637 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/base_config_class.py
--rw-r--r--   0        0        0    13559 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/config_builder.py
--rw-r--r--   0        0        0      153 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/py.typed
--rw-r--r--   0        0        0     3871 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/replacement_map.py
--rw-r--r--   0        0        0     2642 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/utils.py
--rw-r--r--   0        0        0    10526 2023-05-09 06:24:29.611523 yaml_config_builder-8.0.1/src/config_builder/yaml_constructors.py
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.1/setup.py
--rw-r--r--   0        0        0     2321 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-05-25 13:19:06.793465 yaml_config_builder-8.0.2/LICENSE
+-rw-r--r--   0        0        0      950 2023-05-25 13:19:06.793465 yaml_config_builder-8.0.2/README.md
+-rw-r--r--   0        0        0     2739 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/pyproject.toml
+-rw-r--r--   0        0        0      452 2023-05-25 14:08:10.333408 yaml_config_builder-8.0.2/src/config_builder/__init__.py
+-rw-r--r--   0        0        0    17679 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/base_config_class.py
+-rw-r--r--   0        0        0    13656 2023-05-25 14:08:10.333408 yaml_config_builder-8.0.2/src/config_builder/config_builder.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/py.typed
+-rw-r--r--   0        0        0     3913 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/replacement_map.py
+-rw-r--r--   0        0        0     2684 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/utils.py
+-rw-r--r--   0        0        0    10568 2023-05-25 13:19:06.797466 yaml_config_builder-8.0.2/src/config_builder/yaml_constructors.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.2/setup.py
+-rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 yaml_config_builder-8.0.2/PKG-INFO
```

### Comparing `yaml_config_builder-8.0.1/LICENSE` & `yaml_config_builder-8.0.2/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,237 +1,220 @@
-Open Logistics License
-Version 1.0, March 2022
+Open Logistics Foundation License
+Version 1.3, January 2023
 https://www.openlogisticsfoundation.org/licenses/
 
-TERMS AND CONDITIONS FOR THE USE, REPRODUCTION AND DISTRIBUTION
+TERMS AND CONDITIONS FOR USE, REPRODUCTION AND DISTRIBUTION
 
 §1 Definitions
 
-(1) "Subject Matter of the License" means the copyrighted works of the software
-components in source code or object code as well as the other components
-protected under copyright, design and/or patent law which are made available
-under this license in accordance with a copyright notice inserted into or
-attached to the work as well as the application and user documentation.
+(1) "Subject Matter of the License" shall mean the works of software components
+in Source or Object form as well as any other components protected under
+copyright, design and/or patent law which are made available under this License.
 
-(2) "License" means the terms and conditions for the use, reproduction and
+(2) "License" shall mean the terms and conditions for the use, reproduction and
 distribution of the Subject Matter of the License in accordance with the
 provisions of this document.
 
-(3) "Licensor(s)" means the copyright holder(s) or the entity authorised by law
-or contract by the copyright holder(s) to grant the license.
+(3) "Licensor(s)" shall mean the copyright holder(s) or the entity authorized by
+law or contract by the copyright holder(s) to grant the License.
 
-(4) "You" (or "Your") means a natural or legal person exercising the
+(4) "You" (or "Your") shall mean a natural or legal person exercising the
 permissions granted by this License.
 
-(5) "Source Code" means the version of the code of the software components of
-the Subject Matter of the License in the programming language.
+(5) "Source" form shall mean the preferred form for making modifications,
+including but not limited to software source code, documentation source, and
+configuration files.
+
+(6) "Object" form shall mean any form resulting from mechanical transformation
+or translation of a Source form, including but not limited to compiled object
+code, generated documentation, and conversions to other media types.
 
-(6) "Object Code" means the interim product after compilation or interpretation
-of the Source Code.
-
-(7) "Derivative Works" shall mean any work, whether in Source or Object Code or
+(7) "Derivative Works" shall mean any work, whether in Source or Object form or
 any other form, that is based on (or derived from) the Subject Matter of the
 License and for which the editorial revisions, annotations, elaborations, or
 other modifications represent, as a whole, an original work of authorship. For
 the purposes of this License, Derivative Works shall not include works that
 remain separable from, or merely link (or bind by name) to the interfaces of,
 the Subject Matter of the License and Derivative Works thereof.
 
-(8) "Contribution" means any proprietary work, including the original version
-of the Subject Matter of the License and any changes or additions to such work,
-or Derivative Works of such work, that the copyright holder, or a natural or
-legal person authorised to make submissions, intentionally submits to the
-Licensor or one of the Licensors to be incorporated into the Subject Matter of
-the License.  For the purposes of this definition, "submit" means any form of
-electronic or written communication which is sent to the Licensor (or one of
-the Licensors) or its representatives to discuss or improve the Subject Matter
-of the License, including, but not limited to, communications sent via
-electronic mailing lists, source code control systems and issue tracking
-systems; however, communications that are clearly labelled as "no contribution"
-by the copyright holder or otherwise identified as such in writing are
-excluded.
-
-(9) "Contributor" means the Licensor and/or any natural or legal person on
-whose behalf the Licensor receives any Contribution subsequently incorporated
-into the Subject Matter of the License.
+(8) "Contribution" shall mean any proprietary work, including the original
+version of the Subject Matter of the License and any changes or additions to
+such work, or Derivative Works of such work, that the rights holder, or a
+natural or legal person authorized to make submissions, intentionally submits to
+a Licensor to be incorporated into the Subject Matter of the License. For the
+purposes of this definition, "submit" shall mean any form of electronic or
+written communication which is sent to a Licensor or its representatives for the
+purpose of discussing or improving the Subject Matter of the License, including
+but not limited to communications sent via electronic mailing lists, source code
+control systems and issue tracking systems; however, communications that are
+clearly marked by the copyright holder as "not a contribution" or otherwise
+identified as such in writing are excluded.
+
+(9) "Contributor" shall mean the Licensor(s) and/or any natural or legal person
+on whose behalf the Licensor(s) receive(s) any Contribution subsequently
+incorporated into the Subject Matter of the License.
 
-§2 Granting of usage rights
+§2 Grant of usage rights
 
 Subject to the terms and conditions of this License and compliance with the
-provisions of this License, You are hereby granted by all Contributors, for the
-term of the copyrights in the Subject Matter of the License, the
+provisions of this License, You are hereby granted by each Contributor, insofar
+as applicable to the respective Subject Matter of the License the
 
 - royalty-free and non-exclusive,
 - sub-licensable for commercial and non-commercial purposes,
 - worldwide and perpetual,
 - irrevocable and non-terminable
 
-right
-
-- to use in any hardware and software environment, - with regard to the
-  software and data components – in particular to store or load it permanently
-  or temporarily, to display it and run it, including to the extent
-  reproductions are necessary to that end,
-- to modify, interpret, edit or redesign in another way,
-- to store, reproduce, exhibit, publish, distribute in tangible or intangible
+right to reproduce, prepare Derivative Works of, publicly display, publicly
+perform, and distribute the Subject Matter of the License and such Derivative
+Works in any form. This right of use includes but is not limited to the right
+
+- to use the Subject Matter of the License in any hardware and software
+  environment (with regard to the software and data components), in particular
+  to store or load it permanently or temporarily, to display it and run it,
+  including to the extent reproductions are necessary to that end,
+- to otherwise modify, interpret, edit or redesign it,
+- to store, reproduce, exhibit, publish, distribute it in tangible or intangible
   form, on any medium or in any other way, for commercial and non-commercial
-  purposes, in particular to communicate privately or publicly, also through
+  purposes, in particular to communicate it privately or publicly, including via
   image, audio and other information carriers, irrespective of whether by wire
   or wireless means,
-- to use in databases, data networks and online services, including the right
+- to use it in databases, data networks and online services, including the right
   to make the software and data components of the Subject Matter of the License
-  available in source code or object code to users of the aforementioned
-  databases, networks and online services for research and retrieval purposes,
-- to allow third parties to use or operate,
-- to use for own purposes but also to provide services to third parties,
-- to distribute
-
-the Subject Matter of the License in its original or modified, interpreted,
-edited or redesigned form.
-
-This right of use relates to the Subject Matter of the License in particular
-its source code and object code of the software components in all forms
-(including - where applicable - design rights).
+  available in Source or Object form to users of the aforementioned databases,
+  networks and online services for research and retrieval purposes,
+- to allow third parties to use or operate it,
+- to use it for own purposes but also to provide services to third parties,
+- to distribute it
+
+in its original or modified, interpreted, edited or redesigned form.
+
+The foregoing right of use relates to the Subject Matter of the License, in
+particular to its Source and Object form of software components (including
+design rights, where applicable).
 
-§3 Grant of a patent license
+§3 Grant of patent license
 
 Subject to the terms and conditions of this License and compliance with the
 provisions of this License, You are hereby granted by each Contributor a
-
-- perpetual,
-- worldwide,
-- non-exclusive,
-- free of charge,
-- irrevocable (with the exception of the restrictions set out in this
-  Section 3)
+- royalty-free and non-exclusive,
+- worldwide and perpetual,
+- irrevocable (with the exception of the restrictions set out in this Section 3)
 
 patent license in all rights deriving from the patents, owned and licensable by
 the Contributor at the time of the submission of the Contribution, to
 
 - produce,
 - have produced,
 - use,
 - offer for sale,
 - sell,
 - import and otherwise transfer
 
 the Subject Matter of the License.
 
-However, this patent license covers only those rights deriving from the patents
-of the respective Contributors as are indispensable in order not to infringe
-that patent and only to the extent that the use of the Contributor’s respective
-Contributions, whether in itself or as a combination with other Contributions
-of the Contributors or any third parties together with the Subject Matter of
-the License for which these Contributions were submitted, would otherwise
-infringe that patent. For avoidance of doubt, no patent licenses are granted
-for the use of the Subject Matter of the License or the Contributions which
-become necessary for lawful use because third party modifications are made to
-the Subject Matter of the License or the respective Contributions after the
-Contributions has been submitted by the Contributors. Under no circumstances
-will anything in this Section 3 be construed as granting, by implication,
-estoppel or otherwise, a license to any patent for which the respective
-Contributors have not granted patent rights when they submitted their
-respective Contributions.
-
-In the event that You institute judicial patent proceedings against any entity
-or person (including a counterclaim or countersuit in a legal dispute), arguing
-that the Subject Matter of the License or a Contribution incorporated or
-contained therein constitutes a patent infringement or a contributory factor to
-a patent infringement, all patent licenses which have been granted to You under
-this License for the Subject Matter of the License as well as this License in
-itself shall be deemed terminated as of the date on which the action is filed.
-
-For avoidance of doubt, the Contributors are entitled to decide in their own
-discretion to abandon respectively maintain any patent designated by patent
-number upon delivery of the Subject Matter of the License.
+However, said patent license shall cover only those rights deriving from the
+patents of the respective Contributors which are indispensable in order not to
+infringe that patent and only to the extent that the use of the Contributor’s
+respective Contributions, whether alone or in combination with other
+Contributions of the Contributors or any third parties together with the Subject
+Matter of the License for which these Contributions were submitted, would
+otherwise infringe that patent. The grant of license shall not include rights
+deriving from the patents which may in future become necessary for their lawful
+use due to subsequent modifications to the Subject Matter or Contributions made
+by third parties after the original submission.
+
+In the event that You institute patent litigation against any entity or person
+(including a counterclaim or countersuit in a legal action), alleging that the
+Subject Matter of the License or a Contribution incorporated or contained
+therein constitutes patent infringement or indirect infringement, all patent
+licenses which have been granted to You under this License for the Subject
+Matter of the License as well as this License itself shall be deemed terminated
+as of the date on which the action is filed.
 
 §4 Distribution
 
 You may reproduce and distribute copies of the Subject Matter of the License or
-Derivative Works on any medium, with or without modifications, (with regard to
-software components) in Source or Object Code, provided that You comply with
+Derivative Works on any medium, with or without modifications (with regard to
+software components in Source or Object form), provided that You comply with
 the following rules:
 
 - You must provide all other recipients of the Subject Matter of the License or
   of Derivative Works with a copy of this License and inform them that the
   Subject Matter of the License was originally licensed under this License.
 - You must ensure that modified files contain prominent notices indicating that
   You have modified the files.
-- You must retain all copyright, patent, trademark and name credit notices in
-  the Subject Matter of the License in the source code of any Derivative Works
-  You distribute, with the exception of those notices which do not belong to
-  any part of the Derivative Works.
-- You must oblige the recipients of the Subject Matter of the License or
-  Derivative Works to incorporate the provisions of this Section 4 into any
-  license under which they distribute the the Subject Matter of the License or
-  Derivative Works to any other recipients.
+- You must retain all copyright, patent, trademark and attribution notices in
+  the Subject Matter of the License in the Source form of any Derivative Works
+  You distribute, with the exception of those notices that do not pertain to any
+  part of the Derivative Works.
 
 You may add Your own copyright notices to Your modifications and state any
 additional or different license conditions and conditions for the use,
-reproduction or distribution of Your modifications or for these Derivative
-Works as a whole, provided that Your use, reproduction and distribution of the
-work in all other respects complies with the terms and conditions set out in
-this License.
+reproduction or distribution of Your modifications or for those Derivative Works
+as a whole, provided that Your use, reproduction and distribution of the work
+complies with the terms and conditions set out in this License in all other
+respects.
 
 §5 Submission of Contributions
 
 Unless expressly stated otherwise, every Contribution that You have
 intentionally submitted for inclusion in the Subject Matter of the License is
 subject to this License without any additional terms or conditions applying.
 Irrespective of the above, none of the terms or conditions contained herein may
-be interpreted to replace or change the terms or conditions of a separate
+be interpreted to supersede or modify the terms or conditions of any separate
 licensing agreement that You may have concluded with a Licensor for such
 Contributions, such as a so-called "Contributor License Agreement" (CLA).
 
 §6 Trademarks
 
 This License does not grant permission to use the trade names, trademarks,
-service marks or product names of the Licensor or of a Contributor.
+service marks or product names of the Licensor(s) or of a Contributor.
 
 §7 Limited warranty
 
-This License is granted free of charge and thus constitutes a gift.
-Accordingly, any warranty is excluded. Work on the Subject Matter of the
-License continues on an ongoing basis; it is constantly improved by countless
-Contributors. The Subject Matter of the License is not completed and may
-therefore contain errors ("bugs") or additional patents of Contributors or
-third parties, as is inherent to this type of development.
+This License is granted free of charge and thus constitutes a gift. Accordingly,
+any warranty is excluded. The Subject Matter of the License is a work in
+progress; it is constantly being improved by countless Contributors. The Subject
+Matter of the License is not complete and may therefore contain errors ("bugs")
+or additional patents of Contributors or third parties, as is inherent in this
+type of development.
 
 §8 Limitation of liability
 
-Except in cases of intent and gross negligence or causing personal injury, the
-Contributors, their legal representatives, trustees, officers and employees
-shall not be liable for direct or indirect, material or immaterial loss or
-damage of any kind arising from the License or the use of the Subject Matter of
-the License; this applies, among other things, but not exclusively, to loss of
-goodwill, loss of production, computer failures or errors, loss of data or
-economic loss or damage, even if the Contributor has been notified of the
-possibility of such loss or damage. Irrespective of the above, the Licensor
-shall only be liable in the scope of statutory product liability, to the extent
-the respective provisions are applicable to the Subject Matter of the License
-or the Contribution.
-
-Except in the case of intent, the Contributors, their legal representatives,
-trustees, officers and employees shall not be liable that any of the
-Contributions are free from any claim of infringement of any patent or any
-other intellectual property right owned by any third party, accurate, devoid of
-mistakes, complete and/or usable for any purpose.
+Except in cases of intentional and grossly negligent conduct, the Contributors,
+their legal representatives, trustees, officers and employees shall not be
+liable for direct or indirect, material or immaterial loss or damage of any kind
+arising from the License or the use of the Subject Matter of the License; this
+applies, among other things, but not exclusively, to loss of goodwill, loss of
+production, computer failures or errors, loss of data or economic loss or
+damage, even if the Contributor has been notified of the possibility of such
+loss or damage. Irrespective of the above, the Licensor shall only be liable
+within the scope of statutory product liability to the extent that the
+respective provisions are applicable to the Subject Matter of the License or the
+Contribution.
+
+Except in cases of intentional conduct, the Contributors, their legal
+representatives, trustees, officers and employees shall not be liable for any
+infringement of third-party patent or intellectual property rights arising from
+the Contributions nor do they warrant that the Contributions are accurate,
+devoid of mistakes, complete and/or fit for any particular purpose.
 
-§9 Provision of warranties or assumption of additional liability in the event
-of distribution of the Subject Matter of the License
+§9 Provision of warranties or assumption of additional liability in the event of
+distribution of the Subject Matter of the License
 
 In the event of distribution of the Subject Matter of the License or Derivative
-Works, You are free to assume support, warranty, indemnity or other liability
-obligations and/or rights in accordance with this License and to charge a fee
-in return. However, in accepting such obligations, You may act only on Your own
+Works, You are free to accept support, warranty, indemnity or other liability
+obligations and/or rights consistent with this License and to charge a fee in
+return. However, in accepting such obligations, You may act only on Your own
 behalf and on Your sole responsibility, not on behalf of any other Contributor,
 and You hereby agree to indemnify, defend, and hold each Contributor harmless
 for any liability incurred by, or claims asserted against, such Contributor by
-reason of your accepting any such warranty or additional liability.
+reason of Your accepting any such warranty or additional liability.
 
 §10 Applicable law
 
-This License is governed by German law with the exclusion of its provisions on
-the conflict of laws and with the exclusion of the UN Convention on Contracts
-for the International Sale of Goods (CISG).
+This License is governed by German law, excluding its conflict of laws
+provisions and the provisions of the UN Convention on Contracts for the
+International Sale of Goods (CISG).
 
 END OF TERMS AND CONDITIONS
```

### Comparing `yaml_config_builder-8.0.1/README.md` & `yaml_config_builder-8.0.2/README.md`

 * *Files identical despite different names*

### Comparing `yaml_config_builder-8.0.1/pyproject.toml` & `yaml_config_builder-8.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "yaml-config-builder"
-version = "8.0.1"
-license = "Open Logistics License Version 1.0"
 description = "Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files"
+version = "8.0.2"
+license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -22,33 +22,30 @@
     { include = "config_builder", from="src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 related-mltoolbox = { version = ">=1.0.1,<2" }
 attrs = { version = ">=20" }
-PyYAML = { version = "^5.4" }
-future = { version = "^0.18" }
-python-dateutil = { version = "^2.8" }
+PyYAML = { version = ">5.4" }
+future = { version = ">0.18" }
+python-dateutil = { version = ">2.8" }
 
 [tool.poetry.dev-dependencies]
-mock = { version = ">=4.0,<6" }
-pytest = { version = ">=6.2,<8" }
-pytest-cov = { version = ">=2.12,<=4" }
-pytest-flake8 = { version = "*" }
-pytest-mccabe = { version = "*" }
-pytest-pep8 = { version = "*" }
-pytest-pythonpath = { version = "*" }
-pytest-sugar = { version = "*" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
-mypy = { version = ">=0.910" }
+mypy = { version = ">=0.961" }
 pylint = { version = ">=2.9.6" }
-isort = { version = ">=5.9" }
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
+pytest-mock = { version = ">=3.7" }
 # This always needed as a development tool
-setuptools = { version = "*" }
+setuptools = { version = ">=67" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `yaml_config_builder-8.0.1/src/config_builder/base_config_class.py` & `yaml_config_builder-8.0.2/src/config_builder/base_config_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of the BaseConfigClass that should be used as superclass for any configuration
 class that should be built with the ConfigBuilder.
 """
 from __future__ import annotations
```

### Comparing `yaml_config_builder-8.0.1/src/config_builder/config_builder.py` & `yaml_config_builder-8.0.2/src/config_builder/config_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
+
+""" Main class for building configuration classes """
 
 import argparse
 import logging
 import os
 from collections import OrderedDict
 from pathlib import Path
 from typing import Callable, Dict, Optional, Type, cast
```

### Comparing `yaml_config_builder-8.0.1/src/config_builder/replacement_map.py` & `yaml_config_builder-8.0.2/src/config_builder/replacement_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition and handling of a replacement-map that is used in the ConfigBuilder
 to provide information that is used to apply placeholder replacement in strings.
 """
 
 import copy
```

### Comparing `yaml_config_builder-8.0.1/src/config_builder/utils.py` & `yaml_config_builder-8.0.2/src/config_builder/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of utility methods that are used across the config-builder
 """
 
 from __future__ import absolute_import, division, print_function
```

### Comparing `yaml_config_builder-8.0.1/src/config_builder/yaml_constructors.py` & `yaml_config_builder-8.0.2/src/config_builder/yaml_constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of constructors that can be added to the python yaml package
 """
 
 from __future__ import absolute_import, annotations, division, print_function
```

### Comparing `yaml_config_builder-8.0.1/setup.py` & `yaml_config_builder-8.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 packages = \
 ['config_builder']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=5.4,<6.0',
+['PyYAML>5.4',
  'attrs>=20',
- 'future>=0.18,<0.19',
- 'python-dateutil>=2.8,<3.0',
+ 'future>0.18',
+ 'python-dateutil>2.8',
  'related-mltoolbox>=1.0.1,<2']
 
 setup_kwargs = {
     'name': 'yaml-config-builder',
-    'version': '8.0.1',
+    'version': '8.0.2',
     'description': 'Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files',
     'long_description': '# Config Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes on the basis of \ngiven content from YAML configuration files. Details about the ConfigBuilder can be\nfound in the [documentation](documentation/index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder is described in [chapter 11](documentation/12_tutorial.adoc) \nof the documentation.\n\n# Technology stack\n\n- Python \n\n## License\nSee the license file in the top directory.\n\n## Contact information\n\n\nMaintainer: \n- Maximilian Otten <a href="mailto:maximilian.otten@iml.fraunhofer.de?">maximilian.otten@iml.fraunhofer.de</a>\n\nDevelopment Team: \n- Christian Hoppe <a href="mailto:christian.hoppe@iml.fraunhofer.de?">christian.hoppe@iml.fraunhofer.de</a>\n- Oliver Bredtmann <a href="mailto:oliver.bredtmann@dbschenker.com?">oliver.bredtmann@dbschenker.com</a>\n- Thilo Bauer <a href="mailto:thilo.bauer@dbschenker.com?">thilo.bauer@dbschenker.com</a>\n\n\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder',
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['config_builder'] package_data = \ {'': ['*']}
-install_requires = \ ['PyYAML>=5.4,<6.0', 'attrs>=20', 'future>=0.18,<0.19',
-'python-dateutil>=2.8,<3.0', 'related-mltoolbox>=1.0.1,<2'] setup_kwargs =
-{ 'name': 'yaml-config-builder', 'version': '8.0.1', 'description': 'Yaml-
-Config-Builder: SDK for building configuration classes on the basis of given
-content from YAML configuration files', 'long_description': '# Config
-Builder\n\nThe ConfigBuilder provides an SDK for building configuration classes
-on the basis of \ngiven content from YAML configuration files. Details about
-the ConfigBuilder can be\nfound in the [documentation](documentation/
+install_requires = \ ['PyYAML>5.4', 'attrs>=20', 'future>0.18', 'python-
+dateutil>2.8', 'related-mltoolbox>=1.0.1,<2'] setup_kwargs = { 'name': 'yaml-
+config-builder', 'version': '8.0.2', 'description': 'Yaml-Config-Builder: SDK
+for building configuration classes on the basis of given content from YAML
+configuration files', 'long_description': '# Config Builder\n\nThe
+ConfigBuilder provides an SDK for building configuration classes on the basis
+of \ngiven content from YAML configuration files. Details about the
+ConfigBuilder can be\nfound in the [documentation](documentation/
 index.adoc).\n\n## Install\n\nThe installation and setup of the ConfigBuilder
 is described in [chapter 11](documentation/12_tutorial.adoc) \nof the
 documentation.\n\n# Technology stack\n\n- Python \n\n## License\nSee the
 license file in the top directory.\n\n## Contact information\n\n\nMaintainer:
 \n- Maximilian Otten maximilian.otten@iml.fraunhofer.de\n\nDevelopment Team:
 \n- Christian Hoppe christian.hoppe@iml.fraunhofer.de\n- Oliver Bredtmann
 oliver.bredtmann@dbschenker.com\n- Thilo Bauer
```

### Comparing `yaml_config_builder-8.0.1/PKG-INFO` & `yaml_config_builder-8.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: yaml-config-builder
-Version: 8.0.1
+Version: 8.0.2
 Summary: Yaml-Config-Builder: SDK for building configuration classes on the basis of given content from YAML configuration files
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
-License: Open Logistics License Version 1.0
+License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=5.4,<6.0)
+Requires-Dist: PyYAML (>5.4)
 Requires-Dist: attrs (>=20)
-Requires-Dist: future (>=0.18,<0.19)
-Requires-Dist: python-dateutil (>=2.8,<3.0)
+Requires-Dist: future (>0.18)
+Requires-Dist: python-dateutil (>2.8)
 Requires-Dist: related-mltoolbox (>=1.0.1,<2)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 Description-Content-Type: text/markdown
 
 # Config Builder
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.0.1 Summary: Yaml-
+Metadata-Version: 2.1 Name: yaml-config-builder Version: 8.0.2 Summary: Yaml-
 Config-Builder: SDK for building configuration classes on the basis of given
 content from YAML configuration files Home-page: https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
-License: Open Logistics License Version 1.0 Author: Maximilian Otten Author-
+License: Open Logistics Foundation License 1.3 Author: Maximilian Otten Author-
 email: maximilian.otten@iml.fraunhofer.de Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: PyYAML (>=5.4,<6.0) Requires-Dist: attrs (>=20) Requires-Dist: future
-(>=0.18,<0.19) Requires-Dist: python-dateutil (>=2.8,<3.0) Requires-Dist:
-related-mltoolbox (>=1.0.1,<2) Project-URL: Documentation, https://
+Dist: PyYAML (>5.4) Requires-Dist: attrs (>=20) Requires-Dist: future (>0.18)
+Requires-Dist: python-dateutil (>2.8) Requires-Dist: related-mltoolbox
+(>=1.0.1,<2) Project-URL: Documentation, https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder/
 -/blob/main/documentation/index.adoc Project-URL: Repository, https://
 git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/config-builder
 Description-Content-Type: text/markdown # Config Builder The ConfigBuilder
 provides an SDK for building configuration classes on the basis of given
 content from YAML configuration files. Details about the ConfigBuilder can be
 found in the [documentation](documentation/index.adoc). ## Install The
```

