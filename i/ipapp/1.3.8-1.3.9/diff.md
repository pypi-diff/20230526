# Comparing `tmp/ipapp-1.3.8.tar.gz` & `tmp/ipapp-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipapp-1.3.8.tar", max compression
+gzip compressed data, was "ipapp-1.3.9.tar", max compression
```

## Comparing `ipapp-1.3.8.tar` & `ipapp-1.3.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1085 2022-06-10 08:24:13.799391 ipapp-1.3.8/LICENSE
--rw-r--r--   0        0        0     1050 2022-06-10 08:24:13.799391 ipapp-1.3.8/README.md
--rw-r--r--   0        0        0      679 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/__init__.py
--rw-r--r--   0        0        0     6049 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/app.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/asgi/__init__.py
--rw-r--r--   0        0        0     8014 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/asgi/uvicorn.py
--rw-r--r--   0        0        0     3652 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/autoreload.py
--rw-r--r--   0        0        0     4407 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/cli.py
--rw-r--r--   0        0        0      690 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/component.py
--rw-r--r--   0        0        0     9744 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/config.py
--rw-r--r--   0        0        0     6930 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/ctx.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.799391 ipapp-1.3.8/ipapp/db/__init__.py
--rw-r--r--   0        0        0    22205 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/db/oracle.py
--rw-r--r--   0        0        0    39149 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/db/pg.py
--rw-r--r--   0        0        0      158 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/error.py
--rw-r--r--   0        0        0      268 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/http/__init__.py
--rw-r--r--   0        0        0     5581 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/http/_base.py
--rw-r--r--   0        0        0     5177 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/http/client.py
--rw-r--r--   0        0        0    14968 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/http/server.py
--rw-r--r--   0        0        0     3259 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/logger/__init__.py
--rw-r--r--   0        0        0      472 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/logger/adapters/__init__.py
--rw-r--r--   0        0        0      810 2022-06-10 08:24:13.803391 ipapp-1.3.8/ipapp/logger/adapters/_abc.py
--rw-r--r--   0        0        0     5180 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/adapters/prometheus.py
--rw-r--r--   0        0        0    18741 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/adapters/requests.py
--rw-r--r--   0        0        0     1351 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/adapters/sentry.py
--rw-r--r--   0        0        0     3065 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/adapters/zipkin.py
--rw-r--r--   0        0        0     3163 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/logger.py
--rw-r--r--   0        0        0    14493 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/logger/span.py
--rw-r--r--   0        0        0     6111 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/misc.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/mq/__init__.py
--rw-r--r--   0        0        0    32899 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/mq/pika.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/openapi/__init__.py
--rw-r--r--   0        0        0     8694 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/openapi/misc.py
--rw-r--r--   0        0        0    10428 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/openapi/models.py
--rw-r--r--   0        0        0     2879 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/openapi/templates.py
--rw-r--r--   0        0        0      210 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/__init__.py
--rw-r--r--   0        0        0       66 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/const.py
--rw-r--r--   0        0        0      124 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/error.py
--rw-r--r--   0        0        0      294 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/http/__init__.py
--rw-r--r--   0        0        0     2509 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/http/client.py
--rw-r--r--   0        0        0    15026 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/http/server.py
--rw-r--r--   0        0        0      173 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/__init__.py
--rw-r--r--   0        0        0      880 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/error.py
--rw-r--r--   0        0        0      424 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/http/__init__.py
--rw-r--r--   0        0        0     2260 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/http/client.py
--rw-r--r--   0        0        0     5719 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/http/server.py
--rw-r--r--   0        0        0    23314 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/main.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/mq/__init__.py
--rw-r--r--   0        0        0     8451 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/mq/pika.py
--rw-r--r--   0        0        0       51 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/openrpc/__init__.py
--rw-r--r--   0        0        0    11725 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/openrpc/discover.py
--rw-r--r--   0        0        0     5853 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/jsonrpc/openrpc/models.py
--rw-r--r--   0        0        0    17002 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/main.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/mq/__init__.py
--rw-r--r--   0        0        0    10032 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/mq/pika.py
--rw-r--r--   0        0        0      495 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/__init__.py
--rw-r--r--   0        0        0     2488 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/error.py
--rw-r--r--   0        0        0      424 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/http/__init__.py
--rw-r--r--   0        0        0     2143 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/http/client.py
--rw-r--r--   0        0        0    19283 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/http/server.py
--rw-r--r--   0        0        0    18441 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/main.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/openapi/__init__.py
--rw-r--r--   0        0        0     9426 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/rpc/restrpc/openapi/misc.py
--rw-r--r--   0        0        0      136 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/s3/__init__.py
--rw-r--r--   0        0        0    20855 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/s3/boto.py
--rw-r--r--   0        0        0       90 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/s3/exceptions.py
--rw-r--r--   0        0        0     5293 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/s3/models.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/sftp/__init__.py
--rw-r--r--   0        0        0    17841 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/sftp/client.py
--rw-r--r--   0        0        0       56 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/sphinx/__init__.py
--rw-r--r--   0        0        0     4115 2022-06-10 08:24:13.807391 ipapp-1.3.8/ipapp/sphinx/config.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/task/__init__.py
--rw-r--r--   0        0        0    39913 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/task/db.py
--rw-r--r--   0        0        0        0 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/__init__.py
--rw-r--r--   0        0        0       69 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/lock/__init__.py
--rw-r--r--   0        0        0     1223 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/lock/local.py
--rw-r--r--   0        0        0     3643 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/lock/main.py
--rw-r--r--   0        0        0     4350 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/lock/pg.py
--rw-r--r--   0        0        0     5804 2022-06-10 08:24:13.811391 ipapp-1.3.8/ipapp/utils/lock/redis.py
--rw-r--r--   0        0        0     3680 2022-06-10 08:25:07.650569 ipapp-1.3.8/pyproject.toml
--rw-r--r--   0        0        0     3585 2022-06-10 08:25:08.491834 ipapp-1.3.8/setup.py
--rw-r--r--   0        0        0     4326 2022-06-10 08:25:08.492384 ipapp-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-06 14:22:54.552915 ipapp-1.3.9/LICENSE
+-rw-r--r--   0        0        0     1050 2022-07-06 14:22:54.552915 ipapp-1.3.9/README.md
+-rw-r--r--   0        0        0      679 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/__init__.py
+-rw-r--r--   0        0        0     6049 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/app.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/asgi/__init__.py
+-rw-r--r--   0        0        0     8014 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/asgi/uvicorn.py
+-rw-r--r--   0        0        0     3652 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/autoreload.py
+-rw-r--r--   0        0        0     4407 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/cli.py
+-rw-r--r--   0        0        0      690 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/component.py
+-rw-r--r--   0        0        0     9744 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/config.py
+-rw-r--r--   0        0        0     6930 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/ctx.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/__init__.py
+-rw-r--r--   0        0        0    22205 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/oracle.py
+-rw-r--r--   0        0        0    39149 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/db/pg.py
+-rw-r--r--   0        0        0      158 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/error.py
+-rw-r--r--   0        0        0      268 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/__init__.py
+-rw-r--r--   0        0        0     5581 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/_base.py
+-rw-r--r--   0        0        0     5290 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/client.py
+-rw-r--r--   0        0        0    14968 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/http/server.py
+-rw-r--r--   0        0        0     3259 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/__init__.py
+-rw-r--r--   0        0        0      472 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/__init__.py
+-rw-r--r--   0        0        0      810 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/_abc.py
+-rw-r--r--   0        0        0     5180 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/prometheus.py
+-rw-r--r--   0        0        0    18741 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/requests.py
+-rw-r--r--   0        0        0     1351 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/sentry.py
+-rw-r--r--   0        0        0     3065 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/adapters/zipkin.py
+-rw-r--r--   0        0        0     3163 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/logger.py
+-rw-r--r--   0        0        0    14493 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/logger/span.py
+-rw-r--r--   0        0        0     6111 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/misc.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/mq/__init__.py
+-rw-r--r--   0        0        0    32899 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/mq/pika.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.552915 ipapp-1.3.9/ipapp/openapi/__init__.py
+-rw-r--r--   0        0        0     8694 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/misc.py
+-rw-r--r--   0        0        0    10428 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/models.py
+-rw-r--r--   0        0        0     2879 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/openapi/templates.py
+-rw-r--r--   0        0        0      210 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/__init__.py
+-rw-r--r--   0        0        0       66 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/const.py
+-rw-r--r--   0        0        0      124 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/error.py
+-rw-r--r--   0        0        0      294 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/__init__.py
+-rw-r--r--   0        0        0     2599 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/client.py
+-rw-r--r--   0        0        0    15026 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/http/server.py
+-rw-r--r--   0        0        0      173 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/__init__.py
+-rw-r--r--   0        0        0      880 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/error.py
+-rw-r--r--   0        0        0      424 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/__init__.py
+-rw-r--r--   0        0        0     2352 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/client.py
+-rw-r--r--   0        0        0     5719 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/http/server.py
+-rw-r--r--   0        0        0    23314 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/main.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/__init__.py
+-rw-r--r--   0        0        0     8451 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/pika.py
+-rw-r--r--   0        0        0       51 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/__init__.py
+-rw-r--r--   0        0        0    11725 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/discover.py
+-rw-r--r--   0        0        0     5853 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/models.py
+-rw-r--r--   0        0        0    17002 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/main.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/mq/__init__.py
+-rw-r--r--   0        0        0    10032 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/mq/pika.py
+-rw-r--r--   0        0        0      495 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/__init__.py
+-rw-r--r--   0        0        0     2488 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/error.py
+-rw-r--r--   0        0        0      424 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/__init__.py
+-rw-r--r--   0        0        0     2235 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/client.py
+-rw-r--r--   0        0        0    19283 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/http/server.py
+-rw-r--r--   0        0        0    18441 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/main.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/openapi/__init__.py
+-rw-r--r--   0        0        0     9426 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/rpc/restrpc/openapi/misc.py
+-rw-r--r--   0        0        0      136 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/__init__.py
+-rw-r--r--   0        0        0    20855 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/boto.py
+-rw-r--r--   0        0        0       90 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/exceptions.py
+-rw-r--r--   0        0        0     5293 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/s3/models.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sftp/__init__.py
+-rw-r--r--   0        0        0    17841 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sftp/client.py
+-rw-r--r--   0        0        0       56 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sphinx/__init__.py
+-rw-r--r--   0        0        0     4115 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/sphinx/config.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/task/__init__.py
+-rw-r--r--   0        0        0    39913 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/task/db.py
+-rw-r--r--   0        0        0        0 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/__init__.py
+-rw-r--r--   0        0        0       69 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/__init__.py
+-rw-r--r--   0        0        0     1223 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/local.py
+-rw-r--r--   0        0        0     3643 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/main.py
+-rw-r--r--   0        0        0     4350 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/pg.py
+-rw-r--r--   0        0        0     5804 2022-07-06 14:22:54.556915 ipapp-1.3.9/ipapp/utils/lock/redis.py
+-rw-r--r--   0        0        0     3680 2022-07-06 14:23:30.787729 ipapp-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3585 2022-07-06 14:23:31.479622 ipapp-1.3.9/setup.py
+-rw-r--r--   0        0        0     4326 2022-07-06 14:23:31.480138 ipapp-1.3.9/PKG-INFO
```

### Comparing `ipapp-1.3.8/LICENSE` & `ipapp-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/README.md` & `ipapp-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/__init__.py` & `ipapp-1.3.9/ipapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/app.py` & `ipapp-1.3.9/ipapp/app.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/asgi/uvicorn.py` & `ipapp-1.3.9/ipapp/asgi/uvicorn.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/autoreload.py` & `ipapp-1.3.9/ipapp/autoreload.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/cli.py` & `ipapp-1.3.9/ipapp/cli.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/component.py` & `ipapp-1.3.9/ipapp/component.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/config.py` & `ipapp-1.3.9/ipapp/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/ctx.py` & `ipapp-1.3.9/ipapp/ctx.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/db/oracle.py` & `ipapp-1.3.9/ipapp/db/oracle.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/db/pg.py` & `ipapp-1.3.9/ipapp/db/pg.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/http/_base.py` & `ipapp-1.3.9/ipapp/http/_base.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/http/client.py` & `ipapp-1.3.9/ipapp/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,25 @@
 
     cfg = ClientConfig()
 
     def __init__(
         self,
         cfg: Optional[ClientConfig] = None,
         json_encode: Callable[[Any], str] = default_json_encode,
+        session_kwargs: Optional[Dict[str, Any]] = None,
     ):
+        _session_kwargs = session_kwargs or {}
+        timeout = getattr(cfg, 'timeout', None)
+        if timeout:
+            _session_kwargs.update({'timeout': ClientTimeout(timeout)})
+
         if cfg is not None:
             self.cfg = cfg
         self._json_encode = json_encode
+        self._session = ClientSession(**_session_kwargs)
 
     async def prepare(self) -> None:
         pass
 
     async def start(self) -> None:
         pass
 
@@ -94,15 +101,14 @@
         method: str,
         url: StrOrURL,
         *,
         body: Optional[bytes] = None,
         headers: Dict[str, str] = None,
         timeout: Optional[ClientTimeout] = None,
         ssl: Optional[SSLContext] = None,
-        session_kwargs: Optional[Dict[str, Any]] = None,
         request_kwargs: Optional[Dict[str, Any]] = None,
         propagate_trace: bool = True,
     ) -> ClientResponse:
         span: 'ClientHttpSpan'
         with wrap2span(  # type: ignore
             kind=HttpSpan.KIND_CLIENT, cls=ClientHttpSpan, app=self.app
         ) as span:
@@ -124,38 +130,36 @@
             if headers is None:
                 headers = {}
             if propagate_trace:
                 headers.update(span.to_headers())
             if 'User-Agent' not in headers:
                 headers['User-Agent'] = USER_AGENT
 
-            async with ClientSession(
+            ts1 = time.time()
+            async with self._session.request(
+                method=method,
+                url=url,
+                data=body,
+                headers=headers,
+                ssl=ssl,
                 timeout=timeout,
-                **(session_kwargs or {}),
-            ) as session:
-                ts1 = time.time()
-                resp = await session.request(
-                    method=method,
-                    url=url,
-                    data=body,
-                    headers=headers,
-                    ssl=ssl,
-                    **(request_kwargs or {}),
-                )
+                **(request_kwargs or {}),
+            ) as resp:
                 ts2 = time.time()
                 if self.cfg.log_req_hdrs:
                     self._span_annotate_req_hdrs(
                         span, resp.request_info.headers, ts1
                     )
                 if self.cfg.log_req_body:
                     self._span_annotate_req_body(span, body, ts1)
                 if self.cfg.log_resp_hdrs:
                     self._span_annotate_resp_hdrs(span, resp.headers, ts2)
+
+                resp_body = await resp.read()
                 if self.cfg.log_resp_body:
-                    resp_body = await resp.read()
                     self._span_annotate_resp_body(span, resp_body, ts2)
 
                 span.tag(HttpSpan.TAG_HTTP_RESPONSE_SIZE, resp.content_length)
                 span.tag(HttpSpan.TAG_HTTP_STATUS_CODE, str(resp.status))
 
                 return resp
```

### Comparing `ipapp-1.3.8/ipapp/http/server.py` & `ipapp-1.3.9/ipapp/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/__init__.py` & `ipapp-1.3.9/ipapp/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/adapters/_abc.py` & `ipapp-1.3.9/ipapp/logger/adapters/_abc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/adapters/prometheus.py` & `ipapp-1.3.9/ipapp/logger/adapters/prometheus.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/adapters/requests.py` & `ipapp-1.3.9/ipapp/logger/adapters/requests.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/adapters/sentry.py` & `ipapp-1.3.9/ipapp/logger/adapters/sentry.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/adapters/zipkin.py` & `ipapp-1.3.9/ipapp/logger/adapters/zipkin.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/logger.py` & `ipapp-1.3.9/ipapp/logger/logger.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/logger/span.py` & `ipapp-1.3.9/ipapp/logger/span.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/misc.py` & `ipapp-1.3.9/ipapp/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/mq/pika.py` & `ipapp-1.3.9/ipapp/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/openapi/misc.py` & `ipapp-1.3.9/ipapp/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/openapi/models.py` & `ipapp-1.3.9/ipapp/openapi/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/openapi/templates.py` & `ipapp-1.3.9/ipapp/openapi/templates.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/http/client.py` & `ipapp-1.3.9/ipapp/rpc/http/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,29 +34,33 @@
 class RpcClient(Client):
     cfg: RpcClientConfig
 
     def __init__(
         self,
         cfg: RpcClientConfig,
         json_encode: Callable[[Any], str] = default_json_encode,
+        session_kwargs: Optional[Dict[str, Any]] = None,
     ) -> None:
-        super().__init__(cfg, json_encode=json_encode)
+        super().__init__(
+            cfg,
+            json_encode=json_encode,
+            session_kwargs=session_kwargs,
+        )
         self.cfg = cfg
 
     async def call(
         self, method: str, params: Dict[str, Any], timeout: float = 60.0
     ) -> Any:
         body = self._json_encode({"method": method, "params": params}).encode()
 
         with self.app.logger.capture_span(ClientHttpSpan) as trap:
             req_err: Optional[Exception] = None
             try:
-                tout = timeout or self.cfg.timeout
-                if tout:
-                    otout = ClientTimeout(tout)
+                if timeout:
+                    otout = ClientTimeout(timeout)
                 resp = await self.request(
                     'POST', self.cfg.url, body=body, timeout=otout
                 )
             except Exception as err:
                 req_err = err
 
             if trap.is_captured:
```

### Comparing `ipapp-1.3.8/ipapp/rpc/http/server.py` & `ipapp-1.3.9/ipapp/rpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/error.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/http/client.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/http/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Iterable, Mapping, Optional, Tuple, Type, Union
+from typing import Any, Dict, Iterable, Mapping, Optional, Tuple, Type, Union
 
 from aiohttp import ClientTimeout
 from pydantic import BaseModel, Field
 
 from ipapp.http.client import Client, ClientConfig
 from ipapp.rpc.jsonrpc.main import JsonRpcCall
 from ipapp.rpc.jsonrpc.main import JsonRpcClient as _JsonRpcClient
@@ -15,16 +15,20 @@
     timeout: float = Field(60.0, description="Таймаут JSON-RPC вызова")
 
 
 class JsonRpcHttpClient(Client):
     cfg: JsonRpcHttpClientConfig
     clt: _JsonRpcClient
 
-    def __init__(self, cfg: JsonRpcHttpClientConfig) -> None:
-        super().__init__(cfg)
+    def __init__(
+        self,
+        cfg: JsonRpcHttpClientConfig,
+        session_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        super().__init__(cfg, session_kwargs=session_kwargs)
         self.cfg = cfg
 
     async def prepare(self) -> None:
         self.clt = _JsonRpcClient(
             self._send_request,
             self.app,
             exception_mapping_callback=self._raise_jsonrpc_error,
@@ -62,10 +66,9 @@
         _clt_timeout: Optional[ClientTimeout] = None
         if _timeout:
             _clt_timeout = ClientTimeout(_timeout)
 
         resp = await self.request(
             'POST', self.cfg.url, body=request, timeout=_clt_timeout
         )
-        res = await resp.read()
 
-        return res
+        return resp._body
```

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/http/server.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/main.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/mq/pika.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/openrpc/discover.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/discover.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/jsonrpc/openrpc/models.py` & `ipapp-1.3.9/ipapp/rpc/jsonrpc/openrpc/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/main.py` & `ipapp-1.3.9/ipapp/rpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/mq/pika.py` & `ipapp-1.3.9/ipapp/rpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/restrpc/error.py` & `ipapp-1.3.9/ipapp/rpc/restrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/restrpc/http/client.py` & `ipapp-1.3.9/ipapp/rpc/restrpc/http/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Mapping, Optional, Type
+from typing import Any, Dict, Mapping, Optional, Type
 
 from aiohttp import ClientTimeout
 from pydantic import BaseModel, Field
 
 from ipapp.http.client import Client, ClientConfig
 from ipapp.rpc.restrpc.error import RestRpcError
 from ipapp.rpc.restrpc.main import RestRpcCall
@@ -14,16 +14,20 @@
     timeout: float = Field(60.0, description="Таймаут Rest-RPC вызова")
 
 
 class RestRpcHttpClient(Client):
     cfg: RestRpcHttpClientConfig
     clt: _RestRpcClient
 
-    def __init__(self, cfg: RestRpcHttpClientConfig) -> None:
-        super().__init__(cfg)
+    def __init__(
+        self,
+        cfg: RestRpcHttpClientConfig,
+        session_kwargs: Optional[Dict[str, Any]] = None,
+    ) -> None:
+        super().__init__(cfg, session_kwargs=session_kwargs)
         self.cfg = cfg
 
     async def prepare(self) -> None:
         self.clt = _RestRpcClient(
             self._send_request,
             self.app,
             exception_mapping_callback=self._raise_restrpc_error,
@@ -61,9 +65,8 @@
             url = url[:-1]
         resp = await self.request(
             'POST',
             f'{url}/{method_name}/',
             body=request,
             timeout=_clt_timeout,
         )
-        res = await resp.read()
-        return res
+        return resp._body
```

### Comparing `ipapp-1.3.8/ipapp/rpc/restrpc/http/server.py` & `ipapp-1.3.9/ipapp/rpc/restrpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/restrpc/main.py` & `ipapp-1.3.9/ipapp/rpc/restrpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/rpc/restrpc/openapi/misc.py` & `ipapp-1.3.9/ipapp/rpc/restrpc/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/s3/boto.py` & `ipapp-1.3.9/ipapp/s3/boto.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/s3/models.py` & `ipapp-1.3.9/ipapp/s3/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/sftp/client.py` & `ipapp-1.3.9/ipapp/sftp/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/sphinx/config.py` & `ipapp-1.3.9/ipapp/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/task/db.py` & `ipapp-1.3.9/ipapp/task/db.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/utils/lock/local.py` & `ipapp-1.3.9/ipapp/utils/lock/local.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/utils/lock/main.py` & `ipapp-1.3.9/ipapp/utils/lock/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/utils/lock/pg.py` & `ipapp-1.3.9/ipapp/utils/lock/pg.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/ipapp/utils/lock/redis.py` & `ipapp-1.3.9/ipapp/utils/lock/redis.py`

 * *Files identical despite different names*

### Comparing `ipapp-1.3.8/pyproject.toml` & `ipapp-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 force_grid_wrap = 0
 multi_line_output = 3
 use_parentheses = true
 include_trailing_comma = true
 
 [tool.poetry]
 name = "ipapp"
-version = "1.3.8"
+version = "1.3.9"
 description = "InPlat application framework"
 authors = ["InPlat"]
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Intended Audience :: System Administrators',
     'Operating System :: Unix',
@@ -48,15 +48,15 @@
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/inplat/ipapp"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = "^1.8.2"
-aiohttp = "^3.6.2"
+aiohttp = "^3.8.1"
 aiozipkin = ">=0.7,<1.2"
 aiojobs = "^1.0.0"
 prometheus-client = ">=0.8,<0.12"
 sentry-sdk = "^1.0.0"
 deepmerge = ">=0.2.1,<0.4.0"
 async-timeout = "^4.0.0"
 pyyaml = "^5.4"
```

### Comparing `ipapp-1.3.8/setup.py` & `ipapp-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'ipapp.utils',
  'ipapp.utils.lock']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiohttp>=3.6.2,<4.0.0',
+['aiohttp>=3.8.1,<4.0.0',
  'aiojobs>=1.0.0,<2.0.0',
  'aiozipkin>=0.7,<1.2',
  'async-timeout>=4.0.0,<5.0.0',
  'deepmerge>=0.2.1,<0.4.0',
  'docstring-parser>=0.7.1,<0.9.0',
  'jsonschema>=3.2.0,<4.0.0',
  'prometheus-client>=0.8,<0.12',
@@ -70,15 +70,15 @@
              'sphinx-rtd-theme>=0.5.1,<0.6.0',
              'tox>=3.23.0,<4.0.0',
              'docker-compose>=1.27.4,<2.0.0',
              'watchdog>=2.0.2,<3.0.0']}
 
 setup_kwargs = {
     'name': 'ipapp',
-    'version': '1.3.8',
+    'version': '1.3.9',
     'description': 'InPlat application framework',
     'long_description': "# InPlat application framework\n> Framework with asyncio based on python.\n\n![PyPI](https://img.shields.io/pypi/v/ipapp?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ipapp?style=for-the-badge) ![Read the Docs](https://img.shields.io/readthedocs/ipapp?style=for-the-badge)\n\n## Documentation\nDocumentation can be found at [readthedocs](https://ipapp.readthedocs.io/ru/latest/).\n\n## Installation\nUsing pip:\n```sh\npip install ipapp\n```\nUsing poetry:\n```sh\npoetry add ipapp\n```\nInstallation with all dependencies: \n```sh\npoetry add ipapp[fastapi,oracle,postgres,rabbitmq,s3,sftp,dbtm,testing,redis]\n```\n\n## Usage example\nFor examples and usage, please refer to the [examples](examples) folder.\n\n## Release History\nFor release history refer to [release-notes](release-notes.rst).\n\n## Contributing\n1. Fork it\n2. Create your feature branch (`git checkout -b feature/fooBar`)\n3. Commit your changes (`git commit -am 'Add some fooBar'`)\n4. Push to the branch (`git push origin feature/fooBar`)\n5. Create a new Pull Request\n",
     'author': 'InPlat',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/inplat/ipapp',
```

### Comparing `ipapp-1.3.8/PKG-INFO` & `ipapp-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipapp
-Version: 1.3.8
+Version: 1.3.9
 Summary: InPlat application framework
 Home-page: https://github.com/inplat/ipapp
 License: MIT
 Author: InPlat
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -26,15 +26,15 @@
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Provides-Extra: s3
 Provides-Extra: sftp
 Provides-Extra: testing
 Requires-Dist: Sphinx (>=3.5.2,<5.0.0); extra == "testing"
 Requires-Dist: aiobotocore (>=1.2.2,<2.0.0); extra == "s3"
-Requires-Dist: aiohttp (>=3.6.2,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiojobs (>=1.0.0,<2.0.0)
 Requires-Dist: aioredis (>=1.3.1,<2.0.0); extra == "redis"
 Requires-Dist: aiozipkin (>=0.7,<1.2)
 Requires-Dist: async-timeout (>=4.0.0,<5.0.0)
 Requires-Dist: asyncpg (>=0.22,<0.24); extra == "postgres" or extra == "dbtm"
 Requires-Dist: asyncssh[pyOpenSSL] (>=2.3.0,<3.0.0); extra == "sftp"
 Requires-Dist: bandit (==1.6.3); extra == "testing"
```

