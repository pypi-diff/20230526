# Comparing `tmp/propan-0.1.2.1.tar.gz` & `tmp/propan-0.1.2.2.tar.gz`

## Comparing `propan-0.1.2.1.tar` & `propan-0.1.2.2.tar`

### file list

```diff
@@ -1,127 +1,131 @@
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.1/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 propan-0.1.2.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/kafka/1_direct.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.1/examples/redis/pattern.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__about__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/__main__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/log/logging.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/kafka.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.1/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.1/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.1/LICENSE
--rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 propan-0.1.2.1/README.md
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 propan-0.1.2.1/pyproject.toml
--rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 propan-0.1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.2.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.2/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/redis/pattern.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__about__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__main__.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/logging.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/nats.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/redis.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.2/LICENSE
+-rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 propan-0.1.2.2/README.md
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 propan-0.1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 propan-0.1.2.2/PKG-INFO
```

### Comparing `propan-0.1.2.1/CONTRIBUTING.md` & `propan-0.1.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/SECURITY.md` & `propan-0.1.2.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/.github/workflows/documentation.yml` & `propan-0.1.2.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/.github/workflows/publish_coverage.yml` & `propan-0.1.2.2/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/.github/workflows/publish_pypi.yml` & `propan-0.1.2.2/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/.github/workflows/tests.yml` & `propan-0.1.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/3_lifespan_events.py` & `propan-0.1.2.2/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.2/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/5_publishing.py` & `propan-0.1.2.2/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/6_arguments_casting.py` & `propan-0.1.2.2/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/7_handler_errors_processing.py` & `propan-0.1.2.2/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.2/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.2/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.2/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.2/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.2/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/dependencies/7_annotated.py` & `propan-0.1.2.2/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.2/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/rabbit/direct.py` & `propan-0.1.2.2/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/rabbit/fanout.py` & `propan-0.1.2.2/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/rabbit/header.py` & `propan-0.1.2.2/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/rabbit/topic.py` & `propan-0.1.2.2/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/redis/direct.py` & `propan-0.1.2.2/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/examples/redis/pattern.py` & `propan-0.1.2.2/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/__init__.py` & `propan-0.1.2.2/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/annotations.py` & `propan-0.1.2.2/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/types.py` & `propan-0.1.2.2/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/push_back_watcher.py` & `propan-0.1.2.2/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.2/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.2/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/model/broker_usecase.py` & `propan-0.1.2.2/propan/brokers/model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/model/schemas.py` & `propan-0.1.2.2/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/model/utils.py` & `propan-0.1.2.2/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.2/propan/brokers/nats/nats_broker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import asyncio
 from functools import wraps
+from secrets import token_hex
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
 import nats
 from nats.aio.client import Client
 from nats.aio.msg import Msg
 
 from propan.brokers.model import BrokerUsecase
@@ -41,31 +43,18 @@
 
     def handle(
         self,
         subject: str,
         queue: str = "",
         **original_kwargs,
     ) -> Callable[[DecoratedCallable], None]:
-        i = len(subject)
-        if i > self.__max_subject_len:
-            self.__max_subject_len = i
-
-        i = len(queue)
-        if i > self.__max_queue_len:
-            self.__max_queue_len = i
+        self.__max_subject_len = max((self.__max_subject_len, len(subject)))
+        self.__max_queue_len = max((self.__max_queue_len, len(queue)))
 
         def wrapper(func: DecoratedCallable) -> None:
-            for handler in self.handlers:
-                if handler.subject == subject and handler.queue == queue:
-                    raise ValueError(
-                        f"`{func.__name__}` uses already "
-                        f"using `{subject}` subject with "
-                        f"`{queue}` queue"
-                    )
-
             func = self._wrap_handler(
                 func, queue=queue, subject=subject, **original_kwargs
             )
             handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
             return func
@@ -84,31 +73,66 @@
             sub = await self._connection.subscribe(handler.subject, cb=func)
             handler.subscription = sub
 
     async def publish(
         self,
         message: SendableMessage,
         subject: str,
-        **publish_args: Any,
+        *,
+        headers: Optional[Dict[str, str]] = None,
+        reply_to: str = "",
+        callback: bool = False,
+        callback_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
     ) -> None:
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
         msg, content_type = self._encode_message(message)
 
-        return await self._connection.publish(
-            subject,
-            msg,
+        client = self._connection
+
+        if callback is True and not reply_to:
+            token = client._nuid.next()
+            token.extend(token_hex(2).encode())
+            reply_to = token.decode()
+
+        if reply_to:
+            future: asyncio.Future[Msg] = asyncio.Future()
+            sub = await client.subscribe(reply_to, future=future, max_msgs=1)
+            await sub.unsubscribe(limit=1)
+
+        await self._connection.publish(
+            subject=subject,
+            payload=msg,
+            reply=reply_to,
             headers={
-                **publish_args.pop("headers", {}),
-                "content-type": content_type,
+                **(headers or {}),
+                "content-type": content_type or "",
             },
-            **publish_args,
         )
 
+        if reply_to:
+            try:
+                msg = await asyncio.wait_for(future, callback_timeout)
+                if msg.headers:  # pragma: no branch
+                    if (
+                        msg.headers.get(nats.js.api.Header.STATUS)
+                        == nats.aio.client.NO_RESPONDERS_STATUS
+                    ):
+                        raise nats.errors.NoRespondersError
+            except asyncio.TimeoutError as e:
+                await sub.unsubscribe()
+                future.cancel()
+                if raise_timeout is True:
+                    raise e
+                return None
+            else:
+                return await self._decode_message(await self._parse_message(msg))
+
     async def close(self) -> None:
         for h in self.handlers:
             if h.subscription is not None:
                 await h.subscription.unsubscribe()
                 h.subscription = None
 
         if self._connection is not None:
@@ -136,21 +160,27 @@
             + (f"%(queue)-{self.__max_queue_len}s | " if self.__max_queue_len else "")
             + "%(message_id)-10s "
             "- %(message)s"
         )
 
     async def _parse_message(self, message: Msg) -> PropanMessage:
         return PropanMessage(
-            body=message.dat,
+            body=message.data,
             content_type=message.header.get("content-type", ""),
             headers=message.header,
+            reply_to=message.reply,
             raw_message=message,
         )
 
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher] = None
     ) -> Callable[[PropanMessage], T]:
         @wraps(func)
         async def wrapper(message: PropanMessage) -> T:
-            return await func(message)
+            r = await func(message)
+
+            if message.reply_to:
+                await self.publish(r, message.reply_to)
+
+            return r
 
         return wrapper
```

### Comparing `propan-0.1.2.1/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.2/propan/brokers/nats/nats_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,20 @@
         pending_size: int = DEFAULT_PENDING_SIZE,
         flush_timeout: Optional[float] = None,
     ) -> Client: ...
     async def publish(  # type: ignore[override]
         self,
         message: SendableMessage,
         subject: str,
-        reply: str = "",
+        *,
         headers: Optional[Dict[str, str]] = None,
+        reply_to: str = "",
+        callback: bool = False,
+        callback_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
     ) -> None: ...
     def handle(  # type: ignore[override]
         self,
         subject: str,
         queue: str = "",
         *,
         retry: Union[bool, int] = False,
```

### Comparing `propan-0.1.2.1/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.2/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/nats/schemas.py` & `propan-0.1.2.2/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.2/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.2/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.2/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/brokers/redis/schemas.py` & `propan-0.1.2.2/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/app.py` & `propan-0.1.2.2/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/main.py` & `propan-0.1.2.2/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/core.py` & `propan-0.1.2.2/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.2/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/supervisors/basereload.py` & `propan-0.1.2.2/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.2/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/supervisors/utils.py` & `propan-0.1.2.2/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.2/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/utils/imports.py` & `propan-0.1.2.2/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/utils/logs.py` & `propan-0.1.2.2/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/cli/utils/parser.py` & `propan-0.1.2.2/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/fastapi/__init__.py` & `propan-0.1.2.2/propan/fastapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,10 +11,15 @@
     RedisRouter = None  # type: ignore
 
 try:
     from propan.fastapi.kafka import KafkaRouter
 except Exception:
     KafkaRouter = None  # type: ignore
 
-assert any((RabbitRouter, RedisRouter, KafkaRouter)), INSTALL_MESSAGE
+try:
+    from propan.fastapi.nats import NatsRouter
+except Exception:
+    NatsRouter = None  # type: ignore
+
+assert any((RabbitRouter, RedisRouter, KafkaRouter, NatsRouter)), INSTALL_MESSAGE
 
-__all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter")
+__all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter")
```

### Comparing `propan-0.1.2.1/propan/fastapi/core/route.py` & `propan-0.1.2.2/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/fastapi/core/router.py` & `propan-0.1.2.2/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.2/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.2/propan/fastapi/rabbit/router.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -59,21 +59,19 @@
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         endpoint: AnyCallable,
-        name: Optional[str] = None,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         *,
         exchange: Union[str, RabbitExchange, None] = None,
         retry: Union[bool, int] = False,
-        name: Optional[str] = None,
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.1/propan/fastapi/redis/router.pyi` & `propan-0.1.2.2/propan/fastapi/redis/router.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -59,27 +59,24 @@
             generate_unique_id
         ),
         # Broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
-        consumers: Optional[int] = None,
     ) -> None:
         pass
     def add_api_mq_route(  # type: ignore[override]
         self,
         channel: str,
         *,
         endpoint: AnyCallable,
-        name: Optional[str] = None,
         pattern: bool = False,
     ) -> None:
         pass
     def event(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
-        name: Optional[str] = None,
     ) -> None:
         pass
```

### Comparing `propan-0.1.2.1/propan/log/formatter.py` & `propan-0.1.2.2/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/log/logging.py` & `propan-0.1.2.2/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/test/__init__.py` & `propan-0.1.2.2/propan/test/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,22 @@
     TestRedisBroker = None  # type: ignore
 
 try:
     from propan.test.kafka import TestKafkaBroker
 except Exception:
     TestKafkaBroker = None  # type: ignore
 
-assert any((TestRabbitBroker, TestRedisBroker, TestKafkaBroker)), INSTALL_MESSAGE
+try:
+    from propan.test.nats import TestNatsBroker
+except Exception:
+    TestNatsBroker = None  # type: ignore
+
+assert any(
+    (TestRabbitBroker, TestRedisBroker, TestKafkaBroker, TestNatsBroker)
+), INSTALL_MESSAGE
 
 __all__ = (
     "TestRabbitBroker",
     "TestRedisBroker",
     "TestKafkaBroker",
+    "TestNatsBroker",
 )
```

### Comparing `propan-0.1.2.1/propan/test/kafka.py` & `propan-0.1.2.2/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/test/rabbit.py` & `propan-0.1.2.2/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/test/redis.py` & `propan-0.1.2.2/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/test/utils.py` & `propan-0.1.2.2/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/utils/functions.py` & `propan-0.1.2.2/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/utils/context/main.py` & `propan-0.1.2.2/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/propan/utils/context/types.py` & `propan-0.1.2.2/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/LICENSE` & `propan-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.1/README.md` & `propan-0.1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 
 ### Supported MQ brokers
 
 |                   | async                                                   | sync                 |
 |-------------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
+| **Nats**          | :heavy_check_mark: **beta** :heavy_check_mark:          | :mag: planning :mag: |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
-| **Nats**          | :warning: **beta** :warning:                            | :mag: planning :mag: |
+| **SQS**           | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
-| **SQS**           | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
 If you are interested in this project, please give me feedback by star or/and watch repository.
 
 If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
```

#### html2text {}

```diff
@@ -22,97 +22,98 @@
 the project environment * application code *hot reload* * robust application
 templates * **Testability**: **Propan** allows you to test your app without
 external dependencies: you do not have to set up a Message Broker, you can use
 a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
 |:-------------------------------------------------------:|:-------------------
 -:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
 planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Kafka** | :warning: **beta** :warning: | :mag:
-planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag: planning :
-mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
-:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
-| | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
-**Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag:
-planning :mag: | :mag: planning :mag: | ### Community If you are interested in
-this project, please give me feedback by star or/and watch repository. If you
-have any questions or ideas about features to implement, welcome to
-[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
-Declarative? With declarative tools you can define **what you need to get**.
-With traditional imperative tools you must write **what you need to do**. Take
-a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
-etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
-import aio_pika async def main(): connection = await aio_pika.connect_robust
-( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
-connection: channel = await connection.channel() queue = await
-channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
-async for message in queue_iter: async with message.process(): print
-(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
-really easy learning curve. But it's still imperative. You need to *connect*,
-declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
-*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
-way, but it can be much easier. ```python from propan import PropanApp,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
-print(body) ``` This is the **Propan** declarative way to write the same code.
-That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
-nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
-kafka]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
-NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
-6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
-(body): '''Handle all default exchange messages with `test` routing key'''
-print(body) ``` And just run it: ```shell propan run serve:app ``` --- ## Type
-casting Propan uses `pydantic` to cast incoming function arguments to types
-according to their annotation. ```python from pydantic import BaseModel from
-propan import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage
-(BaseModel): key: int @broker.handle("test2") async def second_handler(body:
-SimpleMessage): assert isinstance(body.key, int) ``` --- ## Dependencies
-**Propan** a has dependencies management policy close to `pytest fixtures`. You
-can specify in functions arguments which dependencies you would to use.
-Framework passes them from the global Context object. Already existed context
-fields are: *app*, *broker*, *context* (itself), *logger* and *message*. If you
-call not existing field, raises *pydantic.ValidationError* value. But you can
-specify your own dependencies, call dependencies functions (like `Fastapi
-Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
-dependencies). ```python import aio_pika from propan import PropanApp,
-RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(rabbit_broker) async def dependency
-(body: dict) -> bool: return True @rabbit_broker.handle("test") async def
-base_handler(body: dict, dep: bool = Depends(dependency), broker: RabbitBroker
-= Context()): assert dep is True assert broker is rabbit_broker ``` --- ## CLI
-power **Propan** has its own CLI tool that provided the following features: *
-project generation * multiprocessing workers * project hot reloading * custom
-command line arguments passing ### Context passing For example: pass your
-current *.env* project setting to context ```bash propan run serve:app --
-env=.env.dev ``` ```python from propan import PropanApp, RabbitBroker from
-propan.annotations import ContextRepo from pydantic import BaseSettings broker
-= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
-class Settings(BaseSettings): ... @app.on_startup async def setup(env: str,
-context: ContextRepo): settings = Settings(_env_file=env) context.set_global
-("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
-generate a production-ready application template: ```bash propan create async
-rabbit [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
-*installation.* Run the created project: ```bash # Run rabbimq first docker
-compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
-[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations ### Any Framework
-You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
-them according to your application lifespan. ```python from propan import
-NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
-NatsBroker("nats://localhost:4222") @broker.handle("test") async def
-base_handler(body): print(body) @app.after_server_start async def start_broker
-(app, loop): await broker.start() @app.after_server_stop async def stop_broker
-(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
-be used as part of **FastAPI**. Just import a **PropanRouter** you need and
-declare the message handler using the `@event` decorator. This decorator is
-similar to the decorator `@handle` for the corresponding brokers. ```python
-from fastapi import Depends, FastAPI from pydantic import BaseModel from
-propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
-//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
-return True @router.event("test") async def hello(m: Incoming, d = Depends
-(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
-(router) ``` ## Examples To see more framework usages go to [**examples/**]
-(https://github.com/Lancetnik/Propan/tree/main/examples)
+| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **beta** :
+heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
+warning: | :mag: planning :mag: | | **SQS** | :hammer_and_wrench: **in
+progress** :hammer_and_wrench: | :mag: planning :mag: | | **NatsJS** | :
+hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
+| **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams**
+| :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :
+mag: | :mag: planning :mag: | ### Community If you are interested in this
+project, please give me feedback by star or/and watch repository. If you have
+any questions or ideas about features to implement, welcome to [discussions]
+(https://github.com/Lancetnik/Propan/discussions). --- ## Declarative? With
+declarative tools you can define **what you need to get**. With traditional
+imperative tools you must write **what you need to do**. Take a look at classic
+imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
+**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
+async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
+guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
+await connection.channel() queue = await channel.declare_queue(queue_name)
+async with queue.iterator() as queue_iter: async for message in queue_iter:
+async with message.process(): print(message.body) asyncio.run(main()) ```
+**aio-pika** is a great tool with a really easy learning curve. But it's still
+imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
+yourself. Also, you need to manage *connection*, *message*, *queue* context to
+avoid any troubles. It is not a bad way, but it can be much easier. ```python
+from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
+async def base_handler(body): print(body) ``` This is the **Propan**
+declarative way to write the same code. That is so much easier, isn't it? --
+- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
+rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
+redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
+application with the following code at `serve.py`: ```python from propan import
+PropanApp from propan import RabbitBroker # from propan import RedisBroker #
+from propan import NatsBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
+= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+("test") async def base_handler(body): '''Handle all default exchange messages
+with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
+def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
+-- ## Dependencies **Propan** a has dependencies management policy close to
+`pytest fixtures`. You can specify in functions arguments which dependencies
+you would to use. Framework passes them from the global Context object. Already
+existed context fields are: *app*, *broker*, *context* (itself), *logger* and
+*message*. If you call not existing field, raises *pydantic.ValidationError*
+value. But you can specify your own dependencies, call dependencies functions
+(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
+main/examples/dependencies). ```python import aio_pika from propan import
+PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
+dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
+def base_handler(body: dict, dep: bool = Depends(dependency), broker:
+RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
+``` --- ## CLI power **Propan** has its own CLI tool that provided the
+following features: * project generation * multiprocessing workers * project
+hot reloading * custom command line arguments passing ### Context passing For
+example: pass your current *.env* project setting to context ```bash propan run
+serve:app --env=.env.dev ``` ```python from propan import PropanApp,
+RabbitBroker from propan.annotations import ContextRepo from pydantic import
+BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
+setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
+context.set_global("settings", settings) ``` ### Project template Also,
+**Propan CLI** is able to generate a production-ready application template:
+```bash propan create async rabbit [projectname] ``` *Notice: project template
+require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
+Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
+d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
+Now you can enjoy a new development experience! --- ## HTTP Frameworks
+integrations ### Any Framework You can use **Propan** `MQBrokers` without
+`PropanApp`. Just *start* and *stop* them according to your application
+lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
+Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
+@broker.handle("test") async def base_handler(body): print(body)
+@app.after_server_start async def start_broker(app, loop): await broker.start()
+@app.after_server_stop async def stop_broker(app, loop): await broker.close()
+``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
+Just import a **PropanRouter** you need and declare the message handler using
+the `@event` decorator. This decorator is similar to the decorator `@handle`
+for the corresponding brokers. ```python from fastapi import Depends, FastAPI
+from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
+FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
+Incoming(BaseModel): m: dict def call(): return True @router.event("test")
+async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
+"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
+framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
+tree/main/examples)
```

### Comparing `propan-0.1.2.1/pyproject.toml` & `propan-0.1.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 [project]
 name = "propan"
 description = "Propan framework: the simplest way to work with a messaging queues"
 readme = "README.md"
 authors = [
     { name = "Pastukhov Nikita", email = "diementros@yandex.ru" },
 ]
-license = "MIT"
 
-homepage = "https://github.com/Lancetnik/Propan"
 keywords = ["rabbitmq", "framework", "message brokers"]
 
 requires-python = ">=3.7"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -41,15 +39,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends>=1.1.3",
+    "fast-depends>=1.1.4",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
 
@@ -84,15 +82,14 @@
     "propan[async-nats]",
     "propan[async-redis]",
     "propan[async-kafka]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
-    "pytest-xdist[psutil]",
 
     "fastapi",
 
     "asyncmock; python_version < '3.8'",
 ]
 
 doc = [
```

### Comparing `propan-0.1.2.1/PKG-INFO` & `propan-0.1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
-License-Expression: MIT
 License-File: LICENSE
 Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
@@ -32,15 +31,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: fast-depends>=1.1.3
+Requires-Dist: fast-depends>=1.1.4
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-kafka
 Requires-Dist: aiokafka>=0.8; extra == 'async-kafka'
 Provides-Extra: async-nats
 Requires-Dist: nats-py>=2; extra == 'async-nats'
@@ -68,15 +67,14 @@
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
-Requires-Dist: pytest-xdist[psutil]; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://lancetnik.github.io/Propan/" target="_blank">
         <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
     </a>
@@ -138,21 +136,21 @@
 
 ### Supported MQ brokers
 
 |                   | async                                                   | sync                 |
 |-------------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
+| **Nats**          | :heavy_check_mark: **beta** :heavy_check_mark:          | :mag: planning :mag: |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
-| **Nats**          | :warning: **beta** :warning:                            | :mag: planning :mag: |
+| **SQS**           | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
-| **SQS**           | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
 If you are interested in this project, please give me feedback by star or/and watch repository.
 
 If you have any questions or ideas about features to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/discussions).
```

#### html2text {}

```diff
@@ -1,55 +1,53 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.1 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.2 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
-yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
-framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
-Production/Stable Classifier: Environment :: Web Environment Classifier:
-Framework :: AsyncIO Classifier: Framework :: Pydantic Classifier: Framework ::
-Pydantic :: 1 Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Information Technology Classifier: Intended Audience :: System
-Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: Implementation :: CPython Classifier: Topic :: Internet
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Application Frameworks Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7
-Requires-Dist: fast-depends>=1.1.3 Requires-Dist: typer Requires-Dist:
-uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform !=
-'cygwin' and platform_python_implementation != 'PyPy') Requires-Dist:
-watchfiles Provides-Extra: async-kafka Requires-Dist: aiokafka>=0.8; extra ==
-'async-kafka' Provides-Extra: async-nats Requires-Dist: nats-py>=2; extra ==
-'async-nats' Provides-Extra: async-rabbit Requires-Dist: aio-pika>=9; extra ==
-'async-rabbit' Provides-Extra: async-redis Requires-Dist: redis>=4.2.0rc1;
-extra == 'async-redis' Provides-Extra: dev Requires-Dist: black==23.3.0; extra
-== 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-Dist: mypy==1.1.1;
-extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev' Requires-Dist: propan
-[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra == 'dev' Requires-
-Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis; extra == 'dev'
-Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
-Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
-Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist:
-mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all]; extra == 'doc'
-Provides-Extra: test Requires-Dist: asyncmock; python_version < '3.8' and extra
-== 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist:
-fastapi; extra == 'test' Requires-Dist: propan[async-kafka]; extra == 'test'
-Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan[async-
-rabbit]; extra == 'test' Requires-Dist: propan[async-redis]; extra == 'test'
-Requires-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest-
-xdist[psutil]; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
-Description-Content-Type: text/markdown
+yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Web Environment Classifier: Framework :: AsyncIO Classifier: Framework ::
+Pydantic Classifier: Framework :: Pydantic :: 1 Classifier: Intended Audience
+:: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Application Frameworks Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Classifier: Typing ::
+Typed Requires-Python: >=3.7 Requires-Dist: fast-depends>=1.1.4 Requires-Dist:
+typer Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32'
+and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
+Requires-Dist: watchfiles Provides-Extra: async-kafka Requires-Dist:
+aiokafka>=0.8; extra == 'async-kafka' Provides-Extra: async-nats Requires-Dist:
+nats-py>=2; extra == 'async-nats' Provides-Extra: async-rabbit Requires-Dist:
+aio-pika>=9; extra == 'async-rabbit' Provides-Extra: async-redis Requires-Dist:
+redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: dev Requires-Dist:
+black==23.3.0; extra == 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-
+Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev'
+Requires-Dist: propan[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra
+== 'dev' Requires-Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis;
+extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1;
+extra == 'doc' Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7;
+extra == 'doc' Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
+Requires-Dist: mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all];
+extra == 'doc' Provides-Extra: test Requires-Dist: asyncmock; python_version <
+'3.8' and extra == 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test'
+Requires-Dist: fastapi; extra == 'test' Requires-Dist: propan[async-kafka];
+extra == 'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-
+Dist: propan[async-rabbit]; extra == 'test' Requires-Dist: propan[async-redis];
+extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-
+Dist: pytest>=7; extra == 'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by *fastapi*, simplify Message Brokers around code
 writing and provides a helpful development toolkit, which existed only in HTTP-
 frameworks world until now. It's designed to create reactive microservices
@@ -70,97 +68,98 @@
 the project environment * application code *hot reload* * robust application
 templates * **Testability**: **Propan** allows you to test your app without
 external dependencies: you do not have to set up a Message Broker, you can use
 a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
 |:-------------------------------------------------------:|:-------------------
 -:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
 planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Kafka** | :warning: **beta** :warning: | :mag:
-planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag: planning :
-mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
-:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
-| | **Redis Streams** | :mag: planning :mag: | :mag: planning :mag: | |
-**Pulsar** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag:
-planning :mag: | :mag: planning :mag: | ### Community If you are interested in
-this project, please give me feedback by star or/and watch repository. If you
-have any questions or ideas about features to implement, welcome to
-[discussions](https://github.com/Lancetnik/Propan/discussions). --- ##
-Declarative? With declarative tools you can define **what you need to get**.
-With traditional imperative tools you must write **what you need to do**. Take
-a look at classic imperative tools, such as aio-pika, pika, redis-py, nats-py,
-etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
-import aio_pika async def main(): connection = await aio_pika.connect_robust
-( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
-connection: channel = await connection.channel() queue = await
-channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
-async for message in queue_iter: async with message.process(): print
-(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
-really easy learning curve. But it's still imperative. You need to *connect*,
-declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
-*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
-way, but it can be much easier. ```python from propan import PropanApp,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
-print(body) ``` This is the **Propan** declarative way to write the same code.
-That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
-```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
-nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
-kafka]" ``` ### Basic usage Create an application with the following code at
-`serve.py`: ```python from propan import PropanApp from propan import
-RabbitBroker # from propan import RedisBroker # from propan import NatsBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker =
-NatsBroker("nats://localhost:4222") # broker = RedisBroker("redis://localhost:
-6379") app = PropanApp(broker) @broker.handle("test") async def base_handler
-(body): '''Handle all default exchange messages with `test` routing key'''
-print(body) ``` And just run it: ```shell propan run serve:app ``` --- ## Type
-casting Propan uses `pydantic` to cast incoming function arguments to types
-according to their annotation. ```python from pydantic import BaseModel from
-propan import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://
-guest:guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage
-(BaseModel): key: int @broker.handle("test2") async def second_handler(body:
-SimpleMessage): assert isinstance(body.key, int) ``` --- ## Dependencies
-**Propan** a has dependencies management policy close to `pytest fixtures`. You
-can specify in functions arguments which dependencies you would to use.
-Framework passes them from the global Context object. Already existed context
-fields are: *app*, *broker*, *context* (itself), *logger* and *message*. If you
-call not existing field, raises *pydantic.ValidationError* value. But you can
-specify your own dependencies, call dependencies functions (like `Fastapi
-Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
-dependencies). ```python import aio_pika from propan import PropanApp,
-RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(rabbit_broker) async def dependency
-(body: dict) -> bool: return True @rabbit_broker.handle("test") async def
-base_handler(body: dict, dep: bool = Depends(dependency), broker: RabbitBroker
-= Context()): assert dep is True assert broker is rabbit_broker ``` --- ## CLI
-power **Propan** has its own CLI tool that provided the following features: *
-project generation * multiprocessing workers * project hot reloading * custom
-command line arguments passing ### Context passing For example: pass your
-current *.env* project setting to context ```bash propan run serve:app --
-env=.env.dev ``` ```python from propan import PropanApp, RabbitBroker from
-propan.annotations import ContextRepo from pydantic import BaseSettings broker
-= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
-class Settings(BaseSettings): ... @app.on_startup async def setup(env: str,
-context: ContextRepo): settings = Settings(_env_file=env) context.set_global
-("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
-generate a production-ready application template: ```bash propan create async
-rabbit [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
-*installation.* Run the created project: ```bash # Run rabbimq first docker
-compose --file [projectname]/docker-compose.yaml up -d # Run project propan run
-[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations ### Any Framework
-You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
-them according to your application lifespan. ```python from propan import
-NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
-NatsBroker("nats://localhost:4222") @broker.handle("test") async def
-base_handler(body): print(body) @app.after_server_start async def start_broker
-(app, loop): await broker.start() @app.after_server_stop async def stop_broker
-(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
-be used as part of **FastAPI**. Just import a **PropanRouter** you need and
-declare the message handler using the `@event` decorator. This decorator is
-similar to the decorator `@handle` for the corresponding brokers. ```python
-from fastapi import Depends, FastAPI from pydantic import BaseModel from
-propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
-//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
-return True @router.event("test") async def hello(m: Incoming, d = Depends
-(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
-(router) ``` ## Examples To see more framework usages go to [**examples/**]
-(https://github.com/Lancetnik/Propan/tree/main/examples)
+| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **beta** :
+heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
+warning: | :mag: planning :mag: | | **SQS** | :hammer_and_wrench: **in
+progress** :hammer_and_wrench: | :mag: planning :mag: | | **NatsJS** | :
+hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
+| **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams**
+| :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :
+mag: | :mag: planning :mag: | ### Community If you are interested in this
+project, please give me feedback by star or/and watch repository. If you have
+any questions or ideas about features to implement, welcome to [discussions]
+(https://github.com/Lancetnik/Propan/discussions). --- ## Declarative? With
+declarative tools you can define **what you need to get**. With traditional
+imperative tools you must write **what you need to do**. Take a look at classic
+imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
+**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
+async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
+guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
+await connection.channel() queue = await channel.declare_queue(queue_name)
+async with queue.iterator() as queue_iter: async for message in queue_iter:
+async with message.process(): print(message.body) asyncio.run(main()) ```
+**aio-pika** is a great tool with a really easy learning curve. But it's still
+imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
+yourself. Also, you need to manage *connection*, *message*, *queue* context to
+avoid any troubles. It is not a bad way, but it can be much easier. ```python
+from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
+async def base_handler(body): print(body) ``` This is the **Propan**
+declarative way to write the same code. That is so much easier, isn't it? --
+- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
+rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
+redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
+application with the following code at `serve.py`: ```python from propan import
+PropanApp from propan import RabbitBroker # from propan import RedisBroker #
+from propan import NatsBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
+= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+("test") async def base_handler(body): '''Handle all default exchange messages
+with `test` routing key''' print(body) ``` And just run it: ```shell propan run
+serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
+broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
+(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
+def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
+-- ## Dependencies **Propan** a has dependencies management policy close to
+`pytest fixtures`. You can specify in functions arguments which dependencies
+you would to use. Framework passes them from the global Context object. Already
+existed context fields are: *app*, *broker*, *context* (itself), *logger* and
+*message*. If you call not existing field, raises *pydantic.ValidationError*
+value. But you can specify your own dependencies, call dependencies functions
+(like `Fastapi Depends`) and [more](https://github.com/Lancetnik/Propan/tree/
+main/examples/dependencies). ```python import aio_pika from propan import
+PropanApp, RabbitBroker, Context, Depends rabbit_broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(rabbit_broker) async def
+dependency(body: dict) -> bool: return True @rabbit_broker.handle("test") async
+def base_handler(body: dict, dep: bool = Depends(dependency), broker:
+RabbitBroker = Context()): assert dep is True assert broker is rabbit_broker
+``` --- ## CLI power **Propan** has its own CLI tool that provided the
+following features: * project generation * multiprocessing workers * project
+hot reloading * custom command line arguments passing ### Context passing For
+example: pass your current *.env* project setting to context ```bash propan run
+serve:app --env=.env.dev ``` ```python from propan import PropanApp,
+RabbitBroker from propan.annotations import ContextRepo from pydantic import
+BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async def
+setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
+context.set_global("settings", settings) ``` ### Project template Also,
+**Propan CLI** is able to generate a production-ready application template:
+```bash propan create async rabbit [projectname] ``` *Notice: project template
+require* `pydantic[dotenv]` *installation.* Run the created project: ```bash #
+Run rabbimq first docker compose --file [projectname]/docker-compose.yaml up -
+d # Run project propan run [projectname].app.serve:app --env=.env --reload ```
+Now you can enjoy a new development experience! --- ## HTTP Frameworks
+integrations ### Any Framework You can use **Propan** `MQBrokers` without
+`PropanApp`. Just *start* and *stop* them according to your application
+lifespan. ```python from propan import NatsBroker from sanic import Sanic app =
+Sanic("MyHelloWorldApp") broker = NatsBroker("nats://localhost:4222")
+@broker.handle("test") async def base_handler(body): print(body)
+@app.after_server_start async def start_broker(app, loop): await broker.start()
+@app.after_server_stop async def stop_broker(app, loop): await broker.close()
+``` ### FastAPI Plugin Also, **Propan** can be used as part of **FastAPI**.
+Just import a **PropanRouter** you need and declare the message handler using
+the `@event` decorator. This decorator is similar to the decorator `@handle`
+for the corresponding brokers. ```python from fastapi import Depends, FastAPI
+from pydantic import BaseModel from propan.fastapi import RabbitRouter app =
+FastAPI() router = RabbitRouter("amqp://guest:guest@localhost:5672") class
+Incoming(BaseModel): m: dict def call(): return True @router.event("test")
+async def hello(m: Incoming, d = Depends(call)) -> dict: return { "response":
+"Hello, Propan!" } app.include_router(router) ``` ## Examples To see more
+framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/
+tree/main/examples)
```

