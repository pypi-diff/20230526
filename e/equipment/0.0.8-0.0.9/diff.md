# Comparing `tmp/equipment-0.0.8.tar.gz` & `tmp/equipment-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equipment-0.0.8.tar", last modified: Mon Mar 21 10:23:56 2022, max compression
+gzip compressed data, was "equipment-0.0.9.tar", last modified: Mon Mar 21 15:29:48 2022, max compression
```

## Comparing `equipment-0.0.8.tar` & `equipment-0.0.9.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/.github/
--rwxr-xr-x   0 runner    (1001) docker     (121)      899 2022-03-21 10:22:25.000000 equipment-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2006 2022-03-21 10:22:25.000000 equipment-0.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-03-21 10:22:25.000000 equipment-0.0.8/.github/workflows/codeql-analysis.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     2032 2022-03-21 10:22:25.000000 equipment-0.0.8/.github/workflows/publish.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2022-03-21 10:22:25.000000 equipment-0.0.8/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-21 10:22:25.000000 equipment-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-03-21 10:22:25.000000 equipment-0.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-21 10:22:25.000000 equipment-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-21 10:22:25.000000 equipment-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-21 10:23:56.155290 equipment-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-21 10:22:25.000000 equipment-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/console/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/console/Commands/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/Commands/AbstractCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/Commands/MakeJobCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/Commands/NewCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/console/stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/stubs/Job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/console/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/tests/BaseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/console/tests/Commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/tests/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/tests/Commands/test_MakeJobCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/tests/Commands/test_NewCommandTest.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/console/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment/framework/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/App/
--rwxr-xr-x   0 runner    (1001) docker     (121)      847 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/App/Container.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/App/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/Config/
--rwxr-xr-x   0 runner    (1001) docker     (121)      372 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Config/AbstractConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Config/ConfigFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1573 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Config/LocalConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/Connection/
--rwxr-xr-x   0 runner    (1001) docker     (121)      241 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/AbstractConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1496 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/MongoDBConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1192 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/MySQLConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1426 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/Neo4JConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1127 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/PostgreSQLConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1124 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/RedisConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      930 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/SQLAlchemyConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1155 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/SQLServerConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1179 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/SQLiteConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/Environment/
--rwxr-xr-x   0 runner    (1001) docker     (121)      283 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Environment/AbstractEnvironment.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Environment/EnvironmentFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Environment/LocalEnvironment.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Exceptions/ContainerModuleNotFound.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.135290 equipment-0.0.8/equipment/framework/Jobs/
--rwxr-xr-x   0 runner    (1001) docker     (121)      626 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Jobs/AbstractJob.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Log/
--rwxr-xr-x   0 runner    (1001) docker     (121)      653 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/AbstractLog.py
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/ConsoleLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      689 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/GELFLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      690 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/LocalLog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/LogFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1560 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/NativeLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      344 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/NoneLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Mail/
--rwxr-xr-x   0 runner    (1001) docker     (121)      288 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/AbstractMail.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Mail/Email/
--rwxr-xr-x   0 runner    (1001) docker     (121)      240 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/Email/Email.py
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/Email/EmailFactory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/Email/HTMLEmailFactory.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/Email/TextEmailFactory.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/Email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/LogMail.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/MailFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2900 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/SESMail.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1384 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/SMTPMail.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Queue/
--rwxr-xr-x   0 runner    (1001) docker     (121)      266 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/AbstractQueue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/QueueFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1429 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/RedisQueue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      346 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/SQSQueue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      770 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/SyncQueue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Scheduler/
--rwxr-xr-x   0 runner    (1001) docker     (121)      108 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Scheduler/AbstractScheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      873 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Scheduler/Scheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.139290 equipment-0.0.8/equipment/framework/Storage/
--rwxr-xr-x   0 runner    (1001) docker     (121)      428 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Storage/AbstractStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1608 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Storage/LocalStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2599 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Storage/S3Storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Storage/StorageFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/Storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)      852 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/BaseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Config/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Config/test_AbstractConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2597 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Config/test_LocalConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Connection/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      624 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_AbstractConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1055 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_MongoDBConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1291 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_Neo4JConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1043 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_RedisConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      763 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_SQLAlchemyConnection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1410 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Connection/test_SQLiteConnection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Environment/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Environment/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      639 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Environment/test_AbstractEnvironment.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1039 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Environment/test_LocalEnvironment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Exceptions/test_ContainerModuleNotFound.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Helpers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Helpers/test_base_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Helpers/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Helpers/test_print_if.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Jobs/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Jobs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      465 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Jobs/test_AbstractJob.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.143291 equipment-0.0.8/equipment/framework/tests/Log/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Log/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Log/test_AbstractLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1364 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Log/test_LocalLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      918 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Log/test_NativeLog.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1150 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Log/test_NoneLog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.147291 equipment-0.0.8/equipment/framework/tests/Mail/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Mail/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      874 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Mail/test_AbstractMail.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2336 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Mail/test_SESMail.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2109 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Mail/test_SMTPMail.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.147291 equipment-0.0.8/equipment/framework/tests/Queue/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Queue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Queue/test_AbstractQueue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1166 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Queue/test_RedisQueue.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1261 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Queue/test_SyncQueue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.147291 equipment-0.0.8/equipment/framework/tests/Scheduler/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Scheduler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      431 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Scheduler/test_AbstractScheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      794 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Scheduler/test_Scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.147291 equipment-0.0.8/equipment/framework/tests/Storage/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Storage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      701 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Storage/test_AbstractStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1285 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Storage/test_LocalStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1504 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/Storage/test_S3Storage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/equipment/framework/tests/_stubs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.147291 equipment-0.0.8/equipment/framework/tests/_stubs/config/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/app.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/connection.conf
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/log.conf
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/mail.conf
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/queue.conf
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/framework/tests/_stubs/config/storage.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/.env.example
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/.env.test
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/.pylintrc
--rwxr-xr-x   0 runner    (1001) docker     (121)     1876 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/equipment/project/app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/app/App/
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/App/Container.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/App/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/app/Commands/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Commands/ExampleCommand.py
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/app/Jobs/
--rwxr-xr-x   0 runner    (1001) docker     (121)      335 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Jobs/ExampleJob.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/app/Mail/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Mail/WelcomeEmail.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Mail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/app/Scheduler/
--rwxr-xr-x   0 runner    (1001) docker     (121)      588 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Scheduler/Scheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/app/Scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/config/
--rwxr-xr-x   0 runner    (1001) docker     (121)       26 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/app.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)     1000 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/connection.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)      336 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/log.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)      369 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/mail.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)      141 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/queue.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)      326 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/config/storage.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)     2137 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1138 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/examples/example_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      506 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/examples/example_email.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      281 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/examples/example_job.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      749 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/examples/example_matplotlib.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      580 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/examples/examples_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      695 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/migrations/
--rwxr-xr-x   0 runner    (1001) docker     (121)       38 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/migrations/README
--rwxr-xr-x   0 runner    (1001) docker     (121)     1993 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/migrations/alembic.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)     2201 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/migrations/env.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      494 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.151291 equipment-0.0.8/equipment/project/migrations/versions/
--rwxr-xr-x   0 runner    (1001) docker     (121)      556 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/migrations/versions/0797374c92af_create_example_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-03-21 10:23:54.000000 equipment-0.0.8/equipment/project/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/equipment/project/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/equipment/project/resources/views/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/resources/views/emails/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/resources/views/emails/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/resources/views/emails/welcome.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      176 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.127291 equipment-0.0.8/equipment/project/storage/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/storage/app/
--rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/storage/app/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/storage/logs/
--rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/storage/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/storage/test/
--rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/storage/test/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/BaseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/tests/Commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Commands/test_ExampleCommand.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/tests/Jobs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Jobs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      391 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Jobs/test_ExampleJob.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.155290 equipment-0.0.8/equipment/project/tests/Mail/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/Mail/test_WelcomeEmail.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      912 2022-03-21 10:22:25.000000 equipment-0.0.8/equipment/project/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 10:23:56.131291 equipment-0.0.8/equipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-21 10:23:55.000000 equipment-0.0.8/equipment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 10:23:56.155290 equipment-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-03-21 10:23:54.000000 equipment-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      899 2022-03-21 15:28:38.000000 equipment-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2006 2022-03-21 15:28:38.000000 equipment-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-03-21 15:28:38.000000 equipment-0.0.9/.github/workflows/codeql-analysis.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2032 2022-03-21 15:28:38.000000 equipment-0.0.9/.github/workflows/publish.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2022-03-21 15:28:38.000000 equipment-0.0.9/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-21 15:28:38.000000 equipment-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-03-21 15:28:38.000000 equipment-0.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-21 15:28:38.000000 equipment-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-03-21 15:28:38.000000 equipment-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-21 15:29:48.255891 equipment-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-03-21 15:28:38.000000 equipment-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/console/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/console/Commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/Commands/AbstractCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/Commands/MakeJobCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/Commands/NewCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/console/stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/stubs/Job.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/console/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/tests/BaseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/console/tests/Commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/tests/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/tests/Commands/test_MakeJobCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/tests/Commands/test_NewCommandTest.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/console/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/App/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      847 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/App/Container.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/App/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      372 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Config/AbstractConfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Config/ConfigFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1573 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Config/LocalConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/Connection/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      241 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/AbstractConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1496 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/MongoDBConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1192 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/MySQLConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1426 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/Neo4JConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1127 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/PostgreSQLConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1124 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/RedisConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      930 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/SQLAlchemyConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1155 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/SQLServerConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1179 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/SQLiteConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/Environment/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      283 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Environment/AbstractEnvironment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Environment/EnvironmentFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Environment/LocalEnvironment.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Exceptions/ContainerModuleNotFound.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment/framework/Jobs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      626 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Jobs/AbstractJob.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Log/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      653 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/AbstractLog.py
+-rw-r--r--   0 runner    (1001) docker     (121)      547 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/ConsoleLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      689 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/GELFLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      690 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/LocalLog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/LogFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1560 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/NativeLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      344 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/NoneLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Mail/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      288 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/AbstractMail.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Mail/Email/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      240 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/Email/Email.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/Email/EmailFactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/Email/HTMLEmailFactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/Email/TextEmailFactory.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/Email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/LogMail.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/MailFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2900 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/SESMail.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1384 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/SMTPMail.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Queue/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      266 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/AbstractQueue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/QueueFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1429 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/RedisQueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      346 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/SQSQueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      770 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/SyncQueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Scheduler/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      108 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Scheduler/AbstractScheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      873 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Scheduler/Scheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/Storage/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      428 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Storage/AbstractStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1608 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Storage/LocalStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2599 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Storage/S3Storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Storage/StorageFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/Storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      869 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/BaseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Config/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Config/test_AbstractConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2611 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Config/test_LocalConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Connection/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      624 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_AbstractConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1055 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_MongoDBConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1291 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_Neo4JConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1043 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_RedisConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      763 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_SQLAlchemyConnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1410 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Connection/test_SQLiteConnection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Environment/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Environment/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      639 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Environment/test_AbstractEnvironment.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1039 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Environment/test_LocalEnvironment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Exceptions/test_ContainerModuleNotFound.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Helpers/test_base_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Helpers/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Helpers/test_print_if.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.247891 equipment-0.0.9/equipment/framework/tests/Jobs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Jobs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      465 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Jobs/test_AbstractJob.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/Log/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Log/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      731 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Log/test_AbstractLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1364 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Log/test_LocalLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      918 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Log/test_NativeLog.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1150 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Log/test_NoneLog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/Mail/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Mail/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      874 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Mail/test_AbstractMail.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2336 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Mail/test_SESMail.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2109 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Mail/test_SMTPMail.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/Queue/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Queue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      611 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Queue/test_AbstractQueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1166 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Queue/test_RedisQueue.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1261 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Queue/test_SyncQueue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/Scheduler/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Scheduler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      431 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Scheduler/test_AbstractScheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      794 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Scheduler/test_Scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/Storage/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Storage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      701 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Storage/test_AbstractStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1285 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Storage/test_LocalStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1504 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/Storage/test_S3Storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/equipment/framework/tests/_stubs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/framework/tests/_stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/app.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/connection.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/log.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/mail.conf
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/queue.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/framework/tests/_stubs/config/storage.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/.env.example
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/.env.test
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/.pylintrc
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1876 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/equipment/project/app/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/app/App/
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/App/Container.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/App/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/app/Commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Commands/ExampleCommand.py
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/app/Jobs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      335 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Jobs/ExampleJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/app/Mail/
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Mail/WelcomeEmail.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/app/Scheduler/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      588 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Scheduler/Scheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/app/Scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.251891 equipment-0.0.9/equipment/project/config/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       26 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/app.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1000 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/connection.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)      336 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/log.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)      369 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/mail.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)      141 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/queue.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)      326 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/config/storage.conf
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2137 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1138 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/examples/example_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      506 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/examples/example_email.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      281 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/examples/example_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      749 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/examples/example_matplotlib.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      580 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/examples/examples_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      695 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/migrations/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       38 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/migrations/README
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1993 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/migrations/alembic.ini
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2201 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/migrations/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      494 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/migrations/versions/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      556 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/migrations/versions/0797374c92af_create_example_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-03-21 15:29:46.000000 equipment-0.0.9/equipment/project/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/equipment/project/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/equipment/project/resources/views/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/resources/views/emails/
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/resources/views/emails/layout.html
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/resources/views/emails/welcome.html
+-rwxr-xr-x   0 runner    (1001) docker     (121)      176 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.239891 equipment-0.0.9/equipment/project/storage/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/storage/app/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/storage/app/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/storage/logs/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/storage/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/storage/test/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       14 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/storage/test/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/BaseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/tests/Commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Commands/test_ExampleCommand.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/tests/Jobs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Jobs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      391 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Jobs/test_ExampleJob.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.255891 equipment-0.0.9/equipment/project/tests/Mail/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/Mail/test_WelcomeEmail.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      912 2022-03-21 15:28:38.000000 equipment-0.0.9/equipment/project/web.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:29:48.243891 equipment-0.0.9/equipment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-21 15:29:47.000000 equipment-0.0.9/equipment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-03-21 15:29:48.000000 equipment-0.0.9/equipment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:29:47.000000 equipment-0.0.9/equipment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-03-21 15:29:47.000000 equipment-0.0.9/equipment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-21 15:29:47.000000 equipment-0.0.9/equipment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-21 15:29:48.000000 equipment-0.0.9/equipment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 15:29:48.255891 equipment-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-03-21 15:29:46.000000 equipment-0.0.9/setup.py
```

### Comparing `equipment-0.0.8/.github/dependabot.yml` & `equipment-0.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/.github/workflows/build.yml` & `equipment-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/.github/workflows/codeql-analysis.yml` & `equipment-0.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/.github/workflows/publish.yml` & `equipment-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/.github/workflows/pull_request.yml` & `equipment-0.0.9/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/LICENSE` & `equipment-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/PKG-INFO` & `equipment-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: equipment
-Version: 0.0.8
+Version: 0.0.9
 Summary: The root of your next python project
 Home-page: https://github.com/rogervila/equipment
-Download-URL: https://github.com/rogervila/equipment/archive/0.0.8.tar.gz
+Download-URL: https://github.com/rogervila/equipment/archive/0.0.9.tar.gz
 Author: Roger Vilà
 Author-email: rogervila@me.com
 License: MIT
 Keywords: equipment,application scaffolding,framework
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: equipment Version: 0.0.8 Summary: The root of your
+Metadata-Version: 2.1 Name: equipment Version: 0.0.9 Summary: The root of your
 next python project Home-page: https://github.com/rogervila/equipment Download-
-URL: https://github.com/rogervila/equipment/archive/0.0.8.tar.gz Author: Roger
+URL: https://github.com/rogervila/equipment/archive/0.0.9.tar.gz Author: Roger
 VilÃ  Author-email: rogervila@me.com License: MIT Keywords:
 equipment,application scaffolding,framework Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
                          [Equipment python framework]
```

### Comparing `equipment-0.0.8/README.md` & `equipment-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/console/Commands/MakeJobCommand.py` & `equipment-0.0.9/equipment/console/Commands/MakeJobCommand.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/console/Commands/NewCommand.py` & `equipment-0.0.9/equipment/console/Commands/NewCommand.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/console/__init__.py` & `equipment-0.0.9/equipment/console/__init__.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/console/tests/Commands/test_MakeJobCommand.py` & `equipment-0.0.9/equipment/console/tests/Commands/test_MakeJobCommand.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/console/tests/Commands/test_NewCommandTest.py` & `equipment-0.0.9/equipment/console/tests/Commands/test_NewCommandTest.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/App/Container.py` & `equipment-0.0.9/equipment/framework/App/Container.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Config/ConfigFactory.py` & `equipment-0.0.9/equipment/framework/Config/ConfigFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Config/LocalConfig.py` & `equipment-0.0.9/equipment/framework/Config/LocalConfig.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/MongoDBConnection.py` & `equipment-0.0.9/equipment/framework/Connection/MongoDBConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/MySQLConnection.py` & `equipment-0.0.9/equipment/framework/Connection/MySQLConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/Neo4JConnection.py` & `equipment-0.0.9/equipment/framework/Connection/Neo4JConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/PostgreSQLConnection.py` & `equipment-0.0.9/equipment/framework/Connection/PostgreSQLConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/RedisConnection.py` & `equipment-0.0.9/equipment/framework/Connection/RedisConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/SQLAlchemyConnection.py` & `equipment-0.0.9/equipment/framework/Connection/SQLAlchemyConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/SQLServerConnection.py` & `equipment-0.0.9/equipment/framework/Connection/SQLServerConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Connection/SQLiteConnection.py` & `equipment-0.0.9/equipment/framework/Connection/SQLiteConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Environment/EnvironmentFactory.py` & `equipment-0.0.9/equipment/framework/Environment/EnvironmentFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Environment/LocalEnvironment.py` & `equipment-0.0.9/equipment/framework/Environment/LocalEnvironment.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Jobs/AbstractJob.py` & `equipment-0.0.9/equipment/framework/Jobs/AbstractJob.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/AbstractLog.py` & `equipment-0.0.9/equipment/framework/Log/AbstractLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/ConsoleLog.py` & `equipment-0.0.9/equipment/framework/Log/ConsoleLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/GELFLog.py` & `equipment-0.0.9/equipment/framework/Log/GELFLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/LocalLog.py` & `equipment-0.0.9/equipment/framework/Log/LocalLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/LogFactory.py` & `equipment-0.0.9/equipment/framework/Log/LogFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Log/NativeLog.py` & `equipment-0.0.9/equipment/framework/Log/NativeLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/Email/EmailFactory.py` & `equipment-0.0.9/equipment/framework/Mail/Email/EmailFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/Email/HTMLEmailFactory.py` & `equipment-0.0.9/equipment/framework/Mail/Email/HTMLEmailFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/Email/TextEmailFactory.py` & `equipment-0.0.9/equipment/framework/Mail/Email/TextEmailFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/LogMail.py` & `equipment-0.0.9/equipment/framework/Mail/LogMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/MailFactory.py` & `equipment-0.0.9/equipment/framework/Mail/MailFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/SESMail.py` & `equipment-0.0.9/equipment/framework/Mail/SESMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Mail/SMTPMail.py` & `equipment-0.0.9/equipment/framework/Mail/SMTPMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Queue/QueueFactory.py` & `equipment-0.0.9/equipment/framework/Queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Queue/RedisQueue.py` & `equipment-0.0.9/equipment/framework/Queue/RedisQueue.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Queue/SyncQueue.py` & `equipment-0.0.9/equipment/framework/Queue/SyncQueue.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Scheduler/Scheduler.py` & `equipment-0.0.9/equipment/framework/Scheduler/Scheduler.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Storage/LocalStorage.py` & `equipment-0.0.9/equipment/framework/Storage/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Storage/S3Storage.py` & `equipment-0.0.9/equipment/framework/Storage/S3Storage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/Storage/StorageFactory.py` & `equipment-0.0.9/equipment/framework/Storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/helpers.py` & `equipment-0.0.9/equipment/framework/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     return resolved_module.Container
 
 
 def base_path(join: Optional[str] = None, container: Optional[Container] = None) -> Path:
     if container is None:
         container = app()
 
-    # We assume containers always leave under ./App/Container
-    return Path(getfile(container)).parent.parent.absolute().joinpath(
+    # We assume containers always leave under ./app/App/Container
+    return Path(getfile(container)).parent.parent.parent.absolute().joinpath(
         join if join is not None else ''
     )
 
 
 def module(name: str, print_exception: bool = False) -> Any:
     try:
         return import_module(name) if name not in _modules else _modules[name]
```

### Comparing `equipment-0.0.8/equipment/framework/tests/BaseTest.py` & `equipment-0.0.9/equipment/framework/tests/BaseTest.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         # Initialize app
         self.app = app('equipment.framework.App.Container')
 
         # Override config
         self.app.config.override(LocalConfig(
             self.app.environment(),
-            f'tests{os.sep}_stubs{os.sep}config'
+            f'framework{os.sep}tests{os.sep}_stubs{os.sep}config'
         ))
 
         # Override logger
         self.app.log.override(NoneLog(config=self.app.config()))
 
 
 if __name__ == '__main__':
```

### Comparing `equipment-0.0.8/equipment/framework/tests/Config/test_AbstractConfig.py` & `equipment-0.0.9/equipment/framework/tests/Config/test_AbstractConfig.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Config/test_LocalConfig.py` & `equipment-0.0.9/equipment/framework/tests/Config/test_LocalConfig.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class test_LocalConfig(BaseTest):
     def setUp(self):
         super().setUp()
         self.app.config.override(LocalConfig(
             self.app.environment(),
-            f'tests{sep}_stubs{sep}config'
+            f'framework{sep}tests{sep}_stubs{sep}config'
         ))
 
     def test_extends_from_abstract_config(self):
         self.assertTrue(
             isinstance(self.app.config(), AbstractConfig)
         )
```

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_AbstractConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_AbstractConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_MongoDBConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_MongoDBConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_Neo4JConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_Neo4JConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_RedisConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_RedisConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_SQLAlchemyConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_SQLAlchemyConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Connection/test_SQLiteConnection.py` & `equipment-0.0.9/equipment/framework/tests/Connection/test_SQLiteConnection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Environment/test_AbstractEnvironment.py` & `equipment-0.0.9/equipment/framework/tests/Environment/test_AbstractEnvironment.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Environment/test_LocalEnvironment.py` & `equipment-0.0.9/equipment/framework/tests/Environment/test_LocalEnvironment.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Helpers/test_print_if.py` & `equipment-0.0.9/equipment/framework/tests/Helpers/test_print_if.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Log/test_AbstractLog.py` & `equipment-0.0.9/equipment/framework/tests/Log/test_AbstractLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Log/test_LocalLog.py` & `equipment-0.0.9/equipment/framework/tests/Log/test_LocalLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Log/test_NativeLog.py` & `equipment-0.0.9/equipment/framework/tests/Log/test_NativeLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Log/test_NoneLog.py` & `equipment-0.0.9/equipment/framework/tests/Log/test_NoneLog.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Mail/test_AbstractMail.py` & `equipment-0.0.9/equipment/framework/tests/Mail/test_AbstractMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Mail/test_SESMail.py` & `equipment-0.0.9/equipment/framework/tests/Mail/test_SESMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Mail/test_SMTPMail.py` & `equipment-0.0.9/equipment/framework/tests/Mail/test_SMTPMail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Queue/test_AbstractQueue.py` & `equipment-0.0.9/equipment/framework/tests/Queue/test_AbstractQueue.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Queue/test_RedisQueue.py` & `equipment-0.0.9/equipment/framework/tests/Queue/test_RedisQueue.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Queue/test_SyncQueue.py` & `equipment-0.0.9/equipment/framework/tests/Queue/test_SyncQueue.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Scheduler/test_Scheduler.py` & `equipment-0.0.9/equipment/framework/tests/Scheduler/test_Scheduler.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Storage/test_AbstractStorage.py` & `equipment-0.0.9/equipment/framework/tests/Storage/test_AbstractStorage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Storage/test_LocalStorage.py` & `equipment-0.0.9/equipment/framework/tests/Storage/test_LocalStorage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/Storage/test_S3Storage.py` & `equipment-0.0.9/equipment/framework/tests/Storage/test_S3Storage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/framework/tests/_stubs/config/connection.conf` & `equipment-0.0.9/equipment/framework/tests/_stubs/config/connection.conf`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/.env.example` & `equipment-0.0.9/equipment/project/.env.example`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/Dockerfile` & `equipment-0.0.9/equipment/project/Dockerfile`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/app/App/Container.py` & `equipment-0.0.9/equipment/project/app/App/Container.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/app/Scheduler/Scheduler.py` & `equipment-0.0.9/equipment/project/app/Scheduler/Scheduler.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/config/connection.conf` & `equipment-0.0.9/equipment/project/config/connection.conf`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/docker-compose.yml` & `equipment-0.0.9/equipment/project/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/examples/example_connection.py` & `equipment-0.0.9/equipment/project/examples/example_connection.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/examples/example_matplotlib.py` & `equipment-0.0.9/equipment/project/examples/example_matplotlib.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/examples/examples_storage.py` & `equipment-0.0.9/equipment/project/examples/examples_storage.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/main.py` & `equipment-0.0.9/equipment/project/main.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/migrations/alembic.ini` & `equipment-0.0.9/equipment/project/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/migrations/env.py` & `equipment-0.0.9/equipment/project/migrations/env.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/migrations/versions/0797374c92af_create_example_table.py` & `equipment-0.0.9/equipment/project/migrations/versions/0797374c92af_create_example_table.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/requirements.txt` & `equipment-0.0.9/equipment/project/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-equipment==0.0.8
+equipment==0.0.9
 alembic==1.7.7 # Remove if SQLAlchemy is not used
 boto3==1.21.19 # Remove if AWS is not used (affects "ses" email and "s3" storage drivers)
 flask==2.0.3 # Remove if web server is not used
 Flask-WTF==1.0.0 # Remove if web server is not used
 mail1==4.1.0 # Remove if "smtp" email driver is not used
 mysqlclient==2.1.0 # Remove mysqlclient if MySQL is not used
 neomodel==4.0.8 # Remove neomodel if Neo4J is not used
```

### Comparing `equipment-0.0.8/equipment/project/resources/views/emails/layout.html` & `equipment-0.0.9/equipment/project/resources/views/emails/layout.html`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/tests/Commands/test_ExampleCommand.py` & `equipment-0.0.9/equipment/project/tests/Commands/test_ExampleCommand.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/tests/Mail/test_WelcomeEmail.py` & `equipment-0.0.9/equipment/project/tests/Mail/test_WelcomeEmail.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment/project/web.py` & `equipment-0.0.9/equipment/project/web.py`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/equipment.egg-info/PKG-INFO` & `equipment-0.0.9/equipment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: equipment
-Version: 0.0.8
+Version: 0.0.9
 Summary: The root of your next python project
 Home-page: https://github.com/rogervila/equipment
-Download-URL: https://github.com/rogervila/equipment/archive/0.0.8.tar.gz
+Download-URL: https://github.com/rogervila/equipment/archive/0.0.9.tar.gz
 Author: Roger Vilà
 Author-email: rogervila@me.com
 License: MIT
 Keywords: equipment,application scaffolding,framework
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: equipment Version: 0.0.8 Summary: The root of your
+Metadata-Version: 2.1 Name: equipment Version: 0.0.9 Summary: The root of your
 next python project Home-page: https://github.com/rogervila/equipment Download-
-URL: https://github.com/rogervila/equipment/archive/0.0.8.tar.gz Author: Roger
+URL: https://github.com/rogervila/equipment/archive/0.0.9.tar.gz Author: Roger
 VilÃ  Author-email: rogervila@me.com License: MIT Keywords:
 equipment,application scaffolding,framework Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
                          [Equipment python framework]
```

### Comparing `equipment-0.0.8/equipment.egg-info/SOURCES.txt` & `equipment-0.0.9/equipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `equipment-0.0.8/setup.py` & `equipment-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='equipment',
     packages=['equipment'],
-    version='0.0.8',
+    version='0.0.9',
     license='MIT',
     description='The root of your next python project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Roger Vilà',
     author_email='rogervila@me.com',
     url='https://github.com/rogervila/equipment',
-    download_url='https://github.com/rogervila/equipment/archive/0.0.8.tar.gz',
+    download_url='https://github.com/rogervila/equipment/archive/0.0.9.tar.gz',
     keywords=['equipment', 'application scaffolding', 'framework'],
     install_requires=install_requires,
     tests_require=['coverage', 'runtype'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
```

