# Comparing `tmp/openepd-0.1.3.tar.gz` & `tmp/openepd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.1.3.tar", max compression
+gzip compressed data, was "openepd-0.2.0.tar", max compression
```

## Comparing `openepd-0.1.3.tar` & `openepd-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-05-25 13:27:41.578569 openepd-0.1.3/LICENSE
--rw-r--r--   0        0        0     2841 2023-05-25 13:27:41.578569 openepd-0.1.3/README.md
--rw-r--r--   0        0        0     3051 2023-05-25 13:27:41.578569 openepd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/base.py
--rw-r--r--   0        0        0     2573 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/common.py
--rw-r--r--   0        0        0     5740 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3783 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/org.py
--rw-r--r--   0        0        0     2913 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/model/pcr.py
--rw-r--r--   0        0        0        0 2023-05-25 13:27:41.582569 openepd-0.1.3/src/openepd/py.typed
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-26 15:18:34.913564 openepd-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2841 2023-05-26 15:18:34.913564 openepd-0.2.0/README.md
+-rw-r--r--   0        0        0     3051 2023-05-26 15:18:34.913564 openepd-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     1987 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     2178 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0     5838 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     9496 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3690 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2855 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:18:34.913564 openepd-0.2.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.2.0/PKG-INFO
```

### Comparing `openepd-0.1.3/LICENSE` & `openepd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.1.3/README.md` & `openepd-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.1.3/pyproject.toml` & `openepd-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.1.3"
+version = "0.2.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -36,15 +36,15 @@
 teamcity-messages = ">=1.31"
 
 # Dev tools
 #virtualenv = "<=20.23.0" # to avoid conflict with flake plugins
 black = "~=22.3"
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
-flake8-import-graph = "==0.1.3"
+flake8-import-graph = "~=0.1.3"
 flake8-docstrings = "~=1.7.0"
 isort = "~=5.11"
 mypy = ">=1.0.1"
 pre-commit = "~=2.19"
 commitizen = "~=2.42.1"
 
 # Type checking
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.1.3"
+version = "0.2.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.1.3/src/openepd/__init__.py` & `openepd-0.2.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.3/src/openepd/__version__.py` & `openepd-0.2.0/src/openepd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.1.3"
+VERSION = "0.2.0"
```

### Comparing `openepd-0.1.3/src/openepd/model/__init__.py` & `openepd-0.2.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.3/src/openepd/model/base.py` & `openepd-0.2.0/src/openepd/model/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,24 +16,43 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import pydantic
 from pydantic.generics import GenericModel
 
+AnySerializable = int | str | bool | float | list | dict | pydantic.BaseModel | None
+
 
 class BaseOpenEpdSchema(pydantic.BaseModel):
     """Base class for all OpenEPD models."""
 
+    extensions: dict[str, AnySerializable] | None = pydantic.Field(alias="ext", default=None)
+
     class Config:
         allow_mutation = True
         validate_assignment = False
 
     def has_values(self) -> bool:
         """Return True if the model has any values."""
         return len(self.dict(exclude_unset=True, exclude_none=True)) > 0
 
+    @classmethod
+    def is_allowed_field_name(cls, field_name: str) -> bool:
+        """
+        Return True if the field name is defined in the module.
+
+        Both property name and aliases are checked.
+        """
+        if field_name in cls.__fields__:
+            return True
+        else:
+            for x in cls.__fields__.values():
+                if x.alias == field_name:
+                    return True
+        return False
+
 
 class BaseOpenEpdGenericSchema(GenericModel, BaseOpenEpdSchema):
     """Base class for all OpenEPD generic models."""
 
     pass
```

### Comparing `openepd-0.1.3/src/openepd/model/common.py` & `openepd-0.2.0/src/openepd/model/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,29 +32,18 @@
 
 
 class Measurement(BaseOpenEpdSchema):
     """A scientific value with units and uncertainty."""
 
     mean: float = pyd.Field(description="Mean (expected) value of the measurement")
     unit: str = pyd.Field(description="Measurement unit")
-    rsd: pyd.PositiveFloat = pyd.Field(description="Relative standard deviation, i.e. standard_deviation/mean")
-    dist: str | None = pyd.Field(description="Statistical distribution of the measurement error.")
-
-
-class ExternalIdentification(BaseOpenEpdSchema):  # TODO: NEW Object, not in the spec
-    """Represent an external identification of an object."""
-
-    id: str
-    version: str | None
-
-
-class ExternallyIdentifiableMixin:  # TODO: NEW Object, not in the spec
-    """Mixin for objects that can be identified externally."""
-
-    identified: dict[str, ExternalIdentification] = pyd.Field(description="The external identification of the object.")
+    rsd: pyd.PositiveFloat | None = pyd.Field(
+        description="Relative standard deviation, i.e. standard_deviation/mean", default=None
+    )
+    dist: str | None = pyd.Field(description="Statistical distribution of the measurement error.", default=None)
 
 
 class WithAttachmentsMixin:
     """Mixin for objects that can have attachments."""
 
     attachments: dict[Annotated[str, pyd.constr(max_length=200)], pyd.AnyUrl] | None = pyd.Field(
         description="Dict of URLs relevant to this entry",
```

### Comparing `openepd-0.1.3/src/openepd/model/epd.py` & `openepd-0.2.0/src/openepd/model/epd.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 #
 import datetime
 from typing import Literal
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import Amount, ExternallyIdentifiableMixin
-from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet
+from openepd.model.common import Amount
+from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet, Standard
 from openepd.model.org import Org, Plant
 
 
-class Epd(ExternallyIdentifiableMixin, BaseOpenEpdSchema):
+class Epd(BaseOpenEpdSchema):
     """Represent an EPD."""
 
     # TODO: Add validator for open-xpd-uuid on this field
     id: str = pyd.Field(
         description="The unique ID for this EPD.  To ensure global uniqueness, should be registered at "
         "open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="1u7zsed8",
@@ -116,7 +116,10 @@
     resource_uses: ResourceUseSet | None = pyd.Field(
         description="Set of Resource Use Indicators, over various LCA scopes"
     )
     output_flows: OutputFlowSet | None = pyd.Field(
         description="Set of Waste and Output Flow indicators which describe the waste categories "
         "and other material output flows derived from the LCI."
     )
+    compliance: list[Standard] = pyd.Field(
+        description="Standard(s) to which this declaration is compliant.", default_factory=list
+    )
```

### Comparing `openepd-0.1.3/src/openepd/model/lcia.py` & `openepd-0.2.0/src/openepd/model/lcia.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Measurement
+from openepd.model.org import Org
 
 
 class EolScenario(BaseOpenEpdSchema):
     """
     A scenario for end-of-life.
 
     If a particular implementation commits to a specific scenario, then that value can be used;
@@ -163,7 +164,18 @@
     )
 
 
 class OutputFlowSet(BaseOpenEpdSchema):
     """A set of output flows, such as waste, emissions, etc."""
 
     hwd: ScopeSet | None = pyd.Field(description="Hazardous waste disposed")
+
+
+class Standard(BaseOpenEpdSchema):
+    """A standard, such as EN 15804, ISO 14044, ISO 14024:2018, etc."""
+
+    short_name: str = pyd.Field(description="Short-form of name of standard.  Must be unique. Case-insensitive")
+    name: str | None = pyd.Field(description="Full document name.  Must be unique. Case-insensitive", default=None)
+    link: pyd.AnyUrl | None = pyd.Field(
+        description="Link to the exact standard (including version) referred to", default=None
+    )
+    issuer: Org | None = pyd.Field(description="Org that issued this standard", default=None)
```

### Comparing `openepd-0.1.3/src/openepd/model/org.py` & `openepd-0.2.0/src/openepd/model/org.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,30 +18,28 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Annotated, Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import ExternallyIdentifiableMixin, WithAttachmentsMixin
+from openepd.model.common import WithAttachmentsMixin
 
 
 class Contact(BaseOpenEpdSchema):  # TODO: NEW Object, not in the spec
     """Contact information of a person or organization."""
 
     email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
     phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
     website: pyd.AnyUrl | None = pyd.Field(
         description="Url of the website", example="http://buildingtransparency.org", default=None
     )
 
 
-class Org(
-    ExternallyIdentifiableMixin, WithAttachmentsMixin, BaseOpenEpdSchema
-):  # TODO: NEW Identifiable field, not in the spec
+class Org(WithAttachmentsMixin, BaseOpenEpdSchema):  # TODO: NEW Identifiable field, not in the spec
     """Represent an organization."""
 
     web_domain: str = pyd.Field(
         description="A web domain owned by organization. Typically is the org's home website address",
     )
     name: str = pyd.Field(max_length=200, description="Common name for organization", example="C Change Labs")
     alt_names: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
@@ -55,15 +53,15 @@
     subsidiaries: Annotated[list[str], pyd.conlist(pyd.constr(max_length=200), max_items=255)] | None = pyd.Field(
         description="Organizations controlled by this organization",
         example=["cqd.io", "supplychaincarbonpricing.org"],
         default=None,
     )
 
 
-class Plant(ExternallyIdentifiableMixin, WithAttachmentsMixin, BaseOpenEpdSchema):
+class Plant(WithAttachmentsMixin, BaseOpenEpdSchema):
     """Represent a manufacturing plant."""
 
     # TODO: Add proper validator
     id: str = pyd.Field(
         description="Plus code (aka Open Location Code) of plant's location and "
         "owner's web domain joined with `.`(dot).",
         example="865P2W3V+3W.interface.com",
```

### Comparing `openepd-0.1.3/src/openepd/model/pcr.py` & `openepd-0.2.0/src/openepd/model/pcr.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 #
 import datetime
 from typing import Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.common import ExternallyIdentifiableMixin, WithAttachmentsMixin
+from openepd.model.common import WithAttachmentsMixin
 from openepd.model.org import Org
 
 
-class Pcr(ExternallyIdentifiableMixin, WithAttachmentsMixin, BaseOpenEpdSchema):
+class Pcr(WithAttachmentsMixin, BaseOpenEpdSchema):
     """Represent a PCR (Product Category Rules)."""
 
     id: str = pyd.Field(
         description="The unique ID for this PCR.  To ensure global uniqueness, should be registered "
         "at open-xpd-uuid.cqd.io/register or a coordinating registry.",
         example="ec3xpgq2",
     )
```

### Comparing `openepd-0.1.3/PKG-INFO` & `openepd-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.1.3
+Version: 0.2.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.1.3 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.2.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

