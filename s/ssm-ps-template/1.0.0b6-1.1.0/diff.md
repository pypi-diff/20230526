# Comparing `tmp/ssm-ps-template-1.0.0b6.tar.gz` & `tmp/ssm-ps-template-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-ps-template-1.0.0b6.tar", last modified: Mon May 15 20:40:05 2023, max compression
+gzip compressed data, was "ssm-ps-template-1.1.0.tar", last modified: Fri May 26 20:32:47 2023, max compression
```

## Comparing `ssm-ps-template-1.0.0b6.tar` & `ssm-ps-template-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5527 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/README.md
--rw-r--r--   0 root         (0) root         (0)     1857 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/ssm_ps_template/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/config.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/discover.py
--rw-r--r--   0 root         (0) root         (0)     1558 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/render.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/ssm_ps_template/ssm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 20:40:05.000000 ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 20:40:05.817200 ssm-ps-template-1.0.0b6/tests/
--rw-r--r--   0 root         (0) root         (0)     2254 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_discover.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-05-15 20:39:56.000000 ssm-ps-template-1.0.0b6/tests/test_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.702463 ssm-ps-template-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     8651 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6028 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 20:32:47.702463 ssm-ps-template-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/ssm_ps_template/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3171 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/config.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/discover.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/render.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/ssm_ps_template/ssm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8651 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-26 20:32:47.000000 ssm-ps-template-1.1.0/ssm_ps_template.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 20:32:47.698462 ssm-ps-template-1.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      405 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_discover.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_render.py
+-rw-r--r--   0 root         (0) root         (0)     4657 2023-05-26 20:32:38.000000 ssm-ps-template-1.1.0/tests/test_ssm.py
```

### Comparing `ssm-ps-template-1.0.0b6/LICENSE.txt` & `ssm-ps-template-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b6/PKG-INFO` & `ssm-ps-template-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b6
+Version: 1.1.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -65,20 +65,21 @@
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive   | Description                                                                                                                      |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates` | An array of template directives as detailed in the next table.                                                                   |
-| `profile`   | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`    | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`   | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive      | Description                                                                                                                      |
+|----------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`    | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -162,11 +163,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
+  --replace-underscores
+                        Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
-Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
+the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b6/README.md` & `ssm-ps-template-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive   | Description                                                                                                                      |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates` | An array of template directives as detailed in the next table.                                                                   |
-| `profile`   | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`    | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`   | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive      | Description                                                                                                                      |
+|----------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`    | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -113,11 +114,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
+  --replace-underscores
+                        Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
-Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
+the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b6/pyproject.toml` & `ssm-ps-template-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ssm-ps-template"
-version = "1.0.0b6"
+version = "1.1.0"
 description = "CLI for rendering configuration templates with SSM Parameter Store as a data source"
 authors = [
     {name = "Gavin M. Roy", email="gavinmroy@gmail.com"}
 ]
 classifiers = [
     "Topic :: Software Development",
     "License :: OSI Approved :: BSD License",
```

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template/__main__.py` & `ssm-ps-template-1.1.0/ssm_ps_template/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,39 +14,56 @@
 
 
 def parse_cli_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         description='Templating for SSM Parameter Store')
     parser.add_argument('--aws-profile', action='store', help='AWS Profile')
     parser.add_argument('--aws-region', action='store', help='AWS Region')
+    parser.add_argument('--endpoint-url', action='store',
+                        help=('Specify an endpoint URL to use when contacting '
+                              'SSM Parameter Store.'),
+                        default=os.environ.get('ENDPOINT_URL'))
     parser.add_argument('--prefix', action='store',
                         help='Default SSM Key Prefix',
-                        default=os.environ.get('PARAMS_PREFIX'))
+                        default=os.environ.get('PARAMS_PREFIX', ''))
+    parser.add_argument('--replace-underscores', action='store_true',
+                        help=('Replace underscores in variable names to dashes'
+                              ' when looking for values in SSM'))
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('config', type=config.configuration_file, nargs=1)
     return parser.parse_args()
 
 
 def render_templates(args: argparse.Namespace) -> typing.NoReturn:
     parameter_store = ssm.ParameterStore(
         profile=args.aws_profile or args.config[0].profile,
-        region=args.aws_region or args.config[0].region)
+        region=args.aws_region or args.config[0].region,
+        endpoint_url=args.endpoint_url or args.config[0].endpoint_url)
 
     start_time = time.time()
     for template in args.config[0].templates:
+        if not args.prefix and not template.prefix:
+            LOGGER.error('The prefix for %s must not be empty.',
+                         template.source)
+            sys.exit(1)
+
+        prefix = args.prefix or template.prefix
+        if not prefix.endswith('/'):
+            prefix = f'{args.prefix}/'
+
         variable_discovery = discover.Variables(template.source)
         variables = sorted(variable_discovery.discover())
 
         try:
             values = parameter_store.fetch_variables(
-                variables, args.prefix or template.prefix)
+                variables, prefix, args.replace_underscores)
         except (exceptions.ClientError,
                 exceptions.UnauthorizedSSOTokenError) as err:
             LOGGER.error('Error fetching parameters: %s', err)
-            sys.exit(1)
+            sys.exit(2)
 
         renderer = render.Renderer(source=template.source, variables=variables)
         with template.destination.open('w') as handle:
             handle.write(renderer.render(values))
 
         LOGGER.info('Rendered %s in %0.2f seconds', template.destination,
                     time.time() - start_time)
```

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template/config.py` & `ssm-ps-template-1.1.0/ssm_ps_template/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     source: pathlib.Path
     destination: pathlib.Path
     prefix: typing.Optional[str]
 
 
 @dataclasses.dataclass
 class Configuration:
-    templates: list[Template]
+    endpoint_url: typing.Optional[str]
     profile: typing.Optional[str]
     region: typing.Optional[str]
+    replace_underscores: typing.Optional[bool]
+    templates: list[Template]
     verbose: bool
 
 
 def _load_configuration(value: dict) -> Configuration:
     templates = []
     try:
         for template in value['templates'] or []:
@@ -31,17 +33,19 @@
                 source=template['source'],
                 destination=template['destination'],
                 prefix=template.get('prefix')))
     except KeyError as error:
         raise argparse.ArgumentTypeError(
             f'Failed to load configuration due to invalid key: {error}')
     return Configuration(
-        templates=templates,
+        endpoint_url=value.get('endpoint_url'),
         profile=value.get('profile'),
         region=value.get('region'),
+        replace_underscores=value.get('replace_underscores', False),
+        templates=templates,
         verbose=value.get('verbose', False))
 
 
 def _entry_to_template(**kwargs) -> Template:
     source = pathlib.Path(kwargs['source'])
     if not source.exists():
         raise argparse.ArgumentTypeError(
```

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template/discover.py` & `ssm-ps-template-1.1.0/ssm_ps_template/discover.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template/render.py` & `ssm-ps-template-1.1.0/ssm_ps_template/render.py`

 * *Files identical despite different names*

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template/ssm.py` & `ssm-ps-template-1.1.0/ssm_ps_template/ssm.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,51 +7,61 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class ParameterStore:
 
     def __init__(self,
                  profile: typing.Optional[str] = None,
-                 region: typing.Optional[str] = None):
+                 region: typing.Optional[str] = None,
+                 endpoint_url: typing.Optional[str] = None):
         self._session = boto3.Session(profile_name=profile, region_name=region)
-        self._client = self._session.client('ssm')
+        self._client = self._session.client('ssm', endpoint_url=endpoint_url)
         self._ssm = boto3.client('ssm')
 
     def fetch_variables(self,
                         variables: list,
-                        prefix: str) -> typing.Dict[str, str]:
+                        prefix: str,
+                        replace_underscores: bool) -> typing.Dict[str, str]:
+
         # Build the variables
         names = [
             '/'.join([prefix.rstrip('/'), v])
             if prefix and not v.startswith('/') else v for v in variables
         ]
 
         paths = [name for name in names if name.endswith('/')]
         names = [name for name in names if not name.endswith('/')]
 
-        LOGGER.debug('Fetching %r', names)
+        if replace_underscores:
+            paths = [value.replace('_', '-') for value in paths]
+            names = [value.replace('_', '-') for value in names]
 
         values = {}
+
+        LOGGER.debug('Fetching %r', names)
         while names:
             response = self._client.get_parameters(
                 Names=names[:10], WithDecryption=True)
             for param in response['Parameters']:
                 values = self.add_parameter(param, prefix, variables, values)
             names = names[10:]
 
         path_values = flatdict.FlatDict(delimiter='/')
+        LOGGER.debug('Fetching %r', paths)
         for path in paths:
             paginator = self._client.get_paginator('get_parameters_by_path')
             for page in paginator.paginate(
                     Path=path, Recursive=True, WithDecryption=True):
                 for param in page['Parameters']:
                     LOGGER.debug('Param %r', param)
-                    path_values = self.add_parameter(param, prefix, variables,
-                                                     path_values)
+                    path_values = self.add_parameter(
+                        param, prefix, variables, path_values)
         for key, value in path_values.as_dict().items():
+            if replace_underscores:
+                key = key.replace('-', '_')
             values[f'{key}/'] = value
 
         LOGGER.debug('Returning %r', values)
         return values
 
     @staticmethod
     def add_parameter(param: dict,
@@ -59,14 +69,16 @@
                       variables: typing.List[str],
                       values: typing.Union[dict, flatdict.FlatDict]) \
             -> dict:
         """Process a parameter, stripping prefix if needed and coercing
         StringList to a list of strings.
 
         """
+        prefix = prefix.replace('-', '_')
+        param['Name'] = param['Name'].replace('-', '_')
         if param['Name'].startswith(prefix) and param['Name'] not in variables:
             param['Name'] = param['Name'][len(prefix):]
         if param['Type'] == 'StringList':
             values[param['Name']] = [
                 p for p in param['Value'].split(',') if p.strip()
             ]
             LOGGER.debug('%s = %r', param['Name'], values[param['Name']])
```

### Comparing `ssm-ps-template-1.0.0b6/ssm_ps_template.egg-info/PKG-INFO` & `ssm-ps-template-1.1.0/ssm_ps_template.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-ps-template
-Version: 1.0.0b6
+Version: 1.1.0
 Summary: CLI for rendering configuration templates with SSM Parameter Store as a data source
 Author-email: "Gavin M. Roy" <gavinmroy@gmail.com>
 License: Copyright (c) 2023 Gavin M. Roy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -65,20 +65,21 @@
 
 ## Configuration
 
 The configuration file provides the ability to specify multiple templates, override AWS configuration, and change logging levels:
 
 ### Top-Level Configuration Directives
 
-| Directive   | Description                                                                                                                      |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------|
-| `templates` | An array of template directives as detailed in the next table.                                                                   |
-| `profile`   | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
-| `region`    | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
-| `verbose`   | Turn debug logging on. Possible values are `true` and `false`                                                                    |
+| Directive      | Description                                                                                                                      |
+|----------------|----------------------------------------------------------------------------------------------------------------------------------|
+| `templates`    | An array of template directives as detailed in the next table.                                                                   |
+| `endpoint_url` | Specify an endpoint URL to use to override the default URL used to contact SSM Parameter Store                                   |
+| `profile`      | Specify the AWS profile to use. If unspecified will default to the `AWS_DEFAULT_PROFILE` environment variable or is unspecified  |
+| `region`       | Specify the AWS region to use. If unspecified it will default to the `AWS_DEFAULT_REGION` environment variable or is unspecified |
+| `verbose`      | Turn debug logging on. Possible values are `true` and `false`                                                                    |
 
 ### Template Configuration Directives
 
 The `templates` directive in the configuration is an array of objects, defined by a `source` and `destination`.
 
 | Directive     | Description                                                                          |
 |---------------|--------------------------------------------------------------------------------------|
@@ -162,11 +163,16 @@
 
 optional arguments:
   -h, --help            show this help message and exit
   --aws-profile AWS_PROFILE
                         AWS Profile
   --aws-region AWS_REGION
                         AWS Region
+  --endpoint-url ENDPOINT_URL
+                        Specify an endpoint URL to use when contacting SSM Parameter Store.
   --prefix PREFIX       Default SSM Key Prefix
+  --replace-underscores
+                        Replace underscores in variable names to dashes when looking for values in SSM
   --verbose
 ```
-Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable.
+Note that the default SSM prefix can also be set with the `PARAMS_PREFIX` environment variable and
+the endpoint URL setting cn be set with the `ENDPOINT_URL` environment variable.
```

### Comparing `ssm-ps-template-1.0.0b6/tests/test_config.py` & `ssm-ps-template-1.1.0/tests/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,18 @@
                     source=pathlib.Path('tests/templates/case1a.tmpl'),
                     destination=pathlib.Path('build/case1a.out'),
                     prefix='/foo/bar/baz'),
                 config.Template(
                     source=pathlib.Path('tests/templates/case1b.tmpl'),
                     destination=pathlib.Path('build/case1b.out'),
                     prefix=None)],
+            endpoint_url=None,
             profile=None,
             region=None,
+            replace_underscores=False,
             verbose=False)
 
     def test_load_json_file(self):
         self.assertEqual(config.configuration_file('tests/config/case1.json'),
                          self.expectation)
 
     def test_load_toml_file(self):
```

### Comparing `ssm-ps-template-1.0.0b6/tests/test_render.py` & `ssm-ps-template-1.1.0/tests/test_render.py`

 * *Files identical despite different names*

