# Comparing `tmp/configzen-0.1.36.tar.gz` & `tmp/configzen-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.36.tar", max compression
+gzip compressed data, was "configzen-0.1.37.tar", max compression
```

## Comparing `configzen-0.1.36.tar` & `configzen-0.1.37.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.36/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.36/configzen/__main__.py
--rw-r--r--   0        0        0    58117 2023-05-24 14:12:28.462371 configzen-0.1.36/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.36/configzen/errors.py
--rw-r--r--   0        0        0    20443 2023-05-21 16:48:48.942144 configzen-0.1.36/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.36/configzen/py.typed
--rw-r--r--   0        0        0      777 2023-05-19 17:03:50.493938 configzen-0.1.36/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.36/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-24 14:12:54.586341 configzen-0.1.36/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.36/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.37/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.37/configzen/__main__.py
+-rw-r--r--   0        0        0    58282 2023-05-26 07:03:59.357753 configzen-0.1.37/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.37/configzen/errors.py
+-rw-r--r--   0        0        0    20832 2023-05-26 06:54:52.263087 configzen-0.1.37/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.37/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.37/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.37/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-26 07:04:54.911332 configzen-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.37/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.37/PKG-INFO
```

### Comparing `configzen-0.1.36/configzen/__main__.py` & `configzen-0.1.37/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.36/configzen/config.py` & `configzen-0.1.37/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     format_syntax_error,
 )
 from configzen.processor import EXPORT, DirectiveContext, Processor
 from configzen.typedefs import (
     AsyncConfigIO,
     ConfigIO,
     ConfigModelT,
+    NormalizedResourceT,
     RawResourceT,
     SupportsRoute,
     T,
 )
 
 try:
     import aiofiles
@@ -427,15 +428,15 @@
         The URL schemes that are allowed to be used.
 
     Raises
     ------
     ValueError
     """
 
-    _resource: RawResourceT
+    _resource: NormalizedResourceT
     processor_class: type[Processor[ConfigModelT]]
     ac_parser: str | None
     create_if_missing: bool
     allowed_url_schemes: set[str]
     use_pydantic_json: bool = True
     global_load_options: dict[str, Any] = {}
     global_dump_options: dict[str, Any] = {
@@ -506,14 +507,24 @@
             `anyconfig.loads()` and `anyconfig.dumps()`.
         """
         if processor_class is None:
             processor_class = Processor[ConfigModelT]
 
         self.processor_class = processor_class
         self.ac_parser = ac_parser
+
+        if (
+            isinstance(resource, (str, os.PathLike))
+            and not (
+                isinstance(resource, str)
+                and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
+            )
+        ):
+            resource = pathlib.Path(resource)
+
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
         self.default_kwargs = kwargs.pop(
             "default_kwargs", self.predefined_default_kwargs.copy()
         )
         self.allowed_url_schemes = kwargs.pop(
@@ -522,28 +533,28 @@
 
         self.load_options = self.global_load_options.copy()
         self.dump_options = self.global_dump_options.copy()
 
         _delegate_ac_options(self.load_options, self.dump_options, kwargs)
 
     @property
-    def resource(self) -> RawResourceT:
+    def resource(self) -> NormalizedResourceT:
         """
         The resource of the configuration.
 
         This can be a file path, a URL, or a file-like object.
 
         Returns
         -------
         The resource of the configuration.
         """
         return self._resource
 
     @resource.setter
-    def resource(self, value: RawResourceT) -> None:
+    def resource(self, value: NormalizedResourceT) -> None:
         """
         The resource of the configuration.
 
         This can be a file path, a URL, or a file-like object.
 
         .. note::
             If the resource is a file path, the processor will be guessed
@@ -554,16 +565,16 @@
         The resource of the configuration.
         """
         self._resource = value
         self.ac_parser = self.ac_parser or self._guess_ac_parser()
 
     def _guess_ac_parser(self) -> str | None:
         ac_parser = None
-        if isinstance(self.resource, str):
-            ac_parser = pathlib.Path(self.resource).suffix[1:].casefold()
+        if isinstance(self.resource, pathlib.Path):
+            ac_parser = self.resource.suffix[1:].casefold()
             if not ac_parser:
                 msg = f"Could not guess the engine to use for {self.resource!r}."
                 raise UnspecifiedParserError(msg)
         return ac_parser
 
     def load_into(
         self,
@@ -694,18 +705,15 @@
             ac_parser = self.ac_parser
         kwargs = self.dump_options | kwargs
         return anyconfig.dumps(pre_serialize(data), ac_parser=ac_parser, **kwargs)
 
     @property
     def is_url(self) -> bool:
         """Whether the resource is a URL."""
-        return (
-            isinstance(self.resource, str)
-            and urllib.parse.urlparse(self.resource).scheme in _URL_SCHEMES
-        )
+        return isinstance(self.resource, str)
 
     def open_resource(self, **kwds: Any) -> ConfigIO:
         """
         Open the configuration file.
 
         Parameters
         ----------
@@ -727,27 +735,27 @@
                     f"URL scheme {url.scheme!r} is not allowed, "
                     f"must be one of {self.allowed_url_schemes!r}"
                 )
                 raise ValueError(msg)
             kwds = filter_options(self.URLOPEN_KWARGS, kwds)
             request = urllib.request.Request(url.geturl())
             return cast(ConfigIO, urllib.request.urlopen(request, **kwds))  # noqa: S310
-        if isinstance(self.resource, (str, int, os.PathLike, pathlib.Path)):
+        if isinstance(self.resource, (int, pathlib.Path)):
             kwds = filter_options(self.OPEN_KWARGS, kwds)
             if isinstance(self.resource, int):
                 return cast(
                     ConfigIO,
                     # We intentionally do not use the context manager here
                     # because we do not want to close the file.
                     # Moreover, we want to allow the file to be opened
                     # from a file descriptor, not supported by Path().
                     open(self.resource, **kwds),  # noqa: PTH123, SIM115
                 )
             return cast(ConfigIO, pathlib.Path(self.resource).open(**kwds))
-        return self.resource
+        return cast(ConfigIO, self.resource)
 
     def processor_open_resource(self, **kwargs: Any) -> ConfigIO:
         """
         Called by the processor to open a configuration resource with reading intention.
 
         Parameters
         ----------
@@ -781,15 +789,15 @@
             raise NotImplementedError(msg)
         if not AIOFILES_AVAILABLE:
             msg = (
                 "aiofiles is not available, cannot open file "
                 "asynchronously (install with `pip install aiofiles`)"
             )
             raise RuntimeError(msg)
-        if isinstance(self.resource, (str, int, os.PathLike, pathlib.Path)):
+        if isinstance(self.resource, (int, pathlib.Path)):
             kwds = filter_options(self.OPEN_KWARGS, kwds)
             return aiofiles.open(self.resource, **kwds)
         raise RuntimeError("cannot open resource asynchronously")
 
     def _get_default_kwargs(
         self,
         method: Literal["read", "write"],
@@ -1669,15 +1677,15 @@
         create_if_missing: bool | None = None,
     ) -> ConfigLoader[ConfigModelT]:
         if resource is None:
             resource = getattr(cls.__config__, "resource", None)
         if resource is None:
             raise ValueError("No resource specified")
         loader: ConfigLoader[ConfigModelT]
-        if isinstance(resource, (str, bytes)):
+        if isinstance(resource, str):
             loader = ConfigLoader(resource)
         elif isinstance(resource, ConfigLoader):
             loader = resource
         else:
             raise TypeError(f"Invalid resource type: {type(resource).__name__}")
         if create_if_missing is not None:
             loader.create_if_missing = create_if_missing
@@ -1750,17 +1758,15 @@
             context
             # pydantic.BaseModel.__instancecheck__() and __subclasscheck__()...
             and ConfigModel in type(value).mro()
             # We do not check if value was already defined here
             # because it may mess up models that rely on an extension relation.
             # Removed: ``and not hasattr(value, CONTEXT)``
             # Instead, we check if the optional current context points to here.
-            and (
-                value_context and context.route.enter(name) != value_context.route
-            )
+            and (value_context and context.route.enter(name) != value_context.route)
         ):
             context.enter(name).bind_to(value)
         return value
 
     def __deepcopy__(
         self: ConfigModelT, memodict: dict[Any, Any] | None = None
     ) -> ConfigModelT:
```

### Comparing `configzen-0.1.36/configzen/errors.py` & `configzen-0.1.37/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.36/configzen/processor.py` & `configzen-0.1.37/configzen/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
+import pathlib
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import (
+    ConfigPreprocessingError,
     InternalConfigError,
     format_syntax_error,
-    ConfigPreprocessingError,
 )
 from configzen.typedefs import ConfigModelT
 
 if TYPE_CHECKING:
     from configzen.config import AnyContext, ConfigLoader
 
 __all__ = (
@@ -102,15 +103,15 @@
                 return True
         return False
 
 
 class Tokens(str, enum.Enum):
     LPAREN: str = "("
     RPAREN: str = ")"
-    COMMA: str = ",;"
+    COMMAS: str = ",;"
     STRING: str = "\"'"
     ESCAPE: str = "\\"
 
 
 class ArgumentSyntaxError(ValueError):
     """
     Raised when there is a syntax error in an argument.
@@ -127,15 +128,15 @@
     arguments: list[str] = []
     argument = ""
     emit = arguments.append
     explicit_strings_ctx = True
 
     tok_escape = tokens.ESCAPE
     tok_string = tokens.STRING
-    tok_comma = tokens.COMMA
+    tok_commas = tokens.COMMAS
 
     for char_no, char in enumerate(raw_argument_string, start=1):
         if escape_ctx:
             escape_ctx = False
             argument += char
         elif char in tok_escape:
             escape_ctx = True
@@ -149,30 +150,30 @@
                 string_ctx = char
             elif string_ctx == char:
                 # we exit a string
                 string_ctx = None
             else:
                 # we are in a string
                 argument += char
-        elif char in tok_comma:
+        elif char in tok_commas:
             if string_ctx:
                 if not explicit_strings_ctx:
                     string_ctx = None
                     explicit_strings_ctx = True
                     emit(argument)
                     argument = ""
             else:
-                if prev_char in {*tok_comma, None}:
+                if prev_char in {*tok_commas, None}:
                     msg = "Empty argument"
                     raise InternalConfigError(msg, extra=char_no)
                 emit(argument)
                 argument = ""
                 explicit_strings_ctx = False
         elif not string_ctx and not char.isspace():
-            if prev_char in {*tok_comma, None}:
+            if prev_char in {*tok_commas, None}:
                 string_ctx = char
                 argument += char
                 explicit_strings_ctx = False
             if explicit_strings_ctx:
                 msg = "Unexpected character after explicit string"
                 raise InternalConfigError(msg, extra=char_no)
         else:
@@ -183,19 +184,22 @@
 
 def _parse_argument_string(
     raw_argument_string: str,
     tokens: type[Tokens] = Tokens,
 ) -> list[str]:
     """Half for jokes, half for serious use"""
 
-    tok_comma = tokens.COMMA
+    tok_commas = tokens.COMMAS
 
-    if any(raw_argument_string.endswith(tok) for tok in tok_comma):
+    if any(raw_argument_string.endswith(tok) for tok in tok_commas):
         raw_argument_string = raw_argument_string[:-1]
-    raw_argument_string += tok_comma[0]
+    raw_argument_string += tok_commas[0]
+
+    if raw_argument_string in tok_commas:
+        return []
 
     with format_syntax_error(raw_argument_string):
         return _parse_argument_string_impl(raw_argument_string, tokens)
 
 
 def parse_directive_call(
     prefix: str,
@@ -581,14 +585,22 @@
         )
 
         if loader.resource == self.loader.resource:
             raise ConfigPreprocessingError(
                 f"{loader.resource} tried to {ctx.directive!r} on itself"
             )
 
+        if (
+            isinstance(loader.resource, pathlib.Path)
+            and not loader.resource.is_absolute()
+        ):
+            orig_resource = self.loader.resource
+            if isinstance(orig_resource, pathlib.Path) and orig_resource.is_absolute():
+                loader.resource = loader.resource.relative_to(orig_resource.parent)
+
         with loader.processor_open_resource() as reader:
             substituted = loader.load_into_dict(reader.read(), preprocess=preprocess)
 
         if substitution_route:
             substituted = at(substituted, substitution_route, loader=loader)
             if not is_dict_like(substituted):
                 raise ConfigPreprocessingError(
@@ -602,15 +614,15 @@
         if preserve:
             ctx.container |= {
                 CONTEXT: context,
                 EXPORT: ExportMetadata(
                     route=str(substitution_route),
                     context=context,
                     preprocess=preprocess,
-                    key_order=list(ctx.container)
+                    key_order=list(ctx.container),
                 ),
             }
 
     @classmethod
     def _export(
         cls,
         state: dict[str, Any],
@@ -620,15 +632,15 @@
         Exports model state preserving substition directive calls in the model state.
 
         Parameters
         ----------
         metadata
         state
         """
-        from configzen.config import at, pre_serialize, CONTEXT
+        from configzen.config import CONTEXT, at, pre_serialize
 
         overrides = {}
 
         route = metadata["route"]
         context = metadata["context"]
         key_order = metadata["key_order"]
         loader = context.loader
@@ -654,16 +666,15 @@
                 if EXPORT in value:
                     value.pop(CONTEXT, None)
                     cls.export(value, metadata=value.pop(EXPORT))
                 overrides_for_key = {
                     sub_key: comp
                     for sub_key, comp in counterpart_value.items()
                     if (
-                        (orig := value.get(sub_key, missing)) is missing
-                        or orig != comp
+                        (orig := value.get(sub_key, missing)) is missing or orig != comp
                     )
                 }
                 if overrides_for_key:
                     export_key = loader.processor_class.extension_prefix + key
                     overrides[export_key] = overrides_for_key
 
             elif is_list_like(value):
@@ -676,24 +687,22 @@
         for value in state.values():
             cls.export(value, metadata=None)
 
         # TODO: Optimize. We iterate over the same about 3-4 times.
 
         state |= overrides
         extras: dict[str, Any] = {
-            key: state.pop(key)
-            for key in set(state)
-            if key not in key_order
+            key: state.pop(key) for key in set(state) if key not in key_order
         }
 
         if substituted_values:
             substitution_directive = cls.directive(Directives.EXTEND)
-            resource = context.loader.resource
+            resource = str(context.loader.resource)
             if route:
-                resource = cls.route_separator.join((str(resource), route))
+                resource = cls.route_separator.join((resource, route))
             # Put the substitution directive at the beginning of the state in-place.
             state |= {substitution_directive: resource} | {
                 key: state.pop(key) for key in set(state)
             }
 
         # Preserve the order of keys in the original configuration.
         for key in filter(state.__contains__, key_order):
```

### Comparing `configzen-0.1.36/configzen/typedefs.py` & `configzen-0.1.37/configzen/typedefs.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 ConfigModelT = TypeVar("ConfigModelT", bound="ConfigModel")
 SupportsRoute: TypeAlias = Union[str, list[str], "Route"]
 
 ConfigIO: TypeAlias = contextlib.AbstractContextManager[TextIO]
 AsyncConfigIO: TypeAlias = "AiofilesContextManager[None, None, AsyncTextIOWrapper]"
 RawResourceT: TypeAlias = Union[ConfigIO, str, int, os.PathLike, pathlib.Path]
+NormalizedResourceT: TypeAlias = Union[ConfigIO, str, int, pathlib.Path]
```

### Comparing `configzen-0.1.36/LICENSE` & `configzen-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.36/pyproject.toml` & `configzen-0.1.37/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.36"
+version = "0.1.37"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.36/README.md` & `configzen-0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.36/PKG-INFO` & `configzen-0.1.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.36
+Version: 0.1.37
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

