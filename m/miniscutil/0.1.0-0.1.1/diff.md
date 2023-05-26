# Comparing `tmp/miniscutil-0.1.0.tar.gz` & `tmp/miniscutil-0.1.1.tar.gz`

## Comparing `miniscutil-0.1.0.tar` & `miniscutil-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/misc.py
--rw-r--r--   0        0        0    12454 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/type_util.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/README.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/__init__.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/server.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/__init__.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/io_transport.py
--rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/websocket_transport.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_humansize.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.1.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.1.0/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/misc.py
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0    12321 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/extrarpc.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    19393 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.1.1/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_humansize.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.1.1/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.1.1/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.1.1/PKG-INFO
```

### Comparing `miniscutil-0.1.0/miniscutil/__init__.py` & `miniscutil-0.1.1/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/adapt.py` & `miniscutil-0.1.1/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/asyncio_helpers.py` & `miniscutil-0.1.1/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/config.py` & `miniscutil-0.1.1/miniscutil/config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/current.py` & `miniscutil-0.1.1/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/deep.py` & `miniscutil-0.1.1/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/deepeq.py` & `miniscutil-0.1.1/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/dispatch.py` & `miniscutil-0.1.1/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/misc.py` & `miniscutil-0.1.1/miniscutil/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     Set,
     Tuple,
     TypeVar,
 )
 from functools import partial
 import math
 import functools
+import contextvars
+import contextlib
 
 
 X = TypeVar("X")
 Y = TypeVar("Y")
 Z = TypeVar("Z")
 
 
@@ -101,7 +103,27 @@
     parts = urlparse(url)
     query = dict(parse_qsl(parts.query))
     query.update(params)
     parts = parts._replace(query=urlencode(query))
     result = urlunparse(parts)
     assert isinstance(result, str)
     return result
+
+
+T = TypeVar("T")
+
+
+@contextlib.contextmanager
+def set_ctx(v: contextvars.ContextVar[T], t: T):
+    x = v.set(t)
+    try:
+        yield t
+    finally:
+        v.reset(x)
+
+
+@contextlib.contextmanager
+def map_ctx(v: contextvars.ContextVar[T], f: Callable[[T], T]):
+    x = v.get()
+    x2 = f(x)
+    with set_ctx(v, x2):
+        yield x2
```

### Comparing `miniscutil-0.1.0/miniscutil/ofdict.py` & `miniscutil-0.1.1/miniscutil/ofdict.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from collections import ChainMap
+from contextlib import contextmanager
 from dataclasses import fields, is_dataclass
 from datetime import datetime
 from enum import Enum
 from functools import singledispatch
 import inspect
 import json
+from contextvars import ContextVar
 from pathlib import Path
 from typing import (
     Any,
     ClassVar,
     Dict,
     List,
     Literal,
@@ -17,14 +19,15 @@
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 import logging
+from miniscutil.misc import map_ctx
 
 from pydantic import ValidationError
 from .dispatch import classdispatch
 from .type_util import as_list, as_newtype, as_optional, as_set, is_optional
 
 try:
     from typing import TypeGuard
@@ -58,20 +61,44 @@
             else:
                 raise ValueError(
                     f"Missing {f.name} on input dict. Decoding {a} to type {A}."
                 )
         else:
             v = a[k]
         if f.type is not None:
-            d2[k] = ofdict(f.type, v)
+            with dpath(k):
+                d2[k] = ofdict(f.type, v)
         else:
             d2[k] = v
     return A(**d2)  # type: ignore
 
 
+ofdict_context: ContextVar[list[str]] = ContextVar("ofdict_context", default=[])
+
+
+def atstr():
+    p = ofdict_context.get()
+    if len(p) == 0:
+        return ""
+    else:
+        s = ".".join(p)
+        return f" at {s}"
+
+
+@contextmanager
+def dpath(coord: str):
+    with map_ctx(ofdict_context, lambda x: x + [coord]) as p:
+        yield p
+
+
+class OfDictError(TypeError):
+    def __init__(self, msg: str):
+        super().__init__(msg + atstr())
+
+
 @classdispatch
 def ofdict(A: Type[T], a: JsonLike) -> T:
     """Converts an ``a`` to an instance of ``A``, calling recursively if necessary.
 
     We assume that ``a`` is a nested type made of dicts, lists and scalars.
 
     The main usecase is to be able to treat dataclasses as a schema for json.
@@ -88,23 +115,23 @@
     S = as_newtype(A)
     if S is not None:
         return A(ofdict(S, a))
     if inspect.isclass(A) and issubclass(A, OfDictUnion):
         class_key = getattr(A, "_class_key", "__class__")
         ct = getattr(A, "_class_table", None)
         if ct is None:
-            raise TypeError(f"failed to find class table for {A}")
+            raise OfDictError(f"failed to find class table for {A}")
         assert isinstance(a, dict)
         C: Optional[type] = a.get(class_key, None)
         if C is None:
-            raise TypeError(
-                f"ofdict for a subclass of 'OfDictUnion' must include a '{class_key}' key."
+            raise OfDictError(
+                f"ofdict for a subclass of 'OfDictUnion' must include a '{class_key}' key"
             )
         if not issubclass(C, A):
-            raise TypeError(f"Expected {C} to be a subclass of {A}")
+            raise OfDictError(f"Expected {C} to be a subclass of {A}")
         A = C  # type: ignore
 
     if A is Any:
         return a  # type: ignore
     if A is type(None) and a is None:
         return a  # type: ignore
     if get_origin(A) is Literal:
@@ -132,54 +159,62 @@
             return result
     if is_dataclass(A):
         return ofdict_dataclass(A, a)  # type: ignore
     if A in [float, str, int, bytes]:  # [todo] etc
         if isinstance(a, A):
             return a  # type: ignore
         else:
-            raise TypeError(f"Expected an {A} but was {type(a)}")
+            raise OfDictError(
+                f"Expected a {A.__name__} but was {type(a).__name__}: {a}"
+            )
     try:
         if isinstance(a, A):
             return a  # type: ignore
     except TypeError:
         pass
-    raise NotImplementedError(f"No implementation of ofdict for {A}.")
+    raise NotImplementedError(f"No implementation of ofdict for {A.__name__}.")
 
 
 @ofdict.register(list)
 def _list_ofdict(A, a):
     if not isinstance(a, list):
-        raise TypeError(f"Expected a list but got a {type(a)}")
+        raise OfDictError(f"Expected a list but got a {type(a)}")
     X = as_list(A)
     if X is not None:
         return [ofdict(X, y) for y in a]
     else:
         return a
 
 
 @ofdict.register(set)
 def _set_ofdict(A, a):
     if not isinstance(a, list):
-        raise TypeError(f"Expected a list but got a {type(a)}")
+        raise OfDictError(f"Expected a list but got a {type(a)}")
     X = as_set(A)
     if X is not None:
         return set(ofdict(X, y) for y in a)
     else:
         return set(a)
 
 
 @ofdict.register(dict)
 def _dict_ofdict(A, a):
     if not isinstance(a, dict):
-        raise TypeError(f"Expected a {A} but got {type(a)}")
+        raise OfDictError(f"Expected a {A} but got {type(a)}")
     o = get_origin(A)
     if o is None:
         return a
     K, V = get_args(A)
-    return o({ofdict(K, k): ofdict(V, v) for k, v in a.items()})
+    d = {}
+    for k, v in a.items():
+        with dpath(str(k)):
+            vk = ofdict(K, k)
+            vv = ofdict(V, v)
+            d[vk] = vv
+    return o(d)
 
 
 @ofdict.register(Enum)
 def _ofdict_enum(A, a):
     return A(a)
```

### Comparing `miniscutil-0.1.0/miniscutil/sum.py` & `miniscutil-0.1.1/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/type_util.py` & `miniscutil-0.1.1/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/lsp/server.py` & `miniscutil-0.1.1/miniscutil/lsp/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import logging
-from .types import InitializeParams, InitializeResult, PeerInfo, ServerCapabilities
-from miniscutil.rpc import RpcServer, InitializationMode, rpc_method
+from .types import (
+    InitializeParams,
+    InitializeResult,
+    PeerInfo,
+    ServerCapabilities,
+    ApplyWorkspaceEditParams,
+)
+from ..rpc import InitializationMode, rpc_method
+from ..rpc.extrarpc import ExtraRpc
 
 """ Implementation of an LSP server """
 
 logger = logging.getLogger("LSP")
 
 
-class LspServer(RpcServer):
+class LspServer(ExtraRpc):
     capabilities: ServerCapabilities
 
     def __init__(self, transport):
         self.capabilities = ServerCapabilities()
         super().__init__(transport, init_mode=InitializationMode.ExpectInit)
 
     @rpc_method("initialize")
@@ -21,7 +28,10 @@
             serverInfo=PeerInfo(name=self.name, version=None),
             capabilities=self.capabilities,
         )
 
     @rpc_method("initialized")
     async def on_client_initialized(self, params):
         logger.info("client initialized")
+
+    async def apply_workspace_edit(self, params: ApplyWorkspaceEditParams):
+        return await self.request("workspace/applyEdit", params)
```

### Comparing `miniscutil-0.1.0/miniscutil/rpc/io_transport.py` & `miniscutil-0.1.1/miniscutil/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/rpc/jsonrpc.py` & `miniscutil-0.1.1/miniscutil/rpc/jsonrpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 from asyncio import Future, StreamReader, StreamWriter, Task
 import asyncio
 from functools import singledispatch, partial
 from dataclasses import MISSING, asdict, dataclass, field, is_dataclass
 from enum import Enum
 import logging
 import sys
-from typing import Any, Awaitable, Dict, List, Optional, Union, Coroutine
+from typing import (
+    Any,
+    Awaitable,
+    Dict,
+    Generic,
+    List,
+    Optional,
+    TypeVar,
+    Union,
+    Coroutine,
+)
 import inspect
 import warnings
 
 from miniscutil.ofdict import MyJsonEncoder, ofdict
 import json
 from .transport import Transport, TransportClosedError, TransportClosedOK
 
-from websockets.exceptions import ConnectionClosedOK, ConnectionClosedError
-
 logger = logging.getLogger(__name__)
 
 
 class ErrorCode(Enum):
     ### JSON-RPC codes
 
     parse_error = -32700
@@ -214,22 +222,26 @@
 
 
 class ExitNotification(Exception):
     """Thrown when the server recieved an exit notifaction from its peer."""
 
 
 def rpc_method(name: Optional[str] = None):
+    """Decorate your method with this to say that you are implementing a JSON-RPC method."""
+
     def decorator(fn):
         setattr(fn, "rpc_method", name or fn.__name__)
         return fn
 
     return decorator
 
 
 def rpc_request(name: Optional[str] = None):
+    """Decorate your _stub_ method with this to have a client RPC."""
+
     def decorator(fn):
         assert asyncio.iscoroutinefunction(fn)
         fn_name = name or fn.__name__
 
         async def method(self, params):
             return await self.request(fn_name, params)
 
@@ -264,17 +276,17 @@
     dispatcher: Dispatcher
     status: RpcServerStatus
     transport: Transport
     init_mode: InitializationMode
     name: str
     request_counter: int
     """ Unique id for each request I make to the peer. """
-    my_requests: Dict[RequestId, Future[Any]]
+    my_requests: dict[RequestId, Future[Any]]
     """ Requests that I have made to my peer. """
-    their_requests: Dict[RequestId, Task]
+    their_requests: dict[RequestId, Task]
     """ Requests that my peer has made to me. """
     notification_tasks: set[asyncio.Task]
     """ Tasks running from notifications that my peer has sent to me. """
 
     def __init__(
         self,
         transport: Transport,
@@ -334,14 +346,19 @@
                 raise RuntimeError(
                     f"can't make new requests while server is in {self.status.name} state"
                 )
         self.request_counter += 1
         id = self.request_counter
         req = Request(method=method, id=id, params=params)
         fut = asyncio.get_running_loop().create_future()
+        # [todo] I think the pythonic way to do this is to have this dict be a weakref, and the
+        # caller is responsible for holding the request object.
+        # If the request future is disposed then we send a cancel request to client.
+        if id in self.my_requests:
+            raise RuntimeError(f"non-unique request id {id} found")
         self.my_requests[id] = fut
         await self.send(req)
         result = await fut
         return result
 
     async def _send_init(self, init_param):
         await self.request("initialize", init_param)
@@ -351,16 +368,14 @@
     async def serve_forever(self, init_param=None):
         """Runs forever. Serves your client.
 
         It will return when:
         - the transport closes gracefully
         - the exit notification is received.
 
-        [todo] add param for initialise message to send _or_ flag indicating an initialisation message is expected first.
-
         Raises:
             - TransportClosedError:the transport closes with an error
             - TransportError: some other error at the transport level occurred
         """
         # [todo] add a lock to prevent multiple server loops from running at the same time.
 
         if self.init_mode == InitializationMode.SendInit:
@@ -443,14 +458,16 @@
                 self._shutdown()
             task = asyncio.create_task(
                 self._on_request(req),
                 name=f"{self.name} handle {req}",
             )
             id = req.id
             if id is not None:
+                if id in self.their_requests:
+                    raise invalid_request(f"request id {id} is already in use")
                 self.their_requests[id] = task
                 task.add_done_callback(lambda _: self.their_requests.pop(id))
             else:
                 self.notification_tasks.add(task)
                 task.add_done_callback(self.notification_tasks.discard)
 
     async def _on_request(self, req: Request) -> None:
@@ -515,19 +532,21 @@
                 raise invalid_params('params must be a dict with "id" key')
             t = self.their_requests.get(req.params["id"], None)
             if t is not None:
                 t.cancel("requested by peer")
             return None
 
         if req.method not in self.dispatcher:
+            logger.error(f'method "{req.method}" not found')
             raise method_not_found(req.method)
 
         T = self.dispatcher.param_type(req.method)
         try:
             params = ofdict(T, req.params)
         except TypeError as e:
             message = (
                 f"{req.method} {type(e).__name__} failed to decode params to {T}: {e}"
             )
+            logger.exception(message)
             raise invalid_params(message)
         result = await self.dispatcher.dispatch(req.method, params)
         return result
```

### Comparing `miniscutil-0.1.0/miniscutil/rpc/starlette_ws_transport.py` & `miniscutil-0.1.1/miniscutil/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/rpc/transport.py` & `miniscutil-0.1.1/miniscutil/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/miniscutil/rpc/websocket_transport.py` & `miniscutil-0.1.1/miniscutil/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_classdispatch.py` & `miniscutil-0.1.1/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_config.py` & `miniscutil-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_current.py` & `miniscutil-0.1.1/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_deepeq.py` & `miniscutil-0.1.1/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_ofdict.py` & `miniscutil-0.1.1/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/tests/test_typing.py` & `miniscutil-0.1.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/.gitignore` & `miniscutil-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/LICENSE.txt` & `miniscutil-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/README.md` & `miniscutil-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/pyproject.toml` & `miniscutil-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.1.0/PKG-INFO` & `miniscutil-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

