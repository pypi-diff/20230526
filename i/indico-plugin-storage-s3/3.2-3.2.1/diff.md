# Comparing `tmp/indico_plugin_storage_s3-3.2-py3-none-any.whl.zip` & `tmp/indico_plugin_storage_s3-3.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20005 bytes, number of entries: 13
--rw-r--r--  2.0 unx      484 b- defN 22-Jan-05 10:41 indico_storage_s3/__init__.py
--rw-r--r--  2.0 unx      496 b- defN 22-Jan-05 10:41 indico_storage_s3/blueprint.py
--rw-r--r--  2.0 unx     2717 b- defN 22-Jan-05 10:41 indico_storage_s3/controllers.py
--rw-r--r--  2.0 unx    22823 b- defN 22-Jan-05 10:41 indico_storage_s3/migrate.py
--rw-r--r--  2.0 unx     4568 b- defN 22-Jan-05 10:41 indico_storage_s3/plugin.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Feb-16 14:03 indico_storage_s3/storage.py
--rw-r--r--  2.0 unx     1710 b- defN 22-Jan-05 10:41 indico_storage_s3/task.py
--rw-r--r--  2.0 unx      732 b- defN 22-Jan-05 10:41 indico_storage_s3/util.py
--rw-r--r--  2.0 unx     7520 b- defN 22-Aug-24 22:14 indico_plugin_storage_s3-3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-24 22:14 indico_plugin_storage_s3-3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 22-Aug-24 22:14 indico_plugin_storage_s3-3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 22-Aug-24 22:14 indico_plugin_storage_s3-3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1147 b- defN 22-Aug-24 22:14 indico_plugin_storage_s3-3.2.dist-info/RECORD
-13 files, 53735 bytes uncompressed, 18061 bytes compressed:  66.4%
+Zip file size: 20071 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      484 b- defN 23-Jan-08 16:35 indico_storage_s3/__init__.py
+-rw-r--r--  2.0 unx      496 b- defN 23-Jan-08 16:35 indico_storage_s3/blueprint.py
+-rw-r--r--  2.0 unx     2717 b- defN 23-Apr-18 21:21 indico_storage_s3/controllers.py
+-rw-r--r--  2.0 unx    22823 b- defN 23-Jan-08 16:35 indico_storage_s3/migrate.py
+-rw-r--r--  2.0 unx     4568 b- defN 23-Jan-08 16:35 indico_storage_s3/plugin.py
+-rw-r--r--  2.0 unx    11348 b- defN 23-May-02 13:41 indico_storage_s3/storage.py
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jan-08 16:35 indico_storage_s3/task.py
+-rw-r--r--  2.0 unx      722 b- defN 23-May-02 13:41 indico_storage_s3/util.py
+-rw-r--r--  2.0 unx     7665 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1157 b- defN 23-May-26 14:33 indico_plugin_storage_s3-3.2.1.dist-info/RECORD
+13 files, 53871 bytes uncompressed, 18107 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: indico_storage_s3/task.py
 Comment: 
 
 Filename: indico_storage_s3/util.py
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.dist-info/METADATA
+Filename: indico_plugin_storage_s3-3.2.1.dist-info/METADATA
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.dist-info/WHEEL
+Filename: indico_plugin_storage_s3-3.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.dist-info/entry_points.txt
+Filename: indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.dist-info/top_level.txt
+Filename: indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: indico_plugin_storage_s3-3.2.dist-info/RECORD
+Filename: indico_plugin_storage_s3-3.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## indico_storage_s3/__init__.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from indico.core import signals
 from indico.util.i18n import make_bound_gettext
```

## indico_storage_s3/blueprint.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from indico.core.plugins import IndicoPluginBlueprint
```

## indico_storage_s3/controllers.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 from flask import current_app, jsonify, request
 from werkzeug.exceptions import NotFound, Unauthorized
```

## indico_storage_s3/migrate.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import errno
 import json
```

## indico_storage_s3/plugin.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import sys
```

## indico_storage_s3/storage.py

```diff
@@ -1,30 +1,30 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import hashlib
 import hmac
 import threading
 from base64 import b64encode
 from contextlib import contextmanager
 from datetime import date
 from enum import Enum
 from io import BytesIO
 from tempfile import NamedTemporaryFile
+from urllib.parse import quote
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 from botocore.config import Config
 from botocore.exceptions import ClientError
 from werkzeug.datastructures import Headers
-from werkzeug.urls import url_quote
 from werkzeug.utils import cached_property, redirect
 
 from indico.core.config import config
 from indico.core.storage import Storage, StorageError
 from indico.core.storage.backend import ReadOnlyStorageMixin, StorageReadOnlyError
 from indico.util.fs import get_file_checksum
 from indico.web.flask.util import send_file
@@ -152,15 +152,15 @@
                                                              'ResponseContentDisposition': h.get('Content-Disposition'),
                                                              'ResponseContentType': content_type},
                                                      ExpiresIn=120)
             response = redirect(url)
             if self.proxy_downloads == ProxyDownloadsMode.nginx:
                 # nginx can proxy the request to S3 to avoid exposing the redirect and
                 # bucket URL to the end user (since it is quite ugly and temporary)
-                response.headers['X-Accel-Redirect'] = '/.xsf/s3/' + url_quote(url.replace('://', '/', 1))
+                response.headers['X-Accel-Redirect'] = '/.xsf/s3/' + quote(url.replace('://', '/', 1))
             return response
         except Exception as exc:
             raise StorageError(f'Could not send file "{file_id}": {exc}') from exc
 
     def _create_bucket(self, name):
         from indico_storage_s3.plugin import S3StoragePlugin
```

## indico_storage_s3/task.py

```diff
@@ -1,9 +1,9 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import re
 from datetime import date
```

## indico_storage_s3/util.py

```diff
@@ -1,22 +1,21 @@
 # This file is part of the Indico plugins.
-# Copyright (C) 2002 - 2022 CERN
+# Copyright (C) 2002 - 2023 CERN
 #
 # The Indico plugins are free software; you can redistribute
 # them and/or modify them under the terms of the MIT License;
 # see the LICENSE file for more details.
 
 import unicodedata
-
-from werkzeug.urls import url_quote
+from urllib.parse import quote
 
 
 def make_content_disposition_args(attachment_filename):
     try:
         attachment_filename = attachment_filename.encode('ascii')
     except UnicodeEncodeError:
         return {
             'filename': unicodedata.normalize('NFKD', attachment_filename).encode('ascii', 'ignore'),
-            'filename*': "UTF-8''%s" % url_quote(attachment_filename, safe=b''),
+            'filename*': "UTF-8''%s" % quote(attachment_filename, safe=b''),
         }
     else:
         return {'filename': attachment_filename}
```

## Comparing `indico_plugin_storage_s3-3.2.dist-info/METADATA` & `indico_plugin_storage_s3-3.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: indico-plugin-storage-s3
-Version: 3.2
+Version: 3.2.1
 Summary: S3 storage backend for Indico
 Home-page: https://github.com/indico/indico-plugins
 Author: Indico Team
 Author-email: indico-team@cern.ch
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.9.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Requires-Dist: indico (>=3.2)
 Requires-Dist: boto3 (<2.0,>=1.20.51)
 
 # S3 Storage Plugin
 
@@ -28,22 +29,30 @@
 
 It is currently used in production on multiple Indico instances, so we believe it is
 stable, but please be advised that we do not provide a way to move files back from S3
 to local storage (but it would of course be possible to write a script for this).
 
 ## Changelog
 
+### 3.2.1
+
+- Stop using deprecated URL utils from werkzeug
+
+### 3.2
+
+- Update translations
+
 ### 3.1.2
 
 - No technical changes, just fixing a mistake in the README change from 3.1.1
 
 ### 3.1.1
 
 - No technical changes, just adding the missing README to PyPI and updating the nginx
-  config snippet to correclty work with the changes from 3.1 (avoiding an [nginx bug][nginx-bug])
+  config snippet to correctly work with the changes from 3.1 (avoiding an [nginx bug][nginx-bug])
 
 ### 3.1
 
 - Fix "invalid signature" S3 error in some cases when using `proxy=nginx` for downloads
 
 ### 3.0
```

## Comparing `indico_plugin_storage_s3-3.2.dist-info/RECORD` & `indico_plugin_storage_s3-3.2.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-indico_storage_s3/__init__.py,sha256=TX2CiefuZv6tTezfp_qRwLfyq3lM_TGphelvfx2cAi0,484
-indico_storage_s3/blueprint.py,sha256=f1JGluPL3BpPDVm0p3ZlmZ_D86veId8VGclbhZjjp5w,496
-indico_storage_s3/controllers.py,sha256=BSvqQJlPhnSoOenebmwNPgroEnL9k2tK3DVJB3IaWyk,2717
-indico_storage_s3/migrate.py,sha256=7HsJ4xslI-ARvQhVRh8XOJsjNYZFJL6WIs7I_QXDWBw,22823
-indico_storage_s3/plugin.py,sha256=sDe0_w75o8m9hJt7oYDXDIqoNHy_6bVe4OG0txL-kvU,4568
-indico_storage_s3/storage.py,sha256=ofKIW4UodDhpqqj5ScybEPCgIVWMebFb_9rS1-cL4uI,11357
-indico_storage_s3/task.py,sha256=JQYXDQM1-GYRQIEO0zFht7bd_tSddIvS01-nTMSzdM4,1710
-indico_storage_s3/util.py,sha256=emL4QBs58LH2b-vKnlv3D9pcqRXy0QIKMy1QVTHqxy8,732
-indico_plugin_storage_s3-3.2.dist-info/METADATA,sha256=PwFWXACd4wpd9LiOSiqcJxEqis9sQmDR-XyStdJTcvw,7520
-indico_plugin_storage_s3-3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-indico_plugin_storage_s3-3.2.dist-info/entry_points.txt,sha256=rts2AI5QEK9cu2WcFujOUCUtP9YMiABEMTQ-dkafx4Y,71
-indico_plugin_storage_s3-3.2.dist-info/top_level.txt,sha256=wMajir5p9AELlngQV8mOHyzu5xWvybvbG0rJg-YsQpM,18
-indico_plugin_storage_s3-3.2.dist-info/RECORD,,
+indico_storage_s3/__init__.py,sha256=WLQ_qJ1dwoX0newy-E-Jk3hUTA1SBxT0_bR_waCih5Y,484
+indico_storage_s3/blueprint.py,sha256=EqIG8VcrnABsds3PNVybE0mY6rwSHjDh02f0UihMbkY,496
+indico_storage_s3/controllers.py,sha256=nYxqHsJESuVzXzPupBPQb7bofek1mZ7OfDj5pMpNmsg,2717
+indico_storage_s3/migrate.py,sha256=Izla22EGd40_BF8Du_U0PnA6z33WqtWNDznY31gSOWA,22823
+indico_storage_s3/plugin.py,sha256=-Mk44tiQpjbOZSH-Q-xdAYR5YeubgeLhxsH_1emHhBg,4568
+indico_storage_s3/storage.py,sha256=VNuMxPD7kAiCoGQIkCxDvX02qVCmhCuE7FN9GTC-Dto,11348
+indico_storage_s3/task.py,sha256=O7o1-072NVl0JETMALehQ-PkTQF80y11gUaLyYfDnxY,1710
+indico_storage_s3/util.py,sha256=JwSbpGqwj-ownX9t2YYh17xk-KyjTIrFnpyjDS6-8vA,722
+indico_plugin_storage_s3-3.2.1.dist-info/METADATA,sha256=GLxX0YF8jDzBot2qdP9DVB1fuJLpWHXly6ePLMkR7KI,7665
+indico_plugin_storage_s3-3.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+indico_plugin_storage_s3-3.2.1.dist-info/entry_points.txt,sha256=rts2AI5QEK9cu2WcFujOUCUtP9YMiABEMTQ-dkafx4Y,71
+indico_plugin_storage_s3-3.2.1.dist-info/top_level.txt,sha256=wMajir5p9AELlngQV8mOHyzu5xWvybvbG0rJg-YsQpM,18
+indico_plugin_storage_s3-3.2.1.dist-info/RECORD,,
```

