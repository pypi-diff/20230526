# Comparing `tmp/argclass-0.9.1.tar.gz` & `tmp/argclass-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argclass-0.9.1.tar", max compression
+gzip compressed data, was "argclass-0.9.2.tar", max compression
```

## Comparing `argclass-0.9.1.tar` & `argclass-0.9.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9572 2022-12-08 22:05:05.705435 argclass-0.9.1/README.rst
--rw-r--r--   0        0        0    24574 2022-12-08 22:05:05.706103 argclass-0.9.1/argclass.py
--rw-r--r--   0        0        0     2009 2022-12-08 22:06:41.639639 argclass-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10498 1970-01-01 00:00:00.000000 argclass-0.9.1/setup.py
--rw-r--r--   0        0        0    11257 1970-01-01 00:00:00.000000 argclass-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     9576 2022-12-08 22:07:38.382093 argclass-0.9.2/README.rst
+-rw-r--r--   0        0        0    24574 2022-12-08 22:05:05.706103 argclass-0.9.2/argclass.py
+-rw-r--r--   0        0        0     2009 2022-12-08 22:07:58.971598 argclass-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10502 1970-01-01 00:00:00.000000 argclass-0.9.2/setup.py
+-rw-r--r--   0        0        0    11261 1970-01-01 00:00:00.000000 argclass-0.9.2/PKG-INFO
```

### Comparing `argclass-0.9.1/README.rst` & `argclass-0.9.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 argclass
 ========
 
 .. image:: https://coveralls.io/repos/github/mosquito/argclass/badge.svg?branch=master
    :target: https://coveralls.io/github/mosquito/argclass?branch=master
 
-.. image:: https://github.com/mosquito/argclass/workflows/tox/badge.svg
-   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atox
+.. image:: https://github.com/mosquito/argclass/workflows/tests/badge.svg
+   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atests
    :alt: Actions
 
 .. image:: https://img.shields.io/pypi/v/argclass.svg
    :target: https://pypi.python.org/pypi/argclass/
    :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/pyversions/argclass.svg
```

### Comparing `argclass-0.9.1/argclass.py` & `argclass-0.9.2/argclass.py`

 * *Files identical despite different names*

### Comparing `argclass-0.9.1/pyproject.toml` & `argclass-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argclass"
-version = "0.9.1"
+version = "0.9.2"
 description = "A wrapper around the standard argparse module that allows you to describe argument parsers declaratively"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache 2"
 homepage = "https://github.com/mosquito/argclass"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `argclass-0.9.1/setup.py` & `argclass-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['argclass']
 setup_kwargs = {
     'name': 'argclass',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'A wrapper around the standard argparse module that allows you to describe argument parsers declaratively',
-    'long_description': 'argclass\n========\n\n.. image:: https://coveralls.io/repos/github/mosquito/argclass/badge.svg?branch=master\n   :target: https://coveralls.io/github/mosquito/argclass?branch=master\n\n.. image:: https://github.com/mosquito/argclass/workflows/tox/badge.svg\n   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atox\n   :alt: Actions\n\n.. image:: https://img.shields.io/pypi/v/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n   :alt: Latest Version\n\n.. image:: https://img.shields.io/pypi/pyversions/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n\n.. image:: https://img.shields.io/pypi/l/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n\nA wrapper around the standard ``argparse`` module that allows you to describe\nargument parsers declaratively.\n\nBy default, the ``argparse`` module suggests creating parsers imperative,\nwhich is not convenient from the point of view of type checking and\naccess to attributes, of course, IDE autocompletion and type hints not\napplicable in this case.\n\nThis module allows you to declare command-line parsers with classes.\n\nSimple example:\n\n.. code-block:: python\n    :name: test_simple_example\n\n    import logging\n\n    import argclass\n\n\n    class CopyParser(argclass.Parser):\n        recursive: bool\n        preserve_attributes: bool\n\n\n    parser = CopyParser()\n    parser.parse_args(["--recursive", "--preserve-attributes"])\n    assert parser.recursive\n    assert parser.preserve_attributes\n\nAs you can see this example shown a basic module usage, when you want specify\nargument default and other options you have to use ``argclass.Argument``.\n\nFollowing example use ``argclass.Argument`` and argument groups:\n\n.. code-block:: python\n    :name: test_example\n\n    from typing import FrozenSet\n    import logging\n\n    import argclass\n\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class Parser(argclass.Parser):\n        log_level: int = argclass.LogLevel\n        http = AddressPortGroup(title="HTTP options", defaults=dict(port=8080))\n        rpc = AddressPortGroup(title="RPC options", defaults=dict(port=9090))\n        user_id: FrozenSet[int] = argclass.Argument(\n            nargs="*", type=int, converter=frozenset\n        )\n\n\n    parser = Parser(\n        config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],\n        auto_env_var_prefix="EXAMPLE_"\n    )\n    parser.parse_args([])\n\n    # Remove all used environment variables from os.environ\n    parser.sanitize_env()\n\n    logging.basicConfig(level=parser.log_level)\n    logging.info(\'Listening http://%s:%d\', parser.http.address, parser.http.port)\n    logging.info(f\'Listening rpc://%s:%d\', parser.rpc.address, parser.rpc.port)\n\n\n    assert parser.http.address == \'127.0.0.1\'\n    assert parser.rpc.address == \'127.0.0.1\'\n\n    assert parser.http.port == 8080\n    assert parser.rpc.port == 9090\n\n\nRun this script:\n\n.. code-block::\n\n    $ python example.py\n    INFO:root:Listening http://127.0.0.1:8080\n    INFO:root:Listening rpc://127.0.0.1:9090\n\nExample of ``--help`` output:\n\n.. code-block::\n\n    $ python example.py --help\n    usage: example.py [-h] [--log-level {debug,info,warning,error,critical}]\n                     [--http-address HTTP_ADDRESS] [--http-port HTTP_PORT]\n                     [--rpc-address RPC_ADDRESS] [--rpc-port RPC_PORT]\n\n    optional arguments:\n      -h, --help            show this help message and exit\n      --log-level {debug,info,warning,error,critical}\n                            (default: info) [ENV: EXAMPLE_LOG_LEVEL]\n\n    HTTP options:\n      --http-address HTTP_ADDRESS\n                            (default: 127.0.0.1) [ENV: EXAMPLE_HTTP_ADDRESS]\n      --http-port HTTP_PORT\n                            (default: 8080) [ENV: EXAMPLE_HTTP_PORT]\n\n    RPC options:\n      --rpc-address RPC_ADDRESS\n                            (default: 127.0.0.1) [ENV: EXAMPLE_RPC_ADDRESS]\n      --rpc-port RPC_PORT   (default: 9090) [ENV: EXAMPLE_RPC_PORT]\n\n    Default values will based on following configuration files [\'example.ini\',\n    \'~/.example.ini\', \'/etc/example.ini\']. Now 1 files has been applied\n    [\'example.ini\']. The configuration files is INI-formatted files where\n    configuration groups is INI sections.\n    See more https://pypi.org/project/argclass/#configs\n\nSecrets\n+++++++\n\nArguments reflecting some sensitive data, tokens or encryption keys, when\npassed through environment variables or a configuration file, can be printed\nin the output of `--help`. To hide defaults, add the `secret=True` parameter,\nor use the special default constructor `argclass.Secret` instead of\n`argclass.Argument`.\n\n.. code-block:: python\n\n    import argclass\n\n\n    class HttpAuthentication(argclass.Group):\n        username: str = argclass.Argument()\n        password: str = argclass.Secret()\n\n\n    class HttpBearerAuthentication(argclass.Group):\n        token: str = argclass.Argument(secret=True)\n\n\n    class Parser(argclass.Parser):\n        http_basic = HttpAuthentication()\n        http_bearer = HttpBearerAuthentication()\n\n\n    parser = Parser()\n    parser.print_help()\n\nConfigs\n+++++++\n\nThe parser objects might be get default values from environment variables or\none of passed configuration files.\n\n.. code-block:: python\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class Parser(argclass.Parser):\n        spam: str\n        quantity: int\n        log_level: int = argclass.LogLevel\n        http = AddressPortGroup(title="HTTP options")\n        rpc = AddressPortGroup(title="RPC options")\n        user_ids = argclass.Argument(\n            type=int, converter=frozenset, nargs=argclass.Nargs.ONE_OR_MORE\n        )\n\n\n    # Trying to parse all passed configuration files\n    # and break after first success.\n    parser = Parser(\n        config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],\n    )\n    parser.parse_args()\n\n\nIn this case each passed and existent configuration file will be opened.\n\nThe root level arguments might described in the ``[DEFAULT]`` section.\n\nOther arguments might be described in group specific sections.\n\nSo the full example of config file for above example is:\n\n.. code-block:: ini\n\n    [DEFAULT]\n    log_level=info\n    spam=egg\n    quantity=100\n    user_ids=[1, 2, 3]\n\n    [http]\n    address=127.0.0.1\n    port=8080\n\n    [rpc]\n    address=127.0.0.1\n    port=9090\n\n\nSubparsers\n++++++++++\n\nComplex example with subparsers:\n\n.. code-block:: python\n\n    import logging\n    from functools import singledispatch\n    from pathlib import Path\n    from typing import Optional, Any\n\n    import argclass\n\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class CommitCommand(argclass.Parser):\n        comment: str = argclass.Argument()\n\n\n    class PushCommand(argclass.Parser):\n        comment: str = argclass.Argument()\n\n\n    class Parser(argclass.Parser):\n        log_level: int = argclass.LogLevel\n        endpoint = AddressPortGroup(\n            title="Endpoint options",\n            defaults=dict(port=8080)\n        )\n        commit: Optional[CommitCommand] = CommitCommand()\n        push: Optional[PushCommand] = PushCommand()\n\n\n    @singledispatch\n    def handle_subparser(subparser: Any) -> None:\n        raise NotImplementedError(\n            f"Unexpected subparser type {subparser.__class__!r}"\n        )\n\n\n    @handle_subparser.register(type(None))\n    def handle_none(_: None) -> None:\n        Parser().print_help()\n        exit(2)\n\n\n    @handle_subparser.register(CommitCommand)\n    def handle_commit(subparser: CommitCommand) -> None:\n        print("Commit command called", subparser)\n\n\n    @handle_subparser.register(PushCommand)\n    def handle_push(subparser: PushCommand) -> None:\n        print("Push command called", subparser)\n\n\n    parser = Parser(\n        config_files=["example.ini", "~/.example.ini", "/etc/example.ini"],\n        auto_env_var_prefix="EXAMPLE_"\n    )\n    parser.parse_args()\n    handle_subparser(parser.current_subparser)\n\nValue conversion\n++++++++++++++++\n\nIf the argument has a generic or composite type, then you must explicitly\ndescribe it using ``argclass.Argument``, while specifying the converter\nfunction with ``type`` or ``converter`` argument to transform the value\nafter parsing the arguments.\n\nThe exception to this rule is `Optional` with a single type. In this case,\nan argument without a default value will not be required,\nand its value can be None.\n\n.. code-block:: python\n    :name: test_converter\n\n    import argclass\n    from typing import Optional, Union\n\n    def converter(value: str) -> Optional[Union[int, str, bool]]:\n        if value.lower() == "none":\n            return None\n        if value.isdigit():\n            return int(value)\n        if value.lower() in ("yes", "true", "enabled", "enable", "on"):\n            return True\n        return False\n\n\n    class Parser(argclass.Parser):\n        gizmo: Optional[Union[int, str, bool]] = argclass.Argument(\n            converter=converter\n        )\n        optional: Optional[int]\n\n\n    parser = Parser()\n\n    parser.parse_args(["--gizmo=65535"])\n    assert parser.gizmo == 65535\n\n    parser.parse_args(["--gizmo=None"])\n    assert parser.gizmo is None\n\n    parser.parse_args(["--gizmo=on"])\n    assert parser.gizmo is True\n    assert parser.optional is None\n\n    parser.parse_args(["--gizmo=off", "--optional=10"])\n    assert parser.gizmo is False\n    assert parser.optional == 10\n',
+    'long_description': 'argclass\n========\n\n.. image:: https://coveralls.io/repos/github/mosquito/argclass/badge.svg?branch=master\n   :target: https://coveralls.io/github/mosquito/argclass?branch=master\n\n.. image:: https://github.com/mosquito/argclass/workflows/tests/badge.svg\n   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atests\n   :alt: Actions\n\n.. image:: https://img.shields.io/pypi/v/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n   :alt: Latest Version\n\n.. image:: https://img.shields.io/pypi/pyversions/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n\n.. image:: https://img.shields.io/pypi/l/argclass.svg\n   :target: https://pypi.python.org/pypi/argclass/\n\nA wrapper around the standard ``argparse`` module that allows you to describe\nargument parsers declaratively.\n\nBy default, the ``argparse`` module suggests creating parsers imperative,\nwhich is not convenient from the point of view of type checking and\naccess to attributes, of course, IDE autocompletion and type hints not\napplicable in this case.\n\nThis module allows you to declare command-line parsers with classes.\n\nSimple example:\n\n.. code-block:: python\n    :name: test_simple_example\n\n    import logging\n\n    import argclass\n\n\n    class CopyParser(argclass.Parser):\n        recursive: bool\n        preserve_attributes: bool\n\n\n    parser = CopyParser()\n    parser.parse_args(["--recursive", "--preserve-attributes"])\n    assert parser.recursive\n    assert parser.preserve_attributes\n\nAs you can see this example shown a basic module usage, when you want specify\nargument default and other options you have to use ``argclass.Argument``.\n\nFollowing example use ``argclass.Argument`` and argument groups:\n\n.. code-block:: python\n    :name: test_example\n\n    from typing import FrozenSet\n    import logging\n\n    import argclass\n\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class Parser(argclass.Parser):\n        log_level: int = argclass.LogLevel\n        http = AddressPortGroup(title="HTTP options", defaults=dict(port=8080))\n        rpc = AddressPortGroup(title="RPC options", defaults=dict(port=9090))\n        user_id: FrozenSet[int] = argclass.Argument(\n            nargs="*", type=int, converter=frozenset\n        )\n\n\n    parser = Parser(\n        config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],\n        auto_env_var_prefix="EXAMPLE_"\n    )\n    parser.parse_args([])\n\n    # Remove all used environment variables from os.environ\n    parser.sanitize_env()\n\n    logging.basicConfig(level=parser.log_level)\n    logging.info(\'Listening http://%s:%d\', parser.http.address, parser.http.port)\n    logging.info(f\'Listening rpc://%s:%d\', parser.rpc.address, parser.rpc.port)\n\n\n    assert parser.http.address == \'127.0.0.1\'\n    assert parser.rpc.address == \'127.0.0.1\'\n\n    assert parser.http.port == 8080\n    assert parser.rpc.port == 9090\n\n\nRun this script:\n\n.. code-block::\n\n    $ python example.py\n    INFO:root:Listening http://127.0.0.1:8080\n    INFO:root:Listening rpc://127.0.0.1:9090\n\nExample of ``--help`` output:\n\n.. code-block::\n\n    $ python example.py --help\n    usage: example.py [-h] [--log-level {debug,info,warning,error,critical}]\n                     [--http-address HTTP_ADDRESS] [--http-port HTTP_PORT]\n                     [--rpc-address RPC_ADDRESS] [--rpc-port RPC_PORT]\n\n    optional arguments:\n      -h, --help            show this help message and exit\n      --log-level {debug,info,warning,error,critical}\n                            (default: info) [ENV: EXAMPLE_LOG_LEVEL]\n\n    HTTP options:\n      --http-address HTTP_ADDRESS\n                            (default: 127.0.0.1) [ENV: EXAMPLE_HTTP_ADDRESS]\n      --http-port HTTP_PORT\n                            (default: 8080) [ENV: EXAMPLE_HTTP_PORT]\n\n    RPC options:\n      --rpc-address RPC_ADDRESS\n                            (default: 127.0.0.1) [ENV: EXAMPLE_RPC_ADDRESS]\n      --rpc-port RPC_PORT   (default: 9090) [ENV: EXAMPLE_RPC_PORT]\n\n    Default values will based on following configuration files [\'example.ini\',\n    \'~/.example.ini\', \'/etc/example.ini\']. Now 1 files has been applied\n    [\'example.ini\']. The configuration files is INI-formatted files where\n    configuration groups is INI sections.\n    See more https://pypi.org/project/argclass/#configs\n\nSecrets\n+++++++\n\nArguments reflecting some sensitive data, tokens or encryption keys, when\npassed through environment variables or a configuration file, can be printed\nin the output of `--help`. To hide defaults, add the `secret=True` parameter,\nor use the special default constructor `argclass.Secret` instead of\n`argclass.Argument`.\n\n.. code-block:: python\n\n    import argclass\n\n\n    class HttpAuthentication(argclass.Group):\n        username: str = argclass.Argument()\n        password: str = argclass.Secret()\n\n\n    class HttpBearerAuthentication(argclass.Group):\n        token: str = argclass.Argument(secret=True)\n\n\n    class Parser(argclass.Parser):\n        http_basic = HttpAuthentication()\n        http_bearer = HttpBearerAuthentication()\n\n\n    parser = Parser()\n    parser.print_help()\n\nConfigs\n+++++++\n\nThe parser objects might be get default values from environment variables or\none of passed configuration files.\n\n.. code-block:: python\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class Parser(argclass.Parser):\n        spam: str\n        quantity: int\n        log_level: int = argclass.LogLevel\n        http = AddressPortGroup(title="HTTP options")\n        rpc = AddressPortGroup(title="RPC options")\n        user_ids = argclass.Argument(\n            type=int, converter=frozenset, nargs=argclass.Nargs.ONE_OR_MORE\n        )\n\n\n    # Trying to parse all passed configuration files\n    # and break after first success.\n    parser = Parser(\n        config_files=[".example.ini", "~/.example.ini", "/etc/example.ini"],\n    )\n    parser.parse_args()\n\n\nIn this case each passed and existent configuration file will be opened.\n\nThe root level arguments might described in the ``[DEFAULT]`` section.\n\nOther arguments might be described in group specific sections.\n\nSo the full example of config file for above example is:\n\n.. code-block:: ini\n\n    [DEFAULT]\n    log_level=info\n    spam=egg\n    quantity=100\n    user_ids=[1, 2, 3]\n\n    [http]\n    address=127.0.0.1\n    port=8080\n\n    [rpc]\n    address=127.0.0.1\n    port=9090\n\n\nSubparsers\n++++++++++\n\nComplex example with subparsers:\n\n.. code-block:: python\n\n    import logging\n    from functools import singledispatch\n    from pathlib import Path\n    from typing import Optional, Any\n\n    import argclass\n\n\n    class AddressPortGroup(argclass.Group):\n        address: str = argclass.Argument(default="127.0.0.1")\n        port: int\n\n\n    class CommitCommand(argclass.Parser):\n        comment: str = argclass.Argument()\n\n\n    class PushCommand(argclass.Parser):\n        comment: str = argclass.Argument()\n\n\n    class Parser(argclass.Parser):\n        log_level: int = argclass.LogLevel\n        endpoint = AddressPortGroup(\n            title="Endpoint options",\n            defaults=dict(port=8080)\n        )\n        commit: Optional[CommitCommand] = CommitCommand()\n        push: Optional[PushCommand] = PushCommand()\n\n\n    @singledispatch\n    def handle_subparser(subparser: Any) -> None:\n        raise NotImplementedError(\n            f"Unexpected subparser type {subparser.__class__!r}"\n        )\n\n\n    @handle_subparser.register(type(None))\n    def handle_none(_: None) -> None:\n        Parser().print_help()\n        exit(2)\n\n\n    @handle_subparser.register(CommitCommand)\n    def handle_commit(subparser: CommitCommand) -> None:\n        print("Commit command called", subparser)\n\n\n    @handle_subparser.register(PushCommand)\n    def handle_push(subparser: PushCommand) -> None:\n        print("Push command called", subparser)\n\n\n    parser = Parser(\n        config_files=["example.ini", "~/.example.ini", "/etc/example.ini"],\n        auto_env_var_prefix="EXAMPLE_"\n    )\n    parser.parse_args()\n    handle_subparser(parser.current_subparser)\n\nValue conversion\n++++++++++++++++\n\nIf the argument has a generic or composite type, then you must explicitly\ndescribe it using ``argclass.Argument``, while specifying the converter\nfunction with ``type`` or ``converter`` argument to transform the value\nafter parsing the arguments.\n\nThe exception to this rule is `Optional` with a single type. In this case,\nan argument without a default value will not be required,\nand its value can be None.\n\n.. code-block:: python\n    :name: test_converter\n\n    import argclass\n    from typing import Optional, Union\n\n    def converter(value: str) -> Optional[Union[int, str, bool]]:\n        if value.lower() == "none":\n            return None\n        if value.isdigit():\n            return int(value)\n        if value.lower() in ("yes", "true", "enabled", "enable", "on"):\n            return True\n        return False\n\n\n    class Parser(argclass.Parser):\n        gizmo: Optional[Union[int, str, bool]] = argclass.Argument(\n            converter=converter\n        )\n        optional: Optional[int]\n\n\n    parser = Parser()\n\n    parser.parse_args(["--gizmo=65535"])\n    assert parser.gizmo == 65535\n\n    parser.parse_args(["--gizmo=None"])\n    assert parser.gizmo is None\n\n    parser.parse_args(["--gizmo=on"])\n    assert parser.gizmo is True\n    assert parser.optional is None\n\n    parser.parse_args(["--gizmo=off", "--optional=10"])\n    assert parser.gizmo is False\n    assert parser.optional == 10\n',
     'author': 'Dmitry Orlov',
     'author_email': 'me@mosquito.su',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mosquito/argclass',
     'py_modules': modules,
     'python_requires': '>=3.7,<4.0',
```

### Comparing `argclass-0.9.1/PKG-INFO` & `argclass-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argclass
-Version: 0.9.1
+Version: 0.9.2
 Summary: A wrapper around the standard argparse module that allows you to describe argument parsers declaratively
 Home-page: https://github.com/mosquito/argclass
 License: Apache 2
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -37,16 +37,16 @@
 
 argclass
 ========
 
 .. image:: https://coveralls.io/repos/github/mosquito/argclass/badge.svg?branch=master
    :target: https://coveralls.io/github/mosquito/argclass?branch=master
 
-.. image:: https://github.com/mosquito/argclass/workflows/tox/badge.svg
-   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atox
+.. image:: https://github.com/mosquito/argclass/workflows/tests/badge.svg
+   :target: https://github.com/mosquito/argclass/actions?query=workflow%3Atests
    :alt: Actions
 
 .. image:: https://img.shields.io/pypi/v/argclass.svg
    :target: https://pypi.python.org/pypi/argclass/
    :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/pyversions/argclass.svg
```

