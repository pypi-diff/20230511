# Comparing `tmp/celery-5.3.0b1.tar.gz` & `tmp/celery-5.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery-5.3.0b1.tar", last modified: Mon Aug  1 11:20:03 2022, max compression
+gzip compressed data, was "celery-5.3.0b2.tar", last modified: Sun Feb 19 10:26:57 2023, max compression
```

## Comparing `celery-5.3.0b1.tar` & `celery-5.3.0b2.tar`

### file list

```diff
@@ -1,742 +1,750 @@
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.501145 celery-5.3.0b1/
--rw-rw-r--   0 asif      (1000) asif      (1000)     8128 2022-08-01 10:53:57.000000 celery-5.3.0b1/CONTRIBUTORS.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)    11200 2022-08-01 11:13:00.000000 celery-5.3.0b1/Changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2631 2021-10-12 14:26:47.000000 celery-5.3.0b1/LICENSE
--rw-rw-r--   0 asif      (1000) asif      (1000)      709 2021-10-12 14:26:47.000000 celery-5.3.0b1/MANIFEST.in
--rw-rw-r--   0 asif      (1000) asif      (1000)    17770 2022-08-01 11:20:03.501145 celery-5.3.0b1/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    15629 2022-08-01 11:15:00.000000 celery-5.3.0b1/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)       84 2021-10-12 14:26:47.000000 celery-5.3.0b1/TODO
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.297142 celery-5.3.0b1/celery/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5950 2022-08-01 11:14:23.000000 celery-5.3.0b1/celery/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      409 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/__main__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5029 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/_state.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.305142 celery-5.3.0b1/celery/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2430 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/app/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    23163 2022-06-29 11:34:45.000000 celery-5.3.0b1/celery/app/amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1445 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/annotations.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2489 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/app/autoretry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2750 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/app/backends.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    48479 2022-07-28 12:22:51.000000 celery-5.3.0b1/celery/app/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6673 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/builtins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    27841 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14836 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/app/defaults.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1326 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9102 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/app/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2001 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/registry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4527 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/app/routes.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    42666 2022-06-29 11:34:45.000000 celery-5.3.0b1/celery/app/task.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    27220 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/app/trace.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13160 2022-07-28 12:22:51.000000 celery-5.3.0b1/celery/app/utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.305142 celery-5.3.0b1/celery/apps/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/apps/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5268 2022-07-28 12:22:51.000000 celery-5.3.0b1/celery/apps/beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16360 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/apps/multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13215 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/apps/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.313142 celery-5.3.0b1/celery/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7739 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/backends/arangodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10309 2021-11-21 13:37:38.000000 celery-5.3.0b1/celery/backends/asynchronous.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5127 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/backends/azureblockblob.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    43116 2022-06-29 11:34:45.000000 celery-5.3.0b1/celery/backends/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4817 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9026 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/backends/cassandra.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3816 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6797 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/backends/cosmosdbsql.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3393 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/backends/couchbase.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2935 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/couchdb.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.313142 celery-5.3.0b1/celery/backends/database/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7771 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/database/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3351 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/database/models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3011 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/database/session.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17255 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/backends/dynamodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8339 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/elasticsearch.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3776 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/backends/filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10725 2021-12-29 05:20:59.000000 celery-5.3.0b1/celery/backends/mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    26409 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/backends/redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12077 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/rpc.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2752 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/backends/s3.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24339 2022-03-19 09:49:50.000000 celery-5.3.0b1/celery/beat.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.317142 celery-5.3.0b1/celery/bin/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bin/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10023 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/bin/amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8454 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2592 2022-07-28 12:22:51.000000 celery-5.3.0b1/celery/bin/beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2370 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/call.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6767 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7058 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2794 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5796 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bin/graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bin/list.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4267 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bin/logtool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2108 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15364 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bin/multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2547 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/purge.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      976 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4778 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/shell.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3064 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/bin/upgrade.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12869 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/bin/worker.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12297 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/bootsteps.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    73700 2022-07-05 07:04:36.000000 celery-5.3.0b1/celery/canvas.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.321142 celery-5.3.0b1/celery/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)      995 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    51380 2022-08-01 10:53:57.000000 celery-5.3.0b1/celery/concurrency/asynpool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4373 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5126 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/eventlet.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3407 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/gevent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5789 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/prefork.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      693 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/solo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1248 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/concurrency/thread.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.321142 celery-5.3.0b1/celery/contrib/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/contrib/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5003 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/contrib/abortable.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14361 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/contrib/migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6746 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/contrib/pytest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5005 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/contrib/rdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3410 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/contrib/sphinx.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.325142 celery-5.3.0b1/celery/contrib/testing/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/contrib/testing/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3112 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/contrib/testing/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7723 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/contrib/testing/manager.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4158 2021-11-21 13:37:38.000000 celery-5.3.0b1/celery/contrib/testing/mocks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      208 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/contrib/testing/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5750 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/contrib/testing/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.329142 celery-5.3.0b1/celery/events/
--rw-rw-r--   0 asif      (1000) asif      (1000)      477 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17961 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/events/cursesmon.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8987 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/dispatcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3116 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/dumper.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1736 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/event.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4998 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/receiver.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3294 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/events/snapshot.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25640 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/events/state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8995 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/exceptions.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.329142 celery-5.3.0b1/celery/fixups/
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/fixups/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7104 2022-07-28 12:22:51.000000 celery-5.3.0b1/celery/fixups/django.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.329142 celery-5.3.0b1/celery/loaders/
--rw-rw-r--   0 asif      (1000) asif      (1000)      490 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/loaders/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      199 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/loaders/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8825 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/loaders/base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1520 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/loaders/default.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16041 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/local.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25564 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/platforms.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    33881 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28823 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/schedules.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.329142 celery-5.3.0b1/celery/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2363 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/security/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2991 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/security/certificate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1056 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/security/key.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4248 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/security/serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      845 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/security/utils.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4273 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/signals.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3324 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/states.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.337142 celery-5.3.0b1/celery/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)      935 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2874 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/abstract.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25419 2022-04-28 06:12:03.000000 celery-5.3.0b1/celery/utils/collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4709 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3620 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/deprecated.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.337142 celery-5.3.0b1/celery/utils/dispatch/
--rw-rw-r--   0 asif      (1000) asif      (1000)       74 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/dispatch/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13603 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/dispatch/signal.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11949 2022-06-29 11:34:45.000000 celery-5.3.0b1/celery/utils/functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9041 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4779 2022-06-29 10:52:39.000000 celery-5.3.0b1/celery/utils/imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2776 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/iso8601.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8809 2021-11-21 13:37:38.000000 celery-5.3.0b1/celery/utils/log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2858 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/nodenames.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4215 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8937 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/utils/saferepr.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8043 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/serialization.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.341142 celery-5.3.0b1/celery/utils/static/
--rw-rw-r--   0 asif      (1000) asif      (1000)      299 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/static/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/static/celery_128.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/sysinfo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4568 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/term.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5816 2021-11-21 13:37:38.000000 celery-5.3.0b1/celery/utils/text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9592 2021-11-21 13:37:38.000000 celery-5.3.0b1/celery/utils/threads.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12389 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/utils/time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4813 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/utils/timer2.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.341142 celery-5.3.0b1/celery/worker/
--rw-rw-r--   0 asif      (1000) asif      (1000)       95 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4593 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/autoscale.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7517 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/components.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.345142 celery-5.3.0b1/celery/worker/consumer/
--rw-rw-r--   0 asif      (1000) asif      (1000)      391 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      525 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/agent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1026 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/connection.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    27984 2022-08-01 10:53:57.000000 celery-5.3.0b1/celery/worker/consumer/consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      946 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2054 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6833 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/gossip.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      930 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/heart.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2519 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/consumer/mingle.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/worker/consumer/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16885 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2107 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/heartbeat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4433 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/loops.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3630 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/pidbox.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    25526 2022-06-29 11:34:45.000000 celery-5.3.0b1/celery/worker/request.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8394 2022-08-01 10:53:57.000000 celery-5.3.0b1/celery/worker/state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7349 2021-10-12 14:26:47.000000 celery-5.3.0b1/celery/worker/strategy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14480 2022-03-18 11:40:50.000000 celery-5.3.0b1/celery/worker/worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.301142 celery-5.3.0b1/celery.egg-info/
--rw-rw-r--   0 asif      (1000) asif      (1000)    17770 2022-08-01 11:20:02.000000 celery-5.3.0b1/celery.egg-info/PKG-INFO
--rw-rw-r--   0 asif      (1000) asif      (1000)    20951 2022-08-01 11:20:03.000000 celery-5.3.0b1/celery.egg-info/SOURCES.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2022-08-01 11:20:02.000000 celery-5.3.0b1/celery.egg-info/dependency_links.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       48 2022-08-01 11:20:02.000000 celery-5.3.0b1/celery.egg-info/entry_points.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        1 2021-11-08 01:14:46.000000 celery-5.3.0b1/celery.egg-info/not-zip-safe
--rw-rw-r--   0 asif      (1000) asif      (1000)     1543 2022-08-01 11:20:02.000000 celery-5.3.0b1/celery.egg-info/requires.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)        7 2022-08-01 11:20:02.000000 celery-5.3.0b1/celery.egg-info/top_level.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5293 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/AUTHORS.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     8111 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/Makefile
--rw-rw-r--   0 asif      (1000) asif      (1000)      494 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/THANKS
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/_ext/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5164 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/_ext/celerydocs.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/_static/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/_static/.keep
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/_templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/_templates/sidebardonations.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       30 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/changelog.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      981 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/community.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2597 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       83 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/configuration.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       33 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/contributing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      931 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/copyright.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/django/
--rw-rw-r--   0 asif      (1000) asif      (1000)     7888 2021-12-29 05:20:59.000000 celery-5.3.0b1/docs/django/first-steps-with-django.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      137 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/django/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    29794 2022-06-29 10:52:39.000000 celery-5.3.0b1/docs/faq.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.353142 celery-5.3.0b1/docs/getting-started/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.357143 celery-5.3.0b1/docs/getting-started/backends-and-brokers/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3950 2022-06-29 10:52:39.000000 celery-5.3.0b1/docs/getting-started/backends-and-brokers/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5002 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/getting-started/backends-and-brokers/rabbitmq.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6462 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/getting-started/backends-and-brokers/redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10843 2022-03-18 11:40:50.000000 celery-5.3.0b1/docs/getting-started/backends-and-brokers/sqs.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    15015 2022-06-29 10:52:39.000000 celery-5.3.0b1/docs/getting-started/first-steps-with-celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/getting-started/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10903 2021-12-29 05:20:59.000000 celery-5.3.0b1/docs/getting-started/introduction.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    22787 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/getting-started/next-steps.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      132 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/getting-started/resources.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     4448 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/glossary.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.365143 celery-5.3.0b1/docs/history/
--rw-rw-r--   0 asif      (1000) asif      (1000)    58103 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-1.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    34009 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-2.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    23550 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-2.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    33558 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-2.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    11200 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-2.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    13012 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-2.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5414 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-2.5.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    49344 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-3.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    52336 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-3.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6432 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-4.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8950 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-4.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    13593 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-4.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    17251 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/changelog-4.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    24332 2021-11-21 13:37:38.000000 celery-5.3.0b1/docs/history/changelog-4.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5720 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-5.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5592 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/changelog-5.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      675 2021-11-21 13:37:38.000000 celery-5.3.0b1/docs/history/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    16026 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-2.5.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    30892 2021-11-21 13:37:38.000000 celery-5.3.0b1/docs/history/whatsnew-3.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    44129 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-3.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    76465 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-4.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8244 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-4.1.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    35711 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-4.2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    16865 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-4.3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     6999 2021-11-21 13:37:38.000000 celery-5.3.0b1/docs/history/whatsnew-4.4.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    10957 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/history/whatsnew-5.0.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    13498 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/history/whatsnew-5.1.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.369143 celery-5.3.0b1/docs/images/
--rw-rw-r--   0 asif      (1000) asif      (1000)    14168 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/celery-banner-small.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    14038 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/celery-banner.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     2556 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/celery_128.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     8658 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/celery_512.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    77397 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/celeryevshotsm.jpg
--rw-rw-r--   0 asif      (1000) asif      (1000)    88879 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/dashboard.png
--rw-rw-r--   0 asif      (1000) asif      (1000)     4286 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/favicon.ico
--rw-rw-r--   0 asif      (1000) asif      (1000)   146412 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/monitor.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    35894 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/result_graph.png
--rw-rw-r--   0 asif      (1000) asif      (1000)    99783 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/images/worker_graph_full.png
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.373143 celery-5.3.0b1/docs/includes/
--rw-rw-r--   0 asif      (1000) asif      (1000)     4033 2022-04-28 06:12:03.000000 celery-5.3.0b1/docs/includes/installation.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     6421 2022-08-01 11:14:39.000000 celery-5.3.0b1/docs/includes/introduction.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1377 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/includes/resources.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1613 2021-11-21 13:37:38.000000 celery-5.3.0b1/docs/index.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.377143 celery-5.3.0b1/docs/internals/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5985 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/app-overview.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     5696 2022-04-28 06:12:03.000000 celery-5.3.0b1/docs/internals/deprecation.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8586 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/guide.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     9898 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/protocol.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.393143 celery-5.3.0b1/docs/internals/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery._state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.app.annotations.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.app.routes.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.app.trace.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.arangodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.asynchronous.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.azureblockblob.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      243 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.cache.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.cassandra.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.consul.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      284 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.cosmosdbsql.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.couchbase.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      262 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.couchdb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      276 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.database.models.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.database.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      283 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.database.session.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.dynamodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      280 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.elasticsearch.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      269 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.filesystem.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.mongodb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.redis.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.rpc.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      206 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.backends.s3.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      270 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.eventlet.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.gevent.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      307 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.prefork.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      229 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      310 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.solo.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.concurrency.thread.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.events.cursesmon.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.events.dumper.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.events.snapshot.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      231 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.platforms.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      272 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.security.certificate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.security.key.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      278 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.security.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.security.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.abstract.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.collections.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.deprecated.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      252 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.dispatch.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      295 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.dispatch.signal.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      282 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.functional.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.graph.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.imports.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.iso8601.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.nodenames.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.objects.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      195 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.saferepr.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.serialization.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.sysinfo.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.term.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.text.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      251 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.threads.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.time.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      224 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.utils.timer2.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.autoscale.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      259 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.components.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      260 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      266 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.heartbeat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.loops.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/celery.worker.pidbox.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1960 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/reference/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1452 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/internals/worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     7675 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/make.bat
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.413143 celery-5.3.0b1/docs/reference/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1379 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.amqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.autoretry.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      234 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.backends.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      268 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.builtins.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      265 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.defaults.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      213 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.log.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      228 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.registry.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.task.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      219 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.app.utils.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      253 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.apps.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.apps.multi.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.apps.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      220 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      189 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/reference/celery.bin.amqp.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      216 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      254 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.beat.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.call.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.graph.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      258 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.list.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.logtool.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.migrate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.multi.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.purge.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      264 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.result.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.shell.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      267 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.upgrade.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      242 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bin.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.bootsteps.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      290 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.abortable.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      230 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.migrate.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.pytest.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      256 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.rdb.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      184 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.sphinx.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      288 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.testing.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.testing.manager.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.testing.mocks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.contrib.testing.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      304 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.events.dispatcher.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.events.event.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.events.receiver.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      194 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.events.state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      222 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.exceptions.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      227 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.loaders.app.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      250 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.loaders.base.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.loaders.default.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      237 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.loaders.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      204 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.result.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3497 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      261 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.schedules.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      200 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.security.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      257 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.signals.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      106 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.states.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      871 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.utils.debug.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.agent.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      306 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.connection.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      300 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.consumer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      297 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.control.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.events.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.gossip.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.heart.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.mingle.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      273 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      291 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.consumer.tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      244 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.request.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      236 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.state.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      245 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.strategy.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      239 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/celery.worker.worker.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      143 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/cli.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1952 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/reference/index.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.413143 celery-5.3.0b1/docs/sec/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2921 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/sec/CELERYSA-0001.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     2656 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/sec/CELERYSA-0002.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     1551 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/sec/CELERYSA-0003.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)     4879 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/spelling_wordlist.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.413143 celery-5.3.0b1/docs/templates/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1192 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/templates/readme.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.413143 celery-5.3.0b1/docs/tutorials/
--rw-rw-r--   0 asif      (1000) asif      (1000)       86 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/tutorials/daemonizing.html
--rw-rw-r--   0 asif      (1000) asif      (1000)       91 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/tutorials/debugging.html
--rw-rw-r--   0 asif      (1000) asif      (1000)      121 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/tutorials/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     2766 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/tutorials/task-cookbook.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.421143 celery-5.3.0b1/docs/userguide/
--rw-rw-r--   0 asif      (1000) asif      (1000)    14779 2022-04-28 06:12:03.000000 celery-5.3.0b1/docs/userguide/application.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    23296 2022-03-18 11:40:50.000000 celery-5.3.0b1/docs/userguide/calling.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    34029 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/canvas.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.421143 celery-5.3.0b1/docs/userguide/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2667 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/concurrency/eventlet.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      140 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/concurrency/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    95034 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/configuration.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    17707 2022-04-28 06:12:03.000000 celery-5.3.0b1/docs/userguide/daemonizing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     3131 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/debugging.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    30057 2022-03-18 11:40:50.000000 celery-5.3.0b1/docs/userguide/extending.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      372 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/index.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    21759 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/monitoring.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8437 2021-12-29 05:20:59.000000 celery-5.3.0b1/docs/userguide/optimizing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    20676 2022-03-18 11:40:50.000000 celery-5.3.0b1/docs/userguide/periodic-tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    24316 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/routing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     8693 2022-07-28 12:22:51.000000 celery-5.3.0b1/docs/userguide/security.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    17685 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/signals.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      345 2021-10-12 14:26:47.000000 celery-5.3.0b1/docs/userguide/sphinx.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    64497 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/tasks.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    11107 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/testing.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    32326 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/userguide/workers.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)    12812 2022-08-01 10:53:57.000000 celery-5.3.0b1/docs/whatsnew-5.2.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.421143 celery-5.3.0b1/examples/
--rw-rw-r--   0 asif      (1000) asif      (1000)      303 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/README.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.421143 celery-5.3.0b1/examples/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)      822 2022-06-29 10:52:39.000000 celery-5.3.0b1/examples/app/myapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.421143 celery-5.3.0b1/examples/celery_http_gateway/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1382 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/celery_http_gateway/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/celery_http_gateway/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      385 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/celery_http_gateway/manage.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3001 2021-11-21 13:37:38.000000 celery-5.3.0b1/examples/celery_http_gateway/settings.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       88 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/celery_http_gateway/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      678 2022-03-18 11:40:50.000000 celery-5.3.0b1/examples/celery_http_gateway/urls.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.425144 celery-5.3.0b1/examples/django/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1546 2022-08-01 10:53:57.000000 celery-5.3.0b1/examples/django/README.rst
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.425144 celery-5.3.0b1/examples/django/demoapp/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.425144 celery-5.3.0b1/examples/django/demoapp/migrations/
--rw-rw-r--   0 asif      (1000) asif      (1000)      486 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/migrations/0001_initial.py
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/migrations/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      103 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/models.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      437 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       26 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/demoapp/views.py
--rwxrwxr-x   0 asif      (1000) asif      (1000)      248 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/manage.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.429144 celery-5.3.0b1/examples/django/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)      174 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      659 2022-06-29 10:52:39.000000 celery-5.3.0b1/examples/django/proj/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3639 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/proj/settings.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      556 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/proj/urls.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1132 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/proj/wsgi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       47 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/django/requirements.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.429144 celery-5.3.0b1/examples/eventlet/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1449 2022-04-28 06:12:03.000000 celery-5.3.0b1/examples/eventlet/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)     1673 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/eventlet/bulk_task_producer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      312 2022-04-28 06:12:03.000000 celery-5.3.0b1/examples/eventlet/celeryconfig.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      306 2022-04-28 06:12:03.000000 celery-5.3.0b1/examples/eventlet/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2009 2022-04-28 06:12:03.000000 celery-5.3.0b1/examples/eventlet/webcrawler.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.429144 celery-5.3.0b1/examples/gevent/
--rw-rw-r--   0 asif      (1000) asif      (1000)      255 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/gevent/celeryconfig.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      325 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/gevent/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.429144 celery-5.3.0b1/examples/next-steps/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.429144 celery-5.3.0b1/examples/next-steps/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/next-steps/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      294 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/next-steps/proj/celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      167 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/next-steps/proj/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1224 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/next-steps/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/examples/periodic-tasks/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1518 2022-08-01 10:53:57.000000 celery-5.3.0b1/examples/periodic-tasks/myapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/examples/resultgraph/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2860 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/resultgraph/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/examples/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1058 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/security/mysecureapp.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/examples/security/ssl/
--rw-rw-r--   0 asif      (1000) asif      (1000)     3243 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/security/ssl/worker.key
--rw-rw-r--   0 asif      (1000) asif      (1000)     1923 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/security/ssl/worker.pem
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/examples/tutorial/
--rw-rw-r--   0 asif      (1000) asif      (1000)      158 2021-10-12 14:26:47.000000 celery-5.3.0b1/examples/tutorial/tasks.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.289142 celery-5.3.0b1/extra/
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/extra/bash-completion/
--rw-rw-r--   0 asif      (1000) asif      (1000)      636 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/bash-completion/celery.bash
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/extra/generic-init.d/
--rwxrwxr-x   0 asif      (1000) asif      (1000)     9068 2022-08-01 10:53:57.000000 celery-5.3.0b1/extra/generic-init.d/celerybeat
--rwxrwxr-x   0 asif      (1000) asif      (1000)    10814 2022-08-01 10:53:57.000000 celery-5.3.0b1/extra/generic-init.d/celeryd
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.433144 celery-5.3.0b1/extra/macOS/
--rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/macOS/org.celeryq.beat.plist
--rw-rw-r--   0 asif      (1000) asif      (1000)      757 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/macOS/org.celeryq.worker.plist
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.437144 celery-5.3.0b1/extra/supervisord/
--rw-rw-r--   0 asif      (1000) asif      (1000)      134 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/supervisord/celery.sh
--rw-rw-r--   0 asif      (1000) asif      (1000)      699 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/supervisord/celerybeat.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      949 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/supervisord/celeryd.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      981 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/supervisord/supervisord.conf
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.437144 celery-5.3.0b1/extra/systemd/
--rw-rw-r--   0 asif      (1000) asif      (1000)      506 2022-08-01 10:53:57.000000 celery-5.3.0b1/extra/systemd/celery.conf
--rw-rw-r--   0 asif      (1000) asif      (1000)      740 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/systemd/celery.service
--rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/systemd/celery.tmpfiles
--rw-rw-r--   0 asif      (1000) asif      (1000)      395 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/systemd/celerybeat.service
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.437144 celery-5.3.0b1/extra/zsh-completion/
--rw-rw-r--   0 asif      (1000) asif      (1000)     6244 2021-10-12 14:26:47.000000 celery-5.3.0b1/extra/zsh-completion/celery.zsh
--rw-rw-r--   0 asif      (1000) asif      (1000)      581 2022-04-28 06:12:03.000000 celery-5.3.0b1/pyproject.toml
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.441144 celery-5.3.0b1/requirements/
--rw-rw-r--   0 asif      (1000) asif      (1000)     1454 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/README.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      204 2022-08-01 10:53:57.000000 celery-5.3.0b1/requirements/default.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.441144 celery-5.3.0b1/requirements/deps/
--rw-rw-r--   0 asif      (1000) asif      (1000)       10 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/deps/mock.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      145 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/dev.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      180 2022-07-28 12:22:51.000000 celery-5.3.0b1/requirements/docs.txt
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.449144 celery-5.3.0b1/requirements/extras/
--rw-rw-r--   0 asif      (1000) asif      (1000)       16 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/arangodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       21 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/auth.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/azureblockblob.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      111 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/brotli.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/cassandra.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       22 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/consul.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/cosmosdbsql.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      119 2021-12-29 05:20:59.000000 celery-5.3.0b1/requirements/extras/couchbase.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/couchdb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/django.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/dynamodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-03-18 11:40:50.000000 celery-5.3.0b1/requirements/extras/elasticsearch.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       40 2021-11-21 13:37:38.000000 celery-5.3.0b1/requirements/extras/eventlet.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-11-21 13:37:38.000000 celery-5.3.0b1/requirements/extras/gevent.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/librabbitmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       45 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/memcache.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       20 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/mongodb.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/msgpack.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       23 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/pymemcache.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       12 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/pyro.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       21 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/pytest.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/extras/redis.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       15 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/s3.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/slmq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       53 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/solar.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       27 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/sphinxautobuild.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/sqlalchemy.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/extras/sqs.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       73 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/tblib.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       39 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/thread.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/yaml.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       14 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/zeromq.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       13 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/extras/zookeeper.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2022-07-28 12:22:51.000000 celery-5.3.0b1/requirements/extras/zstd.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      235 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/pkgutils.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       19 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/security.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      191 2022-07-28 12:22:51.000000 celery-5.3.0b1/requirements/test-ci-base.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      539 2022-06-29 10:52:39.000000 celery-5.3.0b1/requirements/test-ci-default.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      157 2022-04-28 06:12:03.000000 celery-5.3.0b1/requirements/test-integration.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)       17 2021-10-12 14:26:47.000000 celery-5.3.0b1/requirements/test-pypy3.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      262 2022-07-28 12:22:51.000000 celery-5.3.0b1/requirements/test.txt
--rw-rw-r--   0 asif      (1000) asif      (1000)      872 2022-08-01 11:20:03.501145 celery-5.3.0b1/setup.cfg
--rwxrwxr-x   0 asif      (1000) asif      (1000)     5068 2022-06-29 10:52:39.000000 celery-5.3.0b1/setup.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.449144 celery-5.3.0b1/t/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.449144 celery-5.3.0b1/t/benchmarks/
--rw-rw-r--   0 asif      (1000) asif      (1000)     2816 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/benchmarks/bench_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.453144 celery-5.3.0b1/t/integration/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/integration/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1904 2022-06-29 11:34:45.000000 celery-5.3.0b1/t/integration/conftest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10538 2022-06-29 11:34:45.000000 celery-5.3.0b1/t/integration/tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1120 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/integration/test_backend.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    97769 2022-07-05 07:04:36.000000 celery-5.3.0b1/t/integration/test_canvas.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7796 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/integration/test_inspect.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3459 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/integration/test_security.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10855 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/integration/test_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      688 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/integration/test_worker.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      293 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/integration/test_worker_config.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      226 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/skip.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.453144 celery-5.3.0b1/t/unit/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.461144 celery-5.3.0b1/t/unit/app/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13761 2022-04-28 06:12:03.000000 celery-5.3.0b1/t/unit/app/test_amqp.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1331 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_annotations.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    39388 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/app/test_app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4542 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_backends.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28783 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/app/test_beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5472 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/app/test_builtins.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      356 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_celery.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    17779 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1594 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/app/test_defaults.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      801 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_exceptions.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8809 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/app/test_loaders.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11799 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/app/test_log.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2342 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_registry.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8019 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_routes.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    30244 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/app/test_schedules.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1790 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/app/test_utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.461144 celery-5.3.0b1/t/unit/apps/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/apps/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    16220 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/apps/test_multi.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.469144 celery-5.3.0b1/t/unit/backends/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4355 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_arangodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6874 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/backends/test_asynchronous.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6780 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_azureblockblob.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    43970 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/backends/test_base.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10305 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/backends/test_cache.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8662 2022-04-28 06:12:03.000000 celery-5.3.0b1/t/unit/backends/test_cassandra.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1441 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_consul.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4987 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_cosmosdbsql.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4839 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_couchbase.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3964 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_couchdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    14877 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/backends/test_database.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    19257 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_dynamodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    32594 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_elasticsearch.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4428 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_filesystem.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    28221 2021-12-29 05:20:59.000000 celery-5.3.0b1/t/unit/backends/test_mongodb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    50581 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/backends/test_redis.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3685 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_rpc.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6654 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/backends/test_s3.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.469144 celery-5.3.0b1/t/unit/bin/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/bin/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       18 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/bin/celery.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.469144 celery-5.3.0b1/t/unit/bin/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)       64 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/bin/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      121 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/bin/proj/app.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       28 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/bin/proj/app2.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      109 2022-07-28 12:22:51.000000 celery-5.3.0b1/t/unit/bin/proj/scheduler.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1116 2022-07-28 12:22:51.000000 celery-5.3.0b1/t/unit/bin/test_beat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/bin/test_multi.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      529 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/bin/test_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.473144 celery-5.3.0b1/t/unit/concurrency/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5577 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_concurrency.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     4636 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_eventlet.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3132 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_gevent.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1830 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_pool.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    15832 2022-04-28 06:12:03.000000 celery-5.3.0b1/t/unit/concurrency/test_prefork.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      848 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_solo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      728 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/concurrency/test_thread.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    23213 2022-06-29 11:34:45.000000 celery-5.3.0b1/t/unit/conftest.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.477144 celery-5.3.0b1/t/unit/contrib/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/__init__.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.477144 celery-5.3.0b1/t/unit/contrib/proj/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/proj/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      183 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/proj/conf.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       93 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/proj/contents.rst
--rw-rw-r--   0 asif      (1000) asif      (1000)      249 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/proj/foo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      113 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/proj/xyzzy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1387 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/test_abortable.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10615 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/contrib/test_migrate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      785 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/test_pytest.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3146 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/test_rdb.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      737 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/contrib/test_sphinx.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1473 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/contrib/test_worker.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.477144 celery-5.3.0b1/t/unit/events/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/events/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2297 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/events/test_cursesmon.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11372 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/events/test_events.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3345 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/events/test_snapshot.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    22260 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/events/test_state.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.481144 celery-5.3.0b1/t/unit/fixups/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/fixups/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10745 2022-07-28 12:22:51.000000 celery-5.3.0b1/t/unit/fixups/test_django.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.481144 celery-5.3.0b1/t/unit/security/
--rw-rw-r--   0 asif      (1000) asif      (1000)     5799 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/security/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      102 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/security/case.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3242 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/security/test_certificate.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1376 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/security/test_key.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6212 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/security/test_security.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2224 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/security/test_serialization.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.485144 celery-5.3.0b1/t/unit/tasks/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/tasks/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    77558 2022-06-29 11:34:45.000000 celery-5.3.0b1/t/unit/tasks/test_canvas.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12494 2022-07-05 07:04:36.000000 celery-5.3.0b1/t/unit/tasks/test_chord.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3134 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/tasks/test_context.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    34939 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/tasks/test_result.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1085 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/tasks/test_states.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    55039 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/tasks/test_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    21964 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/tasks/test_trace.py
--rw-rw-r--   0 asif      (1000) asif      (1000)       78 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/tasks/unit_tasks.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      989 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/test_canvas.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.493145 celery-5.3.0b1/t/unit/utils/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    12840 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_collections.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2357 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_debug.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1737 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_deprecated.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5233 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_dispatcher.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    13582 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_functional.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_graph.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3272 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_imports.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     8161 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_local.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      202 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_nodenames.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      172 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_objects.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1386 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_pickle.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    33131 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_platforms.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     5555 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_saferepr.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3283 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_serialization.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      751 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_sysinfo.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1734 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_term.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     1935 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_text.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2427 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_threads.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    11637 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/utils/test_time.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     3215 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_timer2.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      624 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/utils/test_utils.py
-drwxrwxr-x   0 asif      (1000) asif      (1000)        0 2022-08-01 11:20:03.497145 celery-5.3.0b1/t/unit/worker/
--rw-rw-r--   0 asif      (1000) asif      (1000)        0 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/__init__.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     7567 2021-11-21 13:37:38.000000 celery-5.3.0b1/t/unit/worker/test_autoscale.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     9401 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_bootsteps.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2454 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_components.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    29315 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/worker/test_consumer.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    24534 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_control.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     2384 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_heartbeat.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    18242 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/worker/test_loops.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    47007 2022-03-18 11:40:50.000000 celery-5.3.0b1/t/unit/worker/test_request.py
--rw-rw-r--   0 asif      (1000) asif      (1000)      238 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_revoke.py
--rw-rw-r--   0 asif      (1000) asif      (1000)     6299 2022-08-01 10:53:57.000000 celery-5.3.0b1/t/unit/worker/test_state.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    10968 2021-10-12 14:26:47.000000 celery-5.3.0b1/t/unit/worker/test_strategy.py
--rw-rw-r--   0 asif      (1000) asif      (1000)    39878 2022-06-29 10:52:39.000000 celery-5.3.0b1/t/unit/worker/test_worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.049834 celery-5.3.0b2/
+-rw-r--r--   0 okatz6     (503) staff       (20)     8184 2023-01-09 15:13:51.000000 celery-5.3.0b2/CONTRIBUTORS.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)    11199 2023-01-09 15:13:51.000000 celery-5.3.0b2/Changelog.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     2631 2023-01-09 15:13:51.000000 celery-5.3.0b2/LICENSE
+-rw-r--r--   0 okatz6     (503) staff       (20)      709 2023-01-09 15:13:51.000000 celery-5.3.0b2/MANIFEST.in
+-rw-r--r--   0 okatz6     (503) staff       (20)    17763 2023-02-19 10:26:57.050052 celery-5.3.0b2/PKG-INFO
+-rw-r--r--   0 okatz6     (503) staff       (20)    15613 2023-02-19 10:26:01.000000 celery-5.3.0b2/README.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)       84 2023-01-09 15:13:51.000000 celery-5.3.0b2/TODO
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.710044 celery-5.3.0b2/celery/
+-rw-r--r--   0 okatz6     (503) staff       (20)     5950 2023-02-19 10:26:01.000000 celery-5.3.0b2/celery/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      409 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/__main__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5029 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/_state.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.724234 celery-5.3.0b2/celery/app/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2430 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    23151 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/amqp.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1445 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/annotations.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2489 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/autoretry.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2702 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/backends.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    49215 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/app/base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6673 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/builtins.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    29170 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    15014 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/defaults.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1326 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/events.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     9067 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/log.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2001 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/registry.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4527 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/routes.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    42898 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/app/task.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    28226 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/trace.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    13160 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/app/utils.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.726211 celery-5.3.0b2/celery/apps/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/apps/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5268 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/apps/beat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    16360 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/apps/multi.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    13208 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/apps/worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.736775 celery-5.3.0b2/celery/backends/
+-rw-r--r--   0 okatz6     (503) staff       (20)       23 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7739 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/arangodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10309 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/asynchronous.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5127 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/azureblockblob.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    43964 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/backends/base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4817 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/cache.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     9006 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/cassandra.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3816 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/consul.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6777 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/cosmosdbsql.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3393 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/couchbase.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2935 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/couchdb.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.738236 celery-5.3.0b2/celery/backends/database/
+-rw-r--r--   0 okatz6     (503) staff       (20)     7751 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/database/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3351 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/database/models.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3011 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/database/session.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    17179 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/dynamodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8319 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/elasticsearch.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3776 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/filesystem.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10666 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/mongodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    26389 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/redis.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12077 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/rpc.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2752 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/backends/s3.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    24338 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/beat.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.744801 celery-5.3.0b2/celery/bin/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10023 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/amqp.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8525 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/bin/base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2592 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/beat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2370 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/call.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7317 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/celery.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7058 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2794 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/events.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5796 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/graph.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1058 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/list.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4267 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/logtool.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2108 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/migrate.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    15364 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/multi.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2547 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/purge.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      976 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/result.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4778 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/bin/shell.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3064 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/upgrade.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12869 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bin/worker.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12277 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/bootsteps.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    95874 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/canvas.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.748018 celery-5.3.0b2/celery/concurrency/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1457 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/concurrency/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    51360 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/concurrency/asynpool.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4706 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5126 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/eventlet.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3387 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/gevent.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5850 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/prefork.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      754 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/solo.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1920 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/concurrency/thread.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.750079 celery-5.3.0b2/celery/contrib/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5003 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/abortable.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    14361 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/migrate.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6754 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/contrib/pytest.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5005 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/rdb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3391 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/sphinx.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.751936 celery-5.3.0b2/celery/contrib/testing/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/testing/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3112 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/contrib/testing/app.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7739 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/contrib/testing/manager.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4182 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/contrib/testing/mocks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      208 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/contrib/testing/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5792 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/contrib/testing/worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.754627 celery-5.3.0b2/celery/events/
+-rw-r--r--   0 okatz6     (503) staff       (20)      477 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    17961 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/cursesmon.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8987 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/dispatcher.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3116 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/dumper.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1736 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/event.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4998 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/receiver.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3294 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/events/snapshot.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    25648 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/events/state.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8995 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/exceptions.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.755343 celery-5.3.0b2/celery/fixups/
+-rw-r--r--   0 okatz6     (503) staff       (20)       14 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/fixups/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7161 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/fixups/django.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.756606 celery-5.3.0b2/celery/loaders/
+-rw-r--r--   0 okatz6     (503) staff       (20)      490 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/loaders/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      199 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/loaders/app.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8825 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/loaders/base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1520 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/loaders/default.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    16087 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/local.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    25290 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/platforms.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    35305 2023-01-09 15:13:51.000000 celery-5.3.0b2/celery/result.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    30339 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/schedules.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.758487 celery-5.3.0b2/celery/security/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2363 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/security/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3205 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/security/certificate.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1189 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/security/key.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4248 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/security/serialization.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      845 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/security/utils.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4273 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/signals.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3324 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/states.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.767775 celery-5.3.0b2/celery/utils/
+-rw-r--r--   0 okatz6     (503) staff       (20)      935 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2874 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/abstract.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    25427 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/utils/collections.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4709 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/debug.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3620 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/deprecated.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.768811 celery-5.3.0b2/celery/utils/dispatch/
+-rw-r--r--   0 okatz6     (503) staff       (20)       74 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/dispatch/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    13603 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/dispatch/signal.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12017 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/functional.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     9041 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/graph.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5032 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/imports.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2776 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/iso8601.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8757 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/utils/log.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2858 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/nodenames.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4215 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/objects.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8945 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/utils/saferepr.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8043 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/serialization.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.770012 celery-5.3.0b2/celery/utils/static/
+-rw-r--r--   0 okatz6     (503) staff       (20)      299 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/static/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2556 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/static/celery_128.png
+-rw-r--r--   0 okatz6     (503) staff       (20)     1085 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/sysinfo.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4532 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/term.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5824 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/utils/text.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     9552 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/threads.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12437 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/utils/time.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4813 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/utils/timer2.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.775920 celery-5.3.0b2/celery/worker/
+-rw-r--r--   0 okatz6     (503) staff       (20)       95 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4593 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/autoscale.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7497 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/components.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.780394 celery-5.3.0b2/celery/worker/consumer/
+-rw-r--r--   0 okatz6     (503) staff       (20)      391 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      525 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/agent.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1026 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/connection.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    28320 2023-02-19 10:24:09.000000 celery-5.3.0b2/celery/worker/consumer/consumer.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      946 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2054 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/events.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6833 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/gossip.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      930 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/heart.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2519 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/mingle.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1960 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/consumer/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    18945 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2107 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/heartbeat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4433 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/loops.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3630 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/pidbox.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    27031 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/request.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8585 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/state.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7349 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/strategy.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    14460 2023-01-09 15:13:52.000000 celery-5.3.0b2/celery/worker/worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.712712 celery-5.3.0b2/celery.egg-info/
+-rw-r--r--   0 okatz6     (503) staff       (20)    17763 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/PKG-INFO
+-rw-r--r--   0 okatz6     (503) staff       (20)    21159 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/SOURCES.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)        1 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/dependency_links.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       48 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/entry_points.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)        1 2023-01-09 15:22:00.000000 celery-5.3.0b2/celery.egg-info/not-zip-safe
+-rw-r--r--   0 okatz6     (503) staff       (20)     1546 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/requires.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)        7 2023-02-19 10:26:56.000000 celery-5.3.0b2/celery.egg-info/top_level.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.787354 celery-5.3.0b2/docs/
+-rw-r--r--   0 okatz6     (503) staff       (20)     5293 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/AUTHORS.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     8111 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/Makefile
+-rw-r--r--   0 okatz6     (503) staff       (20)      494 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/THANKS
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.787937 celery-5.3.0b2/docs/_ext/
+-rw-r--r--   0 okatz6     (503) staff       (20)     5164 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/_ext/celerydocs.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.788322 celery-5.3.0b2/docs/_static/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/_static/.keep
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.788547 celery-5.3.0b2/docs/_templates/
+-rw-r--r--   0 okatz6     (503) staff       (20)      486 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/_templates/sidebardonations.html
+-rw-r--r--   0 okatz6     (503) staff       (20)       30 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/changelog.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      981 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/community.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     2597 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/conf.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       83 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/configuration.html
+-rw-r--r--   0 okatz6     (503) staff       (20)       33 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/contributing.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      931 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/copyright.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.789359 celery-5.3.0b2/docs/django/
+-rw-r--r--   0 okatz6     (503) staff       (20)     7886 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/django/first-steps-with-django.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      137 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/django/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    29934 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/faq.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.791610 celery-5.3.0b2/docs/getting-started/
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.793057 celery-5.3.0b2/docs/getting-started/backends-and-brokers/
+-rw-r--r--   0 okatz6     (503) staff       (20)     3950 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/backends-and-brokers/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     5010 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/getting-started/backends-and-brokers/rabbitmq.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     7239 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/getting-started/backends-and-brokers/redis.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    10843 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/backends-and-brokers/sqs.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    14995 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/first-steps-with-celery.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      226 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    10903 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/introduction.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    22787 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/next-steps.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      132 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/getting-started/resources.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     4448 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/glossary.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.807921 celery-5.3.0b2/docs/history/
+-rw-r--r--   0 okatz6     (503) staff       (20)    58104 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-1.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    34009 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    23550 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    33558 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.2.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    11200 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.3.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    13012 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.4.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     5414 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-2.5.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    49344 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-3.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    52336 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-3.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     6432 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-4.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     8950 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-4.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    13593 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-4.2.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    17251 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-4.3.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    24332 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-4.4.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     5720 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-5.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     5592 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/changelog-5.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      675 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    16026 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-2.5.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    30892 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-3.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    44129 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-3.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    76466 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-4.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     8244 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-4.1.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    35711 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-4.2.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    16865 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-4.3.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     6999 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-4.4.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    10957 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-5.0.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    14128 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/history/whatsnew-5.1.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.814725 celery-5.3.0b2/docs/images/
+-rw-r--r--   0 okatz6     (503) staff       (20)    14168 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/celery-banner-small.png
+-rw-r--r--   0 okatz6     (503) staff       (20)    14038 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/celery-banner.png
+-rw-r--r--   0 okatz6     (503) staff       (20)     2556 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/celery_128.png
+-rw-r--r--   0 okatz6     (503) staff       (20)     8658 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/celery_512.png
+-rw-r--r--   0 okatz6     (503) staff       (20)    77397 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/celeryevshotsm.jpg
+-rw-r--r--   0 okatz6     (503) staff       (20)    88879 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/dashboard.png
+-rw-r--r--   0 okatz6     (503) staff       (20)     4286 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/favicon.ico
+-rw-r--r--   0 okatz6     (503) staff       (20)   146412 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/monitor.png
+-rw-r--r--   0 okatz6     (503) staff       (20)    35894 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/result_graph.png
+-rw-r--r--   0 okatz6     (503) staff       (20)    99783 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/images/worker_graph_full.png
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.817245 celery-5.3.0b2/docs/includes/
+-rw-r--r--   0 okatz6     (503) staff       (20)     4023 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/includes/installation.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     6421 2023-02-19 10:26:01.000000 celery-5.3.0b2/docs/includes/introduction.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     1375 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/includes/resources.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     1613 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/index.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.820295 celery-5.3.0b2/docs/internals/
+-rw-r--r--   0 okatz6     (503) staff       (20)     5985 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/app-overview.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     5696 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/deprecation.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     8586 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/guide.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      206 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     9898 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/protocol.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.858363 celery-5.3.0b2/docs/internals/reference/
+-rw-r--r--   0 okatz6     (503) staff       (20)      226 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery._state.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      257 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.app.annotations.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      224 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.app.routes.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      239 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.app.trace.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.arangodb.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.asynchronous.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      293 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.azureblockblob.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      243 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.base.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      256 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.cache.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      278 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.cassandra.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      253 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.consul.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      284 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.cosmosdbsql.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      270 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.couchbase.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      262 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.couchdb.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      276 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.database.models.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      293 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.database.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      283 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.database.session.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      265 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.dynamodb.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      280 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.elasticsearch.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      269 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.filesystem.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      264 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.mongodb.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      254 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.redis.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      242 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.rpc.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      206 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      245 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.backends.s3.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      270 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.base.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      310 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.eventlet.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      304 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.gevent.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      307 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.prefork.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      229 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      310 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.solo.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      304 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.concurrency.thread.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      260 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.events.cursesmon.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      251 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.events.dumper.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      257 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.events.snapshot.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      231 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.platforms.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      272 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.security.certificate.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      248 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.security.key.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      278 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.security.serialization.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      254 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.security.utils.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      256 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.abstract.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      252 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.collections.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      260 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.deprecated.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      252 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.dispatch.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      295 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.dispatch.signal.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      282 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.functional.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      245 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.graph.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      273 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.imports.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.iso8601.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      261 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.log.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      257 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.nodenames.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.objects.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      195 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      256 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.saferepr.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      273 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.serialization.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.sysinfo.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      264 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.term.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      264 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.text.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      251 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.threads.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      258 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.time.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      224 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.utils.timer2.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      256 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.autoscale.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      259 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.components.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      260 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.control.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      266 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.heartbeat.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      236 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.loops.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      239 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/celery.worker.pidbox.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     1960 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/reference/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     1452 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/internals/worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     7675 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/make.bat
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.917998 celery-5.3.0b2/docs/reference/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1379 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.amqp.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      237 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.autoretry.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      234 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.backends.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      268 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.builtins.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      265 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.control.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      290 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.defaults.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      222 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.events.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      213 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.log.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      228 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.registry.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      288 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      226 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.task.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      219 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.app.utils.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      253 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.apps.beat.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      236 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.apps.multi.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      239 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.apps.worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      220 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.beat.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      189 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.amqp.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      216 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.base.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      254 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.beat.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      258 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.call.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      242 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.celery.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.control.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      264 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.events.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      261 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.graph.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      258 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.list.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.logtool.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.migrate.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      249 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.multi.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      261 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.purge.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      264 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.result.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      261 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.shell.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      267 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.upgrade.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      242 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bin.worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      239 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.bootsteps.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      290 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.abortable.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      230 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.migrate.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      273 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.pytest.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      256 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.rdb.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      184 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.sphinx.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      288 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.testing.app.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      300 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.testing.manager.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.testing.mocks.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      297 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.contrib.testing.worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      304 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.events.dispatcher.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.events.event.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      303 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.events.receiver.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      194 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.events.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.events.state.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      222 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.exceptions.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      227 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.loaders.app.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      250 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.loaders.base.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      255 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.loaders.default.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      237 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.loaders.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      204 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.result.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     3497 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      261 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.schedules.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      200 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.security.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      257 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.signals.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      106 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.states.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      871 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.utils.debug.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      291 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.agent.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      306 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.connection.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      300 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.consumer.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      297 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.control.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.events.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.gossip.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      291 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.heart.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.mingle.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      273 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      291 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.consumer.tasks.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      244 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.request.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      226 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      236 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.state.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      245 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.strategy.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      239 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/celery.worker.worker.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      143 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/cli.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     1952 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/reference/index.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.920123 celery-5.3.0b2/docs/sec/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2921 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/sec/CELERYSA-0001.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     2656 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/sec/CELERYSA-0002.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     1551 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/sec/CELERYSA-0003.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)     4879 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/spelling_wordlist.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.920884 celery-5.3.0b2/docs/templates/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1186 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/templates/readme.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.923510 celery-5.3.0b2/docs/tutorials/
+-rw-r--r--   0 okatz6     (503) staff       (20)       86 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/tutorials/daemonizing.html
+-rw-r--r--   0 okatz6     (503) staff       (20)       91 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/tutorials/debugging.html
+-rw-r--r--   0 okatz6     (503) staff       (20)      121 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/tutorials/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     2766 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/tutorials/task-cookbook.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.934984 celery-5.3.0b2/docs/userguide/
+-rw-r--r--   0 okatz6     (503) staff       (20)    14779 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/application.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    25233 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/userguide/calling.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    39349 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/userguide/canvas.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.936008 celery-5.3.0b2/docs/userguide/concurrency/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2665 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/concurrency/eventlet.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      140 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/concurrency/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    98220 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/userguide/configuration.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    17699 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/daemonizing.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     3131 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/debugging.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    30057 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/extending.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      372 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/index.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    21759 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/userguide/monitoring.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     8437 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/optimizing.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    20676 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/periodic-tasks.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    24323 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/routing.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     8693 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/security.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    17685 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/signals.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      345 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/sphinx.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    64543 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/tasks.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    11146 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/userguide/testing.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    34758 2023-02-19 10:24:09.000000 celery-5.3.0b2/docs/userguide/workers.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)    12812 2023-01-09 15:13:52.000000 celery-5.3.0b2/docs/whatsnew-5.2.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.936520 celery-5.3.0b2/examples/
+-rw-r--r--   0 okatz6     (503) staff       (20)      303 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/README.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.936860 celery-5.3.0b2/examples/app/
+-rw-r--r--   0 okatz6     (503) staff       (20)      822 2023-02-19 10:24:16.000000 celery-5.3.0b2/examples/app/myapp.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.938728 celery-5.3.0b2/examples/celery_http_gateway/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1382 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/celery_http_gateway/README.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/celery_http_gateway/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      385 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/celery_http_gateway/manage.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3001 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/celery_http_gateway/settings.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       88 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/celery_http_gateway/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      678 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/celery_http_gateway/urls.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.939825 celery-5.3.0b2/examples/django/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1546 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/README.rst
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.941087 celery-5.3.0b2/examples/django/demoapp/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/__init__.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.941678 celery-5.3.0b2/examples/django/demoapp/migrations/
+-rw-r--r--   0 okatz6     (503) staff       (20)      486 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/migrations/0001_initial.py
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/migrations/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      103 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/models.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      437 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       26 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/demoapp/views.py
+-rwxr-xr-x   0 okatz6     (503) staff       (20)      248 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/manage.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.943972 celery-5.3.0b2/examples/django/proj/
+-rw-r--r--   0 okatz6     (503) staff       (20)      174 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/proj/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      659 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/proj/celery.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3639 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/proj/settings.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      556 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/django/proj/urls.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1132 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/proj/wsgi.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       47 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/django/requirements.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.945462 celery-5.3.0b2/examples/eventlet/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1449 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/eventlet/README.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)     1673 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/eventlet/bulk_task_producer.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      312 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/eventlet/celeryconfig.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      306 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/eventlet/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2009 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/eventlet/webcrawler.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.946071 celery-5.3.0b2/examples/gevent/
+-rw-r--r--   0 okatz6     (503) staff       (20)      255 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/gevent/celeryconfig.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      325 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/gevent/tasks.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.946368 celery-5.3.0b2/examples/next-steps/
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.947165 celery-5.3.0b2/examples/next-steps/proj/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/next-steps/proj/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      294 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/next-steps/proj/celery.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      167 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/next-steps/proj/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1224 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/next-steps/setup.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.947451 celery-5.3.0b2/examples/periodic-tasks/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1518 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/periodic-tasks/myapp.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.947737 celery-5.3.0b2/examples/resultgraph/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2860 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/resultgraph/tasks.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.948059 celery-5.3.0b2/examples/security/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1058 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/security/mysecureapp.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.948728 celery-5.3.0b2/examples/security/ssl/
+-rw-r--r--   0 okatz6     (503) staff       (20)     3243 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/security/ssl/worker.key
+-rw-r--r--   0 okatz6     (503) staff       (20)     1923 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/security/ssl/worker.pem
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.950731 celery-5.3.0b2/examples/stamping/
+-rw-r--r--   0 okatz6     (503) staff       (20)      103 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/stamping/config.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1358 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/stamping/examples.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1806 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/stamping/myapp.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2548 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/stamping/revoke_example.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3311 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/stamping/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2410 2023-02-19 10:24:09.000000 celery-5.3.0b2/examples/stamping/visitors.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.951037 celery-5.3.0b2/examples/tutorial/
+-rw-r--r--   0 okatz6     (503) staff       (20)      158 2023-01-09 15:13:52.000000 celery-5.3.0b2/examples/tutorial/tasks.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.694257 celery-5.3.0b2/extra/
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.951388 celery-5.3.0b2/extra/bash-completion/
+-rw-r--r--   0 okatz6     (503) staff       (20)      636 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/bash-completion/celery.bash
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.952010 celery-5.3.0b2/extra/generic-init.d/
+-rwxr-xr-x   0 okatz6     (503) staff       (20)     9068 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/generic-init.d/celerybeat
+-rwxr-xr-x   0 okatz6     (503) staff       (20)    10813 2023-02-19 10:24:09.000000 celery-5.3.0b2/extra/generic-init.d/celeryd
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.952617 celery-5.3.0b2/extra/macOS/
+-rw-r--r--   0 okatz6     (503) staff       (20)      751 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/macOS/org.celeryq.beat.plist
+-rw-r--r--   0 okatz6     (503) staff       (20)      757 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/macOS/org.celeryq.worker.plist
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.953854 celery-5.3.0b2/extra/supervisord/
+-rw-r--r--   0 okatz6     (503) staff       (20)      134 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/supervisord/celery.sh
+-rw-r--r--   0 okatz6     (503) staff       (20)      699 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/supervisord/celerybeat.conf
+-rw-r--r--   0 okatz6     (503) staff       (20)      949 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/supervisord/celeryd.conf
+-rw-r--r--   0 okatz6     (503) staff       (20)      982 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/supervisord/supervisord.conf
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.955121 celery-5.3.0b2/extra/systemd/
+-rw-r--r--   0 okatz6     (503) staff       (20)      506 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/systemd/celery.conf
+-rw-r--r--   0 okatz6     (503) staff       (20)      740 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/systemd/celery.service
+-rw-r--r--   0 okatz6     (503) staff       (20)       78 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/systemd/celery.tmpfiles
+-rw-r--r--   0 okatz6     (503) staff       (20)      395 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/systemd/celerybeat.service
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.955473 celery-5.3.0b2/extra/zsh-completion/
+-rw-r--r--   0 okatz6     (503) staff       (20)     6244 2023-01-09 15:13:52.000000 celery-5.3.0b2/extra/zsh-completion/celery.zsh
+-rw-r--r--   0 okatz6     (503) staff       (20)     1095 2023-01-09 15:13:52.000000 celery-5.3.0b2/pyproject.toml
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.959326 celery-5.3.0b2/requirements/
+-rw-r--r--   0 okatz6     (503) staff       (20)     1454 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/README.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      200 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/default.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.959628 celery-5.3.0b2/requirements/deps/
+-rw-r--r--   0 okatz6     (503) staff       (20)       10 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/deps/mock.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      156 2023-02-19 10:24:09.000000 celery-5.3.0b2/requirements/dev.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      187 2023-02-19 10:24:09.000000 celery-5.3.0b2/requirements/docs.txt
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.973034 celery-5.3.0b2/requirements/extras/
+-rw-r--r--   0 okatz6     (503) staff       (20)       16 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/arangodb.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       21 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/auth.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       28 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/azureblockblob.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      111 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/brotli.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       28 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/cassandra.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       22 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/consul.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       20 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/cosmosdbsql.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      119 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/couchbase.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       18 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/couchdb.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       13 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/django.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       14 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/dynamodb.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       18 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/elasticsearch.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       40 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/eventlet.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       14 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/gevent.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       19 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/librabbitmq.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       45 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/memcache.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       20 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/mongodb.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       15 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/msgpack.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       23 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/pymemcache.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       12 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/pyro.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       21 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/pytest.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       20 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/redis.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       15 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/s3.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       27 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/slmq.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       53 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/solar.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       27 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/sphinxautobuild.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       19 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/sqlalchemy.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       18 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/sqs.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       73 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/tblib.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       39 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/thread.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       13 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/yaml.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       14 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/zeromq.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       13 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/zookeeper.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       18 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/extras/zstd.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      235 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/pkgutils.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       19 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/security.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      191 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/test-ci-base.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      539 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/test-ci-default.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      157 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/test-integration.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)       17 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/test-pypy3.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      304 2023-01-09 15:13:52.000000 celery-5.3.0b2/requirements/test.txt
+-rw-r--r--   0 okatz6     (503) staff       (20)      437 2023-02-19 10:26:57.050648 celery-5.3.0b2/setup.cfg
+-rwxr-xr-x   0 okatz6     (503) staff       (20)     5077 2023-01-09 15:13:52.000000 celery-5.3.0b2/setup.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.977452 celery-5.3.0b2/t/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/__init__.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.978154 celery-5.3.0b2/t/benchmarks/
+-rw-r--r--   0 okatz6     (503) staff       (20)     2816 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/benchmarks/bench_worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.984106 celery-5.3.0b2/t/integration/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2350 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/conftest.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    11549 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1120 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_backend.py
+-rw-r--r--   0 okatz6     (503) staff       (20)   131273 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/integration/test_canvas.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7796 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_inspect.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3459 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_security.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    16106 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      688 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_worker.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      293 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/integration/test_worker_config.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      226 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/skip.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.985755 celery-5.3.0b2/t/unit/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/__init__.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.996006 celery-5.3.0b2/t/unit/app/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    13768 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_amqp.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1338 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_annotations.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    40027 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/app/test_app.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4542 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_backends.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    28873 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/app/test_beat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5528 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_builtins.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      356 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_celery.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    19105 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1608 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_defaults.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      801 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_exceptions.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8823 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_loaders.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    11820 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_log.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2349 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_registry.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8026 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_routes.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    37785 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/app/test_schedules.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1790 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/app/test_utils.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:56.996744 celery-5.3.0b2/t/unit/apps/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/apps/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    16234 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/apps/test_multi.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.007459 celery-5.3.0b2/t/unit/backends/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4362 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_arangodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6874 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_asynchronous.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6794 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_azureblockblob.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    45439 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/backends/test_base.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10318 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_cache.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8669 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_cassandra.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1448 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_consul.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4994 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_cosmosdbsql.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4846 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_couchbase.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3971 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_couchdb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    14891 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/backends/test_database.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    19214 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_dynamodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    32601 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_elasticsearch.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4435 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_filesystem.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    28228 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_mongodb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    50595 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_redis.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3692 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_rpc.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6654 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/backends/test_s3.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.009229 celery-5.3.0b2/t/unit/bin/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       18 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/celery.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.011108 celery-5.3.0b2/t/unit/bin/proj/
+-rw-r--r--   0 okatz6     (503) staff       (20)       64 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/proj/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      121 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/proj/app.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       22 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/bin/proj/app2.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      109 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/proj/scheduler.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1116 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/test_beat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/test_multi.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      529 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/bin/test_worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.015542 celery-5.3.0b2/t/unit/concurrency/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5687 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_concurrency.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     4721 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/concurrency/test_eventlet.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3146 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_gevent.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1837 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_pool.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    15846 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_prefork.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      848 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_solo.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      728 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/concurrency/test_thread.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    23214 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/conftest.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.019628 celery-5.3.0b2/t/unit/contrib/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/__init__.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.022588 celery-5.3.0b2/t/unit/contrib/proj/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/proj/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      183 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/proj/conf.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       93 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/proj/contents.rst
+-rw-r--r--   0 okatz6     (503) staff       (20)      249 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/contrib/proj/foo.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      113 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/proj/xyzzy.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1394 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/test_abortable.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10615 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/test_migrate.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      785 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/test_pytest.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3146 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/contrib/test_rdb.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      731 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/contrib/test_sphinx.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1474 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/contrib/test_worker.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.025614 celery-5.3.0b2/t/unit/events/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/events/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2304 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/events/test_cursesmon.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    11372 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/events/test_events.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3359 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/events/test_snapshot.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    22261 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/events/test_state.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.026704 celery-5.3.0b2/t/unit/fixups/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/fixups/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    11013 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/fixups/test_django.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.029493 celery-5.3.0b2/t/unit/security/
+-rw-r--r--   0 okatz6     (503) staff       (20)     7344 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      109 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/case.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3333 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/test_certificate.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1570 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/test_key.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6219 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/test_security.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2224 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/security/test_serialization.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.035244 celery-5.3.0b2/t/unit/tasks/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/tasks/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    68472 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/tasks/test_canvas.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12308 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/tasks/test_chord.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3134 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/tasks/test_context.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    34984 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/tasks/test_result.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    51828 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/tasks/test_stamping.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1085 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/tasks/test_states.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    55713 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/tasks/test_tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    21991 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/tasks/test_trace.py
+-rw-r--r--   0 okatz6     (503) staff       (20)       78 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/tasks/unit_tasks.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      989 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/test_canvas.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.044284 celery-5.3.0b2/t/unit/utils/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    12855 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_collections.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2357 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_debug.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1739 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_deprecated.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5233 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_dispatcher.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    13576 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/utils/test_functional.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1935 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_graph.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3272 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_imports.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     8515 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_local.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      202 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_nodenames.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      172 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_objects.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1386 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_pickle.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    32949 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_platforms.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     5555 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_saferepr.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3108 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_serialization.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      751 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_sysinfo.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1734 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_term.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     1935 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_text.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2427 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_threads.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    11637 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_time.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     3215 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_timer2.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      624 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/utils/test_utils.py
+drwxr-xr-x   0 okatz6     (503) staff       (20)        0 2023-02-19 10:26:57.049072 celery-5.3.0b2/t/unit/worker/
+-rw-r--r--   0 okatz6     (503) staff       (20)        0 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/__init__.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     7574 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_autoscale.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     9415 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_bootsteps.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2461 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_components.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    30428 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/worker/test_consumer.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    25333 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_control.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     2384 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_heartbeat.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    18256 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_loops.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    47040 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_request.py
+-rw-r--r--   0 okatz6     (503) staff       (20)      238 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_revoke.py
+-rw-r--r--   0 okatz6     (503) staff       (20)     6340 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_state.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    10989 2023-01-09 15:13:52.000000 celery-5.3.0b2/t/unit/worker/test_strategy.py
+-rw-r--r--   0 okatz6     (503) staff       (20)    39912 2023-02-19 10:24:09.000000 celery-5.3.0b2/t/unit/worker/test_worker.py
```

### Comparing `celery-5.3.0b1/CONTRIBUTORS.txt` & `celery-5.3.0b2/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -286,7 +286,9 @@
 Patrick Zhang, 2017/08/19
 Konstantin Kochin, 2021/07/11
 kronion, 2021/08/26
 Gabor Boros, 2021/11/09
 Tizian Seehaus, 2022/02/09
 Oleh Romanovskyi, 2022/06/09
 JoonHwan Kim, 2022/08/01
+Kaustav Banerjee, 2022/11/10
+Austin Snoeyink 2022/12/06
```

### Comparing `celery-5.3.0b1/Changelog.rst` & `celery-5.3.0b2/Changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _changelog:
 
 ================
  Change history
 ================
 
 This document contains change notes for bugfix & new features
-in the master branch & 5.2.x series, please see :ref:`whatsnew-5.2` for
+in the main branch & 5.2.x series, please see :ref:`whatsnew-5.2` for
 an overview of what's new in Celery 5.2.
 
 .. _version-5.3.0b1:
 
 5.3.0b1
 =======
 
@@ -46,15 +46,15 @@
 - Limit elasticsearch support to below version 8.0.
 - try new major release of pytest 7 (#7330).
 - broker_connection_retry should no longer apply on startup (#7300).
 - Remove __ne__ methods (#7257).
 - fix #7200 uid and gid.
 - Remove exception-throwing from the signal handler.
 - Add mypy to the pipeline (#7383).
-- Expose more debugging information when receiving unkown tasks. (#7405)
+- Expose more debugging information when receiving unknown tasks. (#7405)
 - Avoid importing buf_t from billiard's compat module as it was removed.
 - Avoid negating a constant in a loop. (#7443)
 - Ensure expiration is of float type when migrating tasks (#7385).
 - load_extension_class_names - correct module_name (#7406)
 - Bump pymongo[srv]>=4.0.2.
 - Use inspect.getgeneratorstate in asynpool.gen_not_started (#7476).
 - Fix test with missing .get() (#7479).
```

### Comparing `celery-5.3.0b1/LICENSE` & `celery-5.3.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/MANIFEST.in` & `celery-5.3.0b2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/PKG-INFO` & `celery-5.3.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0b1
+Version: 5.3.0b2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
-License: BSD
+License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
 Project-URL: Code, https://github.com/celery/celery
 Project-URL: Tracker, https://github.com/celery/celery/issues
 Project-URL: Funding, https://opencollective.com/celery
 Keywords: task job queue distributed messaging actor
 Platform: any
@@ -25,52 +25,52 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Provides-Extra: auth
-Provides-Extra: pyro
-Provides-Extra: solar
-Provides-Extra: cosmosdbsql
-Provides-Extra: sqs
-Provides-Extra: tblib
-Provides-Extra: brotli
-Provides-Extra: yaml
-Provides-Extra: pymemcache
-Provides-Extra: consul
-Provides-Extra: slmq
+Provides-Extra: eventlet
+Provides-Extra: memcache
 Provides-Extra: gevent
-Provides-Extra: s3
-Provides-Extra: arangodb
-Provides-Extra: couchbase
-Provides-Extra: couchdb
-Provides-Extra: sqlalchemy
-Provides-Extra: pytest
 Provides-Extra: mongodb
 Provides-Extra: redis
-Provides-Extra: elasticsearch
-Provides-Extra: zstd
-Provides-Extra: msgpack
+Provides-Extra: sqs
+Provides-Extra: auth
 Provides-Extra: cassandra
-Provides-Extra: memcache
-Provides-Extra: azureblockblob
+Provides-Extra: brotli
+Provides-Extra: s3
+Provides-Extra: couchbase
+Provides-Extra: pyro
+Provides-Extra: slmq
+Provides-Extra: cosmosdbsql
+Provides-Extra: arangodb
 Provides-Extra: zookeeper
+Provides-Extra: pytest
+Provides-Extra: solar
 Provides-Extra: librabbitmq
-Provides-Extra: eventlet
+Provides-Extra: azureblockblob
+Provides-Extra: pymemcache
+Provides-Extra: yaml
 Provides-Extra: django
+Provides-Extra: elasticsearch
 Provides-Extra: dynamodb
+Provides-Extra: zstd
+Provides-Extra: consul
+Provides-Extra: sqlalchemy
+Provides-Extra: couchdb
+Provides-Extra: tblib
+Provides-Extra: msgpack
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0b1 (dawn-chorus)
+:Version: 5.3.0b2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -128,19 +128,19 @@
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.6: Celery 5.1 or earlier.
+- Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
-- Python 2.7: Celery 4.x series.
-- Python 3.6: Celery 5.1 or earlier.
 
 Celery is a project with minimal funding,
 so we don't support Microsoft Windows.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
@@ -451,19 +451,19 @@
 
 You can install the latest snapshot of these using the following
 pip commands:
 
 ::
 
 
-    $ pip install https://github.com/celery/celery/zipball/master#egg=celery
-    $ pip install https://github.com/celery/billiard/zipball/master#egg=billiard
-    $ pip install https://github.com/celery/py-amqp/zipball/master#egg=amqp
-    $ pip install https://github.com/celery/kombu/zipball/master#egg=kombu
-    $ pip install https://github.com/celery/vine/zipball/master#egg=vine
+    $ pip install https://github.com/celery/celery/zipball/main#egg=celery
+    $ pip install https://github.com/celery/billiard/zipball/main#egg=billiard
+    $ pip install https://github.com/celery/py-amqp/zipball/main#egg=amqp
+    $ pip install https://github.com/celery/kombu/zipball/main#egg=kombu
+    $ pip install https://github.com/celery/vine/zipball/main#egg=vine
 
 With git
 ~~~~~~~~
 
 Please see the Contributing section.
 
 .. _getting-help:
@@ -521,15 +521,15 @@
 of `celery`. If you don't like GitHub (for some reason) you're welcome
 to send regular patches.
 
 Be sure to also read the `Contributing to Celery`_ section in the
 documentation.
 
 .. _`Contributing to Celery`:
-    https://docs.celeryq.dev/en/master/contributing.html
+    https://docs.celeryq.dev/en/main/contributing.html
 
 |oc-contributors|
 
 .. |oc-contributors| image:: https://opencollective.com/celery/contributors.svg?width=890&button=false
     :target: https://github.com/celery/celery/graphs/contributors
 
 Backers
@@ -567,16 +567,16 @@
 
 .. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
 
 .. |build-status| image:: https://github.com/celery/celery/actions/workflows/python-package.yml/badge.svg
     :alt: Build status
     :target: https://github.com/celery/celery/actions/workflows/python-package.yml
 
-.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/celery?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/celery?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/celery.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
     :alt: Celery can be installed via wheel
```

### Comparing `celery-5.3.0b1/README.rst` & `celery-5.3.0b2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0b1 (dawn-chorus)
+:Version: 5.3.0b2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -64,19 +64,19 @@
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.6: Celery 5.1 or earlier.
+- Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
-- Python 2.7: Celery 4.x series.
-- Python 3.6: Celery 5.1 or earlier.
 
 Celery is a project with minimal funding,
 so we don't support Microsoft Windows.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
@@ -387,19 +387,19 @@
 
 You can install the latest snapshot of these using the following
 pip commands:
 
 ::
 
 
-    $ pip install https://github.com/celery/celery/zipball/master#egg=celery
-    $ pip install https://github.com/celery/billiard/zipball/master#egg=billiard
-    $ pip install https://github.com/celery/py-amqp/zipball/master#egg=amqp
-    $ pip install https://github.com/celery/kombu/zipball/master#egg=kombu
-    $ pip install https://github.com/celery/vine/zipball/master#egg=vine
+    $ pip install https://github.com/celery/celery/zipball/main#egg=celery
+    $ pip install https://github.com/celery/billiard/zipball/main#egg=billiard
+    $ pip install https://github.com/celery/py-amqp/zipball/main#egg=amqp
+    $ pip install https://github.com/celery/kombu/zipball/main#egg=kombu
+    $ pip install https://github.com/celery/vine/zipball/main#egg=vine
 
 With git
 ~~~~~~~~
 
 Please see the Contributing section.
 
 .. _getting-help:
@@ -457,15 +457,15 @@
 of `celery`. If you don't like GitHub (for some reason) you're welcome
 to send regular patches.
 
 Be sure to also read the `Contributing to Celery`_ section in the
 documentation.
 
 .. _`Contributing to Celery`:
-    https://docs.celeryq.dev/en/master/contributing.html
+    https://docs.celeryq.dev/en/main/contributing.html
 
 |oc-contributors|
 
 .. |oc-contributors| image:: https://opencollective.com/celery/contributors.svg?width=890&button=false
     :target: https://github.com/celery/celery/graphs/contributors
 
 Backers
@@ -503,16 +503,16 @@
 
 .. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
 
 .. |build-status| image:: https://github.com/celery/celery/actions/workflows/python-package.yml/badge.svg
     :alt: Build status
     :target: https://github.com/celery/celery/actions/workflows/python-package.yml
 
-.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/celery?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/celery?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/celery.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
     :alt: Celery can be installed via wheel
```

### Comparing `celery-5.3.0b1/celery/__init__.py` & `celery-5.3.0b2/celery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from collections import namedtuple
 
 # Lazy loading
 from . import local
 
 SERIES = 'dawn-chorus'
 
-__version__ = '5.3.0b1'
+__version__ = '5.3.0b2'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://docs.celeryq.dev/'
 __docformat__ = 'restructuredtext'
 __keywords__ = 'task job queue distributed messaging actor'
 
 # -eof meta-
```

### Comparing `celery-5.3.0b1/celery/_state.py` & `celery-5.3.0b2/celery/_state.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/__init__.py` & `celery-5.3.0b2/celery/app/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/amqp.py` & `celery-5.3.0b2/celery/app/amqp.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             argsrepr = saferepr(args, self.argsrepr_maxsize)
         if kwargsrepr is None:
             kwargsrepr = saferepr(kwargs, self.kwargsrepr_maxsize)
 
         if not root_id:  # empty root_id defaults to task_id
             root_id = task_id
 
-        stamps = {header: maybe_list(options[header]) for header in stamped_headers or []}
+        stamps = {header: options[header] for header in stamped_headers or []}
         headers = {
             'lang': 'py',
             'task': name,
             'id': task_id,
             'shadow': shadow,
             'eta': eta,
             'expires': expires,
```

### Comparing `celery-5.3.0b1/celery/app/annotations.py` & `celery-5.3.0b2/celery/app/annotations.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/autoretry.py` & `celery-5.3.0b2/celery/app/autoretry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/backends.py` & `celery-5.3.0b2/celery/app/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 __all__ = ('by_name', 'by_url')
 
 UNKNOWN_BACKEND = """
 Unknown result backend: {0!r}.  Did you spell that correctly? ({1!r})
 """
 
 BACKEND_ALIASES = {
-    'amqp': 'celery.backends.amqp:AMQPBackend',
     'rpc': 'celery.backends.rpc.RPCBackend',
     'cache': 'celery.backends.cache:CacheBackend',
     'redis': 'celery.backends.redis:RedisBackend',
     'rediss': 'celery.backends.redis:RedisBackend',
     'sentinel': 'celery.backends.redis:SentinelBackend',
     'mongodb': 'celery.backends.mongodb:MongoBackend',
     'db': 'celery.backends.database:DatabaseBackend',
```

### Comparing `celery-5.3.0b1/celery/app/base.py` & `celery-5.3.0b2/celery/app/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 from celery.utils.functional import first, head_from_fun, maybe_list
 from celery.utils.imports import gen_task_name, instantiate, symbol_by_name
 from celery.utils.log import get_logger
 from celery.utils.objects import FallbackContext, mro_lookup
 from celery.utils.time import maybe_make_aware, timezone, to_utc
 
 # Load all builtin tasks
-from . import builtins  # noqa
-from . import backends
+from . import backends, builtins  # noqa
 from .annotations import prepare as prepare_annotations
 from .autoretry import add_autoretry_behaviour
 from .defaults import DEFAULT_SECURITY_DIGEST, find_deprecated_settings
 from .registry import TaskRegistry
 from .utils import (AppPickler, Settings, _new_key_to_old, _old_key_to_new, _unpickle_app, _unpickle_app_v2, appstr,
                     bugreport, detect_settings)
 
@@ -226,14 +225,15 @@
                  amqp=None, events=None, log=None, control=None,
                  set_as_current=True, tasks=None, broker=None, include=None,
                  changes=None, config_source=None, fixups=None, task_cls=None,
                  autofinalize=True, namespace=None, strict_typing=True,
                  **kwargs):
 
         self._local = threading.local()
+        self._backend_cache = None
 
         self.clock = LamportClock()
         self.main = main
         self.amqp_cls = amqp or self.amqp_cls
         self.events_cls = events or self.events_cls
         self.loader_cls = loader or self._get_default_loader()
         self.log_cls = log or self.log_cls
@@ -454,14 +454,17 @@
             raise TypeError('argument 1 to @task() must be a callable')
         if args:
             raise TypeError(
                 '@task() takes exactly 1 argument ({} given)'.format(
                     sum([len(args), len(opts)])))
         return inner_create_task_cls(**opts)
 
+    def type_checker(self, fun, bound=False):
+        return staticmethod(head_from_fun(fun, bound=bound))
+
     def _task_from_fun(self, fun, name=None, base=None, bind=False, **options):
         if not self.finalized and not self.autofinalize:
             raise RuntimeError('Contract breach: app not finalized')
         name = name or self.gen_task_name(fun.__name__, fun.__module__)
         base = base or self.Task
 
         if name not in self._tasks:
@@ -470,15 +473,15 @@
                 'app': self,
                 'name': name,
                 'run': run,
                 '_decorated': True,
                 '__doc__': fun.__doc__,
                 '__module__': fun.__module__,
                 '__annotations__': fun.__annotations__,
-                '__header__': staticmethod(head_from_fun(fun, bound=bind)),
+                '__header__': self.type_checker(fun, bound=bind),
                 '__wrapped__': run}, **options))()
             # for some reason __qualname__ cannot be set in type()
             # so we have to set it here.
             try:
                 task.__qualname__ = fun.__qualname__
             except AttributeError:
                 pass
@@ -774,14 +777,18 @@
             reply_to or self.thread_oid, time_limit, soft_time_limit,
             self.conf.task_send_sent_event,
             root_id, parent_id, shadow, chain,
             ignore_result=ignore_result,
             **options
         )
 
+        stamped_headers = options.pop('stamped_headers', [])
+        for stamp in stamped_headers:
+            options.pop(stamp)
+
         if connection:
             producer = amqp.Producer(connection, auto_declare=False)
 
         with self.producer_or_acquire(producer) as P:
             with P.connection._reraise_as_library_errors():
                 if not ignore_result:
                     self.backend.on_task_call(P, task_id)
@@ -1240,21 +1247,38 @@
 
     @cached_property
     def amqp(self):
         """AMQP related functionality: :class:`~@amqp`."""
         return instantiate(self.amqp_cls, app=self)
 
     @property
+    def _backend(self):
+        """A reference to the backend object
+
+        Uses self._backend_cache if it is thread safe.
+        Otherwise, use self._local
+        """
+        if self._backend_cache is not None:
+            return self._backend_cache
+        return getattr(self._local, "backend", None)
+
+    @_backend.setter
+    def _backend(self, backend):
+        """Set the backend object on the app"""
+        if backend.thread_safe:
+            self._backend_cache = backend
+        else:
+            self._local.backend = backend
+
+    @property
     def backend(self):
         """Current backend instance."""
-        try:
-            return self._local.backend
-        except AttributeError:
-            self._local.backend = new_backend = self._get_backend()
-            return new_backend
+        if self._backend is None:
+            self._backend = self._get_backend()
+        return self._backend
 
     @property
     def conf(self):
         """Current configuration."""
         if self._conf is None:
             self._conf = self._load_config()
         return self._conf
```

### Comparing `celery-5.3.0b1/celery/app/builtins.py` & `celery-5.3.0b2/celery/app/builtins.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/control.py` & `celery-5.3.0b2/celery/app/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,14 +495,49 @@
         """
         return self.broadcast('revoke', destination=destination, arguments={
             'task_id': task_id,
             'terminate': terminate,
             'signal': signal,
         }, **kwargs)
 
+    def revoke_by_stamped_headers(self, headers, destination=None, terminate=False,
+                                  signal=TERM_SIGNAME, **kwargs):
+        """
+        Tell all (or specific) workers to revoke a task by headers.
+
+        If a task is revoked, the workers will ignore the task and
+        not execute it after all.
+
+        Arguments:
+            headers (dict[str, Union(str, list)]): Headers to match when revoking tasks.
+            terminate (bool): Also terminate the process currently working
+                on the task (if any).
+            signal (str): Name of signal to send to process if terminate.
+                Default is TERM.
+
+        See Also:
+            :meth:`broadcast` for supported keyword arguments.
+        """
+        result = self.broadcast('revoke_by_stamped_headers', destination=destination, arguments={
+            'headers': headers,
+            'terminate': terminate,
+            'signal': signal,
+        }, **kwargs)
+
+        task_ids = set()
+        if result:
+            for host in result:
+                for response in host.values():
+                    task_ids.update(response['ok'])
+
+        if task_ids:
+            return self.revoke(list(task_ids), destination=destination, terminate=terminate, signal=signal, **kwargs)
+        else:
+            return result
+
     def terminate(self, task_id,
                   destination=None, signal=TERM_SIGNAME, **kwargs):
         """Tell all (or specific) workers to terminate a task by id (or list of ids).
 
         See Also:
             This is just a shortcut to :meth:`revoke` with the terminate
             argument enabled.
```

### Comparing `celery-5.3.0b1/celery/app/defaults.py` & `celery-5.3.0b2/celery/app/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from celery.utils.serialization import strtobool
 
 __all__ = ('Option', 'NAMESPACES', 'flatten', 'find')
 
 
 DEFAULT_POOL = 'prefork'
 
-DEFAULT_ACCEPT_CONTENT = ['json']
+DEFAULT_ACCEPT_CONTENT = ('json',)
 DEFAULT_PROCESS_LOG_FMT = """
     [%(asctime)s: %(levelname)s/%(processName)s] %(message)s
 """.strip()
 DEFAULT_TASK_LOG_FMT = """[%(asctime)s: %(levelname)s/%(processName)s] \
 %(task_name)s[%(task_id)s]: %(message)s"""
 
 DEFAULT_SECURITY_DIGEST = 'sha256'
@@ -74,25 +74,27 @@
         __old__=OLD_NS_BEAT,
 
         max_loop_interval=Option(0, type='float'),
         schedule=Option({}, type='dict'),
         scheduler=Option('celery.beat:PersistentScheduler'),
         schedule_filename=Option('celerybeat-schedule'),
         sync_every=Option(0, type='int'),
+        cron_starting_deadline=Option(None, type=int)
     ),
     broker=Namespace(
         url=Option(None, type='string'),
         read_url=Option(None, type='string'),
         write_url=Option(None, type='string'),
         transport=Option(type='string'),
         transport_options=Option({}, type='dict'),
         connection_timeout=Option(4, type='float'),
         connection_retry=Option(True, type='bool'),
         connection_retry_on_startup=Option(None, type='bool'),
         connection_max_retries=Option(100, type='int'),
+        channel_error_retry=Option(False, type='bool'),
         failover_strategy=Option(None, type='string'),
         heartbeat=Option(120, type='int'),
         heartbeat_checkrate=Option(3.0, type='int'),
         login_method=Option(None, type='string'),
         pool_limit=Option(10, type='int'),
         use_ssl=Option(False, type='bool'),
 
@@ -287,14 +289,15 @@
             type='float', old={'celeryd_task_soft_time_limit'},
         ),
         time_limit=Option(
             type='float', old={'celeryd_task_time_limit'},
         ),
         store_errors_even_if_ignored=Option(False, type='bool'),
         track_started=Option(False, type='bool'),
+        allow_error_cb_on_chord_header=Option(False, type='bool'),
     ),
     worker=Namespace(
         __old__=OLD_NS_WORKER,
         agent=Option(None, type='string'),
         autoscaler=Option('celery.worker.autoscale:Autoscaler'),
         cancel_long_running_tasks_on_connection_loss=Option(
             False, type='bool'
```

### Comparing `celery-5.3.0b1/celery/app/events.py` & `celery-5.3.0b2/celery/app/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/log.py` & `celery-5.3.0b2/celery/app/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from kombu.utils.encoding import set_default_encoding_file
 
 from celery import signals
 from celery._state import get_current_task
 from celery.exceptions import CDeprecationWarning, CPendingDeprecationWarning
 from celery.local import class_property
-from celery.platforms import isatty
 from celery.utils.log import (ColorFormatter, LoggingProxy, get_logger, get_multiprocessing_logger, mlevel,
                               reset_multiprocessing_logger)
 from celery.utils.nodenames import node_format
 from celery.utils.term import colored
 
 __all__ = ('TaskFormatter', 'Logging')
 
@@ -200,15 +199,15 @@
         colorize = self.colorize if colorize is None else colorize
         if self.app.IS_WINDOWS:
             # Windows does not support ANSI color codes.
             return False
         if colorize or colorize is None:
             # Only use color if there's no active log file
             # and stderr is an actual terminal.
-            return logfile is None and isatty(sys.stderr)
+            return logfile is None and sys.stderr.isatty()
         return colorize
 
     def colored(self, logfile=None, enabled=None):
         return colored(enabled=self.supports_color(enabled, logfile))
 
     def setup_handlers(self, logger, logfile, format, colorize,
                        formatter=ColorFormatter, **kwargs):
```

### Comparing `celery-5.3.0b1/celery/app/registry.py` & `celery-5.3.0b2/celery/app/registry.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/routes.py` & `celery-5.3.0b2/celery/app/routes.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/app/task.py` & `celery-5.3.0b2/celery/app/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Task implementation: request context and the task base class."""
 import sys
 
-from billiard.einfo import ExceptionInfo
+from billiard.einfo import ExceptionInfo, ExceptionWithTraceback
 from kombu import serialization
 from kombu.exceptions import OperationalError
 from kombu.utils.uuid import uuid
 
 from celery import current_app, states
 from celery._state import _task_stack
-from celery.canvas import GroupStampingVisitor, _chain, group, signature
+from celery.canvas import _chain, group, signature
 from celery.exceptions import Ignore, ImproperlyConfigured, MaxRetriesExceededError, Reject, Retry
 from celery.local import class_property
 from celery.result import EagerResult, denied_join_result
 from celery.utils import abstract
 from celery.utils.functional import mattrgetter, maybe_list
 from celery.utils.imports import instantiate
 from celery.utils.nodenames import gethostname
@@ -248,15 +248,15 @@
     #: running.
     #:
     #: The application default can be overridden using the
     #: :setting:`task_track_started` setting.
     track_started = None
 
     #: When enabled messages for this task will be acknowledged **after**
-    #: the task has been executed, and not *just before* (the
+    #: the task has been executed, and not *right before* (the
     #: default behavior).
     #:
     #: Please note that this means the task may be executed twice if the
     #: worker crashes mid execution.
     #:
     #: The application default can be overridden with the
     #: :setting:`task_acks_late` setting.
@@ -809,14 +809,16 @@
             task.name, task, eager=True,
             propagate=throw, app=self._get_app(),
         )
         ret = tracer(task_id, args, kwargs, request)
         retval = ret.retval
         if isinstance(retval, ExceptionInfo):
             retval, tb = retval.exception, retval.traceback
+            if isinstance(retval, ExceptionWithTraceback):
+                retval = retval.exc
         if isinstance(retval, Retry) and retval.sig is not None:
             return retval.sig.apply(retries=retries + 1)
         state = states.SUCCESS if ret.info is None else ret.info.state
         return EagerResult(task_id, retval, state, traceback=tb)
 
     def AsyncResult(self, task_id, **kwargs):
         """Get AsyncResult instance for the specified task.
@@ -900,14 +902,15 @@
         Execution of the host task ends immediately and no subsequent statements
         will be run.
 
         .. versionadded:: 4.0
 
         Arguments:
             sig (Signature): signature to replace with.
+            visitor (StampingVisitor): Visitor API object.
 
         Raises:
             ~@Ignore: This is always raised when called in asynchronous context.
             It is best to always use ``return self.replace(...)`` to convey
             to the reader that the task won't continue after being replaced.
         """
         chord = self.request.chord
@@ -946,26 +949,15 @@
             replaced_task_nesting=replaced_task_nesting
         )
         # If the task being replaced is part of a chain, we need to re-create
         # it with the replacement signature - these subsequent tasks will
         # retain their original task IDs as well
         for t in reversed(self.request.chain or []):
             sig |= signature(t, app=self.app)
-        # Stamping sig with parents groups
-        stamped_headers = self.request.stamped_headers
-        if self.request.stamps:
-            groups = self.request.stamps.get("groups")
-            sig.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-
-        # Finally, either apply or delay the new signature!
-        if self.request.is_eager:
-            return sig.apply().get()
-        else:
-            sig.delay()
-            raise Ignore('Replaced by new task')
+        return self.on_replace(sig)
 
     def add_to_chord(self, sig, lazy=False):
         """Add signature to the chord the current task is a member of.
 
         .. versionadded:: 4.0
 
         Currently only supported by the Redis result backend.
@@ -1073,14 +1065,32 @@
             kwargs (Dict): Original keyword arguments for the task.
             einfo (~billiard.einfo.ExceptionInfo): Exception information.
 
         Returns:
             None: The return value of this handler is ignored.
         """
 
+    def on_replace(self, sig):
+        """Handler called when the task is replaced.
+
+        Must return super().on_replace(sig) when overriding to ensure the task replacement
+        is properly handled.
+
+        .. versionadded:: 5.3
+
+        Arguments:
+            sig (Signature): signature to replace with.
+        """
+        # Finally, either apply or delay the new signature!
+        if self.request.is_eager:
+            return sig.apply().get()
+        else:
+            sig.delay()
+            raise Ignore('Replaced by new task')
+
     def add_trail(self, result):
         if self.trail:
             self.request.children.append(result)
         return result
 
     def push_request(self, *args, **kwargs):
         self.request_stack.push(Context(*args, **kwargs))
```

### Comparing `celery-5.3.0b1/celery/app/trace.py` & `celery-5.3.0b2/celery/app/trace.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 errors are recorded, handlers are applied and so on.
 """
 import logging
 import os
 import sys
 import time
 from collections import namedtuple
+from typing import Any, Callable, Dict, FrozenSet, Optional, Sequence, Tuple, Type, Union
 from warnings import warn
 
-from billiard.einfo import ExceptionInfo
+from billiard.einfo import ExceptionInfo, ExceptionWithTraceback
 from kombu.exceptions import EncodeError
 from kombu.serialization import loads as loads_message
 from kombu.serialization import prepare_accept_content
 from kombu.utils.encoding import safe_repr, safe_str
 
+import celery
+import celery.loaders.app
 from celery import current_app, group, signals, states
 from celery._state import _task_stack
 from celery.app.task import Context
 from celery.app.task import Task as BaseTask
 from celery.exceptions import BackendGetMetaError, Ignore, InvalidTaskError, Reject, Retry
 from celery.result import AsyncResult
 from celery.utils.log import get_logger
@@ -234,14 +237,16 @@
             self._log_error(task, req, einfo)
             return einfo
         finally:
             del tb
 
     def _log_error(self, task, req, einfo):
         eobj = einfo.exception = get_pickled_exception(einfo.exception)
+        if isinstance(eobj, ExceptionWithTraceback):
+            eobj = einfo.exception = eobj.exc
         exception, traceback, exc_info, sargs, skwargs = (
             safe_repr(eobj),
             safe_str(einfo.traceback),
             einfo.exc_info,
             safe_repr(req.args),
             safe_repr(req.kwargs),
         )
@@ -282,18 +287,28 @@
             tb.tb_frame.f_locals
         except RuntimeError:
             # Ignore the exception raised if the frame is still executing.
             pass
         tb = tb.tb_next
 
 
-def build_tracer(name, task, loader=None, hostname=None, store_errors=True,
-                 Info=TraceInfo, eager=False, propagate=False, app=None,
-                 monotonic=time.monotonic, trace_ok_t=trace_ok_t,
-                 IGNORE_STATES=IGNORE_STATES):
+def build_tracer(
+        name: str,
+        task: Union[celery.Task, celery.local.PromiseProxy],
+        loader: Optional[celery.loaders.app.AppLoader] = None,
+        hostname: Optional[str] = None,
+        store_errors: bool = True,
+        Info: Type[TraceInfo] = TraceInfo,
+        eager: bool = False,
+        propagate: bool = False,
+        app: Optional[celery.Celery] = None,
+        monotonic: Callable[[], int] = time.monotonic,
+        trace_ok_t: Type[trace_ok_t] = trace_ok_t,
+        IGNORE_STATES: FrozenSet[str] = IGNORE_STATES) -> \
+        Callable[[str, Tuple[Any, ...], Dict[str, Any], Any], trace_ok_t]:
     """Return a function that traces task execution.
 
     Catches all exceptions and updates result backend with the
     state and result.
 
     If the call was successful, it saves the result to the task result
     backend, and sets the task status to `"SUCCESS"`.
@@ -365,24 +380,35 @@
     prerun_receivers = signals.task_prerun.receivers
     postrun_receivers = signals.task_postrun.receivers
     success_receivers = signals.task_success.receivers
 
     from celery import canvas
     signature = canvas.maybe_signature  # maybe_ does not clone if already
 
-    def on_error(request, exc, state=FAILURE, call_errbacks=True):
+    def on_error(
+            request: celery.app.task.Context,
+            exc: Union[Exception, Type[Exception]],
+            state: str = FAILURE,
+            call_errbacks: bool = True) -> Tuple[Info, Any, Any, Any]:
+        """Handle any errors raised by a `Task`'s execution."""
         if propagate:
             raise
         I = Info(state, exc)
         R = I.handle_error_state(
             task, request, eager=eager, call_errbacks=call_errbacks,
         )
         return I, R, I.state, I.retval
 
-    def trace_task(uuid, args, kwargs, request=None):
+    def trace_task(
+            uuid: str,
+            args: Sequence[Any],
+            kwargs: Dict[str, Any],
+            request: Optional[Dict[str, Any]] = None) -> trace_ok_t:
+        """Execute and trace a `Task`."""
+
         # R      - is the possibly prepared return value.
         # I      - is the Info object.
         # T      - runtime
         # Rstr   - textual representation of return value
         # retval - is the always unmodified return value.
         # state  - is the resulting task state.
```

### Comparing `celery-5.3.0b1/celery/app/utils.py` & `celery-5.3.0b2/celery/app/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/apps/beat.py` & `celery-5.3.0b2/celery/apps/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/apps/multi.py` & `celery-5.3.0b2/celery/apps/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/apps/worker.py` & `celery-5.3.0b2/celery/apps/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from billiard.common import REMAP_SIGTERM
 from billiard.process import current_process
 from kombu.utils.encoding import safe_str
 
 from celery import VERSION_BANNER, platforms, signals
 from celery.app import trace
 from celery.loaders.app import AppLoader
-from celery.platforms import EX_FAILURE, EX_OK, check_privileges, isatty
+from celery.platforms import EX_FAILURE, EX_OK, check_privileges
 from celery.utils import static, term
 from celery.utils.debug import cry
 from celery.utils.imports import qualname
 from celery.utils.log import get_logger, in_sighandler, set_in_sighandler
 from celery.utils.text import pluralize
 from celery.worker import WorkController
 
@@ -102,15 +102,15 @@
         self.redirect_stdouts = self.app.either(
             'worker_redirect_stdouts', redirect_stdouts)
         self.redirect_stdouts_level = self.app.either(
             'worker_redirect_stdouts_level', redirect_stdouts_level)
         super().setup_defaults(**kwargs)
         self.purge = purge
         self.no_color = no_color
-        self._isatty = isatty(sys.stdout)
+        self._isatty = sys.stdout.isatty()
         self.colored = self.app.log.colored(
             self.logfile,
             enabled=not no_color if no_color is not None else no_color
         )
 
     def on_init_blueprint(self):
         self._custom_logging = self.setup_logging()
```

### Comparing `celery-5.3.0b1/celery/backends/arangodb.py` & `celery-5.3.0b2/celery/backends/arangodb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/asynchronous.py` & `celery-5.3.0b2/celery/backends/asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/azureblockblob.py` & `celery-5.3.0b2/celery/backends/azureblockblob.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/base.py` & `celery-5.3.0b2/celery/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         self.accept = conf.accept_content if self.accept is None else self.accept
         self.accept = prepare_accept_content(self.accept)
 
         self.always_retry = conf.get('result_backend_always_retry', False)
         self.max_sleep_between_retries_ms = conf.get('result_backend_max_sleep_between_retries_ms', 10000)
         self.base_sleep_between_retries_ms = conf.get('result_backend_base_sleep_between_retries_ms', 10)
         self.max_retries = conf.get('result_backend_max_retries', float("inf"))
+        self.thread_safe = conf.get('result_backend_thread_safe', False)
 
         self._pending_results = pending_results_t({}, WeakValueDictionary())
         self._pending_messages = BufferMap(MESSAGE_BUFFER_MAX)
         self.url = url
 
     def as_uri(self, include_password=False):
         """Return the backend as an URI, sanitizing the password or not."""
@@ -813,19 +814,33 @@
     group_keyprefix = 'celery-taskset-meta-'
     chord_keyprefix = 'chord-unlock-'
     implements_incr = False
 
     def __init__(self, *args, **kwargs):
         if hasattr(self.key_t, '__func__'):  # pragma: no cover
             self.key_t = self.key_t.__func__  # remove binding
-        self._encode_prefixes()
         super().__init__(*args, **kwargs)
+        self._add_global_keyprefix()
+        self._encode_prefixes()
         if self.implements_incr:
             self.apply_chord = self._apply_chord_incr
 
+    def _add_global_keyprefix(self):
+        """
+        This method prepends the global keyprefix to the existing keyprefixes.
+
+        This method checks if a global keyprefix is configured in `result_backend_transport_options` using the
+        `global_keyprefix` key. If so, then it is prepended to the task, group and chord key prefixes.
+        """
+        global_keyprefix = self.app.conf.get('result_backend_transport_options', {}).get("global_keyprefix", None)
+        if global_keyprefix:
+            self.task_keyprefix = f"{global_keyprefix}_{self.task_keyprefix}"
+            self.group_keyprefix = f"{global_keyprefix}_{self.group_keyprefix}"
+            self.chord_keyprefix = f"{global_keyprefix}_{self.chord_keyprefix}"
+
     def _encode_prefixes(self):
         self.task_keyprefix = self.key_t(self.task_keyprefix)
         self.group_keyprefix = self.key_t(self.group_keyprefix)
         self.chord_keyprefix = self.key_t(self.chord_keyprefix)
 
     def get(self, key):
         raise NotImplementedError('Must implement the get method.')
```

### Comparing `celery-5.3.0b1/celery/backends/cache.py` & `celery-5.3.0b2/celery/backends/cache.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/cassandra.py` & `celery-5.3.0b2/celery/backends/cassandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .base import BaseBackend
 
 try:  # pragma: no cover
     import cassandra
     import cassandra.auth
     import cassandra.cluster
     import cassandra.query
-except ImportError:  # pragma: no cover
+except ImportError:
     cassandra = None
 
 
 __all__ = ('CassandraBackend',)
 
 logger = get_logger(__name__)
```

### Comparing `celery-5.3.0b1/celery/backends/consul.py` & `celery-5.3.0b2/celery/backends/consul.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/cosmosdbsql.py` & `celery-5.3.0b2/celery/backends/cosmosdbsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 try:
     import pydocumentdb
     from pydocumentdb.document_client import DocumentClient
     from pydocumentdb.documents import ConnectionPolicy, ConsistencyLevel, PartitionKind
     from pydocumentdb.errors import HTTPFailure
     from pydocumentdb.retry_options import RetryOptions
-except ImportError:  # pragma: no cover
+except ImportError:
     pydocumentdb = DocumentClient = ConsistencyLevel = PartitionKind = \
         HTTPFailure = ConnectionPolicy = RetryOptions = None
 
 __all__ = ("CosmosDBSQLBackend",)
 
 
 ERROR_NOT_FOUND = 404
```

### Comparing `celery-5.3.0b1/celery/backends/couchbase.py` & `celery-5.3.0b2/celery/backends/couchbase.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/couchdb.py` & `celery-5.3.0b2/celery/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/database/__init__.py` & `celery-5.3.0b2/celery/backends/database/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .models import Task, TaskExtended, TaskSet
 from .session import SessionManager
 
 try:
     from sqlalchemy.exc import DatabaseError, InvalidRequestError
     from sqlalchemy.orm.exc import StaleDataError
-except ImportError:  # pragma: no cover
+except ImportError:
     raise ImproperlyConfigured(
         'The database result backend requires SQLAlchemy to be installed.'
         'See https://pypi.org/project/SQLAlchemy/')
 
 logger = logging.getLogger(__name__)
 
 __all__ = ('DatabaseBackend',)
```

### Comparing `celery-5.3.0b1/celery/backends/database/models.py` & `celery-5.3.0b2/celery/backends/database/models.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/database/session.py` & `celery-5.3.0b2/celery/backends/database/session.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/dynamodb.py` & `celery-5.3.0b2/celery/backends/dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from celery.utils.log import get_logger
 
 from .base import KeyValueStoreBackend
 
 try:
     import boto3
     from botocore.exceptions import ClientError
-except ImportError:  # pragma: no cover
+except ImportError:
     boto3 = ClientError = None
 
 __all__ = ('DynamoDBBackend',)
 
 
 # Helper class that describes a DynamoDB attribute
 DynamoDBAttribute = namedtuple('DynamoDBAttribute', ('name', 'data_type'))
@@ -197,36 +197,33 @@
             }
         }
 
     def _get_or_create_table(self):
         """Create table if not exists, otherwise return the description."""
         table_schema = self._get_table_schema()
         try:
-            table_description = self._client.create_table(**table_schema)
-            logger.info(
-                'DynamoDB Table {} did not exist, creating.'.format(
-                    self.table_name
-                )
-            )
-            # In case we created the table, wait until it becomes available.
-            self._wait_for_table_status('ACTIVE')
-            logger.info(
-                'DynamoDB Table {} is now available.'.format(
-                    self.table_name
-                )
-            )
-            return table_description
+            return self._client.describe_table(TableName=self.table_name)
         except ClientError as e:
             error_code = e.response['Error'].get('Code', 'Unknown')
 
-            # If table exists, do not fail, just return the description.
-            if error_code == 'ResourceInUseException':
-                return self._client.describe_table(
-                    TableName=self.table_name
+            if error_code == 'ResourceNotFoundException':
+                table_description = self._client.create_table(**table_schema)
+                logger.info(
+                    'DynamoDB Table {} did not exist, creating.'.format(
+                        self.table_name
+                    )
+                )
+                # In case we created the table, wait until it becomes available.
+                self._wait_for_table_status('ACTIVE')
+                logger.info(
+                    'DynamoDB Table {} is now available.'.format(
+                        self.table_name
+                    )
                 )
+                return table_description
             else:
                 raise e
 
     def _has_ttl(self):
         """Return the desired Time to Live config.
 
         - True:  Enable TTL on the table; use expiry.
```

### Comparing `celery-5.3.0b1/celery/backends/elasticsearch.py` & `celery-5.3.0b2/celery/backends/elasticsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from celery import states
 from celery.exceptions import ImproperlyConfigured
 
 from .base import KeyValueStoreBackend
 
 try:
     import elasticsearch
-except ImportError:  # pragma: no cover
+except ImportError:
     elasticsearch = None
 
 __all__ = ('ElasticsearchBackend',)
 
 E_LIB_MISSING = """\
 You need to install the elasticsearch library to use the Elasticsearch \
 result backend.\
```

### Comparing `celery-5.3.0b1/celery/backends/filesystem.py` & `celery-5.3.0b2/celery/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/mongodb.py` & `celery-5.3.0b2/celery/backends/mongodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from celery import states
 from celery.exceptions import ImproperlyConfigured
 
 from .base import BaseBackend
 
 try:
     import pymongo
-except ImportError:  # pragma: no cover
+except ImportError:
     pymongo = None
 
 if pymongo:
     try:
         from bson.binary import Binary
-    except ImportError:                     # pragma: no cover
+    except ImportError:
         from pymongo.binary import Binary
     from pymongo.errors import InvalidDocument
 else:                                       # pragma: no cover
     Binary = None
 
     class InvalidDocument(Exception):
         pass
```

### Comparing `celery-5.3.0b1/celery/backends/redis.py` & `celery-5.3.0b2/celery/backends/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from .asynchronous import AsyncBackendMixin, BaseResultConsumer
 from .base import BaseKeyValueStoreBackend
 
 try:
     import redis.connection
     from kombu.transport.redis import get_redis_error_classes
-except ImportError:  # pragma: no cover
+except ImportError:
     redis = None
     get_redis_error_classes = None
 
 try:
     import redis.sentinel
 except ImportError:
     pass
```

### Comparing `celery-5.3.0b1/celery/backends/rpc.py` & `celery-5.3.0b2/celery/backends/rpc.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/backends/s3.py` & `celery-5.3.0b2/celery/backends/s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/beat.py` & `celery-5.3.0b2/celery/beat.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 
 class SchedulingError(Exception):
     """An error occurred while scheduling a task."""
 
 
 class BeatLazyFunc:
-    """An lazy function declared in 'beat_schedule' and called before sending to worker.
+    """A lazy function declared in 'beat_schedule' and called before sending to worker.
 
     Example:
 
         beat_schedule = {
             'test-every-5-minutes': {
                 'task': 'test',
                 'schedule': 300,
@@ -289,15 +289,15 @@
             return n + drift
         return n
 
     def is_due(self, entry):
         return entry.is_due()
 
     def _when(self, entry, next_time_to_run, mktime=timegm):
-        """Return a utc timestamp, make sure heapq in currect order."""
+        """Return a utc timestamp, make sure heapq in correct order."""
         adjust = self.adjust
 
         as_now = maybe_make_aware(entry.default_now())
 
         return (mktime(as_now.utctimetuple()) +
                 as_now.microsecond / 1e6 +
                 (adjust(next_time_to_run) or 0))
```

### Comparing `celery-5.3.0b1/celery/bin/amqp.py` & `celery-5.3.0b2/celery/bin/amqp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/base.py` & `celery-5.3.0b2/celery/bin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,16 @@
 
 class CeleryDaemonCommand(CeleryCommand):
     """Daemon commands."""
 
     def __init__(self, *args, **kwargs):
         """Initialize a Celery command with common daemon options."""
         super().__init__(*args, **kwargs)
-        self.params.append(CeleryOption(('-f', '--logfile'), help_group="Daemonization Options"))
+        self.params.append(CeleryOption(('-f', '--logfile'), help_group="Daemonization Options",
+                           help="Log destination; defaults to stderr"))
         self.params.append(CeleryOption(('--pidfile',), help_group="Daemonization Options"))
         self.params.append(CeleryOption(('--uid',), help_group="Daemonization Options"))
         self.params.append(CeleryOption(('--gid',), help_group="Daemonization Options"))
         self.params.append(CeleryOption(('--umask',), help_group="Daemonization Options"))
         self.params.append(CeleryOption(('--executable',), help_group="Daemonization Options"))
```

### Comparing `celery-5.3.0b1/celery/bin/beat.py` & `celery-5.3.0b2/celery/bin/beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/call.py` & `celery-5.3.0b2/celery/bin/call.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/celery.py` & `celery-5.3.0b2/celery/bin/celery.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Celery Command Line Interface."""
 import os
 import pathlib
+import sys
 import traceback
 
 try:
     from importlib.metadata import entry_points
 except ImportError:
     from importlib_metadata import entry_points
 
@@ -71,15 +72,24 @@
                 UNABLE_TO_LOAD_APP_ERROR_OCCURRED.format(value, exc)
             )
 
 
 APP = App()
 
 
-@with_plugins(entry_points().get('celery.commands', []))
+if sys.version_info >= (3, 10):
+    _PLUGINS = entry_points(group='celery.commands')
+else:
+    try:
+        _PLUGINS = entry_points().get('celery.commands', [])
+    except AttributeError:
+        _PLUGINS = entry_points().select(group='celery.commands')
+
+
+@with_plugins(_PLUGINS)
 @click.group(cls=DYMGroup, invoke_without_command=True)
 @click.option('-A',
               '--app',
               envvar='APP',
               cls=CeleryOption,
               type=APP,
               help_group="Global Options")
@@ -117,17 +127,23 @@
               is_flag=True,
               cls=CeleryOption,
               help_group="Global Options")
 @click.option('--version',
               cls=CeleryOption,
               is_flag=True,
               help_group="Global Options")
+@click.option('--skip-checks',
+              envvar='SKIP_CHECKS',
+              cls=CeleryOption,
+              is_flag=True,
+              help_group="Global Options",
+              help="Skip Django core checks on startup.")
 @click.pass_context
 def celery(ctx, app, broker, result_backend, loader, config, workdir,
-           no_color, quiet, version):
+           no_color, quiet, version, skip_checks):
     """Celery command entrypoint."""
     if version:
         click.echo(VERSION_BANNER)
         ctx.exit()
     elif ctx.invoked_subcommand is None:
         click.echo(ctx.get_help())
         ctx.exit()
@@ -137,14 +153,16 @@
         os.environ['CELERY_LOADER'] = loader
     if broker:
         os.environ['CELERY_BROKER_URL'] = broker
     if result_backend:
         os.environ['CELERY_RESULT_BACKEND'] = result_backend
     if config:
         os.environ['CELERY_CONFIG_MODULE'] = config
+    if skip_checks:
+        os.environ['CELERY_SKIP_CHECKS'] = skip_checks
     ctx.obj = CLIContext(app=app, no_color=no_color, workdir=workdir,
                          quiet=quiet)
 
     # User options
     worker.params.extend(ctx.obj.app.user_options.get('worker', []))
     beat.params.extend(ctx.obj.app.user_options.get('beat', []))
     events.params.extend(ctx.obj.app.user_options.get('events', []))
```

### Comparing `celery-5.3.0b1/celery/bin/control.py` & `celery-5.3.0b2/celery/bin/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/events.py` & `celery-5.3.0b2/celery/bin/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/graph.py` & `celery-5.3.0b2/celery/bin/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/list.py` & `celery-5.3.0b2/celery/bin/list.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/logtool.py` & `celery-5.3.0b2/celery/bin/logtool.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/migrate.py` & `celery-5.3.0b2/celery/bin/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/multi.py` & `celery-5.3.0b2/celery/bin/multi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/purge.py` & `celery-5.3.0b2/celery/bin/purge.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/result.py` & `celery-5.3.0b2/celery/bin/result.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/shell.py` & `celery-5.3.0b2/celery/bin/shell.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/upgrade.py` & `celery-5.3.0b2/celery/bin/upgrade.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bin/worker.py` & `celery-5.3.0b2/celery/bin/worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/bootsteps.py` & `celery-5.3.0b2/celery/bootsteps.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .utils.graph import DependencyGraph, GraphFormatter
 from .utils.imports import instantiate, qualname
 from .utils.log import get_logger
 
 try:
     from greenlet import GreenletExit
-except ImportError:  # pragma: no cover
+except ImportError:
     IGNORE_ERRORS = ()
 else:
     IGNORE_ERRORS = (GreenletExit,)
 
 __all__ = ('Blueprint', 'Step', 'StartStopStep', 'ConsumerStep')
 
 #: States
```

### Comparing `celery-5.3.0b1/celery/canvas.py` & `celery-5.3.0b2/t/unit/tasks/test_canvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1906 +1,1795 @@
-"""Composing task work-flows.
+import json
+import math
+from collections.abc import Iterable
+from unittest.mock import ANY, MagicMock, Mock, call, patch, sentinel
+
+import pytest
+import pytest_subtests  # noqa
+
+from celery._state import _task_stack
+from celery.canvas import (Signature, _chain, _maybe_group, _merge_dictionaries, chain, chord, chunks, group,
+                           maybe_signature, maybe_unroll_group, signature, xmap, xstarmap)
+from celery.result import AsyncResult, EagerResult, GroupResult
+
+SIG = Signature({
+    'task': 'TASK',
+    'args': ('A1',),
+    'kwargs': {'K1': 'V1'},
+    'options': {'task_id': 'TASK_ID'},
+    'subtask_type': ''},
+)
 
-.. seealso:
 
-    You should import these from :mod:`celery` and not this module.
-"""
+def return_True(*args, **kwargs):
+    # Task run functions can't be closures/lambdas, as they're pickled.
+    return True
 
-import itertools
-import operator
-from abc import ABCMeta, abstractmethod
-from collections import deque
-from collections.abc import MutableSequence
-from copy import deepcopy
-from functools import partial as _partial
-from functools import reduce
-from operator import itemgetter
-from types import GeneratorType
-
-from kombu.utils.functional import fxrange, reprcall
-from kombu.utils.objects import cached_property
-from kombu.utils.uuid import uuid
-from vine import barrier
-
-from celery._state import current_app
-from celery.result import GroupResult, allow_join_result
-from celery.utils import abstract
-from celery.utils.collections import ChainMap
-from celery.utils.functional import _regen
-from celery.utils.functional import chunks as _chunks
-from celery.utils.functional import is_list, maybe_list, regen, seq_concat_item, seq_concat_seq
-from celery.utils.objects import getitem_property
-from celery.utils.text import remove_repeating_from_task, truncate
-
-__all__ = (
-    'Signature', 'chain', 'xmap', 'xstarmap', 'chunks',
-    'group', 'chord', 'signature', 'maybe_signature',
-)
 
+class test_maybe_unroll_group:
 
-def maybe_unroll_group(group):
-    """Unroll group with only one member."""
-    # Issue #1656
-    try:
-        size = len(group.tasks)
-    except TypeError:
-        try:
-            size = group.tasks.__length_hint__()
-        except (AttributeError, TypeError):
-            return group
-        else:
-            return list(group.tasks)[0] if size == 1 else group
-    else:
-        return group.tasks[0] if size == 1 else group
-
-
-def task_name_from(task):
-    return getattr(task, 'name', task)
-
-
-def _stamp_regen_task(task, visitor, **headers):
-    task.stamp(visitor=visitor, **headers)
-    return task
-
-
-def _merge_dictionaries(d1, d2):
-    for key, value in d1.items():
-        if key in d2:
-            if isinstance(value, dict):
-                _merge_dictionaries(d1[key], d2[key])
-            else:
-                if isinstance(value, (int, float, str)):
-                    d1[key] = [value]
-                if isinstance(d2[key], list):
-                    d1[key].extend(d2[key])
-                else:
-                    if d1[key] is None:
-                        d1[key] = []
-                    else:
-                        d1[key] = list(d1[key])
-                    d1[key].append(d2[key])
-    for key, value in d2.items():
-        if key not in d1:
-            d1[key] = value
-
-
-class StampingVisitor(metaclass=ABCMeta):
-    """Stamping API.  A class that provides a stamping API possibility for
-    canvas primitives. If you want to implement stamping behavior for
-    a canvas primitive override method that represents it.
-    """
-
-    @abstractmethod
-    def on_group_start(self, group, **headers) -> dict:
-        """Method that is called on group stamping start.
-
-         Arguments:
-             group (group): Group that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         Returns:
-             Dict: headers to update.
-         """
-        pass
-
-    def on_group_end(self, group, **headers) -> None:
-        """Method that is called on group stamping end.
-
-         Arguments:
-             group (group): Group that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         """
-        pass
-
-    @abstractmethod
-    def on_chain_start(self, chain, **headers) -> dict:
-        """Method that is called on chain stamping start.
-
-         Arguments:
-             chain (chain): Chain that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         Returns:
-             Dict: headers to update.
-         """
-        pass
-
-    def on_chain_end(self, chain, **headers) -> None:
-        """Method that is called on chain stamping end.
-
-         Arguments:
-             chain (chain): Chain that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         """
-        pass
-
-    @abstractmethod
-    def on_signature(self, sig, **headers) -> dict:
-        """Method that is called on signature stamping.
-
-         Arguments:
-             sig (Signature): Signature that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         Returns:
-             Dict: headers to update.
-         """
-        pass
-
-    def on_chord_header_start(self, chord, **header) -> dict:
-        """Method that is called on сhord header stamping start.
-
-         Arguments:
-             chord (chord): chord that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         Returns:
-             Dict: headers to update.
-         """
-        if not isinstance(chord.tasks, group):
-            chord.tasks = group(chord.tasks)
-        return self.on_group_start(chord.tasks, **header)
-
-    def on_chord_header_end(self, chord, **header) -> None:
-        """Method that is called on сhord header stamping end.
-
-           Arguments:
-               chord (chord): chord that is stamped.
-               headers (Dict): Partial headers that could be merged with existing headers.
-        """
-        self.on_group_end(chord.tasks, **header)
-
-    def on_chord_body(self, chord, **header) -> dict:
-        """Method that is called on chord body stamping.
-
-         Arguments:
-             chord (chord): chord that is stamped.
-             headers (Dict): Partial headers that could be merged with existing headers.
-         Returns:
-             Dict: headers to update.
-        """
-        return self.on_signature(chord.body, **header)
-
-
-class GroupStampingVisitor(StampingVisitor):
-    """
-    Group stamping implementation based on Stamping API.
-    """
-
-    def __init__(self, groups=None, stamped_headers=None):
-        self.groups = groups or []
-        self.stamped_headers = stamped_headers or []
-        if "groups" not in self.stamped_headers:
-            self.stamped_headers.append("groups")
-
-    def on_group_start(self, group, **headers) -> dict:
-        if group.id is None:
-            group.set(task_id=uuid())
-
-        if group.id not in self.groups:
-            self.groups.append(group.id)
-        return {'groups': list(self.groups), "stamped_headers": list(self.stamped_headers)}
-
-    def on_group_end(self, group, **headers) -> None:
-        self.groups.pop()
-
-    def on_chain_start(self, chain, **headers) -> dict:
-        return {'groups': list(self.groups), "stamped_headers": list(self.stamped_headers)}
-
-    def on_signature(self, sig, **headers) -> dict:
-        return {'groups': list(self.groups), "stamped_headers": list(self.stamped_headers)}
-
-
-@abstract.CallableSignature.register
-class Signature(dict):
-    """Task Signature.
-
-    Class that wraps the arguments and execution options
-    for a single task invocation.
-
-    Used as the parts in a :class:`group` and other constructs,
-    or to pass tasks around as callbacks while being compatible
-    with serializers with a strict type subset.
-
-    Signatures can also be created from tasks:
-
-    - Using the ``.signature()`` method that has the same signature
-      as ``Task.apply_async``:
-
-        .. code-block:: pycon
-
-            >>> add.signature(args=(1,), kwargs={'kw': 2}, options={})
-
-    - or the ``.s()`` shortcut that works for star arguments:
-
-        .. code-block:: pycon
-
-            >>> add.s(1, kw=2)
-
-    - the ``.s()`` shortcut does not allow you to specify execution options
-      but there's a chaning `.set` method that returns the signature:
-
-        .. code-block:: pycon
-
-            >>> add.s(2, 2).set(countdown=10).set(expires=30).delay()
-
-    Note:
-        You should use :func:`~celery.signature` to create new signatures.
-        The ``Signature`` class is the type returned by that function and
-        should be used for ``isinstance`` checks for signatures.
-
-    See Also:
-        :ref:`guide-canvas` for the complete guide.
-
-    Arguments:
-        task (Union[Type[celery.app.task.Task], str]): Either a task
-            class/instance, or the name of a task.
-        args (Tuple): Positional arguments to apply.
-        kwargs (Dict): Keyword arguments to apply.
-        options (Dict): Additional options to :meth:`Task.apply_async`.
-
-    Note:
-        If the first argument is a :class:`dict`, the other
-        arguments will be ignored and the values in the dict will be used
-        instead::
-
-            >>> s = signature('tasks.add', args=(2, 2))
-            >>> signature(s)
-            {'task': 'tasks.add', args=(2, 2), kwargs={}, options={}}
-    """
-
-    TYPES = {}
-    _app = _type = None
-    # The following fields must not be changed during freezing/merging because
-    # to do so would disrupt completion of parent tasks
-    _IMMUTABLE_OPTIONS = {"group_id", "stamped_headers"}
-
-    @classmethod
-    def register_type(cls, name=None):
-        def _inner(subclass):
-            cls.TYPES[name or subclass.__name__] = subclass
-            return subclass
-
-        return _inner
-
-    @classmethod
-    def from_dict(cls, d, app=None):
-        typ = d.get('subtask_type')
-        if typ:
-            target_cls = cls.TYPES[typ]
-            if target_cls is not cls:
-                return target_cls.from_dict(d, app=app)
-        return Signature(d, app=app)
-
-    def __init__(self, task=None, args=None, kwargs=None, options=None,
-                 type=None, subtask_type=None, immutable=False,
-                 app=None, **ex):
-        self._app = app
+    def test_when_no_len_and_no_length_hint(self):
+        g = MagicMock(name='group')
+        g.tasks.__len__.side_effect = TypeError()
+        g.tasks.__length_hint__ = Mock()
+        g.tasks.__length_hint__.return_value = 0
+        assert maybe_unroll_group(g) is g
+        g.tasks.__length_hint__.side_effect = AttributeError()
+        assert maybe_unroll_group(g) is g
 
-        if isinstance(task, dict):
-            super().__init__(task)  # works like dict(d)
-        else:
-            # Also supports using task class/instance instead of string name.
+
+class CanvasCase:
+
+    def setup_method(self):
+        @self.app.task(shared=False)
+        def add(x, y):
+            return x + y
+
+        self.add = add
+
+        @self.app.task(shared=False)
+        def mul(x, y):
+            return x * y
+
+        self.mul = mul
+
+        @self.app.task(shared=False)
+        def div(x, y):
+            return x / y
+
+        self.div = div
+
+        @self.app.task(shared=False)
+        def xsum(numbers):
+            return sum(sum(num) if isinstance(num, Iterable) else num for num in numbers)
+
+        self.xsum = xsum
+
+        @self.app.task(shared=False, bind=True)
+        def replaced(self, x, y):
+            return self.replace(add.si(x, y))
+
+        self.replaced = replaced
+
+        @self.app.task(shared=False, bind=True)
+        def replaced_group(self, x, y):
+            return self.replace(group(add.si(x, y), mul.si(x, y)))
+
+        self.replaced_group = replaced_group
+
+        @self.app.task(shared=False, bind=True)
+        def replace_with_group(self, x, y):
+            return self.replace(group(add.si(x, y), mul.si(x, y)))
+
+        self.replace_with_group = replace_with_group
+
+        @self.app.task(shared=False, bind=True)
+        def replace_with_chain(self, x, y):
+            return self.replace(group(add.si(x, y) | mul.s(y), add.si(x, y)))
+
+        self.replace_with_chain = replace_with_chain
+
+        @self.app.task(shared=False)
+        def xprod(numbers):
             try:
-                task_name = task.name
+                return math.prod(numbers)
             except AttributeError:
-                task_name = task
-            else:
-                self._type = task
-
-            super().__init__(
-                task=task_name, args=tuple(args or ()),
-                kwargs=kwargs or {},
-                options=dict(options or {}, **ex),
-                subtask_type=subtask_type,
-                immutable=immutable,
-            )
+                #  TODO: Drop this backport once
+                #        we drop support for Python 3.7
+                import operator
+                from functools import reduce
 
-    def __call__(self, *partial_args, **partial_kwargs):
-        """Call the task directly (in the current process)."""
-        args, kwargs, _ = self._merge(partial_args, partial_kwargs, None)
-        return self.type(*args, **kwargs)
-
-    def delay(self, *partial_args, **partial_kwargs):
-        """Shortcut to :meth:`apply_async` using star arguments."""
-        return self.apply_async(partial_args, partial_kwargs)
-
-    def apply(self, args=None, kwargs=None, **options):
-        """Call task locally.
-
-        Same as :meth:`apply_async` but executed the task inline instead
-        of sending a task message.
-        """
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        # Extra options set to None are dismissed
-        options = {k: v for k, v in options.items() if v is not None}
-        # For callbacks: extra args are prepended to the stored args.
-        args, kwargs, options = self._merge(args, kwargs, options)
-        return self.type.apply(args, kwargs, **options)
-
-    def apply_async(self, args=None, kwargs=None, route_name=None, **options):
-        """Apply this task asynchronously.
-
-        Arguments:
-            args (Tuple): Partial args to be prepended to the existing args.
-            kwargs (Dict): Partial kwargs to be merged with existing kwargs.
-            options (Dict): Partial options to be merged
-                with existing options.
-
-        Returns:
-            ~@AsyncResult: promise of future evaluation.
-
-        See also:
-            :meth:`~@Task.apply_async` and the :ref:`guide-calling` guide.
-        """
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        # Extra options set to None are dismissed
-        options = {k: v for k, v in options.items() if v is not None}
-        try:
-            _apply = self._apply_async
-        except IndexError:  # pragma: no cover
-            # no tasks for chain, etc to find type
-            return
-        # For callbacks: extra args are prepended to the stored args.
-        if args or kwargs or options:
-            args, kwargs, options = self._merge(args, kwargs, options)
-        else:
-            args, kwargs, options = self.args, self.kwargs, self.options
-        # pylint: disable=too-many-function-args
-        #   Borks on this, as it's a property
-        return _apply(args, kwargs, **options)
-
-    def _merge(self, args=None, kwargs=None, options=None, force=False):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        if options is not None:
-            # We build a new options dictionary where values in `options`
-            # override values in `self.options` except for keys which are
-            # noted as being immutable (unrelated to signature immutability)
-            # implying that allowing their value to change would stall tasks
-            immutable_options = self._IMMUTABLE_OPTIONS
-            if "stamped_headers" in self.options:
-                immutable_options = self._IMMUTABLE_OPTIONS.union(set(self.options["stamped_headers"]))
-            new_options = {**self.options, **{
-                k: v for k, v in options.items()
-                if k not in immutable_options or k not in self.options
-            }}
-        else:
-            new_options = self.options
-        if self.immutable and not force:
-            return (self.args, self.kwargs, new_options)
-        return (tuple(args) + tuple(self.args) if args else self.args,
-                dict(self.kwargs, **kwargs) if kwargs else self.kwargs,
-                new_options)
-
-    def clone(self, args=None, kwargs=None, **opts):
-        """Create a copy of this signature.
-
-        Arguments:
-            args (Tuple): Partial args to be prepended to the existing args.
-            kwargs (Dict): Partial kwargs to be merged with existing kwargs.
-            options (Dict): Partial options to be merged with
-                existing options.
-        """
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        # need to deepcopy options so origins links etc. is not modified.
-        if args or kwargs or opts:
-            args, kwargs, opts = self._merge(args, kwargs, opts)
-        else:
-            args, kwargs, opts = self.args, self.kwargs, self.options
-        signature = Signature.from_dict({'task': self.task,
-                                         'args': tuple(args),
-                                         'kwargs': kwargs,
-                                         'options': deepcopy(opts),
-                                         'subtask_type': self.subtask_type,
-                                         'immutable': self.immutable},
-                                        app=self._app)
-        signature._type = self._type
-        return signature
-
-    partial = clone
-
-    def freeze(self, _id=None, group_id=None, chord=None,
-               root_id=None, parent_id=None, group_index=None):
-        """Finalize the signature by adding a concrete task id.
-
-        The task won't be called and you shouldn't call the signature
-        twice after freezing it as that'll result in two task messages
-        using the same task id.
-
-        Returns:
-            ~@AsyncResult: promise of future evaluation.
-        """
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        opts = self.options
-        try:
-            # if there is already an id for this task, return it
-            tid = opts['task_id']
-        except KeyError:
-            # otherwise, use the _id sent to this function, falling back on a generated UUID
-            tid = opts['task_id'] = _id or uuid()
-        if root_id:
-            opts['root_id'] = root_id
-        if parent_id:
-            opts['parent_id'] = parent_id
-        if 'reply_to' not in opts:
-            # fall back on unique ID for this thread in the app
-            opts['reply_to'] = self.app.thread_oid
-        if group_id and "group_id" not in opts:
-            opts['group_id'] = group_id
-        if chord:
-            opts['chord'] = chord
-        if group_index is not None:
-            opts['group_index'] = group_index
-        # pylint: disable=too-many-function-args
-        #   Borks on this, as it's a property.
-        return self.AsyncResult(tid)
-
-    _freeze = freeze
-
-    def replace(self, args=None, kwargs=None, options=None):
-        """Replace the args, kwargs or options set for this signature.
-
-        These are only replaced if the argument for the section is
-        not :const:`None`.
-        """
-        signature = self.clone()
-        if args is not None:
-            signature.args = args
-        if kwargs is not None:
-            signature.kwargs = kwargs
-        if options is not None:
-            signature.options = options
-        return signature
-
-    def set(self, immutable=None, **options):
-        """Set arbitrary execution options (same as ``.options.update(…)``).
-
-        Returns:
-            Signature: This is a chaining method call
-                (i.e., it will return ``self``).
-        """
-        if immutable is not None:
-            self.set_immutable(immutable)
-        self.options.update(options)
-        return self
-
-    def set_immutable(self, immutable):
-        self.immutable = immutable
-
-    def stamp(self, visitor=None, **headers):
-        """Apply this task asynchronously.
-
-        Arguments:
-            visitor (StampingVisitor): Visitor API object.
-            headers (Dict): Stamps that should be added to headers.
-        """
-        headers = headers.copy()
-        if visitor is not None:
-            headers.update(visitor.on_signature(self, **headers))
-        else:
-            headers["stamped_headers"] = [header for header in headers.keys() if header not in self.options]
-            _merge_dictionaries(headers, self.options)
-        return self.set(**headers)
-
-    def _with_list_option(self, key):
-        items = self.options.setdefault(key, [])
-        if not isinstance(items, MutableSequence):
-            items = self.options[key] = [items]
-        return items
-
-    def append_to_list_option(self, key, value):
-        items = self._with_list_option(key)
-        if value not in items:
-            items.append(value)
-        return value
-
-    def extend_list_option(self, key, value):
-        items = self._with_list_option(key)
-        items.extend(maybe_list(value))
-
-    def link(self, callback):
-        """Add callback task to be applied if this task succeeds.
-
-        Returns:
-            Signature: the argument passed, for chaining
-                or use with :func:`~functools.reduce`.
-        """
-        return self.append_to_list_option('link', callback)
-
-    def link_error(self, errback):
-        """Add callback task to be applied on error in task execution.
-
-        Returns:
-            Signature: the argument passed, for chaining
-                or use with :func:`~functools.reduce`.
-        """
-        return self.append_to_list_option('link_error', errback)
-
-    def on_error(self, errback):
-        """Version of :meth:`link_error` that supports chaining.
-
-        on_error chains the original signature, not the errback so::
-
-            >>> add.s(2, 2).on_error(errback.s()).delay()
-
-        calls the ``add`` task, not the ``errback`` task, but the
-        reverse is true for :meth:`link_error`.
-        """
-        self.link_error(errback)
-        return self
-
-    def flatten_links(self):
-        """Return a recursive list of dependencies.
-
-        "unchain" if you will, but with links intact.
-        """
-        return list(itertools.chain.from_iterable(itertools.chain(
-            [[self]],
-            (link.flatten_links()
-             for link in maybe_list(self.options.get('link')) or [])
-        )))
-
-    def __or__(self, other):
-        if isinstance(other, _chain):
-            # task | chain -> chain
-            return _chain(seq_concat_seq(
-                (self,), other.unchain_tasks()), app=self._app)
-        elif isinstance(other, group):
-            # unroll group with one member
-            other = maybe_unroll_group(other)
-            # task | group() -> chain
-            return _chain(self, other, app=self.app)
-        elif isinstance(other, Signature):
-            # task | task -> chain
-            return _chain(self, other, app=self._app)
-        return NotImplemented
-
-    def __ior__(self, other):
-        # Python 3.9 introduces | as the merge operator for dicts.
-        # We override the in-place version of that operator
-        # so that canvases continue to work as they did before.
-        return self.__or__(other)
-
-    def election(self):
-        type = self.type
-        app = type.app
-        tid = self.options.get('task_id') or uuid()
-
-        with app.producer_or_acquire(None) as producer:
-            props = type.backend.on_task_call(producer, tid)
-            app.control.election(tid, 'task',
-                                 self.clone(task_id=tid, **props),
-                                 connection=producer.connection)
-            return type.AsyncResult(tid)
-
-    def reprcall(self, *args, **kwargs):
-        args, kwargs, _ = self._merge(args, kwargs, {}, force=True)
-        return reprcall(self['task'], args, kwargs)
-
-    def __deepcopy__(self, memo):
-        memo[id(self)] = self
-        return dict(self)
-
-    def __invert__(self):
-        return self.apply_async().get()
-
-    def __reduce__(self):
-        # for serialization, the task type is lazily loaded,
-        # and not stored in the dict itself.
-        return signature, (dict(self),)
-
-    def __json__(self):
-        return dict(self)
-
-    def __repr__(self):
-        return self.reprcall()
-
-    def items(self):
-        for k, v in super().items():
-            yield k.decode() if isinstance(k, bytes) else k, v
-
-    @property
-    def name(self):
-        # for duck typing compatibility with Task.name
-        return self.task
-
-    @cached_property
-    def type(self):
-        return self._type or self.app.tasks[self['task']]
-
-    @cached_property
-    def app(self):
-        return self._app or current_app
+                return reduce(operator.mul, numbers)
 
-    @cached_property
-    def AsyncResult(self):
-        try:
-            return self.type.AsyncResult
-        except KeyError:  # task not registered
-            return self.app.AsyncResult
+        self.xprod = xprod
 
-    @cached_property
-    def _apply_async(self):
-        try:
-            return self.type.apply_async
-        except KeyError:
-            return _partial(self.app.send_task, self['task'])
-
-    id = getitem_property('options.task_id', 'Task UUID')
-    parent_id = getitem_property('options.parent_id', 'Task parent UUID.')
-    root_id = getitem_property('options.root_id', 'Task root UUID.')
-    task = getitem_property('task', 'Name of task.')
-    args = getitem_property('args', 'Positional arguments to task.')
-    kwargs = getitem_property('kwargs', 'Keyword arguments to task.')
-    options = getitem_property('options', 'Task execution options.')
-    subtask_type = getitem_property('subtask_type', 'Type of signature')
-    immutable = getitem_property(
-        'immutable', 'Flag set if no longer accepts new arguments')
-
-
-def _prepare_chain_from_options(options, tasks, use_link):
-    # When we publish groups we reuse the same options dictionary for all of
-    # the tasks in the group. See:
-    # https://github.com/celery/celery/blob/fb37cb0b8/celery/canvas.py#L1022.
-    # Issue #5354 reported that the following type of canvases
-    # causes a Celery worker to hang:
-    # group(
-    #   add.s(1, 1),
-    #   add.s(1, 1)
-    # ) | tsum.s() | add.s(1) | group(add.s(1), add.s(1))
-    # The resolution of #5354 in PR #5681 was to only set the `chain` key
-    # in the options dictionary if it is not present.
-    # Otherwise we extend the existing list of tasks in the chain with the new
-    # tasks: options['chain'].extend(chain_).
-    # Before PR #5681 we overrode the `chain` key in each iteration
-    # of the loop which applies all the tasks in the group:
-    # options['chain'] = tasks if not use_link else None
-    # This caused Celery to execute chains correctly in most cases since
-    # in each iteration the `chain` key would reset itself to a new value
-    # and the side effect of mutating the key did not propagate
-    # to the next task in the group.
-    # Since we now mutated the `chain` key, a *list* which is passed
-    # by *reference*, the next task in the group will extend the list
-    # of tasks in the chain instead of setting a new one from the chain_
-    # variable above.
-    # This causes Celery to execute a chain, even though there might not be
-    # one to begin with. Alternatively, it causes Celery to execute more tasks
-    # that were previously present in the previous task in the group.
-    # The solution is to be careful and never mutate the options dictionary
-    # to begin with.
-    # Here is an example of a canvas which triggers this issue:
-    # add.s(5, 6) | group((add.s(1) | add.s(2), add.s(3))).
-    # The expected result is [14, 14]. However, when we extend the `chain`
-    # key the `add.s(3)` task erroneously has `add.s(2)` in its chain since
-    # it was previously applied to `add.s(1)`.
-    # Without being careful not to mutate the options dictionary, the result
-    # in this case is [16, 14].
-    # To avoid deep-copying the entire options dictionary every single time we
-    # run a chain we use a ChainMap and ensure that we never mutate
-    # the original `chain` key, hence we use list_a + list_b to create a new
-    # list.
-    if use_link:
-        return ChainMap({'chain': None}, options)
-    elif 'chain' not in options:
-        return ChainMap({'chain': tasks}, options)
-    elif tasks is not None:
-        # chain option may already be set, resulting in
-        # "multiple values for keyword argument 'chain'" error.
-        # Issue #3379.
-        # If a chain already exists, we need to extend it with the next
-        # tasks in the chain.
-        # Issue #5354.
-        # WARNING: Be careful not to mutate `options['chain']`.
-        return ChainMap({'chain': options['chain'] + tasks},
-                        options)
-
-
-@Signature.register_type(name='chain')
-class _chain(Signature):
-    tasks = getitem_property('kwargs.tasks', 'Tasks in chain.')
-
-    @classmethod
-    def from_dict(cls, d, app=None):
-        tasks = d['kwargs']['tasks']
-        if tasks:
-            if isinstance(tasks, tuple):  # aaaargh
-                tasks = d['kwargs']['tasks'] = list(tasks)
-            tasks = [maybe_signature(task, app=app) for task in tasks]
-        return cls(tasks, app=app, **d['options'])
-
-    def __init__(self, *tasks, **options):
-        tasks = (regen(tasks[0]) if len(tasks) == 1 and is_list(tasks[0])
-                 else tasks)
-        super().__init__('celery.chain', (), {'tasks': tasks}, **options
-                         )
-        self._use_link = options.pop('use_link', None)
-        self.subtask_type = 'chain'
-        self._frozen = None
-
-    def __call__(self, *args, **kwargs):
-        if self.tasks:
-            return self.apply_async(args, kwargs)
-
-    def __or__(self, other):
-        if isinstance(other, group):
-            # unroll group with one member
-            other = maybe_unroll_group(other)
-            # chain | group() -> chain
-            tasks = self.unchain_tasks()
-            if not tasks:
-                # If the chain is empty, return the group
-                return other
-            # use type(self) for _chain subclasses
-            return type(self)(seq_concat_item(
-                tasks, other), app=self._app)
-        elif isinstance(other, _chain):
-            # chain | chain -> chain
-            # use type(self) for _chain subclasses
-            return type(self)(seq_concat_seq(
-                self.unchain_tasks(), other.unchain_tasks()), app=self._app)
-        elif isinstance(other, Signature):
-            if self.tasks and isinstance(self.tasks[-1], group):
-                # CHAIN [last item is group] | TASK -> chord
-                sig = self.clone()
-                sig.tasks[-1] = chord(
-                    sig.tasks[-1], other, app=self._app)
-                return sig
-            elif self.tasks and isinstance(self.tasks[-1], chord):
-                # CHAIN [last item is chord] -> chain with chord body.
-                sig = self.clone()
-                sig.tasks[-1].body = sig.tasks[-1].body | other
-                return sig
-            else:
-                # chain | task -> chain
-                # use type(self) for _chain subclasses
-                return type(self)(seq_concat_item(
-                    self.unchain_tasks(), other), app=self._app)
-        else:
-            return NotImplemented
 
-    def clone(self, *args, **kwargs):
-        to_signature = maybe_signature
-        signature = super().clone(*args, **kwargs)
-        signature.kwargs['tasks'] = [
-            to_signature(sig, app=self._app, clone=True)
-            for sig in signature.kwargs['tasks']
-        ]
-        return signature
+@Signature.register_type()
+class chord_subclass(chord):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subtask_type = "chord_subclass"
 
-    def unchain_tasks(self):
-        # Clone chain's tasks assigning signatures from link_error
-        # to each task
-        tasks = [t.clone() for t in self.tasks]
-        for sig in self.options.get('link_error', []):
-            for task in tasks:
-                task.link_error(sig)
-        return tasks
-
-    def apply_async(self, args=None, kwargs=None, **options):
-        # python is best at unpacking kwargs, so .run is here to do that.
-        args = args if args else ()
-        kwargs = kwargs if kwargs else []
-        app = self.app
-
-        if app.conf.task_always_eager:
-            with allow_join_result():
-                return self.apply(args, kwargs, **options)
-        return self.run(args, kwargs, app=app, **(
-            dict(self.options, **options) if options else self.options))
-
-    def run(self, args=None, kwargs=None, group_id=None, chord=None,
-            task_id=None, link=None, link_error=None, publisher=None,
-            producer=None, root_id=None, parent_id=None, app=None,
-            group_index=None, **options):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        args = args if args else ()
-        kwargs = kwargs if kwargs else []
-        app = app or self.app
-        use_link = self._use_link
-        if use_link is None and app.conf.task_protocol == 1:
-            use_link = True
-        args = (tuple(args) + tuple(self.args)
-                if args and not self.immutable else self.args)
-
-        tasks, results_from_prepare = self.prepare_steps(
-            args, kwargs, self.tasks, root_id, parent_id, link_error, app,
-            task_id, group_id, chord, group_index=group_index,
-        )
-
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-
-        if results_from_prepare:
-            if link:
-                tasks[0].extend_list_option('link', link)
-            first_task = tasks.pop()
-            options = _prepare_chain_from_options(options, tasks, use_link)
-
-            result_from_apply = first_task.apply_async(**options)
-            # If we only have a single task, it may be important that we pass
-            # the real result object rather than the one obtained via freezing.
-            # e.g. For `GroupResult`s, we need to pass back the result object
-            # which will actually have its promise fulfilled by the subtasks,
-            # something that will never occur for the frozen result.
-            if not tasks:
-                return result_from_apply
-            else:
-                return results_from_prepare[0]
-
-    # in order for a chain to be frozen, each of the members of the chain individually needs to be frozen
-    # TODO figure out why we are always cloning before freeze
-    def freeze(self, _id=None, group_id=None, chord=None,
-               root_id=None, parent_id=None, group_index=None):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        _, results = self._frozen = self.prepare_steps(
-            self.args, self.kwargs, self.tasks, root_id, parent_id, None,
-            self.app, _id, group_id, chord, clone=False,
+
+@Signature.register_type()
+class group_subclass(group):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subtask_type = "group_subclass"
+
+
+@Signature.register_type()
+class chain_subclass(chain):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subtask_type = "chain_subclass"
+
+
+@Signature.register_type()
+class chunks_subclass(chunks):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.subtask_type = "chunks_subclass"
+
+
+class test_Signature(CanvasCase):
+    def test_getitem_property_class(self):
+        assert Signature.task
+        assert Signature.args
+        assert Signature.kwargs
+        assert Signature.options
+        assert Signature.subtask_type
+
+    def test_getitem_property(self):
+        assert SIG.task == 'TASK'
+        assert SIG.args == ('A1',)
+        assert SIG.kwargs == {'K1': 'V1'}
+        assert SIG.options == {'task_id': 'TASK_ID'}
+        assert SIG.subtask_type == ''
+
+    def test_call(self):
+        x = Signature('foo', (1, 2), {'arg1': 33}, app=self.app)
+        x.type = Mock(name='type')
+        x(3, 4, arg2=66)
+        x.type.assert_called_with(3, 4, 1, 2, arg1=33, arg2=66)
+
+    def test_link_on_scalar(self):
+        x = Signature('TASK', link=Signature('B'))
+        assert x.options['link']
+        x.link(Signature('C'))
+        assert isinstance(x.options['link'], list)
+        assert Signature('B') in x.options['link']
+        assert Signature('C') in x.options['link']
+
+    def test_json(self):
+        x = Signature('TASK', link=Signature('B', app=self.app), app=self.app)
+        assert x.__json__() == dict(x)
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_reduce(self):
+        x = Signature('TASK', (2, 4), app=self.app)
+        fun, args = x.__reduce__()
+        assert fun(*args) == x
+
+    def test_replace(self):
+        x = Signature('TASK', ('A',), {})
+        assert x.replace(args=('B',)).args == ('B',)
+        assert x.replace(kwargs={'FOO': 'BAR'}).kwargs == {
+            'FOO': 'BAR',
+        }
+        assert x.replace(options={'task_id': '123'}).options == {
+            'task_id': '123',
+        }
+
+    def test_set(self):
+        assert Signature('TASK', x=1).set(task_id='2').options == {
+            'x': 1, 'task_id': '2',
+        }
+
+    def test_link(self):
+        x = signature(SIG)
+        x.link(SIG)
+        x.link(SIG)
+        assert SIG in x.options['link']
+        assert len(x.options['link']) == 1
+
+    def test_link_error(self):
+        x = signature(SIG)
+        x.link_error(SIG)
+        x.link_error(SIG)
+        assert SIG in x.options['link_error']
+        assert len(x.options['link_error']) == 1
+
+    def test_flatten_links(self):
+        tasks = [self.add.s(2, 2), self.mul.s(4), self.div.s(2)]
+        tasks[0].link(tasks[1])
+        tasks[1].link(tasks[2])
+        assert tasks[0].flatten_links() == tasks
+
+    def test_OR(self, subtests):
+        x = self.add.s(2, 2) | self.mul.s(4)
+        assert isinstance(x, _chain)
+        y = self.add.s(4, 4) | self.div.s(2)
+        z = x | y
+        assert isinstance(y, _chain)
+        assert isinstance(z, _chain)
+        assert len(z.tasks) == 4
+        with pytest.raises(TypeError):
+            x | 10
+        ax = self.add.s(2, 2) | (self.add.s(4) | self.add.s(8))
+        assert isinstance(ax, _chain)
+        assert len(ax.tasks), 3 == 'consolidates chain to chain'
+
+        with subtests.test('Test chaining with a non-signature object'):
+            with pytest.raises(TypeError):
+                assert signature('foo') | None
+
+    def test_INVERT(self):
+        x = self.add.s(2, 2)
+        x.apply_async = Mock()
+        x.apply_async.return_value = Mock()
+        x.apply_async.return_value.get = Mock()
+        x.apply_async.return_value.get.return_value = 4
+        assert ~x == 4
+        x.apply_async.assert_called()
+
+    def test_merge_immutable(self):
+        x = self.add.si(2, 2, foo=1)
+        args, kwargs, options = x._merge((4,), {'bar': 2}, {'task_id': 3})
+        assert args == (2, 2)
+        assert kwargs == {'foo': 1}
+        assert options == {'task_id': 3}
+
+    def test_merge_options__none(self):
+        sig = self.add.si()
+        _, _, new_options = sig._merge()
+        assert new_options is sig.options
+        _, _, new_options = sig._merge(options=None)
+        assert new_options is sig.options
+
+    @pytest.mark.parametrize("immutable_sig", (True, False))
+    def test_merge_options__group_id(self, immutable_sig):
+        # This is to avoid testing the behaviour in `test_set_immutable()`
+        if immutable_sig:
+            sig = self.add.si()
+        else:
+            sig = self.add.s()
+        # If the signature has no group ID, it can be set
+        assert not sig.options
+        _, _, new_options = sig._merge(options={"group_id": sentinel.gid})
+        assert new_options == {"group_id": sentinel.gid}
+        # But if one is already set, the new one is silently ignored
+        sig.set(group_id=sentinel.old_gid)
+        _, _, new_options = sig._merge(options={"group_id": sentinel.new_gid})
+        assert new_options == {"group_id": sentinel.old_gid}
+
+    def test_set_immutable(self):
+        x = self.add.s(2, 2)
+        assert not x.immutable
+        x.set(immutable=True)
+        assert x.immutable
+        x.set(immutable=False)
+        assert not x.immutable
+
+    def test_election(self):
+        x = self.add.s(2, 2)
+        x.freeze('foo')
+        x.type.app.control = Mock()
+        r = x.election()
+        x.type.app.control.election.assert_called()
+        assert r.id == 'foo'
+
+    def test_AsyncResult_when_not_registered(self):
+        s = signature('xxx.not.registered', app=self.app)
+        assert s.AsyncResult
+
+    def test_apply_async_when_not_registered(self):
+        s = signature('xxx.not.registered', app=self.app)
+        assert s._apply_async
+
+    def test_keeping_link_error_on_chaining(self):
+        x = self.add.s(2, 2) | self.mul.s(4)
+        assert isinstance(x, _chain)
+        x.link_error(SIG)
+        assert SIG in x.options['link_error']
+
+        t = signature(SIG)
+        z = x | t
+        assert isinstance(z, _chain)
+        assert t in z.tasks
+        assert not z.options.get('link_error')
+        assert SIG in z.tasks[0].options['link_error']
+        assert not z.tasks[2].options.get('link_error')
+        assert SIG in x.options['link_error']
+        assert t not in x.tasks
+        assert not x.tasks[0].options.get('link_error')
+
+        z = t | x
+        assert isinstance(z, _chain)
+        assert t in z.tasks
+        assert not z.options.get('link_error')
+        assert SIG in z.tasks[1].options['link_error']
+        assert not z.tasks[0].options.get('link_error')
+        assert SIG in x.options['link_error']
+        assert t not in x.tasks
+        assert not x.tasks[0].options.get('link_error')
+
+        y = self.add.s(4, 4) | self.div.s(2)
+        assert isinstance(y, _chain)
+
+        z = x | y
+        assert isinstance(z, _chain)
+        assert not z.options.get('link_error')
+        assert SIG in z.tasks[0].options['link_error']
+        assert not z.tasks[2].options.get('link_error')
+        assert SIG in x.options['link_error']
+        assert not x.tasks[0].options.get('link_error')
+
+        z = y | x
+        assert isinstance(z, _chain)
+        assert not z.options.get('link_error')
+        assert SIG in z.tasks[3].options['link_error']
+        assert not z.tasks[1].options.get('link_error')
+        assert SIG in x.options['link_error']
+        assert not x.tasks[0].options.get('link_error')
+
+    def test_signature_on_error_adds_error_callback(self):
+        sig = signature('sig').on_error(signature('on_error'))
+        assert sig.options['link_error'] == [signature('on_error')]
+
+    @pytest.mark.parametrize('_id, group_id, chord, root_id, parent_id, group_index', [
+        ('_id', 'group_id', 'chord', 'root_id', 'parent_id', 1),
+    ])
+    def test_freezing_args_set_in_options(self, _id, group_id, chord, root_id, parent_id, group_index):
+        sig = self.add.s(1, 1)
+        sig.freeze(
+            _id=_id,
+            group_id=group_id,
+            chord=chord,
+            root_id=root_id,
+            parent_id=parent_id,
             group_index=group_index,
         )
-        return results[0]
+        options = sig.options
 
-    def stamp(self, visitor=None, **headers):
-        if visitor is not None:
-            headers.update(visitor.on_chain_start(self, **headers))
-
-        super().stamp(visitor=visitor, **headers)
-        for task in self.tasks:
-            task.stamp(visitor=visitor, **headers)
-
-        if visitor is not None:
-            visitor.on_chain_end(self, **headers)
-
-    def prepare_steps(self, args, kwargs, tasks,
-                      root_id=None, parent_id=None, link_error=None, app=None,
-                      last_task_id=None, group_id=None, chord_body=None,
-                      clone=True, from_dict=Signature.from_dict,
-                      group_index=None):
-        app = app or self.app
-        # use chain message field for protocol 2 and later.
-        # this avoids pickle blowing the stack on the recursion
-        # required by linking task together in a tree structure.
-        # (why is pickle using recursion? or better yet why cannot python
-        #  do tail call optimization making recursion actually useful?)
-        use_link = self._use_link
-        if use_link is None and app.conf.task_protocol == 1:
-            use_link = True
-        steps = deque(tasks)
-
-        # optimization: now the pop func is a local variable
-        steps_pop = steps.pop
-        steps_extend = steps.extend
-
-        prev_task = None
-        prev_res = None
-        tasks, results = [], []
-        i = 0
-        # NOTE: We are doing this in reverse order.
-        # The result is a list of tasks in reverse order, that is
-        # passed as the ``chain`` message field.
-        # As it's reversed the worker can just do ``chain.pop()`` to
-        # get the next task in the chain.
-        while steps:
-            task = steps_pop()
-            # if steps is not empty, this is the first task - reverse order
-            # if i = 0, this is the last task - again, because we're reversed
-            is_first_task, is_last_task = not steps, not i
-
-            if not isinstance(task, abstract.CallableSignature):
-                task = from_dict(task, app=app)
-            if isinstance(task, group):
-                # when groups are nested, they are unrolled - all tasks within
-                # groups should be called in parallel
-                task = maybe_unroll_group(task)
-
-            # first task gets partial args from chain
-            if clone:
-                if is_first_task:
-                    task = task.clone(args, kwargs)
-                else:
-                    task = task.clone()
-            elif is_first_task:
-                task.args = tuple(args) + tuple(task.args)
-
-            if isinstance(task, _chain):
-                # splice (unroll) the chain
-                steps_extend(task.tasks)
-                continue
-
-            # TODO why isn't this asserting is_last_task == False?
-            if isinstance(task, group) and prev_task:
-                # automatically upgrade group(...) | s to chord(group, s)
-                # for chords we freeze by pretending it's a normal
-                # signature instead of a group.
-                tasks.pop()
-                results.pop()
-                try:
-                    task = chord(
-                        task, body=prev_task,
-                        task_id=prev_res.task_id, root_id=root_id, app=app,
-                    )
-                except AttributeError:
-                    # A GroupResult does not have a task_id since it consists
-                    # of multiple tasks.
-                    # We therefore, have to construct the chord without it.
-                    # Issues #5467, #3585.
-                    task = chord(
-                        task, body=prev_task,
-                        root_id=root_id, app=app,
-                    )
-
-            if is_last_task:
-                # chain(task_id=id) means task id is set for the last task
-                # in the chain.  If the chord is part of a chord/group
-                # then that chord/group must synchronize based on the
-                # last task in the chain, so we only set the group_id and
-                # chord callback for the last task.
-                res = task.freeze(
-                    last_task_id,
-                    root_id=root_id, group_id=group_id, chord=chord_body,
-                    group_index=group_index,
-                )
-            else:
-                res = task.freeze(root_id=root_id)
-
-            i += 1
-
-            if prev_task:
-                if use_link:
-                    # link previous task to this task.
-                    task.link(prev_task)
-
-                if prev_res and not prev_res.parent:
-                    prev_res.parent = res
-
-            if link_error:
-                for errback in maybe_list(link_error):
-                    task.link_error(errback)
-
-            tasks.append(task)
-            results.append(res)
-
-            prev_task, prev_res = task, res
-            if isinstance(task, chord):
-                app.backend.ensure_chords_allowed()
-                # If the task is a chord, and the body is a chain
-                # the chain has already been prepared, and res is
-                # set to the last task in the callback chain.
-
-                # We need to change that so that it points to the
-                # group result object.
-                node = res
-                while node.parent:
-                    node = node.parent
-                prev_res = node
-        return tasks, results
-
-    def apply(self, args=None, kwargs=None, **options):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        last, (fargs, fkwargs) = None, (args, kwargs)
-        for task in self.tasks:
-            res = task.clone(fargs, fkwargs).apply(
-                last and (last.get(),), **dict(self.options, **options))
-            res.parent, last, (fargs, fkwargs) = last, res, (None, None)
-        return last
-
-    @property
-    def app(self):
-        app = self._app
-        if app is None:
-            try:
-                app = self.tasks[0]._app
-            except LookupError:
-                pass
-        return app or current_app
+        assert options['task_id'] == _id
+        assert options['group_id'] == group_id
+        assert options['chord'] == chord
+        assert options['root_id'] == root_id
+        assert options['parent_id'] == parent_id
+        assert options['group_index'] == group_index
+
+
+class test_xmap_xstarmap(CanvasCase):
+
+    def test_apply(self):
+        for type, attr in [(xmap, 'map'), (xstarmap, 'starmap')]:
+            args = [(i, i) for i in range(10)]
+            s = getattr(self.add, attr)(args)
+            s.type = Mock()
+
+            s.apply_async(foo=1)
+            s.type.apply_async.assert_called_with(
+                (), {'task': self.add.s(), 'it': args}, foo=1,
+                route_name=self.add.name,
+            )
 
-    def __repr__(self):
-        if not self.tasks:
-            return f'<{type(self).__name__}@{id(self):#x}: empty>'
-        return remove_repeating_from_task(
-            self.tasks[0]['task'],
-            ' | '.join(repr(t) for t in self.tasks))
-
-
-class chain(_chain):
-    """Chain tasks together.
-
-    Each tasks follows one another,
-    by being applied as a callback of the previous task.
-
-    Note:
-        If called with only one argument, then that argument must
-        be an iterable of tasks to chain: this allows us
-        to use generator expressions.
-
-    Example:
-        This is effectively :math:`((2 + 2) + 4)`:
-
-        .. code-block:: pycon
-
-            >>> res = chain(add.s(2, 2), add.s(4))()
-            >>> res.get()
-            8
-
-        Calling a chain will return the result of the last task in the chain.
-        You can get to the other tasks by following the ``result.parent``'s:
-
-        .. code-block:: pycon
-
-            >>> res.parent.get()
-            4
-
-        Using a generator expression:
-
-        .. code-block:: pycon
-
-            >>> lazy_chain = chain(add.s(i) for i in range(10))
-            >>> res = lazy_chain(3)
-
-    Arguments:
-        *tasks (Signature): List of task signatures to chain.
-            If only one argument is passed and that argument is
-            an iterable, then that'll be used as the list of signatures
-            to chain instead.  This means that you can use a generator
-            expression.
-
-    Returns:
-        ~celery.chain: A lazy signature that can be called to apply the first
-            task in the chain.  When that task succeeds the next task in the
-            chain is applied, and so on.
-    """
-
-    # could be function, but must be able to reference as :class:`chain`.
-    def __new__(cls, *tasks, **kwargs):
-        # This forces `chain(X, Y, Z)` to work the same way as `X | Y | Z`
-        if not kwargs and tasks:
-            if len(tasks) != 1 or is_list(tasks[0]):
-                tasks = tasks[0] if len(tasks) == 1 else tasks
-                # if is_list(tasks) and len(tasks) == 1:
-                #     return super(chain, cls).__new__(cls, tasks, **kwargs)
-                new_instance = reduce(operator.or_, tasks, _chain())
-                if cls != chain and isinstance(new_instance, _chain) and not isinstance(new_instance, cls):
-                    return super().__new__(cls, new_instance.tasks, **kwargs)
-                return new_instance
-        return super().__new__(cls, *tasks, **kwargs)
-
-
-class _basemap(Signature):
-    _task_name = None
-    _unpack_args = itemgetter('task', 'it')
-
-    @classmethod
-    def from_dict(cls, d, app=None):
-        return cls(*cls._unpack_args(d['kwargs']), app=app, **d['options'])
-
-    def __init__(self, task, it, **options):
-        super().__init__(self._task_name, (),
-                         {'task': task, 'it': regen(it)}, immutable=True, **options
-                         )
-
-    def apply_async(self, args=None, kwargs=None, **opts):
-        # need to evaluate generators
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        task, it = self._unpack_args(self.kwargs)
-        return self.type.apply_async(
-            (), {'task': task, 'it': list(it)},
-            route_name=task_name_from(self.kwargs.get('task')), **opts
-        )
+            assert type.from_dict(dict(s)) == s
+            assert repr(s)
 
 
-@Signature.register_type()
-class xmap(_basemap):
-    """Map operation for tasks.
+class test_chunks(CanvasCase):
 
-    Note:
-        Tasks executed sequentially in process, this is not a
-        parallel operation like :class:`group`.
-    """
-
-    _task_name = 'celery.map'
-
-    def __repr__(self):
-        task, it = self._unpack_args(self.kwargs)
-        return f'[{task.task}(x) for x in {truncate(repr(it), 100)}]'
+    def test_chunks_preserves_state(self):
+        x = self.add.chunks(range(100), 10)
+        d = dict(x)
+        d['subtask_type'] = "chunks_subclass"
+        isinstance(chunks_subclass.from_dict(d), chunks_subclass)
+        isinstance(chunks_subclass.from_dict(d).clone(), chunks_subclass)
+
+    def test_chunks(self):
+        x = self.add.chunks(range(100), 10)
+        assert dict(chunks.from_dict(dict(x), app=self.app)) == dict(x)
+
+        assert x.group()
+        assert len(x.group().tasks) == 10
+
+        x.group = Mock()
+        gr = x.group.return_value = Mock()
+
+        x.apply_async()
+        gr.apply_async.assert_called_with((), {}, route_name=self.add.name)
+        gr.apply_async.reset_mock()
+        x()
+        gr.apply_async.assert_called_with((), {}, route_name=self.add.name)
+
+        self.app.conf.task_always_eager = True
+        chunks.apply_chunks(app=self.app, **x['kwargs'])
+
+
+class test_chain(CanvasCase):
+
+    def test_chain_of_chain_with_a_single_task(self):
+        s = self.add.s(1, 1)
+        assert chain([chain(s)]).tasks == list(chain(s).tasks)
+
+    @pytest.mark.parametrize("chain_type", (_chain, chain_subclass))
+    def test_clone_preserves_state(self, chain_type):
+        x = chain_type(self.add.s(i, i) for i in range(10))
+        assert x.clone().tasks == x.tasks
+        assert x.clone().kwargs == x.kwargs
+        assert x.clone().args == x.args
+        assert isinstance(x.clone(), chain_type)
+
+    def test_repr(self):
+        x = self.add.s(2, 2) | self.add.s(2)
+        assert repr(x) == f'{self.add.name}(2, 2) | add(2)'
+
+    def test_apply_async(self):
+        c = self.add.s(2, 2) | self.add.s(4) | self.add.s(8)
+        result = c.apply_async()
+        assert result.parent
+        assert result.parent.parent
+        assert result.parent.parent.parent is None
+
+    @pytest.mark.parametrize("chain_type", (_chain, chain_subclass))
+    def test_splices_chains(self, chain_type):
+        c = chain_type(
+            self.add.s(5, 5),
+            chain_type(self.add.s(6), self.add.s(7), self.add.s(8), app=self.app),
+            app=self.app,
+        )
+        c.freeze()
+        tasks, _ = c._frozen
+        assert len(tasks) == 4
+        assert isinstance(c, chain_type)
+
+    @pytest.mark.parametrize("chain_type", [_chain, chain_subclass])
+    def test_from_dict_no_tasks(self, chain_type):
+        assert chain_type.from_dict(dict(chain_type(app=self.app)), app=self.app)
+        assert isinstance(chain_type.from_dict(dict(chain_type(app=self.app)), app=self.app), chain_type)
+
+    @pytest.mark.parametrize("chain_type", [_chain, chain_subclass])
+    def test_from_dict_full_subtasks(self, chain_type):
+        c = chain_type(self.add.si(1, 2), self.add.si(3, 4), self.add.si(5, 6))
+        serialized = json.loads(json.dumps(c))
+        deserialized = chain_type.from_dict(serialized)
+        assert all(isinstance(task, Signature) for task in deserialized.tasks)
+        assert isinstance(deserialized, chain_type)
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_app_falls_back_to_default(self):
+        from celery._state import current_app
+        assert chain().app is current_app
+
+    def test_handles_dicts(self):
+        c = chain(
+            self.add.s(5, 5), dict(self.add.s(8)), app=self.app,
+        )
+        c.freeze()
+        tasks, _ = c._frozen
+        assert all(isinstance(task, Signature) for task in tasks)
+        assert all(task.app is self.app for task in tasks)
+
+    def test_groups_in_chain_to_chord(self):
+        g1 = group([self.add.s(2, 2), self.add.s(4, 4)])
+        g2 = group([self.add.s(3, 3), self.add.s(5, 5)])
+        c = g1 | g2
+        assert isinstance(c, chord)
+
+    def test_group_to_chord(self):
+        c = (
+            self.add.s(5) |
+            group([self.add.s(i, i) for i in range(5)], app=self.app) |
+            self.add.s(10) |
+            self.add.s(20) |
+            self.add.s(30)
+        )
+        c._use_link = True
+        tasks, results = c.prepare_steps((), {}, c.tasks)
 
+        assert tasks[-1].args[0] == 5
+        assert isinstance(tasks[-2], chord)
+        assert len(tasks[-2].tasks) == 5
+
+        body = tasks[-2].body
+        assert len(body.tasks) == 3
+        assert body.tasks[0].args[0] == 10
+        assert body.tasks[1].args[0] == 20
+        assert body.tasks[2].args[0] == 30
+
+        c2 = self.add.s(2, 2) | group(self.add.s(i, i) for i in range(10))
+        c2._use_link = True
+        tasks2, _ = c2.prepare_steps((), {}, c2.tasks)
+        assert isinstance(tasks2[0], group)
+
+    def test_group_to_chord__protocol_2__or(self):
+        c = (
+            group([self.add.s(i, i) for i in range(5)], app=self.app) |
+            self.add.s(10) |
+            self.add.s(20) |
+            self.add.s(30)
+        )
+        assert isinstance(c, chord)
 
-@Signature.register_type()
-class xstarmap(_basemap):
-    """Map operation for tasks, using star arguments."""
+    def test_group_to_chord__protocol_2(self):
+        c = chain(
+            group([self.add.s(i, i) for i in range(5)], app=self.app),
+            self.add.s(10),
+            self.add.s(20),
+            self.add.s(30)
+        )
+        assert isinstance(c, chord)
+        assert isinstance(c.body, _chain)
+        assert len(c.body.tasks) == 3
+
+        c2 = self.add.s(2, 2) | group(self.add.s(i, i) for i in range(10))
+        c2._use_link = False
+        tasks2, _ = c2.prepare_steps((), {}, c2.tasks)
+        assert isinstance(tasks2[0], group)
+
+    def test_chord_to_chain(self):
+        c = (
+            chord([self.add.s('x0', 'y0'), self.add.s('x1', 'y1')],
+                  self.add.s(['foo'])) |
+            chain(self.add.s(['y']), self.add.s(['z']))
+        )
+        assert isinstance(c, _chain)
+        assert c.apply().get() == ['x0y0', 'x1y1', 'foo', 'y', 'z']
 
-    _task_name = 'celery.starmap'
+    def test_chord_to_group(self):
+        c = (
+            chord([self.add.s('x0', 'y0'), self.add.s('x1', 'y1')],
+                  self.add.s(['foo'])) |
+            group([self.add.s(['y']), self.add.s(['z'])])
+        )
+        assert isinstance(c, _chain)
+        assert c.apply().get() == [
+            ['x0y0', 'x1y1', 'foo', 'y'],
+            ['x0y0', 'x1y1', 'foo', 'z']
+        ]
 
-    def __repr__(self):
-        task, it = self._unpack_args(self.kwargs)
-        return f'[{task.task}(*x) for x in {truncate(repr(it), 100)}]'
+    def test_chain_of_chord__or__group_of_single_task(self):
+        c = chord([signature('header')], signature('body'))
+        c = chain(c)
+        g = group(signature('t'))
+        new_chain = c | g  # g should be chained with the body of c[0]
+        assert isinstance(new_chain, _chain)
+        assert isinstance(new_chain.tasks[0].body, _chain)
 
+    def test_chain_of_chord_upgrade_on_chaining(self):
+        c = chord([signature('header')], group(signature('body')))
+        c = chain(c)
+        t = signature('t')
+        new_chain = c | t  # t should be chained with the body of c[0] and create a new chord
+        assert isinstance(new_chain, _chain)
+        assert isinstance(new_chain.tasks[0].body, chord)
 
-@Signature.register_type()
-class chunks(Signature):
-    """Partition of tasks into chunks of size n."""
+    def test_apply_options(self):
 
-    _unpack_args = itemgetter('task', 'it', 'n')
+        class static(Signature):
 
-    @classmethod
-    def from_dict(cls, d, app=None):
-        return cls(*cls._unpack_args(d['kwargs']), app=app, **d['options'])
-
-    def __init__(self, task, it, n, **options):
-        super().__init__('celery.chunks', (),
-                         {'task': task, 'it': regen(it), 'n': n},
-                         immutable=True, **options
-                         )
-
-    def __call__(self, **options):
-        return self.apply_async(**options)
-
-    def apply_async(self, args=None, kwargs=None, **opts):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        return self.group().apply_async(
-            args, kwargs,
-            route_name=task_name_from(self.kwargs.get('task')), **opts
-        )
-
-    def group(self):
-        # need to evaluate generators
-        task, it, n = self._unpack_args(self.kwargs)
-        return group((xstarmap(task, part, app=self._app)
-                      for part in _chunks(iter(it), n)),
-                     app=self._app)
-
-    @classmethod
-    def apply_chunks(cls, task, it, n, app=None):
-        return cls(task, it, n, app=app)()
-
-
-def _maybe_group(tasks, app):
-    if isinstance(tasks, dict):
-        tasks = signature(tasks, app=app)
-
-    if isinstance(tasks, (group, _chain)):
-        tasks = tasks.tasks
-    elif isinstance(tasks, abstract.CallableSignature):
-        tasks = [tasks]
-    else:
-        if isinstance(tasks, GeneratorType):
-            tasks = regen(signature(t, app=app) for t in tasks)
-        else:
-            tasks = [signature(t, app=app) for t in tasks]
-    return tasks
+            def clone(self, *args, **kwargs):
+                return self
 
+        def s(*args, **kwargs):
+            return static(self.add, args, kwargs, type=self.add, app=self.app)
 
-@Signature.register_type()
-class group(Signature):
-    """Creates a group of tasks to be executed in parallel.
+        c = s(2, 2) | s(4) | s(8)
+        r1 = c.apply_async(task_id='some_id')
+        assert r1.id == 'some_id'
 
-    A group is lazy so you must call it to take action and evaluate
-    the group.
+        c.apply_async(group_id='some_group_id')
+        assert c.tasks[-1].options['group_id'] == 'some_group_id'
 
-    Note:
-        If only one argument is passed, and that argument is an iterable
-        then that'll be used as the list of tasks instead: this
-        allows us to use ``group`` with generator expressions.
-
-    Example:
-        >>> lazy_group = group([add.s(2, 2), add.s(4, 4)])
-        >>> promise = lazy_group()  # <-- evaluate: returns lazy result.
-        >>> promise.get()  # <-- will wait for the task to return
-        [4, 8]
-
-    Arguments:
-        *tasks (List[Signature]): A list of signatures that this group will
-            call. If there's only one argument, and that argument is an
-            iterable, then that'll define the list of signatures instead.
-        **options (Any): Execution options applied to all tasks
-            in the group.
-
-    Returns:
-        ~celery.group: signature that when called will then call all of the
-            tasks in the group (and return a :class:`GroupResult` instance
-            that can be used to inspect the state of the group).
-    """
-
-    tasks = getitem_property('kwargs.tasks', 'Tasks in group.')
-
-    @classmethod
-    def from_dict(cls, d, app=None):
-        # We need to mutate the `kwargs` element in place to avoid confusing
-        # `freeze()` implementations which end up here and expect to be able to
-        # access elements from that dictionary later and refer to objects
-        # canonicalized here
-        orig_tasks = d["kwargs"]["tasks"]
-        d["kwargs"]["tasks"] = rebuilt_tasks = type(orig_tasks)(
-            maybe_signature(task, app=app) for task in orig_tasks
-        )
-        return cls(rebuilt_tasks, app=app, **d['options'])
-
-    def __init__(self, *tasks, **options):
-        if len(tasks) == 1:
-            tasks = tasks[0]
-            if isinstance(tasks, group):
-                tasks = tasks.tasks
-            if isinstance(tasks, abstract.CallableSignature):
-                tasks = [tasks.clone()]
-            if not isinstance(tasks, _regen):
-                tasks = regen(tasks)
-        super().__init__('celery.group', (), {'tasks': tasks}, **options
-                         )
-        self.subtask_type = 'group'
-
-    def __call__(self, *partial_args, **options):
-        return self.apply_async(partial_args, **options)
-
-    def __or__(self, other):
-        # group() | task -> chord
-        return chord(self, body=other, app=self._app)
-
-    def skew(self, start=1.0, stop=None, step=1.0):
-        it = fxrange(start, stop, step, repeatlast=True)
-        for task in self.tasks:
-            task.set(countdown=next(it))
-        return self
-
-    def apply_async(self, args=None, kwargs=None, add_to_parent=True,
-                    producer=None, link=None, link_error=None, **options):
-        args = args if args else ()
-        if link is not None:
-            raise TypeError('Cannot add link to group: use a chord')
-        if link_error is not None:
-            raise TypeError(
-                'Cannot add link to group: do that on individual tasks')
-        app = self.app
-        if app.conf.task_always_eager:
-            return self.apply(args, kwargs, **options)
-        if not self.tasks:
-            return self.freeze()
-
-        options, group_id, root_id = self._freeze_gid(options)
-        tasks = self._prepared(self.tasks, [], group_id, root_id, app)
-
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-
-        p = barrier()
-        results = list(self._apply_tasks(tasks, producer, app, p,
-                                         args=args, kwargs=kwargs, **options))
-        result = self.app.GroupResult(group_id, results, ready_barrier=p)
-        p.finalize()
-
-        # - Special case of group(A.s() | group(B.s(), C.s()))
-        # That is, group with single item that's a chain but the
-        # last task in that chain is a group.
-        #
-        # We cannot actually support arbitrary GroupResults in chains,
-        # but this special case we can.
-        if len(result) == 1 and isinstance(result[0], GroupResult):
-            result = result[0]
-
-        parent_task = app.current_worker_task
-        if add_to_parent and parent_task:
-            parent_task.add_trail(result)
-        return result
-
-    def apply(self, args=None, kwargs=None, **options):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        app = self.app
-        if not self.tasks:
-            return self.freeze()  # empty group returns GroupResult
-        options, group_id, root_id = self._freeze_gid(options)
-        tasks = self._prepared(self.tasks, [], group_id, root_id, app)
-        return app.GroupResult(group_id, [
-            sig.apply(args=args, kwargs=kwargs, **options) for sig, _, _ in tasks
-        ])
-
-    def set_immutable(self, immutable):
-        for task in self.tasks:
-            task.set_immutable(immutable)
-
-    def stamp(self, visitor=None, **headers):
-        if visitor is not None:
-            headers.update(visitor.on_group_start(self, **headers))
+        c.apply_async(chord='some_chord_id')
+        assert c.tasks[-1].options['chord'] == 'some_chord_id'
 
-        super().stamp(visitor=visitor, **headers)
+        c.apply_async(link=[s(32)])
+        assert c.tasks[-1].options['link'] == [s(32)]
 
-        if isinstance(self.tasks, _regen):
-            self.tasks.map(_partial(_stamp_regen_task, visitor=visitor, **headers))
-        else:
-            new_tasks = []
-            for task in self.tasks:
-                task = maybe_signature(task, app=self.app)
-                task.stamp(visitor=visitor, **headers)
-                new_tasks.append(task)
-            if isinstance(self.tasks, MutableSequence):
-                self.tasks[:] = new_tasks
-            else:
-                self.tasks = new_tasks
-
-        if visitor is not None:
-            visitor.on_group_end(self, **headers)
-
-    def link(self, sig):
-        # Simply link to first task. Doing this is slightly misleading because
-        # the callback may be executed before all children in the group are
-        # completed and also if any children other than the first one fail.
-        #
-        # The callback signature is cloned and made immutable since it the
-        # first task isn't actually capable of passing the return values of its
-        # siblings to the callback task.
-        sig = sig.clone().set(immutable=True)
-        return self.tasks[0].link(sig)
-
-    def link_error(self, sig):
-        # Any child task might error so we need to ensure that they are all
-        # capable of calling the linked error signature. This opens the
-        # possibility that the task is called more than once but that's better
-        # than it not being called at all.
-        #
-        # We return a concretised tuple of the signatures actually applied to
-        # each child task signature, of which there might be none!
-        return tuple(child_task.link_error(sig) for child_task in self.tasks)
-
-    def _prepared(self, tasks, partial_args, group_id, root_id, app,
-                  CallableSignature=abstract.CallableSignature,
-                  from_dict=Signature.from_dict,
-                  isinstance=isinstance, tuple=tuple):
-        for task in tasks:
-            if isinstance(task, CallableSignature):
-                # local sigs are always of type Signature, and we
-                # clone them to make sure we don't modify the originals.
-                task = task.clone()
-            else:
-                # serialized sigs must be converted to Signature.
-                task = from_dict(task, app=app)
-            if isinstance(task, group):
-                # needs yield_from :(
-                unroll = task._prepared(
-                    task.tasks, partial_args, group_id, root_id, app,
-                )
-                yield from unroll
-            else:
-                if partial_args and not task.immutable:
-                    task.args = tuple(partial_args) + tuple(task.args)
-                yield task, task.freeze(group_id=group_id, root_id=root_id), group_id
-
-    def _apply_tasks(self, tasks, producer=None, app=None, p=None,
-                     add_to_parent=None, chord=None,
-                     args=None, kwargs=None, **options):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        app = app or self.app
-        with app.producer_or_acquire(producer) as producer:
-            # Iterate through tasks two at a time. If tasks is a generator,
-            # we are able to tell when we are at the end by checking if
-            # next_task is None.  This enables us to set the chord size
-            # without burning through the entire generator.  See #3021.
-            chord_size = 0
-            tasks_shifted, tasks = itertools.tee(tasks)
-            next(tasks_shifted, None)
-            next_task = next(tasks_shifted, None)
-
-            for task_index, current_task in enumerate(tasks):
-                # We expect that each task must be part of the same group which
-                # seems sensible enough. If that's somehow not the case we'll
-                # end up messing up chord counts and there are all sorts of
-                # awful race conditions to think about. We'll hope it's not!
-                sig, res, group_id = current_task
-                chord_obj = chord if chord is not None else sig.options.get("chord")
-                # We need to check the chord size of each contributing task so
-                # that when we get to the final one, we can correctly set the
-                # size in the backend and the chord can be sensible completed.
-                chord_size += _chord._descend(sig)
-                if chord_obj is not None and next_task is None:
-                    # Per above, sanity check that we only saw one group
-                    app.backend.set_chord_size(group_id, chord_size)
-                sig.apply_async(producer=producer, add_to_parent=False,
-                                chord=chord_obj, args=args, kwargs=kwargs,
-                                **options)
-                # adding callback to result, such that it will gradually
-                # fulfill the barrier.
-                #
-                # Using barrier.add would use result.then, but we need
-                # to add the weak argument here to only create a weak
-                # reference to the object.
-                if p and not p.cancelled and not p.ready:
-                    p.size += 1
-                    res.then(p, weak=True)
-                next_task = next(tasks_shifted, None)
-                yield res  # <-- r.parent, etc set in the frozen result.
-
-    def _freeze_gid(self, options):
-        # remove task_id and use that as the group_id,
-        # if we don't remove it then every task will have the same id...
-        options = {**self.options, **{
-            k: v for k, v in options.items()
-            if k not in self._IMMUTABLE_OPTIONS or k not in self.options
-        }}
-        options['group_id'] = group_id = (
-            options.pop('task_id', uuid()))
-        return options, group_id, options.get('root_id')
-
-    def _freeze_group_tasks(self, _id=None, group_id=None, chord=None,
-                            root_id=None, parent_id=None, group_index=None):
-        # pylint: disable=redefined-outer-name
-        #  XXX chord is also a class in outer scope.
-        opts = self.options
-        try:
-            gid = opts['task_id']
-        except KeyError:
-            gid = opts['task_id'] = group_id or uuid()
-        if group_id:
-            opts['group_id'] = group_id
-        if chord:
-            opts['chord'] = chord
-        if group_index is not None:
-            opts['group_index'] = group_index
-        root_id = opts.setdefault('root_id', root_id)
-        parent_id = opts.setdefault('parent_id', parent_id)
-        if isinstance(self.tasks, _regen):
-            # We are draining from a generator here.
-            # tasks1, tasks2 are each a clone of self.tasks
-            tasks1, tasks2 = itertools.tee(self._unroll_tasks(self.tasks))
-            # freeze each task in tasks1, results now holds AsyncResult for each task
-            results = regen(self._freeze_tasks(tasks1, group_id, chord, root_id, parent_id))
-            # TODO figure out why this makes sense -
-            # we freeze all tasks in the clone tasks1, and then zip the results
-            # with the IDs of tasks in the second clone, tasks2. and then, we build
-            # a generator that takes only the task IDs from tasks2.
-            self.tasks = regen(tasks2)
-        else:
-            new_tasks = []
-            # Need to unroll subgroups early so that chord gets the
-            # right result instance for chord_unlock etc.
-            results = list(self._freeze_unroll(
-                new_tasks, group_id, chord, root_id, parent_id,
-            ))
-            if isinstance(self.tasks, MutableSequence):
-                self.tasks[:] = new_tasks
-            else:
-                self.tasks = new_tasks
-        return gid, results
-
-    def freeze(self, _id=None, group_id=None, chord=None,
-               root_id=None, parent_id=None, group_index=None):
-        return self.app.GroupResult(*self._freeze_group_tasks(
-            _id=_id, group_id=group_id,
-            chord=chord, root_id=root_id, parent_id=parent_id, group_index=group_index
-        ))
-
-    _freeze = freeze
-
-    def _freeze_tasks(self, tasks, group_id, chord, root_id, parent_id):
-        yield from (task.freeze(group_id=group_id,
-                                chord=chord,
-                                root_id=root_id,
-                                parent_id=parent_id,
-                                group_index=group_index)
-                    for group_index, task in enumerate(tasks))
-
-    def _unroll_tasks(self, tasks):
-        # should be refactored to: (maybe_signature(task, app=self._app, clone=True) for task in tasks)
-        yield from (maybe_signature(task, app=self._app).clone() for task in tasks)
-
-    def _freeze_unroll(self, new_tasks, group_id, chord, root_id, parent_id):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        stack = deque(self.tasks)
-        group_index = 0
-        while stack:
-            task = maybe_signature(stack.popleft(), app=self._app).clone()
-            # if this is a group, flatten it by adding all of the group's tasks to the stack
-            if isinstance(task, group):
-                stack.extendleft(task.tasks)
-            else:
-                new_tasks.append(task)
-                yield task.freeze(group_id=group_id,
-                                  chord=chord, root_id=root_id,
-                                  parent_id=parent_id,
-                                  group_index=group_index)
-                group_index += 1
-
-    def __repr__(self):
-        if self.tasks:
-            return remove_repeating_from_task(
-                self.tasks[0]['task'],
-                f'group({self.tasks!r})')
-        return 'group(<empty>)'
-
-    def __len__(self):
-        return len(self.tasks)
-
-    @property
-    def app(self):
-        app = self._app
-        if app is None:
-            try:
-                app = self.tasks[0].app
-            except LookupError:
-                pass
-        return app if app is not None else current_app
+        c.apply_async(link_error=[s('error')])
+        for task in c.tasks:
+            assert task.options['link_error'] == [s('error')]
 
+    def test_apply_options_none(self):
+        class static(Signature):
 
-@Signature.register_type(name="chord")
-class _chord(Signature):
-    r"""Barrier synchronization primitive.
+            def clone(self, *args, **kwargs):
+                return self
 
-    A chord consists of a header and a body.
+            def _apply_async(self, *args, **kwargs):
+                self.args = args
+                self.kwargs = kwargs
 
-    The header is a group of tasks that must complete before the callback is
-    called.  A chord is essentially a callback for a group of tasks.
+        c = static(self.add, (2, 2), type=self.add, app=self.app, priority=5)
 
-    The body is applied with the return values of all the header
-    tasks as a list.
+        c.apply_async(priority=4)
+        assert c.kwargs['priority'] == 4
 
-    Example:
+        c.apply_async(priority=None)
+        assert c.kwargs['priority'] == 5
 
-        The chord:
+    def test_reverse(self):
+        x = self.add.s(2, 2) | self.add.s(2)
+        assert isinstance(signature(x), _chain)
+        assert isinstance(signature(dict(x)), _chain)
 
-        .. code-block:: pycon
+    def test_always_eager(self):
+        self.app.conf.task_always_eager = True
+        assert ~(self.add.s(4, 4) | self.add.s(8)) == 16
 
-            >>> res = chord([add.s(2, 2), add.s(4, 4)])(sum_task.s())
+    def test_chain_always_eager(self):
+        self.app.conf.task_always_eager = True
+        from celery import _state, result
 
-        is effectively :math:`\Sigma ((2 + 2) + (4 + 4))`:
+        fixture_task_join_will_block = _state.task_join_will_block
+        try:
+            _state.task_join_will_block = _state.orig_task_join_will_block
+            result.task_join_will_block = _state.orig_task_join_will_block
 
-        .. code-block:: pycon
+            @self.app.task(shared=False)
+            def chain_add():
+                return (self.add.s(4, 4) | self.add.s(8)).apply_async()
+
+            r = chain_add.apply_async(throw=True).get()
+            assert r.get() == 16
+        finally:
+            _state.task_join_will_block = fixture_task_join_will_block
+            result.task_join_will_block = fixture_task_join_will_block
+
+    def test_apply(self):
+        x = chain(self.add.s(4, 4), self.add.s(8), self.add.s(10))
+        res = x.apply()
+        assert isinstance(res, EagerResult)
+        assert res.get() == 26
+
+        assert res.parent.get() == 16
+        assert res.parent.parent.get() == 8
+        assert res.parent.parent.parent is None
+
+    def test_kwargs_apply(self):
+        x = chain(self.add.s(), self.add.s(8), self.add.s(10))
+        res = x.apply(kwargs={'x': 1, 'y': 1}).get()
+        assert res == 20
+
+    def test_single_expresion(self):
+        x = chain(self.add.s(1, 2)).apply()
+        assert x.get() == 3
+        assert x.parent is None
+
+    def test_empty_chain_returns_none(self):
+        assert chain(app=self.app)() is None
+        assert chain(app=self.app).apply_async() is None
+
+    def test_call_no_tasks(self):
+        x = chain()
+        assert not x()
+
+    def test_call_with_tasks(self):
+        x = self.add.s(2, 2) | self.add.s(4)
+        x.apply_async = Mock()
+        x(2, 2, foo=1)
+        x.apply_async.assert_called_with((2, 2), {'foo': 1})
+
+    def test_from_dict_no_args__with_args(self):
+        x = dict(self.add.s(2, 2) | self.add.s(4))
+        x['args'] = None
+        assert isinstance(chain.from_dict(x), _chain)
+        x['args'] = (2,)
+        assert isinstance(chain.from_dict(x), _chain)
+
+    def test_accepts_generator_argument(self):
+        x = chain(self.add.s(i) for i in range(10))
+        assert x.tasks[0].type, self.add
+        assert x.type
+
+    def test_chord_sets_result_parent(self):
+        g = (self.add.s(0, 0) |
+             group(self.add.s(i, i) for i in range(1, 10)) |
+             self.add.s(2, 2) |
+             self.add.s(4, 4))
+        res = g.freeze()
+
+        assert isinstance(res, AsyncResult)
+        assert not isinstance(res, GroupResult)
+        assert isinstance(res.parent, AsyncResult)
+        assert not isinstance(res.parent, GroupResult)
+        assert isinstance(res.parent.parent, GroupResult)
+        assert isinstance(res.parent.parent.parent, AsyncResult)
+        assert not isinstance(res.parent.parent.parent, GroupResult)
+        assert res.parent.parent.parent.parent is None
+
+        seen = set()
+        node = res
+        while node:
+            assert node.id not in seen
+            seen.add(node.id)
+            node = node.parent
+
+    def test_append_to_empty_chain(self):
+        x = chain()
+        x |= self.add.s(1, 1)
+        x |= self.add.s(1)
+        x.freeze()
+        tasks, _ = x._frozen
+        assert len(tasks) == 2
+
+        assert x.apply().get() == 3
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_chain_single_child_result(self):
+        child_sig = self.add.si(1, 1)
+        chain_sig = chain(child_sig)
+        assert chain_sig.tasks[0] is child_sig
+
+        with patch.object(
+            # We want to get back the result of actually applying the task
+            child_sig, "apply_async",
+        ) as mock_apply, patch.object(
+            # The child signature may be clone by `chain.prepare_steps()`
+            child_sig, "clone", return_value=child_sig,
+        ):
+            res = chain_sig()
+        # `_prepare_chain_from_options()` sets this `chain` kwarg with the
+        # subsequent tasks which would be run - nothing in this case
+        mock_apply.assert_called_once_with(chain=[])
+        assert res is mock_apply.return_value
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_chain_single_child_group_result(self):
+        child_sig = self.add.si(1, 1)
+        # The group will `clone()` the child during instantiation so mock it
+        with patch.object(child_sig, "clone", return_value=child_sig):
+            group_sig = group(child_sig)
+        # Now we can construct the chain signature which is actually under test
+        chain_sig = chain(group_sig)
+        assert chain_sig.tasks[0].tasks[0] is child_sig
+
+        with patch.object(
+            # We want to get back the result of actually applying the task
+            child_sig, "apply_async",
+        ) as mock_apply, patch.object(
+            # The child signature may be clone by `chain.prepare_steps()`
+            child_sig, "clone", return_value=child_sig,
+        ):
+            res = chain_sig()
+        # `_prepare_chain_from_options()` sets this `chain` kwarg with the
+        # subsequent tasks which would be run - nothing in this case
+        mock_apply.assert_called_once_with(chain=[])
+        assert res is mock_apply.return_value
+
+    def test_chain_flattening_keep_links_of_inner_chain(self):
+        def link_chain(sig):
+            sig.link(signature('link_b'))
+            sig.link_error(signature('link_ab'))
+            return sig
 
-            >>> res.get()
-            12
-    """
+        inner_chain = link_chain(chain(signature('a'), signature('b')))
+        assert inner_chain.options['link'][0] == signature('link_b')
+        assert inner_chain.options['link_error'][0] == signature('link_ab')
+        assert inner_chain.tasks[0] == signature('a')
+        assert inner_chain.tasks[0].options == {}
+        assert inner_chain.tasks[1] == signature('b')
+        assert inner_chain.tasks[1].options == {}
+
+        flat_chain = chain(inner_chain, signature('c'))
+        assert flat_chain.options == {}
+        assert flat_chain.tasks[0].name == 'a'
+        assert 'link' not in flat_chain.tasks[0].options
+        assert signature(flat_chain.tasks[0].options['link_error'][0]) == signature('link_ab')
+        assert flat_chain.tasks[1].name == 'b'
+        assert 'link' in flat_chain.tasks[1].options, "b is missing the link from inner_chain.options['link'][0]"
+        assert signature(flat_chain.tasks[1].options['link'][0]) == signature('link_b')
+        assert signature(flat_chain.tasks[1].options['link_error'][0]) == signature('link_ab')
+
+
+class test_group(CanvasCase):
+    def test_repr(self):
+        x = group([self.add.s(2, 2), self.add.s(4, 4)])
+        assert repr(x)
+
+    def test_repr_empty_group(self):
+        x = group([])
+        assert repr(x) == 'group(<empty>)'
+
+    def test_reverse(self):
+        x = group([self.add.s(2, 2), self.add.s(4, 4)])
+        assert isinstance(signature(x), group)
+        assert isinstance(signature(dict(x)), group)
+
+    def test_reverse_with_subclass(self):
+        x = group_subclass([self.add.s(2, 2), self.add.s(4, 4)])
+        assert isinstance(signature(x), group_subclass)
+        assert isinstance(signature(dict(x)), group_subclass)
+
+    def test_cannot_link_on_group(self):
+        x = group([self.add.s(2, 2), self.add.s(4, 4)])
+        with pytest.raises(TypeError):
+            x.apply_async(link=self.add.s(2, 2))
+
+    def test_cannot_link_error_on_group(self):
+        x = group([self.add.s(2, 2), self.add.s(4, 4)])
+        with pytest.raises(TypeError):
+            x.apply_async(link_error=self.add.s(2, 2))
+
+    def test_group_with_group_argument(self):
+        g1 = group(self.add.s(2, 2), self.add.s(4, 4), app=self.app)
+        g2 = group(g1, app=self.app)
+        assert g2.tasks is g1.tasks
+
+    def test_maybe_group_sig(self):
+        assert _maybe_group(self.add.s(2, 2), self.app) == [self.add.s(2, 2)]
+
+    def test_apply(self):
+        x = group([self.add.s(4, 4), self.add.s(8, 8)])
+        res = x.apply()
+        assert res.get(), [8 == 16]
+
+    def test_apply_async(self):
+        x = group([self.add.s(4, 4), self.add.s(8, 8)])
+        x.apply_async()
+
+    def test_prepare_with_dict(self):
+        x = group([self.add.s(4, 4), dict(self.add.s(8, 8))], app=self.app)
+        x.apply_async()
+
+    def test_group_in_group(self):
+        g1 = group(self.add.s(2, 2), self.add.s(4, 4), app=self.app)
+        g2 = group(self.add.s(8, 8), g1, self.add.s(16, 16), app=self.app)
+        g2.apply_async()
+
+    def test_set_immutable(self):
+        g1 = group(Mock(name='t1'), Mock(name='t2'), app=self.app)
+        g1.set_immutable(True)
+        for task in g1.tasks:
+            task.set_immutable.assert_called_with(True)
+
+    def test_link(self):
+        g1 = group(Mock(name='t1'), Mock(name='t2'), app=self.app)
+        sig = Mock(name='sig')
+        g1.link(sig)
+        # Only the first child signature of a group will be given the callback
+        # and it is cloned and made immutable to avoid passing results to it,
+        # since that first task can't pass along its siblings' return values
+        g1.tasks[0].link.assert_called_with(sig.clone().set(immutable=True))
+
+    def test_link_error(self):
+        g1 = group(Mock(name='t1'), Mock(name='t2'), app=self.app)
+        sig = Mock(name='sig')
+        g1.link_error(sig)
+        # We expect that all group children will be given the errback to ensure
+        # it gets called
+        for child_sig in g1.tasks:
+            child_sig.link_error.assert_called_with(sig)
+
+    def test_apply_empty(self):
+        x = group(app=self.app)
+        x.apply()
+        res = x.apply_async()
+        assert res
+        assert not res.results
 
-    @classmethod
-    def from_dict(cls, d, app=None):
-        options = d.copy()
-        args, options['kwargs'] = cls._unpack_args(**options['kwargs'])
-        return cls(*args, app=app, **options)
+    def test_apply_async_with_parent(self):
+        _task_stack.push(self.add)
+        try:
+            self.add.push_request(called_directly=False)
+            try:
+                assert not self.add.request.children
+                x = group([self.add.s(4, 4), self.add.s(8, 8)])
+                res = x()
+                assert self.add.request.children
+                assert res in self.add.request.children
+                assert len(self.add.request.children) == 1
+            finally:
+                self.add.pop_request()
+        finally:
+            _task_stack.pop()
+
+    @pytest.mark.parametrize("group_type", (group, group_subclass))
+    def test_from_dict(self, group_type):
+        x = group_type([self.add.s(2, 2), self.add.s(4, 4)])
+        x['args'] = (2, 2)
+        value = group_type.from_dict(dict(x))
+        assert value and isinstance(value, group_type)
+        x['args'] = None
+        value = group_type.from_dict(dict(x))
+        assert value and isinstance(value, group_type)
+
+    @pytest.mark.parametrize("group_type", (group, group_subclass))
+    def test_from_dict_deep_deserialize(self, group_type):
+        original_group = group_type([self.add.s(1, 2)] * 42)
+        serialized_group = json.loads(json.dumps(original_group))
+        deserialized_group = group_type.from_dict(serialized_group)
+        assert isinstance(deserialized_group, group_type)
+        assert all(
+            isinstance(child_task, Signature)
+            for child_task in deserialized_group.tasks
+        )
+
+    @pytest.mark.parametrize("group_type", (group, group_subclass))
+    def test_from_dict_deeper_deserialize(self, group_type):
+        inner_group = group_type([self.add.s(1, 2)] * 42)
+        outer_group = group_type([inner_group] * 42)
+        serialized_group = json.loads(json.dumps(outer_group))
+        deserialized_group = group_type.from_dict(serialized_group)
+        assert isinstance(deserialized_group, group_type)
+        assert all(
+            isinstance(child_task, group_type)
+            for child_task in deserialized_group.tasks
+        )
+        assert all(
+            isinstance(grandchild_task, Signature)
+            for child_task in deserialized_group.tasks
+            for grandchild_task in child_task.tasks
+        )
+
+    def test_call_empty_group(self):
+        x = group(app=self.app)
+        assert not len(x())
+        x.delay()
+        x.apply_async()
+        x()
+
+    def test_skew(self):
+        g = group([self.add.s(i, i) for i in range(10)])
+        g.skew(start=1, stop=10, step=1)
+        for i, task in enumerate(g.tasks):
+            assert task.options['countdown'] == i + 1
+
+    def test_iter(self):
+        g = group([self.add.s(i, i) for i in range(10)])
+        assert list(iter(g)) == list(g.keys())
+
+    def test_single_task(self):
+        g = group([self.add.s(1, 1)])
+        assert isinstance(g, group)
+        assert len(g.tasks) == 1
+        g = group(self.add.s(1, 1))
+        assert isinstance(g, group)
+        assert len(g.tasks) == 1
 
     @staticmethod
-    def _unpack_args(header=None, body=None, **kwargs):
-        # Python signatures are better at extracting keys from dicts
-        # than manually popping things off.
-        return (header, body), kwargs
-
-    def __init__(self, header, body=None, task='celery.chord',
-                 args=None, kwargs=None, app=None, **options):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {'kwargs': {}}
-        super().__init__(task, args,
-                         {**kwargs, 'header': _maybe_group(header, app),
-                          'body': maybe_signature(body, app=app)}, app=app, **options
-                         )
-        self.subtask_type = 'chord'
-
-    def __call__(self, body=None, **options):
-        return self.apply_async((), {'body': body} if body else {}, **options)
-
-    def __or__(self, other):
-        if (not isinstance(other, (group, _chain)) and
-           isinstance(other, Signature)):
-            # chord | task ->  attach to body
-            sig = self.clone()
-            sig.body = sig.body | other
-            return sig
-        else:
-            return super().__or__(other)
+    def helper_test_get_delay(result):
+        import time
+        t0 = time.time()
+        while not result.ready():
+            time.sleep(0.01)
+            if time.time() - t0 > 1:
+                return None
+        return result.get()
+
+    def test_kwargs_direct(self):
+        res = [self.add(x=1, y=1), self.add(x=1, y=1)]
+        assert res == [2, 2]
+
+    def test_kwargs_apply(self):
+        x = group([self.add.s(), self.add.s()])
+        res = x.apply(kwargs={'x': 1, 'y': 1}).get()
+        assert res == [2, 2]
+
+    def test_kwargs_apply_async(self):
+        self.app.conf.task_always_eager = True
+        x = group([self.add.s(), self.add.s()])
+        res = self.helper_test_get_delay(
+            x.apply_async(kwargs={'x': 1, 'y': 1})
+        )
+        assert res == [2, 2]
+
+    def test_kwargs_delay(self):
+        self.app.conf.task_always_eager = True
+        x = group([self.add.s(), self.add.s()])
+        res = self.helper_test_get_delay(x.delay(x=1, y=1))
+        assert res == [2, 2]
+
+    def test_kwargs_delay_partial(self):
+        self.app.conf.task_always_eager = True
+        x = group([self.add.s(1), self.add.s(x=1)])
+        res = self.helper_test_get_delay(x.delay(y=1))
+        assert res == [2, 2]
+
+    def test_apply_from_generator(self):
+        child_count = 42
+        child_sig = self.add.si(0, 0)
+        child_sigs_gen = (child_sig for _ in range(child_count))
+        group_sig = group(child_sigs_gen)
+        with patch("celery.canvas.Signature.apply_async") as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        assert mock_apply_async.call_count == child_count
+        assert len(res_obj.children) == child_count
+
+    # This needs the current app for some reason not worth digging into
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_apply_from_generator_empty(self):
+        empty_gen = (False for _ in range(0))
+        group_sig = group(empty_gen)
+        with patch("celery.canvas.Signature.apply_async") as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        assert mock_apply_async.call_count == 0
+        assert len(res_obj.children) == 0
+
+    # In the following tests, getting the group ID is a pain so we just use
+    # `ANY` to wildcard it when we're checking on calls made to our mocks
+    def test_apply_contains_chord(self):
+        gchild_count = 42
+        gchild_sig = self.add.si(0, 0)
+        gchild_sigs = (gchild_sig,) * gchild_count
+        child_chord = chord(gchild_sigs, gchild_sig)
+        group_sig = group((child_chord,))
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We only see applies for the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == gchild_count
+        assert len(res_obj.children) == len(group_sig.tasks)
+        # We must have set the chord size for the group of tasks which makes up
+        # the header of the `child_chord`, just before we apply the last task.
+        mock_set_chord_size.assert_called_once_with(ANY, gchild_count)
+
+    def test_apply_contains_chords_containing_chain(self):
+        ggchild_count = 42
+        ggchild_sig = self.add.si(0, 0)
+        gchild_sig = chain((ggchild_sig,) * ggchild_count)
+        child_count = 24
+        child_chord = chord((gchild_sig,), ggchild_sig)
+        group_sig = group((child_chord,) * child_count)
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We only see applies for the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == child_count
+        assert len(res_obj.children) == child_count
+        # We must have set the chord sizes based on the number of tail tasks of
+        # the encapsulated chains - in this case 1 for each child chord
+        mock_set_chord_size.assert_has_calls((call(ANY, 1),) * child_count)
+
+    @pytest.mark.xfail(reason="Invalid canvas setup with bad exception")
+    def test_apply_contains_chords_containing_empty_chain(self):
+        gchild_sig = chain(tuple())
+        child_count = 24
+        child_chord = chord((gchild_sig,), self.add.si(0, 0))
+        group_sig = group((child_chord,) * child_count)
+        # This is an invalid setup because we can't complete a chord header if
+        # there are no actual tasks which will run in it. However, the current
+        # behaviour of an `IndexError` isn't particularly helpful to a user.
+        group_sig.apply_async()
+
+    def test_apply_contains_chords_containing_chain_with_empty_tail(self):
+        ggchild_count = 42
+        ggchild_sig = self.add.si(0, 0)
+        tail_count = 24
+        gchild_sig = chain(
+            (ggchild_sig,) * ggchild_count +
+            (group((ggchild_sig,) * tail_count), group(tuple()),),
+        )
+        child_chord = chord((gchild_sig,), ggchild_sig)
+        group_sig = group((child_chord,))
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We only see applies for the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == 1
+        assert len(res_obj.children) == 1
+        # We must have set the chord sizes based on the size of the last
+        # non-empty task in the encapsulated chains - in this case `tail_count`
+        # for the group preceding the empty one in each grandchild chain
+        mock_set_chord_size.assert_called_once_with(ANY, tail_count)
+
+    def test_apply_contains_chords_containing_group(self):
+        ggchild_count = 42
+        ggchild_sig = self.add.si(0, 0)
+        gchild_sig = group((ggchild_sig,) * ggchild_count)
+        child_count = 24
+        child_chord = chord((gchild_sig,), ggchild_sig)
+        group_sig = group((child_chord,) * child_count)
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We see applies for all of the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == child_count * ggchild_count
+        assert len(res_obj.children) == child_count
+        # We must have set the chord sizes based on the number of tail tasks of
+        # the encapsulated groups - in this case `ggchild_count`
+        mock_set_chord_size.assert_has_calls(
+            (call(ANY, ggchild_count),) * child_count,
+        )
 
-    def freeze(self, _id=None, group_id=None, chord=None,
-               root_id=None, parent_id=None, group_index=None):
-        # pylint: disable=redefined-outer-name
-        #   XXX chord is also a class in outer scope.
-        if not isinstance(self.tasks, group):
-            self.tasks = group(self.tasks, app=self.app)
-        # first freeze all tasks in the header
-        header_result = self.tasks.freeze(
-            parent_id=parent_id, root_id=root_id, chord=self.body)
-        self.id = self.tasks.id
-        # secondly freeze all tasks in the body: those that should be called after the header
-
-        body_result = None
-        if self.body:
-            body_result = self.body.freeze(
-                _id, root_id=root_id, chord=chord, group_id=group_id,
-                group_index=group_index)
-            # we need to link the body result back to the group result,
-            # but the body may actually be a chain,
-            # so find the first result without a parent
-            node = body_result
-            seen = set()
-            while node:
-                if node.id in seen:
-                    raise RuntimeError('Recursive result parents')
-                seen.add(node.id)
-                if node.parent is None:
-                    node.parent = header_result
-                    break
-                node = node.parent
-
-        return body_result
-
-    def stamp(self, visitor=None, **headers):
-        if visitor is not None and self.body is not None:
-            headers.update(visitor.on_chord_body(self, **headers))
-            self.body.stamp(visitor=visitor, **headers)
-
-        if visitor is not None:
-            headers.update(visitor.on_chord_header_start(self, **headers))
-        super().stamp(visitor=visitor, **headers)
-
-        tasks = self.tasks
-        if isinstance(tasks, group):
-            tasks = tasks.tasks
+    @pytest.mark.xfail(reason="Invalid canvas setup but poor behaviour")
+    def test_apply_contains_chords_containing_empty_group(self):
+        gchild_sig = group(tuple())
+        child_count = 24
+        child_chord = chord((gchild_sig,), self.add.si(0, 0))
+        group_sig = group((child_chord,) * child_count)
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We only see applies for the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == child_count
+        assert len(res_obj.children) == child_count
+        # This is actually kind of meaningless because, similar to the empty
+        # chain test, this is an invalid setup. However, we should probably
+        # expect that the chords are dealt with in some other way the probably
+        # being left incomplete forever...
+        mock_set_chord_size.assert_has_calls((call(ANY, 0),) * child_count)
+
+    def test_apply_contains_chords_containing_chord(self):
+        ggchild_count = 42
+        ggchild_sig = self.add.si(0, 0)
+        gchild_sig = chord((ggchild_sig,) * ggchild_count, ggchild_sig)
+        child_count = 24
+        child_chord = chord((gchild_sig,), ggchild_sig)
+        group_sig = group((child_chord,) * child_count)
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We see applies for all of the header great-grandchildren because the
+        # tasks are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == child_count * ggchild_count
+        assert len(res_obj.children) == child_count
+        # We must have set the chord sizes based on the number of tail tasks of
+        # the deeply encapsulated chords' header tasks, as well as for each
+        # child chord. This means we have `child_count` interleaved calls to
+        # set chord sizes of 1 and `ggchild_count`.
+        mock_set_chord_size.assert_has_calls(
+            (call(ANY, 1), call(ANY, ggchild_count),) * child_count,
+        )
 
-        if isinstance(tasks, _regen):
-            tasks.map(_partial(_stamp_regen_task, visitor=visitor, **headers))
-        else:
-            for task in tasks:
-                task.stamp(visitor=visitor, **headers)
+    def test_apply_contains_chords_containing_empty_chord(self):
+        gchild_sig = chord(tuple(), self.add.si(0, 0))
+        child_count = 24
+        child_chord = chord((gchild_sig,), self.add.si(0, 0))
+        group_sig = group((child_chord,) * child_count)
+        with patch.object(
+            self.app.backend, "set_chord_size",
+        ) as mock_set_chord_size, patch(
+            "celery.canvas.Signature.apply_async",
+        ) as mock_apply_async:
+            res_obj = group_sig.apply_async()
+        # We only see applies for the header grandchildren because the tasks
+        # are never actually run due to our mocking of `apply_async()`
+        assert mock_apply_async.call_count == child_count
+        assert len(res_obj.children) == child_count
+        # We must have set the chord sizes based on the number of tail tasks of
+        # the encapsulated chains - in this case 1 for each child chord
+        mock_set_chord_size.assert_has_calls((call(ANY, 1),) * child_count)
+
+    def test_group_prepared(self):
+        # Using both partial and dict based signatures
+        sig = group(dict(self.add.s(0)), self.add.s(0))
+        _, group_id, root_id = sig._freeze_gid({})
+        tasks = sig._prepared(sig.tasks, [42], group_id, root_id, self.app)
+
+        for task, result, group_id in tasks:
+            assert isinstance(task, Signature)
+            assert task.args[0] == 42
+            assert task.args[1] == 0
+            assert isinstance(result, AsyncResult)
+            assert group_id is not None
+
+
+class test_chord(CanvasCase):
+    def test__get_app_does_not_exhaust_generator(self):
+        def build_generator():
+            yield self.add.s(1, 1)
+            self.second_item_returned = True
+            yield self.add.s(2, 2)
+            raise pytest.fail("This should never be reached")
+
+        self.second_item_returned = False
+        c = chord(build_generator(), self.add.s(3))
+        c.app
+        # The second task gets returned due to lookahead in `regen()`
+        assert self.second_item_returned
+        # Access it again to make sure the generator is not further evaluated
+        c.app
+
+    @pytest.mark.parametrize("chord_type", [chord, chord_subclass])
+    def test_reverse(self, chord_type):
+        x = chord_type([self.add.s(2, 2), self.add.s(4, 4)], body=self.mul.s(4))
+        assert isinstance(signature(x), chord_type)
+        assert isinstance(signature(dict(x)), chord_type)
+
+    def test_clone_clones_body(self):
+        x = chord([self.add.s(2, 2), self.add.s(4, 4)], body=self.mul.s(4))
+        y = x.clone()
+        assert x.kwargs['body'] is not y.kwargs['body']
+        y.kwargs.pop('body')
+        z = y.clone()
+        assert z.kwargs.get('body') is None
+
+    def test_argument_is_group(self):
+        x = chord(group(self.add.s(2, 2), self.add.s(4, 4), app=self.app))
+        assert x.tasks
+
+    def test_app_when_app(self):
+        app = Mock(name='app')
+        x = chord([self.add.s(4, 4)], app=app)
+        assert x.app is app
+
+    def test_app_when_app_in_task(self):
+        t1 = Mock(name='t1')
+        t2 = Mock(name='t2')
+        x = chord([t1, self.add.s(4, 4)])
+        assert x.app is x.tasks[0].app
+        t1.app = None
+        x = chord([t1], body=t2)
+        assert x.app is t2._app
+
+    def test_app_when_header_is_empty(self):
+        x = chord([], self.add.s(4, 4))
+        assert x.app is self.add.app
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_app_fallback_to_current(self):
+        from celery._state import current_app
+        t1 = Mock(name='t1')
+        t1.app = t1._app = None
+        x = chord([t1], body=t1)
+        assert x.app is current_app
+
+    def test_chord_size_simple(self):
+        sig = chord(self.add.s())
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_with_body(self):
+        sig = chord(self.add.s(), self.add.s())
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_explicit_group_single(self):
+        sig = chord(group(self.add.s()))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_explicit_group_many(self):
+        sig = chord(group([self.add.s()] * 42))
+        assert sig.__length_hint__() == 42
+
+    def test_chord_size_implicit_group_single(self):
+        sig = chord([self.add.s()])
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_implicit_group_many(self):
+        sig = chord([self.add.s()] * 42)
+        assert sig.__length_hint__() == 42
+
+    def test_chord_size_chain_single(self):
+        sig = chord(chain(self.add.s()))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_chain_many(self):
+        # Chains get flattened into the encapsulating chord so even though the
+        # chain would only count for 1, the tasks we pulled into the chord's
+        # header and are counted as a bunch of simple signature objects
+        sig = chord(chain([self.add.s()] * 42))
+        assert sig.__length_hint__() == 42
+
+    def test_chord_size_nested_chain_chain_single(self):
+        sig = chord(chain(chain(self.add.s())))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_chain_chain_many(self):
+        # The outer chain will be pulled up into the chord but the lower one
+        # remains and will only count as a single final element
+        sig = chord(chain(chain([self.add.s()] * 42)))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_implicit_chain_single(self):
+        sig = chord([self.add.s()])
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_implicit_chain_many(self):
+        # This isn't a chain object so the `tasks` attribute can't be lifted
+        # into the chord - this isn't actually valid and would blow up we tried
+        # to run it but it sanity checks our recursion
+        sig = chord([[self.add.s()] * 42])
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_implicit_chain_chain_single(self):
+        sig = chord([chain(self.add.s())])
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_implicit_chain_chain_many(self):
+        sig = chord([chain([self.add.s()] * 42)])
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_chord_body_simple(self):
+        sig = chord(chord(tuple(), self.add.s()))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_chord_body_implicit_group_single(self):
+        sig = chord(chord(tuple(), [self.add.s()]))
+        assert sig.__length_hint__() == 1
+
+    def test_chord_size_nested_chord_body_implicit_group_many(self):
+        sig = chord(chord(tuple(), [self.add.s()] * 42))
+        assert sig.__length_hint__() == 42
+
+    # Nested groups in a chain only affect the chord size if they are the last
+    # element in the chain - in that case each group element is counted
+    def test_chord_size_nested_group_chain_group_head_single(self):
+        x = chord(
+            group(
+                [group(self.add.s()) | self.add.s()] * 42
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 42
 
-        if visitor is not None:
-            visitor.on_chord_header_end(self, **headers)
+    def test_chord_size_nested_group_chain_group_head_many(self):
+        x = chord(
+            group(
+                [group([self.add.s()] * 4) | self.add.s()] * 2
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 2
+
+    def test_chord_size_nested_group_chain_group_mid_single(self):
+        x = chord(
+            group(
+                [self.add.s() | group(self.add.s()) | self.add.s()] * 42
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 42
 
-    def apply_async(self, args=None, kwargs=None, task_id=None,
-                    producer=None, publisher=None, connection=None,
-                    router=None, result_cls=None, **options):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        args = (tuple(args) + tuple(self.args)
-                if args and not self.immutable else self.args)
-        body = kwargs.pop('body', None) or self.kwargs['body']
-        kwargs = dict(self.kwargs['kwargs'], **kwargs)
-        body = body.clone(**options)
-        app = self._get_app(body)
-        tasks = (self.tasks.clone() if isinstance(self.tasks, group)
-                 else group(self.tasks, app=app))
-        if app.conf.task_always_eager:
-            with allow_join_result():
-                return self.apply(args, kwargs,
-                                  body=body, task_id=task_id, **options)
-
-        groups = self.options.get("groups")
-        stamped_headers = self.options.get("stamped_headers")
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        tasks.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-
-        merged_options = dict(self.options, **options) if options else self.options
-
-        option_task_id = merged_options.pop("task_id", None)
-        if task_id is None:
-            task_id = option_task_id
-
-        # chord([A, B, ...], C)
-        return self.run(tasks, body, args, task_id=task_id, kwargs=kwargs, **merged_options)
-
-    def apply(self, args=None, kwargs=None,
-              propagate=True, body=None, **options):
-        args = args if args else ()
-        kwargs = kwargs if kwargs else {}
-        stamped_headers = self.options.get("stamped_headers")
-        groups = self.options.get("groups")
-        body = self.body if body is None else body
-        tasks = (self.tasks.clone() if isinstance(self.tasks, group)
-                 else group(self.tasks, app=self.app))
-        self.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        tasks.stamp(visitor=GroupStampingVisitor(groups=groups, stamped_headers=stamped_headers))
-        return body.apply(
-            args=(tasks.apply(args, kwargs).get(propagate=propagate),),
-        )
-
-    @classmethod
-    def _descend(cls, sig_obj):
-        # Sometimes serialized signatures might make their way here
-        if not isinstance(sig_obj, Signature) and isinstance(sig_obj, dict):
-            sig_obj = Signature.from_dict(sig_obj)
-        if isinstance(sig_obj, group):
-            # Each task in a group counts toward this chord
-            subtasks = getattr(sig_obj.tasks, "tasks", sig_obj.tasks)
-            return sum(cls._descend(task) for task in subtasks)
-        elif isinstance(sig_obj, _chain):
-            # The last non-empty element in a chain counts toward this chord
-            for child_sig in sig_obj.tasks[-1::-1]:
-                child_size = cls._descend(child_sig)
-                if child_size > 0:
-                    return child_size
-            # We have to just hope this chain is part of some encapsulating
-            # signature which is valid and can fire the chord body
-            return 0
-        elif isinstance(sig_obj, chord):
-            # The child chord's body counts toward this chord
-            return cls._descend(sig_obj.body)
-        elif isinstance(sig_obj, Signature):
-            # Each simple signature counts as 1 completion for this chord
-            return 1
-        # Any other types are assumed to be iterables of simple signatures
-        return len(sig_obj)
-
-    def __length_hint__(self):
-        tasks = getattr(self.tasks, "tasks", self.tasks)
-        return sum(self._descend(task) for task in tasks)
-
-    def run(self, header, body, partial_args, app=None, interval=None,
-            countdown=1, max_retries=None, eager=False,
-            task_id=None, kwargs=None, **options):
-        app = app or self._get_app(body)
-        group_id = header.options.get('task_id') or uuid()
-        root_id = body.options.get('root_id')
-        options = dict(self.options, **options) if options else self.options
-        if options:
-            options.pop('task_id', None)
-            body.options.update(options)
-
-        bodyres = body.freeze(task_id, root_id=root_id)
-
-        # Chains should not be passed to the header tasks. See #3771
-        options.pop('chain', None)
-        # Neither should chords, for deeply nested chords to work
-        options.pop('chord', None)
-        options.pop('task_id', None)
-
-        header_result_args = header._freeze_group_tasks(group_id=group_id, chord=body, root_id=root_id)
-
-        if header.tasks:
-            app.backend.apply_chord(
-                header_result_args,
-                body,
-                interval=interval,
-                countdown=countdown,
-                max_retries=max_retries,
+    def test_chord_size_nested_group_chain_group_mid_many(self):
+        x = chord(
+            group(
+                [self.add.s() | group([self.add.s()] * 4) | self.add.s()] * 2
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 2
+
+    def test_chord_size_nested_group_chain_group_tail_single(self):
+        x = chord(
+            group(
+                [self.add.s() | group(self.add.s())] * 42
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 42
+
+    def test_chord_size_nested_group_chain_group_tail_many(self):
+        x = chord(
+            group(
+                [self.add.s() | group([self.add.s()] * 4)] * 2
+            ),
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 4 * 2
+
+    def test_chord_size_nested_implicit_group_chain_group_tail_single(self):
+        x = chord(
+            [self.add.s() | group(self.add.s())] * 42,
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 42
+
+    def test_chord_size_nested_implicit_group_chain_group_tail_many(self):
+        x = chord(
+            [self.add.s() | group([self.add.s()] * 4)] * 2,
+            body=self.add.s()
+        )
+        assert x.__length_hint__() == 4 * 2
+
+    def test_chord_size_deserialized_element_single(self):
+        child_sig = self.add.s()
+        deserialized_child_sig = json.loads(json.dumps(child_sig))
+        # We have to break in to be sure that a child remains as a `dict` so we
+        # can confirm that the length hint will instantiate a `Signature`
+        # object and then descend as expected
+        chord_sig = chord(tuple())
+        chord_sig.tasks = [deserialized_child_sig]
+        with patch(
+            "celery.canvas.Signature.from_dict", return_value=child_sig
+        ) as mock_from_dict:
+            assert chord_sig.__length_hint__() == 1
+        mock_from_dict.assert_called_once_with(deserialized_child_sig)
+
+    def test_chord_size_deserialized_element_many(self):
+        child_sig = self.add.s()
+        deserialized_child_sig = json.loads(json.dumps(child_sig))
+        # We have to break in to be sure that a child remains as a `dict` so we
+        # can confirm that the length hint will instantiate a `Signature`
+        # object and then descend as expected
+        chord_sig = chord(tuple())
+        chord_sig.tasks = [deserialized_child_sig] * 42
+        with patch(
+            "celery.canvas.Signature.from_dict", return_value=child_sig
+        ) as mock_from_dict:
+            assert chord_sig.__length_hint__() == 42
+        mock_from_dict.assert_has_calls([call(deserialized_child_sig)] * 42)
+
+    def test_set_immutable(self):
+        x = chord([Mock(name='t1'), Mock(name='t2')], app=self.app)
+        x.set_immutable(True)
+
+    def test_links_to_body(self):
+        x = chord([self.add.s(2, 2), self.add.s(4, 4)], body=self.mul.s(4))
+        x.link(self.div.s(2))
+        assert not x.options.get('link')
+        assert x.kwargs['body'].options['link']
+
+        x.link_error(self.div.s(2))
+        assert not x.options.get('link_error')
+        assert x.kwargs['body'].options['link_error']
+
+        assert x.tasks
+        assert x.body
+
+    def test_repr(self):
+        x = chord([self.add.s(2, 2), self.add.s(4, 4)], body=self.mul.s(4))
+        assert repr(x)
+        x.kwargs['body'] = None
+        assert 'without body' in repr(x)
+
+    @pytest.mark.parametrize("group_type", [group,  group_subclass])
+    def test_freeze_tasks_body_is_group(self, subtests, group_type):
+        # Confirm that `group index` values counting up from 0 are set for
+        # elements of a chord's body when the chord is encapsulated in a group
+        body_elem = self.add.s()
+        chord_body = group_type([body_elem] * 42)
+        chord_obj = chord(self.add.s(), body=chord_body)
+        top_group = group_type([chord_obj])
+
+        # We expect the body to be the signature we passed in before we freeze
+        with subtests.test(msg="Validate body type and tasks are retained"):
+            assert isinstance(chord_obj.body, group_type)
+            assert all(
+                embedded_body_elem is body_elem
+                for embedded_body_elem in chord_obj.body.tasks
+            )
+        # We also expect the body to have no initial options - since all of the
+        # embedded body elements are confirmed to be `body_elem` this is valid
+        assert body_elem.options == {}
+        # When we freeze the chord, its body will be cloned and options set
+        top_group.freeze()
+        with subtests.test(
+            msg="Validate body group indices count from 0 after freezing"
+        ):
+            assert isinstance(chord_obj.body, group_type)
+
+            assert all(
+                embedded_body_elem is not body_elem
+                for embedded_body_elem in chord_obj.body.tasks
+            )
+            assert all(
+                embedded_body_elem.options["group_index"] == i
+                for i, embedded_body_elem in enumerate(chord_obj.body.tasks)
             )
-            header_result = header.apply_async(partial_args, kwargs, task_id=group_id, **options)
-        # The execution of a chord body is normally triggered by its header's
-        # tasks completing. If the header is empty this will never happen, so
-        # we execute the body manually here.
-        else:
-            body.delay([])
-            header_result = self.app.GroupResult(*header_result_args)
 
-        bodyres.parent = header_result
-        return bodyres
+    def test_freeze_tasks_is_not_group(self):
+        x = chord([self.add.s(2, 2)], body=self.add.s(), app=self.app)
+        x.freeze()
+        x.tasks = [self.add.s(2, 2)]
+        x.freeze()
+
+    def test_chain_always_eager(self):
+        self.app.conf.task_always_eager = True
+        from celery import _state, result
 
-    def clone(self, *args, **kwargs):
-        signature = super().clone(*args, **kwargs)
-        # need to make copy of body
+        fixture_task_join_will_block = _state.task_join_will_block
         try:
-            signature.kwargs['body'] = maybe_signature(
-                signature.kwargs['body'], clone=True)
-        except (AttributeError, KeyError):
-            pass
-        return signature
-
-    def link(self, callback):
-        self.body.link(callback)
-        return callback
-
-    def link_error(self, errback):
-        self.body.link_error(errback)
-        return errback
-
-    def set_immutable(self, immutable):
-        # changes mutability of header only, not callback.
-        for task in self.tasks:
-            task.set_immutable(immutable)
-
-    def __repr__(self):
-        if self.body:
-            if isinstance(self.body, _chain):
-                return remove_repeating_from_task(
-                    self.body.tasks[0]['task'],
-                    '%({} | {!r})'.format(
-                        self.body.tasks[0].reprcall(self.tasks),
-                        chain(self.body.tasks[1:], app=self._app),
-                    ),
-                )
-            return '%' + remove_repeating_from_task(
-                self.body['task'], self.body.reprcall(self.tasks))
-        return f'<chord without body: {self.tasks!r}>'
-
-    @cached_property
-    def app(self):
-        return self._get_app(self.body)
-
-    def _get_app(self, body=None):
-        app = self._app
-        if app is None:
-            try:
-                tasks = self.tasks.tasks  # is a group
-            except AttributeError:
-                tasks = self.tasks
-            if tasks:
-                app = tasks[0]._app
-            if app is None and body is not None:
-                app = body._app
-        return app if app is not None else current_app
-
-    tasks = getitem_property('kwargs.header', 'Tasks in chord header.')
-    body = getitem_property('kwargs.body', 'Body task of chord.')
-
-
-# Add a back-compat alias for the previous `chord` class name which conflicts
-# with keyword arguments elsewhere in this file
-chord = _chord
-
-
-def signature(varies, *args, **kwargs):
-    """Create new signature.
-
-    - if the first argument is a signature already then it's cloned.
-    - if the first argument is a dict, then a Signature version is returned.
-
-    Returns:
-        Signature: The resulting signature.
-    """
-    app = kwargs.get('app')
-    if isinstance(varies, dict):
-        if isinstance(varies, abstract.CallableSignature):
-            return varies.clone()
-        return Signature.from_dict(varies, app=app)
-    return Signature(varies, *args, **kwargs)
-
-
-subtask = signature  # XXX compat
-
-
-def maybe_signature(d, app=None, clone=False):
-    """Ensure obj is a signature, or None.
-
-    Arguments:
-        d (Optional[Union[abstract.CallableSignature, Mapping]]):
-            Signature or dict-serialized signature.
-        app (celery.Celery):
-            App to bind signature to.
-        clone (bool):
-            If d' is already a signature, the signature
-           will be cloned when this flag is enabled.
-
-    Returns:
-        Optional[abstract.CallableSignature]
-    """
-    if d is not None:
-        if isinstance(d, abstract.CallableSignature):
-            if clone:
-                d = d.clone()
-        elif isinstance(d, dict):
-            d = signature(d)
-
-        if app is not None:
-            d._app = app
-    return d
+            _state.task_join_will_block = _state.orig_task_join_will_block
+            result.task_join_will_block = _state.orig_task_join_will_block
+
+            @self.app.task(shared=False)
+            def finalize(*args):
+                pass
+
+            @self.app.task(shared=False)
+            def chord_add():
+                return chord([self.add.s(4, 4)], finalize.s()).apply_async()
+
+            chord_add.apply_async(throw=True).get()
+        finally:
+            _state.task_join_will_block = fixture_task_join_will_block
+            result.task_join_will_block = fixture_task_join_will_block
+
+    @pytest.mark.parametrize("chord_type", [chord, chord_subclass])
+    def test_from_dict(self, chord_type):
+        header = self.add.s(1, 2)
+        original_chord = chord_type(header=header)
+        rebuilt_chord = chord_type.from_dict(dict(original_chord))
+        assert isinstance(rebuilt_chord, chord_type)
+
+    @pytest.mark.parametrize("chord_type", [chord, chord_subclass])
+    def test_from_dict_with_body(self, chord_type):
+        header = body = self.add.s(1, 2)
+        original_chord = chord_type(header=header, body=body)
+        rebuilt_chord = chord_type.from_dict(dict(original_chord))
+        assert isinstance(rebuilt_chord, chord_type)
+
+    def test_from_dict_deep_deserialize(self, subtests):
+        header = body = self.add.s(1, 2)
+        original_chord = chord(header=header, body=body)
+        serialized_chord = json.loads(json.dumps(original_chord))
+        deserialized_chord = chord.from_dict(serialized_chord)
+        with subtests.test(msg="Verify chord is deserialized"):
+            assert isinstance(deserialized_chord, chord)
+        with subtests.test(msg="Validate chord header tasks is deserialized"):
+            assert all(
+                isinstance(child_task, Signature)
+                for child_task in deserialized_chord.tasks
+            )
+        with subtests.test(msg="Verify chord body is deserialized"):
+            assert isinstance(deserialized_chord.body, Signature)
+
+    @pytest.mark.parametrize("group_type", [group, group_subclass])
+    def test_from_dict_deep_deserialize_group(self, subtests, group_type):
+        header = body = group_type([self.add.s(1, 2)] * 42)
+        original_chord = chord(header=header, body=body)
+        serialized_chord = json.loads(json.dumps(original_chord))
+        deserialized_chord = chord.from_dict(serialized_chord)
+        with subtests.test(msg="Verify chord is deserialized"):
+            assert isinstance(deserialized_chord, chord)
+        # A header which is a group gets unpacked into the chord's `tasks`
+        with subtests.test(
+            msg="Validate chord header tasks are deserialized and unpacked"
+        ):
+            assert all(
+                isinstance(child_task, Signature)
+                and not isinstance(child_task, group_type)
+                for child_task in deserialized_chord.tasks
+            )
+        # A body which is a group remains as it we passed in
+        with subtests.test(
+            msg="Validate chord body is deserialized and not unpacked"
+        ):
+            assert isinstance(deserialized_chord.body, group_type)
+            assert all(
+                isinstance(body_child_task, Signature)
+                for body_child_task in deserialized_chord.body.tasks
+            )
 
+    @pytest.mark.parametrize("group_type", [group, group_subclass])
+    def test_from_dict_deeper_deserialize_group(self, subtests, group_type):
+        inner_group = group_type([self.add.s(1, 2)] * 42)
+        header = body = group_type([inner_group] * 42)
+        original_chord = chord(header=header, body=body)
+        serialized_chord = json.loads(json.dumps(original_chord))
+        deserialized_chord = chord.from_dict(serialized_chord)
+        with subtests.test(msg="Verify chord is deserialized"):
+            assert isinstance(deserialized_chord, chord)
+        # A header which is a group gets unpacked into the chord's `tasks`
+        with subtests.test(
+            msg="Validate chord header tasks are deserialized and unpacked"
+        ):
+            assert all(
+                isinstance(child_task, group_type)
+                for child_task in deserialized_chord.tasks
+            )
+            assert all(
+                isinstance(grandchild_task, Signature)
+                for child_task in deserialized_chord.tasks
+                for grandchild_task in child_task.tasks
+            )
+        # A body which is a group remains as it we passed in
+        with subtests.test(
+            msg="Validate chord body is deserialized and not unpacked"
+        ):
+            assert isinstance(deserialized_chord.body, group)
+            assert all(
+                isinstance(body_child_task, group)
+                for body_child_task in deserialized_chord.body.tasks
+            )
+            assert all(
+                isinstance(body_grandchild_task, Signature)
+                for body_child_task in deserialized_chord.body.tasks
+                for body_grandchild_task in body_child_task.tasks
+            )
 
-maybe_subtask = maybe_signature  # XXX compat
+    def test_from_dict_deep_deserialize_chain(self, subtests):
+        header = body = chain([self.add.s(1, 2)] * 42)
+        original_chord = chord(header=header, body=body)
+        serialized_chord = json.loads(json.dumps(original_chord))
+        deserialized_chord = chord.from_dict(serialized_chord)
+        with subtests.test(msg="Verify chord is deserialized"):
+            assert isinstance(deserialized_chord, chord)
+        # A header which is a chain gets unpacked into the chord's `tasks`
+        with subtests.test(
+            msg="Validate chord header tasks are deserialized and unpacked"
+        ):
+            assert all(
+                isinstance(child_task, Signature)
+                and not isinstance(child_task, chain)
+                for child_task in deserialized_chord.tasks
+            )
+        # A body which is a chain gets mutatated into the hidden `_chain` class
+        with subtests.test(
+            msg="Validate chord body is deserialized and not unpacked"
+        ):
+            assert isinstance(deserialized_chord.body, _chain)
+
+    def test_chord_clone_kwargs(self, subtests):
+        """ Test that chord clone ensures the kwargs are the same """
+
+        with subtests.test(msg='Verify chord cloning clones kwargs correctly'):
+            c = chord([signature('g'), signature('h')], signature('i'), kwargs={'U': 6})
+            c2 = c.clone()
+            assert c2.kwargs == c.kwargs
+
+        with subtests.test(msg='Cloning the chord with overridden kwargs'):
+            override_kw = {'X': 2}
+            c3 = c.clone(args=(1,), kwargs=override_kw)
+
+        with subtests.test(msg='Verify the overridden kwargs were cloned correctly'):
+            new_kw = c.kwargs.copy()
+            new_kw.update(override_kw)
+            assert c3.kwargs == new_kw
+
+    def test_flag_allow_error_cb_on_chord_header(self, subtests):
+        header_mock = [Mock(name='t1'), Mock(name='t2')]
+        header = group(header_mock)
+        body = Mock(name='tbody')
+        errback_sig = Mock(name='errback_sig')
+        chord_sig = chord(header, body, app=self.app)
+
+        with subtests.test(msg='Verify the errback is not linked'):
+            # header
+            for child_sig in header_mock:
+                child_sig.link_error.assert_not_called()
+            # body
+            body.link_error.assert_not_called()
+
+        with subtests.test(msg='Verify flag turned off links only the body'):
+            self.app.conf.task_allow_error_cb_on_chord_header = False
+            chord_sig.link_error(errback_sig)
+            # header
+            for child_sig in header_mock:
+                child_sig.link_error.assert_not_called()
+            # body
+            body.link_error.assert_called_once_with(errback_sig)
+
+        with subtests.test(msg='Verify flag turned on links the header'):
+            self.app.conf.task_allow_error_cb_on_chord_header = True
+            chord_sig.link_error(errback_sig)
+            # header
+            for child_sig in header_mock:
+                child_sig.link_error.assert_called_once_with(errback_sig)
+            # body
+            body.link_error.assert_has_calls([call(errback_sig), call(errback_sig)])
+
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_flag_allow_error_cb_on_chord_header_various_header_types(self):
+        """ Test chord link_error with various header types. """
+        self.app.conf.task_allow_error_cb_on_chord_header = True
+        headers = [
+            signature('t'),
+            [signature('t'), signature('t')],
+            group(signature('t'), signature('t'))
+        ]
+        for chord_header in headers:
+            c = chord(chord_header, signature('t'))
+            sig = signature('t')
+            errback = c.link_error(sig)
+            assert errback == sig
+
+    def test_chord__or__group_of_single_task(self):
+        """ Test chaining a chord to a group of a single task. """
+        c = chord([signature('header')], signature('body'))
+        g = group(signature('t'))
+        stil_chord = c | g  # g should be chained with the body of c
+        assert isinstance(stil_chord, chord)
+        assert isinstance(stil_chord.body, _chain)
+
+    def test_chord_upgrade_on_chaining(self):
+        """ Test that chaining a chord with a group body upgrades to a new chord """
+        c = chord([signature('header')], group(signature('body')))
+        t = signature('t')
+        stil_chord = c | t  # t should be chained with the body of c and create a new chord
+        assert isinstance(stil_chord, chord)
+        assert isinstance(stil_chord.body, chord)
+
+    @pytest.mark.parametrize('header', [
+        [signature('s1'), signature('s2')],
+        group(signature('s1'), signature('s2'))
+    ])
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_link_error_on_chord_header(self, header):
+        """ Test that link_error on a chord also links the header """
+        self.app.conf.task_allow_error_cb_on_chord_header = True
+        c = chord(header, signature('body'))
+        err = signature('err')
+        errback = c.link_error(err)
+        assert errback == err
+        for header_task in c.tasks:
+            assert header_task.options['link_error'] == [err]
+        assert c.body.options['link_error'] == [err]
+
+
+class test_maybe_signature(CanvasCase):
+
+    def test_is_None(self):
+        assert maybe_signature(None, app=self.app) is None
+
+    def test_is_dict(self):
+        assert isinstance(maybe_signature(dict(self.add.s()), app=self.app),
+                          Signature)
+
+    def test_when_sig(self):
+        s = self.add.s()
+        assert maybe_signature(s, app=self.app) is s
+
+
+class test_merge_dictionaries(CanvasCase):
+
+    def test_docstring_example(self):
+        d1 = {'dict': {'a': 1}, 'list': [1, 2], 'tuple': (1, 2)}
+        d2 = {'dict': {'b': 2}, 'list': [3, 4], 'set': {'a', 'b'}}
+        _merge_dictionaries(d1, d2)
+        assert d1 == {
+            'dict': {'a': 1, 'b': 2},
+            'list': [1, 2, 3, 4],
+            'tuple': (1, 2),
+            'set': {'a', 'b'}
+        }
+
+    @pytest.mark.parametrize('d1,d2,expected_result', [
+        (
+            {'None': None},
+            {'None': None},
+            {'None': [None]}
+        ),
+        (
+            {'None': None},
+            {'None': [None]},
+            {'None': [[None]]}
+        ),
+        (
+            {'None': None},
+            {'None': 'Not None'},
+            {'None': ['Not None']}
+        ),
+        (
+            {'None': None},
+            {'None': ['Not None']},
+            {'None': [['Not None']]}
+        ),
+        (
+            {'None': [None]},
+            {'None': None},
+            {'None': [None, None]}
+        ),
+        (
+            {'None': [None]},
+            {'None': [None]},
+            {'None': [None, None]}
+        ),
+        (
+            {'None': [None]},
+            {'None': 'Not None'},
+            {'None': [None, 'Not None']}
+        ),
+        (
+            {'None': [None]},
+            {'None': ['Not None']},
+            {'None': [None, 'Not None']}
+        ),
+    ])
+    def test_none_values(self, d1, d2, expected_result):
+        _merge_dictionaries(d1, d2)
+        assert d1 == expected_result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `celery-5.3.0b1/celery/concurrency/asynpool.py` & `celery-5.3.0b2/celery/concurrency/asynpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # pylint: disable=redefined-outer-name
 # We cache globals and attribute lookups, so disable this warning.
 
 try:
     from _billiard import read as __read__
     readcanbuf = True
 
-except ImportError:  # pragma: no cover
+except ImportError:
 
     def __read__(fd, buf, size, read=os.read):
         chunk = read(fd, size)
         n = len(chunk)
         if n != 0:
             buf.write(chunk)
         return n
```

### Comparing `celery-5.3.0b1/celery/concurrency/base.py` & `celery-5.3.0b2/celery/concurrency/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base Execution Pool."""
 import logging
 import os
 import sys
 import time
+from typing import Any, Dict
 
 from billiard.einfo import ExceptionInfo
 from billiard.exceptions import WorkerLostError
 from kombu.utils.encoding import safe_repr
 
 from celery.exceptions import WorkerShutdown, WorkerTerminate, reraise
 from celery.utils import timer2
@@ -150,16 +151,23 @@
                          truncate(safe_repr(kwargs), 1024))
 
         return self.on_apply(target, args, kwargs,
                              waitforslot=self.putlocks,
                              callbacks_propagate=self.callbacks_propagate,
                              **options)
 
-    def _get_info(self):
+    def _get_info(self) -> Dict[str, Any]:
+        """
+        Return configuration and statistics information. Subclasses should
+        augment the data as required.
+
+        :return: The returned value must be JSON-friendly.
+        """
         return {
+            'implementation': self.__class__.__module__ + ':' + self.__class__.__name__,
             'max-concurrency': self.limit,
         }
 
     @property
     def info(self):
         return self._get_info()
```

### Comparing `celery-5.3.0b1/celery/concurrency/eventlet.py` & `celery-5.3.0b2/celery/concurrency/eventlet.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/concurrency/gevent.py` & `celery-5.3.0b2/celery/concurrency/gevent.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from kombu.asynchronous import timer as _timer
 
 from . import base
 
 try:
     from gevent import Timeout
-except ImportError:  # pragma: no cover
+except ImportError:
     Timeout = None
 
 __all__ = ('TaskPool',)
 
 # pylint: disable=redefined-outer-name
 # We cache globals and attribute lookups, so disable this warning.
```

### Comparing `celery-5.3.0b1/celery/concurrency/prefork.py` & `celery-5.3.0b2/celery/concurrency/prefork.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,20 +151,22 @@
 
     def on_close(self):
         if self._pool is not None and self._pool._state == RUN:
             self._pool.close()
 
     def _get_info(self):
         write_stats = getattr(self._pool, 'human_write_stats', None)
-        return {
+        info = super()._get_info()
+        info.update({
             'max-concurrency': self.limit,
             'processes': [p.pid for p in self._pool._pool],
             'max-tasks-per-child': self._pool._maxtasksperchild or 'N/A',
             'put-guarded-by-semaphore': self.putlocks,
             'timeouts': (self._pool.soft_timeout or 0,
                          self._pool.timeout or 0),
             'writes': write_stats() if write_stats is not None else 'N/A',
-        }
+        })
+        return info
 
     @property
     def num_processes(self):
         return self._pool._processes
```

### Comparing `celery-5.3.0b1/celery/concurrency/solo.py` & `celery-5.3.0b2/celery/concurrency/solo.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.on_apply = apply_target
         self.limit = 1
         signals.worker_process_init.send(sender=None)
 
     def _get_info(self):
-        return {
+        info = super()._get_info()
+        info.update({
             'max-concurrency': 1,
             'processes': [os.getpid()],
             'max-tasks-per-child': None,
             'put-guarded-by-semaphore': True,
             'timeouts': (),
-        }
+        })
+        return info
```

### Comparing `celery-5.3.0b1/celery/contrib/abortable.py` & `celery-5.3.0b2/celery/contrib/abortable.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/contrib/migrate.py` & `celery-5.3.0b2/celery/contrib/migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/contrib/pytest.py` & `celery-5.3.0b2/celery/contrib/pytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Fixtures and testing utilities for :pypi:`pytest <pytest>`."""
 import os
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Mapping, Sequence, Union
+from typing import TYPE_CHECKING, Any, Mapping, Sequence, Union  # noqa
 
 import pytest
 
 if TYPE_CHECKING:
     from celery import Celery
 
     from ..worker import WorkController
```

### Comparing `celery-5.3.0b1/celery/contrib/rdb.py` & `celery-5.3.0b2/celery/contrib/rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/contrib/sphinx.py` & `celery-5.3.0b2/celery/contrib/sphinx.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 task decorated objects (e.g. when using the automodule directive)
 and generate the correct (as well as add a ``(task)`` prefix),
 and you can also refer to the tasks using `:task:proj.tasks.add`
 syntax.
 
 Use ``.. autotask::`` to alternatively manually document a task.
 """
-from inspect import formatargspec, getfullargspec
+from inspect import signature
 
+from docutils import nodes
 from sphinx.domains.python import PyFunction
 from sphinx.ext.autodoc import FunctionDocumenter
 
 from celery.app.task import BaseTask
 
 
 class TaskDocumenter(FunctionDocumenter):
@@ -47,20 +48,18 @@
     @classmethod
     def can_document_member(cls, member, membername, isattr, parent):
         return isinstance(member, BaseTask) and getattr(member, '__wrapped__')
 
     def format_args(self):
         wrapped = getattr(self.object, '__wrapped__', None)
         if wrapped is not None:
-            argspec = getfullargspec(wrapped)
-            if argspec[0] and argspec[0][0] in ('cls', 'self'):
-                del argspec[0][0]
-            fmt = formatargspec(*argspec)
-            fmt = fmt.replace('\\', '\\\\')
-            return fmt
+            sig = signature(wrapped)
+            if "self" in sig.parameters or "cls" in sig.parameters:
+                sig = sig.replace(parameters=list(sig.parameters.values())[1:])
+            return str(sig)
         return ''
 
     def document_members(self, all_members=False):
         pass
 
     def check_module(self):
         # Normally checks if *self.object* is really defined in the module
@@ -73,15 +72,15 @@
         return super().check_module()
 
 
 class TaskDirective(PyFunction):
     """Sphinx task directive."""
 
     def get_signature_prefix(self, sig):
-        return self.env.config.celery_task_prefix
+        return [nodes.Text(self.env.config.celery_task_prefix)]
 
 
 def autodoc_skip_member_handler(app, what, name, obj, skip, options):
     """Handler for autodoc-skip-member event."""
     # Celery tasks created with the @task decorator have the property
     # that *obj.__doc__* and *obj.__class__.__doc__* are equal, which
     # trips up the logic in sphinx.ext.autodoc that is supposed to
```

### Comparing `celery-5.3.0b1/celery/contrib/testing/app.py` & `celery-5.3.0b2/celery/contrib/testing/app.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/contrib/testing/manager.py` & `celery-5.3.0b2/celery/contrib/testing/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Integration testing utilities."""
 import socket
 import sys
 from collections import defaultdict
 from functools import partial
 from itertools import count
-from typing import Any, Callable, Dict, Sequence, TextIO, Tuple
+from typing import Any, Callable, Dict, Sequence, TextIO, Tuple  # noqa
 
 from kombu.utils.functional import retry_over_time
 
 from celery import states
 from celery.exceptions import TimeoutError
-from celery.result import AsyncResult, ResultSet
+from celery.result import AsyncResult, ResultSet  # noqa
 from celery.utils.text import truncate
 from celery.utils.time import humanize_seconds as _humanize_seconds
 
 E_STILL_WAITING = 'Still waiting for {0}.  Trying again {when}: {exc!r}'
 
 humanize_seconds = partial(_humanize_seconds, microseconds=True)
```

### Comparing `celery-5.3.0b1/celery/contrib/testing/mocks.py` & `celery-5.3.0b2/celery/contrib/testing/mocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Useful mocks for unit testing."""
 import numbers
 from datetime import datetime, timedelta
-from typing import Any, Mapping, Sequence
+from typing import Any, Mapping, Sequence  # noqa
 from unittest.mock import Mock
 
-from celery import Celery
-from celery.canvas import Signature
+from celery import Celery  # noqa
+from celery.canvas import Signature  # noqa
 
 
 def TaskMessage(
     name,  # type: str
     id=None,  # type: str
     args=(),  # type: Sequence
     kwargs=None,  # type: Mapping
```

### Comparing `celery-5.3.0b1/celery/contrib/testing/worker.py` & `celery-5.3.0b2/celery/contrib/testing/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Embedded workers for integration tests."""
 import os
 import threading
 from contextlib import contextmanager
-from typing import Any, Iterable, Union
+from typing import Any, Iterable, Union  # noqa
 
-import celery.worker.consumer
-from celery import Celery, worker
+import celery.worker.consumer  # noqa
+from celery import Celery, worker  # noqa
 from celery.result import _set_task_join_will_block, allow_join_result
 from celery.utils.dispatch import Signal
 from celery.utils.nodenames import anon_nodename
 
 WORKER_LOGLEVEL = os.environ.get('WORKER_LOGLEVEL', 'error')
 
 test_worker_starting = Signal(
@@ -68,14 +68,15 @@
     """Start embedded worker.
 
     Yields:
         celery.app.worker.Worker: worker instance.
     """
     test_worker_starting.send(sender=app)
 
+    worker = None
     try:
         with _start_worker_thread(app,
                                   concurrency=concurrency,
                                   pool=pool,
                                   loglevel=loglevel,
                                   logfile=logfile,
                                   perform_ping_check=perform_ping_check,
```

### Comparing `celery-5.3.0b1/celery/events/cursesmon.py` & `celery-5.3.0b2/celery/events/cursesmon.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/dispatcher.py` & `celery-5.3.0b2/celery/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/dumper.py` & `celery-5.3.0b2/celery/events/dumper.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/event.py` & `celery-5.3.0b2/celery/events/event.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/receiver.py` & `celery-5.3.0b2/celery/events/receiver.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/snapshot.py` & `celery-5.3.0b2/celery/events/snapshot.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/events/state.py` & `celery-5.3.0b2/celery/events/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from collections import defaultdict
 from collections.abc import Callable
 from datetime import datetime
 from decimal import Decimal
 from itertools import islice
 from operator import itemgetter
 from time import time
-from typing import Mapping, Optional
+from typing import Mapping, Optional  # noqa
 from weakref import WeakSet, ref
 
 from kombu.clocks import timetuple
 from kombu.utils.objects import cached_property
 
 from celery import states
 from celery.utils.functional import LRUCache, memoize, pass1
```

### Comparing `celery-5.3.0b1/celery/exceptions.py` & `celery-5.3.0b2/celery/exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/fixups/django.py` & `celery-5.3.0b2/celery/fixups/django.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,16 @@
     def django_setup(self) -> None:
         import django
         django.setup()
 
     def validate_models(self) -> None:
         from django.core.checks import run_checks
         self.django_setup()
-        run_checks()
+        if not os.environ.get('CELERY_SKIP_CHECKS'):
+            run_checks()
 
     def install(self) -> "DjangoWorkerFixup":
         signals.beat_embedded_init.connect(self.close_database)
         signals.task_prerun.connect(self.on_task_prerun)
         signals.task_postrun.connect(self.on_task_postrun)
         signals.worker_process_init.connect(self.on_worker_process_init)
         self.close_database()
```

### Comparing `celery-5.3.0b1/celery/loaders/base.py` & `celery-5.3.0b2/celery/loaders/base.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/loaders/default.py` & `celery-5.3.0b2/celery/loaders/default.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/local.py` & `celery-5.3.0b2/celery/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,15 @@
         '_object_origins': origins,
         '__all__': _all,
     }
     new_module = create_module(name, attrs, cls_attrs=cattrs, base=base)
     new_module.__dict__.update({
         mod: get_compat_module(new_module, mod) for mod in compat_modules
     })
+    new_module.__spec__ = old_module.__spec__
     return old_module, new_module
 
 
 def get_compat_module(pkg, name):
     def prepare(attr):
         if isinstance(attr, str):
             return Proxy(getappattr, (attr,))
```

### Comparing `celery-5.3.0b1/celery/platforms.py` & `celery-5.3.0b2/celery/platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 import math
 import numbers
 import os
 import platform as _platform
 import signal as _signal
 import sys
 import warnings
-from collections import namedtuple
 from contextlib import contextmanager
 
 from billiard.compat import close_open_fds, get_fdmax
 from billiard.util import set_pdeathsig as _set_pdeathsig
 # fileno used to be in this module
 from kombu.utils.compat import maybe_fileno
 from kombu.utils.encoding import safe_str
 
 from .exceptions import SecurityError, SecurityWarning, reraise
 from .local import try_import
 
 try:
     from billiard.process import current_process
-except ImportError:  # pragma: no cover
+except ImportError:
     current_process = None
 
 _setproctitle = try_import('setproctitle')
 resource = try_import('resource')
 pwd = try_import('pwd')
 grp = try_import('grp')
 mputil = try_import('multiprocessing.util')
@@ -39,15 +38,15 @@
 __all__ = (
     'EX_OK', 'EX_FAILURE', 'EX_UNAVAILABLE', 'EX_USAGE', 'SYSTEM',
     'IS_macOS', 'IS_WINDOWS', 'SIGMAP', 'pyimplementation', 'LockFailed',
     'get_fdmax', 'Pidfile', 'create_pidlock', 'close_open_fds',
     'DaemonContext', 'detached', 'parse_uid', 'parse_gid', 'setgroups',
     'initgroups', 'setgid', 'setuid', 'maybe_drop_privileges', 'signals',
     'signal_name', 'set_process_title', 'set_mp_process_title',
-    'get_errno_name', 'ignore_errno', 'fd_by_path', 'isatty',
+    'get_errno_name', 'ignore_errno', 'fd_by_path',
 )
 
 # exitcodes
 EX_OK = getattr(os, 'EX_OK', 0)
 EX_FAILURE = 1
 EX_UNAVAILABLE = getattr(os, 'EX_UNAVAILABLE', 69)
 EX_USAGE = getattr(os, 'EX_USAGE', 64)
@@ -61,16 +60,14 @@
 
 PIDFILE_FLAGS = os.O_CREAT | os.O_EXCL | os.O_WRONLY
 PIDFILE_MODE = ((os.R_OK | os.W_OK) << 6) | ((os.R_OK) << 3) | (os.R_OK)
 
 PIDLOCKED = """ERROR: Pidfile ({0}) already exists.
 Seems we're already running? (pid: {1})"""
 
-_range = namedtuple('_range', ('start', 'stop'))
-
 ROOT_DISALLOWED = """\
 Running a worker with superuser privileges when the
 worker accepts messages serialized with pickle is a very bad idea!
 
 If you really want to continue then you have to set the C_FORCE_ROOT
 environment variable (but please think about this before you do).
 
@@ -94,22 +91,14 @@
 SIGNAMES = {
     sig for sig in dir(_signal)
     if sig.startswith('SIG') and '_' not in sig
 }
 SIGMAP = {getattr(_signal, name): name for name in SIGNAMES}
 
 
-def isatty(fh):
-    """Return true if the process has a controlling terminal."""
-    try:
-        return fh.isatty()
-    except AttributeError:
-        pass
-
-
 def pyimplementation():
     """Return string identifying the current Python implementation."""
     if hasattr(_platform, 'python_implementation'):
         return _platform.python_implementation()
     elif sys.platform.startswith('java'):
         return 'Jython ' + sys.platform
     elif hasattr(sys, 'pypy_version_info'):
@@ -182,15 +171,15 @@
         """Remove the lock."""
         with ignore_errno(errno.ENOENT, errno.EACCES):
             os.unlink(self.path)
 
     def remove_if_stale(self):
         """Remove the lock if the process isn't running.
 
-        I.e. process does not respons to signal.
+        I.e. process does not respond to signal.
         """
         try:
             pid = self.read_pid()
         except ValueError:
             print('Broken pidfile found - Removing it.', file=sys.stderr)
             self.remove()
             return True
```

### Comparing `celery-5.3.0b1/celery/result.py` & `celery-5.3.0b2/celery/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,38 @@
             timeout (float): Time in seconds to wait for replies when
                 ``wait`` is enabled.
         """
         self.app.control.revoke(self.id, connection=connection,
                                 terminate=terminate, signal=signal,
                                 reply=wait, timeout=timeout)
 
+    def revoke_by_stamped_headers(self, headers, connection=None, terminate=False, signal=None,
+                                  wait=False, timeout=None):
+        """Send revoke signal to all workers only for tasks with matching headers values.
+
+        Any worker receiving the task, or having reserved the
+        task, *must* ignore it.
+        All header fields *must* match.
+
+        Arguments:
+            headers (dict[str, Union(str, list)]): Headers to match when revoking tasks.
+            terminate (bool): Also terminate the process currently working
+                on the task (if any).
+            signal (str): Name of signal to send to process if terminate.
+                Default is TERM.
+            wait (bool): Wait for replies from workers.
+                The ``timeout`` argument specifies the seconds to wait.
+                Disabled by default.
+            timeout (float): Time in seconds to wait for replies when
+                ``wait`` is enabled.
+        """
+        self.app.control.revoke_by_stamped_headers(headers, connection=connection,
+                                                   terminate=terminate, signal=signal,
+                                                   reply=wait, timeout=timeout)
+
     def get(self, timeout=None, propagate=True, interval=0.5,
             no_ack=True, follow_parents=True, callback=None, on_message=None,
             on_interval=None, disable_sync_subtasks=True,
             EXCEPTION_STATES=states.EXCEPTION_STATES,
             PROPAGATE_STATES=states.PROPAGATE_STATES):
         """Wait until task is ready, and return its result.
 
@@ -623,16 +647,19 @@
             bool: true if all of the tasks have been executed.
         """
         return all(result.ready() for result in self.results)
 
     def completed_count(self):
         """Task completion count.
 
+        Note that `complete` means `successful` in this context. In other words, the
+        return value of this method is the number of ``successful`` tasks.
+
         Returns:
-            int: the number of tasks completed.
+            int: the number of complete (i.e. successful) tasks.
         """
         return sum(int(result.successful()) for result in self.results)
 
     def forget(self):
         """Forget about (and possible remove the result of) all the tasks."""
         for result in self.results:
             result.forget()
```

### Comparing `celery-5.3.0b1/celery/schedules.py` & `celery-5.3.0b2/celery/schedules.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 """
 
 CRON_REPR = """\
 <crontab: {0._orig_minute} {0._orig_hour} {0._orig_day_of_month} {0._orig_month_of_year} \
 {0._orig_day_of_week} (m/h/dM/MY/d)>\
 """
 
-
 SOLAR_INVALID_LATITUDE = """\
 Argument latitude {lat} is invalid, must be between -90 and 90.\
 """
 
 SOLAR_INVALID_LONGITUDE = """\
 Argument longitude {lon} is invalid, must be between -180 and 180.\
 """
@@ -69,16 +68,16 @@
 
     def remaining_estimate(self, last_run_at):
         raise NotImplementedError()
 
     def is_due(self, last_run_at):
         raise NotImplementedError()
 
-    def maybe_make_aware(self, dt):
-        return maybe_make_aware(dt, self.tz)
+    def maybe_make_aware(self, dt, naive_as_utc=True):
+        return maybe_make_aware(dt, self.tz, naive_as_utc=naive_as_utc)
 
     @property
     def app(self):
         return self._app or current_app._get_current_object()
 
     @app.setter
     def app(self, app):
@@ -436,15 +435,15 @@
         elif isinstance(cronspec, set):
             result = cronspec
         elif isinstance(cronspec, Iterable):
             result = set(cronspec)
         else:
             raise TypeError(CRON_INVALID_TYPE.format(type=type(cronspec)))
 
-        # assure the result does not preceed the min or exceed the max
+        # assure the result does not precede the min or exceed the max
         for number in result:
             if number >= max_ + min_ or number < min_:
                 raise ValueError(CRON_PATTERN_INVALID.format(
                     min=min_, max=max_ - 1 + min_, value=number))
         return result
 
     def _delta_to_next(self, last_run_at, next_hour, next_minute):
@@ -465,17 +464,16 @@
             try:
                 datetime(year=year, month=month, day=day)
             except ValueError:
                 return True
             return False
 
         def is_before_last_run(year, month, day):
-            return self.maybe_make_aware(datetime(year,
-                                                  month,
-                                                  day)) < last_run_at
+            return self.maybe_make_aware(datetime(year, month, day, next_hour, next_minute),
+                                         naive_as_utc=False) < last_run_at
 
         def roll_over():
             for _ in range(2000):
                 flag = (datedata.dom == len(days_of_month) or
                         day_out_of_range(datedata.year,
                                          months_of_year[datedata.moy],
                                          days_of_month[datedata.dom]) or
@@ -604,24 +602,56 @@
         # pylint: disable=redefined-outer-name
         # caching global ffwd
         return remaining(*self.remaining_delta(last_run_at, ffwd=ffwd))
 
     def is_due(self, last_run_at):
         """Return tuple of ``(is_due, next_time_to_run)``.
 
+        If :setting:`beat_cron_starting_deadline`  has been specified, the
+        scheduler will make sure that the `last_run_at` time is within the
+        deadline. This prevents tasks that could have been run according to
+        the crontab, but didn't, from running again unexpectedly.
+
         Note:
             Next time to run is in seconds.
 
         SeeAlso:
             :meth:`celery.schedules.schedule.is_due` for more information.
         """
+
         rem_delta = self.remaining_estimate(last_run_at)
-        rem = max(rem_delta.total_seconds(), 0)
+        rem_secs = rem_delta.total_seconds()
+        rem = max(rem_secs, 0)
         due = rem == 0
-        if due:
+
+        deadline_secs = self.app.conf.beat_cron_starting_deadline
+        has_passed_deadline = False
+        if deadline_secs is not None:
+            # Make sure we're looking at the latest possible feasible run
+            # date when checking the deadline.
+            last_date_checked = last_run_at
+            last_feasible_rem_secs = rem_secs
+            while rem_secs < 0:
+                last_date_checked = last_date_checked + abs(rem_delta)
+                rem_delta = self.remaining_estimate(last_date_checked)
+                rem_secs = rem_delta.total_seconds()
+                if rem_secs < 0:
+                    last_feasible_rem_secs = rem_secs
+
+            # if rem_secs becomes 0 or positive, second-to-last
+            # last_date_checked must be the last feasible run date.
+            # Check if the last feasible date is within the deadline
+            # for running
+            has_passed_deadline = -last_feasible_rem_secs > deadline_secs
+            if has_passed_deadline:
+                # Should not be due if we've passed the deadline for looking
+                # at past runs
+                due = False
+
+        if due or has_passed_deadline:
             rem_delta = self.remaining_estimate(self.now())
             rem = max(rem_delta.total_seconds(), 0)
         return schedstate(due, rem)
 
     def __eq__(self, other):
         if isinstance(other, crontab):
             return (
```

### Comparing `celery-5.3.0b1/celery/security/__init__.py` & `celery-5.3.0b2/celery/security/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/security/certificate.py` & `celery-5.3.0b2/celery/security/certificate.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """X.509 certificates."""
 import datetime
 import glob
 import os
 
 from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.x509 import load_pem_x509_certificate
 from kombu.utils.encoding import bytes_to_str, ensure_bytes
 
 from celery.exceptions import SecurityError
 
 from .utils import reraise_errors
 
@@ -21,20 +21,23 @@
     def __init__(self, cert):
         with reraise_errors(
             'Invalid certificate: {0!r}', errors=(ValueError,)
         ):
             self._cert = load_pem_x509_certificate(
                 ensure_bytes(cert), backend=default_backend())
 
+            if not isinstance(self._cert.public_key(), rsa.RSAPublicKey):
+                raise ValueError("Non-RSA certificates are not supported.")
+
     def has_expired(self):
         """Check if the certificate has expired."""
         return datetime.datetime.utcnow() >= self._cert.not_valid_after
 
-    def get_pubkey(self):
-        """Get public key from certificate."""
+    def get_pubkey(self) -> rsa.RSAPublicKey:
+        """Get public key from certificate. Public key type is checked in __init__."""
         return self._cert.public_key()
 
     def get_serial_number(self):
         """Return the serial number in the certificate."""
         return self._cert.serial_number
 
     def get_issuer(self):
@@ -45,20 +48,20 @@
         """Serial number/issuer pair uniquely identifies a certificate."""
         return f'{self.get_issuer()} {self.get_serial_number()}'
 
     def verify(self, data, signature, digest):
         """Verify signature for string containing data."""
         with reraise_errors('Bad signature: {0!r}'):
 
-            padd = padding.PSS(
+            pad = padding.PSS(
                 mgf=padding.MGF1(digest),
                 salt_length=padding.PSS.MAX_LENGTH)
 
             self.get_pubkey().verify(signature,
-                                     ensure_bytes(data), padd, digest)
+                                     ensure_bytes(data), pad, digest)
 
 
 class CertStore:
     """Base class for certificate stores."""
 
     def __init__(self):
         self._certs = {}
```

### Comparing `celery-5.3.0b1/celery/security/key.py` & `celery-5.3.0b2/celery/security/key.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Private keys for the security serializer."""
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
-from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from kombu.utils.encoding import ensure_bytes
 
 from .utils import reraise_errors
 
 __all__ = ('PrivateKey',)
 
 
@@ -17,16 +17,19 @@
             'Invalid private key: {0!r}', errors=(ValueError,)
         ):
             self._key = serialization.load_pem_private_key(
                 ensure_bytes(key),
                 password=ensure_bytes(password),
                 backend=default_backend())
 
+            if not isinstance(self._key, rsa.RSAPrivateKey):
+                raise ValueError("Non-RSA keys are not supported.")
+
     def sign(self, data, digest):
         """Sign string containing data."""
         with reraise_errors('Unable to sign data: {0!r}'):
 
-            padd = padding.PSS(
+            pad = padding.PSS(
                 mgf=padding.MGF1(digest),
                 salt_length=padding.PSS.MAX_LENGTH)
 
-            return self._key.sign(ensure_bytes(data), padd, digest)
+            return self._key.sign(ensure_bytes(data), pad, digest)
```

### Comparing `celery-5.3.0b1/celery/security/serialization.py` & `celery-5.3.0b2/celery/security/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/security/utils.py` & `celery-5.3.0b2/celery/security/utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/signals.py` & `celery-5.3.0b2/celery/signals.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/states.py` & `celery-5.3.0b2/celery/states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/__init__.py` & `celery-5.3.0b2/celery/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/abstract.py` & `celery-5.3.0b2/celery/utils/abstract.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/collections.py` & `celery-5.3.0b2/celery/utils/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from collections import OrderedDict as _OrderedDict
 from collections import deque
 from collections.abc import Callable, Mapping, MutableMapping, MutableSet, Sequence
 from heapq import heapify, heappop, heappush
 from itertools import chain, count
 from queue import Empty
-from typing import Any, Dict, Iterable, List
+from typing import Any, Dict, Iterable, List  # noqa
 
 from .functional import first, uniq
 from .text import match_case
 
 try:
     # pypy: dicts are ordered in recent versions
     from __pypy__ import reversed_dict as _dict_is_ordered
```

### Comparing `celery-5.3.0b1/celery/utils/debug.py` & `celery-5.3.0b2/celery/utils/debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/deprecated.py` & `celery-5.3.0b2/celery/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/dispatch/signal.py` & `celery-5.3.0b2/celery/utils/dispatch/signal.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/functional.py` & `celery-5.3.0b2/celery/utils/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Functional-style utilities."""
 import inspect
-import sys
 from collections import UserList
 from functools import partial
 from itertools import islice, tee, zip_longest
+from typing import Any, Callable
 
 from kombu.utils.functional import LRUCache, dictfilter, is_list, lazy, maybe_evaluate, maybe_list, memoize
 from vine import promise
 
+from celery.utils.log import get_logger
+
+logger = get_logger(__name__)
+
 __all__ = (
     'LRUCache', 'is_list', 'maybe_list', 'memoize', 'mlazy', 'noop',
     'first', 'firstmethod', 'chunks', 'padlist', 'mattrgetter', 'uniq',
     'regen', 'dictfilter', 'lazy', 'maybe_evaluate', 'head_from_fun',
     'maybe', 'fun_accepts_kwargs',
 )
 
@@ -303,15 +307,15 @@
         '*' if (kwonlyargs or kwonlyargs_optional) and not varargs else None,
         ', '.join(kwonlyargs) if kwonlyargs else None,
         ', '.join(f'{k}="{v}"' for k, v in kwonlyargs_optional),
         f'**{varkw}' if varkw else None,
     ]))
 
 
-def head_from_fun(fun, bound=False, debug=False):
+def head_from_fun(fun: Callable[..., Any], bound: bool = False) -> str:
     """Generate signature function from actual function."""
     # we could use inspect.Signature here, but that implementation
     # is very slow since it implements the argument checking
     # in pure-Python.  Instead we use exec to create a new function
     # with an empty body, meaning it has the same performance as
     # as just calling a function.
     is_function = inspect.isfunction(fun)
@@ -324,16 +328,15 @@
     else:
         name = fun.__name__
     definition = FUNHEAD_TEMPLATE.format(
         fun_name=name,
         fun_args=_argsfromspec(inspect.getfullargspec(fun)),
         fun_value=1,
     )
-    if debug:  # pragma: no cover
-        print(definition, file=sys.stderr)
+    logger.debug(definition)
     namespace = {'__name__': fun.__module__}
     # pylint: disable=exec-used
     # Tasks are rarely, if ever, created at runtime - exec here is fine.
     exec(definition, namespace)
     result = namespace[name]
     result._source = definition
     if bound:
```

### Comparing `celery-5.3.0b1/celery/utils/graph.py` & `celery-5.3.0b2/celery/utils/graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/imports.py` & `celery-5.3.0b2/celery/utils/imports.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,22 @@
             module_name = '__main__'
     if module_name == '__main__' and app.main:
         return '.'.join([app.main, name])
     return '.'.join(p for p in (module_name, name) if p)
 
 
 def load_extension_class_names(namespace):
-    for ep in entry_points().get(namespace, []):
+    if sys.version_info >= (3, 10):
+        _entry_points = entry_points(group=namespace)
+    else:
+        try:
+            _entry_points = entry_points().get(namespace, [])
+        except AttributeError:
+            _entry_points = entry_points().select(group=namespace)
+    for ep in _entry_points:
         yield ep.name, ep.value
 
 
 def load_extension_classes(namespace):
     for name, class_name in load_extension_class_names(namespace):
         try:
             cls = symbol_by_name(class_name)
```

### Comparing `celery-5.3.0b1/celery/utils/iso8601.py` & `celery-5.3.0b2/celery/utils/iso8601.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/log.py` & `celery-5.3.0b2/celery/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import numbers
 import os
 import sys
 import threading
 import traceback
 from contextlib import contextmanager
-from typing import AnyStr, Sequence
+from typing import AnyStr, Sequence  # noqa
 
 from kombu.log import LOG_LEVELS
 from kombu.log import get_logger as _get_logger
 from kombu.utils.encoding import safe_str
 
 from .term import colored
 
@@ -260,35 +260,35 @@
         return False
 
 
 def get_multiprocessing_logger():
     """Return the multiprocessing logger."""
     try:
         from billiard import util
-    except ImportError:  # pragma: no cover
+    except ImportError:
         pass
     else:
         return util.get_logger()
 
 
 def reset_multiprocessing_logger():
     """Reset multiprocessing logging setup."""
     try:
         from billiard import util
-    except ImportError:  # pragma: no cover
+    except ImportError:
         pass
     else:
         if hasattr(util, '_logger'):  # pragma: no cover
             util._logger = None
 
 
 def current_process():
     try:
         from billiard import process
-    except ImportError:  # pragma: no cover
+    except ImportError:
         pass
     else:
         return process.current_process()
 
 
 def current_process_index(base=1):
     index = getattr(current_process(), 'index', None)
```

### Comparing `celery-5.3.0b1/celery/utils/nodenames.py` & `celery-5.3.0b2/celery/utils/nodenames.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/objects.py` & `celery-5.3.0b2/celery/utils/objects.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/saferepr.py` & `celery-5.3.0b2/celery/utils/saferepr.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 import traceback
 from collections import deque, namedtuple
 from decimal import Decimal
 from itertools import chain
 from numbers import Number
 from pprint import _recursion
-from typing import Any, AnyStr, Callable, Dict, Iterator, List, Sequence, Set, Tuple
+from typing import Any, AnyStr, Callable, Dict, Iterator, List, Sequence, Set, Tuple  # noqa
 
 from .text import truncate
 
 __all__ = ('saferepr', 'reprstream')
 
 #: Node representing literal text.
 #:   - .value: is the literal text value
```

### Comparing `celery-5.3.0b1/celery/utils/serialization.py` & `celery-5.3.0b2/celery/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/static/celery_128.png` & `celery-5.3.0b2/celery/utils/static/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/sysinfo.py` & `celery-5.3.0b2/celery/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/utils/term.py` & `celery-5.3.0b2/celery/utils/term.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import base64
 import codecs
 import os
 import platform
 import sys
 from functools import reduce
 
-from celery.platforms import isatty
-
 __all__ = ('colored',)
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
 OP_SEQ = '\033[%dm'
 RESET_SEQ = '\033[0m'
 COLOR_SEQ = '\033[1;%dm'
 
@@ -160,15 +158,15 @@
         return self.node(s or [''], RESET_SEQ)
 
     def __add__(self, other):
         return str(self) + str(other)
 
 
 def supports_images():
-    return isatty(sys.stdin) and ITERM_PROFILE
+    return sys.stdin.isatty() and ITERM_PROFILE
 
 
 def _read_as_base64(path):
     with codecs.open(path, mode='rb') as fh:
         encoded = base64.b64encode(fh.read())
         return encoded if type(encoded) == 'str' else encoded.decode('ascii')
```

### Comparing `celery-5.3.0b1/celery/utils/text.py` & `celery-5.3.0b2/celery/utils/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Text formatting utilities."""
 import io
 import re
 from collections.abc import Callable
 from functools import partial
 from pprint import pformat
 from textwrap import fill
-from typing import Any, List, Mapping, Pattern
+from typing import Any, List, Mapping, Pattern  # noqa
 
 __all__ = (
     'abbr', 'abbrtask', 'dedent', 'dedent_initial',
     'ensure_newlines', 'ensure_sep',
     'fill_paragraphs', 'indent', 'join',
     'pluralize', 'pretty', 'str_to_list', 'simple_format', 'truncate',
 )
```

### Comparing `celery-5.3.0b1/celery/utils/threads.py` & `celery-5.3.0b2/celery/utils/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from contextlib import contextmanager
 from threading import TIMEOUT_MAX as THREAD_TIMEOUT_MAX
 
 from celery.local import Proxy
 
 try:
     from greenlet import getcurrent as get_ident
-except ImportError:  # pragma: no cover
+except ImportError:
     try:
         from _thread import get_ident
     except ImportError:
         try:
             from thread import get_ident
-        except ImportError:  # pragma: no cover
+        except ImportError:
             try:
                 from _dummy_thread import get_ident
             except ImportError:
                 from dummy_thread import get_ident
 
 
 __all__ = (
```

### Comparing `celery-5.3.0b1/celery/utils/time.py` & `celery-5.3.0b2/celery/utils/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,18 +301,19 @@
 
 
 def to_utc(dt):
     """Convert naive :class:`~datetime.datetime` to UTC."""
     return make_aware(dt, timezone.utc)
 
 
-def maybe_make_aware(dt, tz=None):
+def maybe_make_aware(dt, tz=None, naive_as_utc=True):
     """Convert dt to aware datetime, do nothing if dt is already aware."""
     if is_naive(dt):
-        dt = to_utc(dt)
+        if naive_as_utc:
+            dt = to_utc(dt)
         return localize(
             dt, timezone.utc if tz is None else timezone.tz_or_local(tz),
         )
     return dt
 
 
 class ffwd:
```

### Comparing `celery-5.3.0b1/celery/utils/timer2.py` & `celery-5.3.0b2/celery/utils/timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/autoscale.py` & `celery-5.3.0b2/celery/worker/autoscale.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/components.py` & `celery-5.3.0b2/celery/worker/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def _patch_thread_primitives(self, w):
         # make clock use dummy lock
         w.app.clock.mutex = DummyLock()
         # multiprocessing's ApplyResult uses this lock.
         try:
             from billiard import pool
-        except ImportError:  # pragma: no cover
+        except ImportError:
             pass
         else:
             pool.Lock = DummyLock
 
 
 class Pool(bootsteps.StartStopStep):
     """Bootstep managing the worker pool.
```

### Comparing `celery-5.3.0b1/celery/worker/consumer/agent.py` & `celery-5.3.0b2/celery/worker/consumer/agent.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/connection.py` & `celery-5.3.0b2/celery/worker/consumer/connection.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/consumer.py` & `celery-5.3.0b2/celery/worker/consumer/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from celery.utils.functional import noop
 from celery.utils.log import get_logger
 from celery.utils.nodenames import gethostname
 from celery.utils.objects import Bunch
 from celery.utils.text import truncate
 from celery.utils.time import humanize_seconds, rate
 from celery.worker import loops
-from celery.worker.state import active_requests, maybe_shutdown, reserved_requests, task_reserved
+from celery.worker.state import active_requests, maybe_shutdown, requests, reserved_requests, task_reserved
 
 __all__ = ('Consumer', 'Evloop', 'dump_body')
 
 CLOSE = bootsteps.CLOSE
 TERMINATE = bootsteps.TERMINATE
 STOP_CONDITIONS = {CLOSE, TERMINATE}
 logger = get_logger(__name__)
@@ -77,15 +77,15 @@
 Please see
 https://docs.celeryq.dev/en/latest/internals/protocol.html
 for more information.
 
 The full contents of the message body was:
 %s
 
-Thw full contents of the message headers:
+The full contents of the message headers:
 %s
 
 The delivery info for this task is:
 %s
 """
 
 #: Error message for when an invalid task message is received.
@@ -117,18 +117,18 @@
 Task %s cannot be acknowledged after a connection loss since late acknowledgement is enabled for it.
 Terminating it instead.
 """
 
 CANCEL_TASKS_BY_DEFAULT = """
 In Celery 5.1 we introduced an optional breaking change which
 on connection loss cancels all currently executed tasks with late acknowledgement enabled.
-These tasks cannot be acknowledged as the connection is gone, and the tasks are automatically redelivered back to the queue.
-You can enable this behavior using the worker_cancel_long_running_tasks_on_connection_loss setting.
-In Celery 5.1 it is set to False by default. The setting will be set to True by default in Celery 6.0.
-"""  # noqa: E501
+These tasks cannot be acknowledged as the connection is gone, and the tasks are automatically redelivered
+back to the queue. You can enable this behavior using the worker_cancel_long_running_tasks_on_connection_loss
+setting. In Celery 5.1 it is set to False by default. The setting will be set to True by default in Celery 6.0.
+"""
 
 
 def dump_body(m, body):
     """Format message body for debugging purposes."""
     # v2 protocol does not deserialize body
     body = m.body if body is None else body
     return '{} ({}b)'.format(truncate(safe_repr(body), 1024),
@@ -324,17 +324,21 @@
             if self.restart_count:
                 try:
                     self._restart_state.step()
                 except RestartFreqExceeded as exc:
                     crit('Frequent restarts detected: %r', exc, exc_info=1)
                     sleep(1)
             self.restart_count += 1
+            if self.app.conf.broker_channel_error_retry:
+                recoverable_errors = (self.connection_errors + self.channel_errors)
+            else:
+                recoverable_errors = self.connection_errors
             try:
                 blueprint.start(self)
-            except self.connection_errors as exc:
+            except recoverable_errors as exc:
                 # If we're not retrying connections, we need to properly shutdown or terminate
                 # the Celery main process instead of abruptly aborting the process without any cleanup.
                 is_connection_loss_on_startup = self.restart_count == 0
                 connection_retry_type = self._get_connection_retry_type(is_connection_loss_on_startup)
                 connection_retry = self.app.conf[connection_retry_type]
                 if not connection_retry:
                     crit(
@@ -440,14 +444,17 @@
         if self.controller and self.controller.semaphore:
             self.controller.semaphore.clear()
         if self.timer:
             self.timer.clear()
         for bucket in self.task_buckets.values():
             if bucket:
                 bucket.clear_pending()
+        for request_id in reserved_requests:
+            if request_id in requests:
+                del requests[request_id]
         reserved_requests.clear()
         if self.pool and self.pool.flush:
             self.pool.flush()
 
     def connect(self):
         """Establish the broker connection used for consuming tasks.
```

### Comparing `celery-5.3.0b1/celery/worker/consumer/control.py` & `celery-5.3.0b2/celery/worker/consumer/control.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/events.py` & `celery-5.3.0b2/celery/worker/consumer/events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/gossip.py` & `celery-5.3.0b2/celery/worker/consumer/gossip.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/heart.py` & `celery-5.3.0b2/celery/worker/consumer/heart.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/mingle.py` & `celery-5.3.0b2/celery/worker/consumer/mingle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/consumer/tasks.py` & `celery-5.3.0b2/celery/worker/consumer/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/control.py` & `celery-5.3.0b2/celery/worker/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Worker remote control command implementations."""
 import io
 import tempfile
+import warnings
 from collections import UserDict, namedtuple
 
 from billiard.common import TERM_SIGNAME
 from kombu.utils.encoding import safe_repr
 
-from celery.exceptions import WorkerShutdown
+from celery.exceptions import CeleryWarning, WorkerShutdown
 from celery.platforms import signals as _signals
 from celery.utils.functional import maybe_list
 from celery.utils.log import get_logger
 from celery.utils.serialization import jsonify, strtobool
 from celery.utils.time import rate
 
 from . import state as worker_state
@@ -142,14 +143,68 @@
         signal (str): Name of signal to use for terminate (e.g., ``KILL``).
     """
     # pylint: disable=redefined-outer-name
     # XXX Note that this redefines `terminate`:
     #     Outside of this scope that is a function.
     # supports list argument since 3.1
     task_ids, task_id = set(maybe_list(task_id) or []), None
+    task_ids = _revoke(state, task_ids, terminate, signal, **kwargs)
+    return ok(f'tasks {task_ids} flagged as revoked')
+
+
+@control_command(
+    variadic='headers',
+    signature='[key1=value1 [key2=value2 [... [keyN=valueN]]]]',
+)
+def revoke_by_stamped_headers(state, headers, terminate=False, signal=None, **kwargs):
+    """Revoke task by header (or list of headers).
+
+    Keyword Arguments:
+        terminate (bool): Also terminate the process if the task is active.
+        signal (str): Name of signal to use for terminate (e.g., ``KILL``).
+    """
+    # pylint: disable=redefined-outer-name
+    # XXX Note that this redefines `terminate`:
+    #     Outside of this scope that is a function.
+    # supports list argument since 3.1
+    if isinstance(headers, list):
+        headers = {h.split('=')[0]: h.split('=')[1] for h in headers}, None
+
+    worker_state.revoked_headers.update(headers)
+
+    if not terminate:
+        return ok(f'headers {headers} flagged as revoked')
+
+    task_ids = set()
+    requests = list(worker_state.active_requests)
+
+    # Terminate all running tasks of matching headers
+    if requests:
+        warnings.warn(
+            "Terminating tasks by headers does not scale well when worker concurrency is high",
+            CeleryWarning
+        )
+
+        for req in requests:
+            if req.stamped_headers:
+                for stamped_header_key, expected_header_value in headers.items():
+                    if stamped_header_key in req.stamped_headers and \
+                            stamped_header_key in req._message.headers['stamps']:
+                        actual_header = req._message.headers['stamps'][stamped_header_key]
+                        if expected_header_value in actual_header:
+                            task_ids.add(req.task_id)
+                            continue
+
+    task_ids = _revoke(state, task_ids, terminate, signal, **kwargs)
+    if isinstance(task_ids, dict):
+        return task_ids
+    return ok(list(task_ids))
+
+
+def _revoke(state, task_ids, terminate=False, signal=None, **kwargs):
     size = len(task_ids)
     terminated = set()
 
     worker_state.revoked.update(task_ids)
     if terminate:
         signum = _signals.signum(signal or TERM_SIGNAME)
         for request in _find_requests_by_id(task_ids):
@@ -162,15 +217,15 @@
 
         if not terminated:
             return ok('terminate: tasks unknown')
         return ok('terminate: {}'.format(', '.join(terminated)))
 
     idstr = ', '.join(task_ids)
     logger.info('Tasks flagged as revoked: %s', idstr)
-    return ok(f'tasks {idstr} flagged as revoked')
+    return task_ids
 
 
 @control_command(
     variadic='task_id',
     args=[('signal', str)],
     signature='<signal> [id1 [id2 [... [idN]]]]'
 )
```

### Comparing `celery-5.3.0b1/celery/worker/heartbeat.py` & `celery-5.3.0b2/celery/worker/heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/loops.py` & `celery-5.3.0b2/celery/worker/loops.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/pidbox.py` & `celery-5.3.0b2/celery/worker/pidbox.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/request.py` & `celery-5.3.0b2/celery/worker/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 import logging
 import sys
 from datetime import datetime
 from time import monotonic, time
 from weakref import ref
 
 from billiard.common import TERM_SIGNAME
+from billiard.einfo import ExceptionWithTraceback
 from kombu.utils.encoding import safe_repr, safe_str
 from kombu.utils.objects import cached_property
 
 from celery import current_app, signals
 from celery.app.task import Context
 from celery.app.trace import fast_trace_task, trace_task, trace_task_ret
+from celery.concurrency.base import BasePool
 from celery.exceptions import (Ignore, InvalidTaskError, Reject, Retry, TaskRevokedError, Terminated,
                                TimeLimitExceeded, WorkerLostError)
 from celery.platforms import signals as _signals
-from celery.utils.functional import maybe, noop
+from celery.utils.functional import maybe, maybe_list, noop
 from celery.utils.log import get_logger
 from celery.utils.nodenames import gethostname
 from celery.utils.serialization import get_pickled_exception
 from celery.utils.time import maybe_iso8601, maybe_make_aware, timezone
 
 from . import state
 
@@ -55,14 +57,15 @@
 tz_or_local = timezone.tz_or_local
 send_revoked = signals.task_revoked.send
 send_retry = signals.task_retry.send
 
 task_accepted = state.task_accepted
 task_ready = state.task_ready
 revoked_tasks = state.revoked
+revoked_headers = state.revoked_headers
 
 
 class Request:
     """A request for task execution."""
 
     acknowledged = False
     time_start = None
@@ -320,22 +323,22 @@
 
     @property
     def stamped_headers(self) -> list:
         return self._request_dict.get('stamped_headers', [])
 
     @property
     def stamps(self) -> dict:
-        return {header: self._request_dict[header] for header in self.stamped_headers}
+        return {header: self._request_dict['stamps'][header] for header in self.stamped_headers}
 
     @property
     def correlation_id(self):
         # used similarly to reply_to
         return self._request_dict['correlation_id']
 
-    def execute_using_pool(self, pool, **kwargs):
+    def execute_using_pool(self, pool: BasePool, **kwargs):
         """Used by the worker to send this task to the pool.
 
         Arguments:
             pool (~celery.concurrency.base.TaskPool): The execution pool
                 used to execute this request.
 
         Raises:
@@ -396,17 +399,17 @@
             self.reject(requeue=False)
         else:
             self.acknowledge()
         return retval
 
     def maybe_expire(self):
         """If expired, mark the task as revoked."""
-        if self._expires:
-            now = datetime.now(self._expires.tzinfo)
-            if now > self._expires:
+        if self.expires:
+            now = datetime.now(self.expires.tzinfo)
+            if now > self.expires:
                 revoked_tasks.add(self.id)
                 return True
 
     def terminate(self, pool, signal=None):
         signal = _signals.signum(signal or TERM_SIGNAME)
         if self.time_start:
             pool.terminate_job(self.worker_pid, signal)
@@ -456,18 +459,41 @@
                      terminated=terminated, signum=signum, expired=expired)
 
     def revoked(self):
         """If revoked, skip task and mark state."""
         expired = False
         if self._already_revoked:
             return True
-        if self._expires:
+        if self.expires:
             expired = self.maybe_expire()
-        if self.id in revoked_tasks:
-            info('Discarding revoked task: %s[%s]', self.name, self.id)
+        revoked_by_id = self.id in revoked_tasks
+        revoked_by_header, revoking_header = False, None
+
+        if not revoked_by_id and self.stamped_headers:
+            for header in self.stamped_headers:
+                if header in revoked_headers:
+                    revoked_header = revoked_headers[header]
+                    stamped_header = self._message.headers['stamps'][header]
+
+                    if isinstance(stamped_header, (list, tuple)):
+                        for stamped_value in stamped_header:
+                            if stamped_value in maybe_list(revoked_header):
+                                revoked_by_header = True
+                                revoking_header = {header: stamped_value}
+                                break
+                    else:
+                        revoked_by_header = stamped_header in revoked_headers[header]
+                        revoking_header = {header: stamped_header}
+                    break
+
+        if any((expired, revoked_by_id, revoked_by_header)):
+            log_msg = 'Discarding revoked task: %s[%s]'
+            if revoked_by_header:
+                log_msg += ' (revoked by header: %s)' % revoking_header
+            info(log_msg, self.name, self.id)
             self._announce_revoked(
                 'expired' if expired else 'revoked', False, None, expired,
             )
             return True
         return False
 
     def send_event(self, type, **fields):
@@ -507,16 +533,19 @@
             if self.task.acks_late and self.task.acks_on_failure_or_timeout:
                 self.acknowledge()
 
     def on_success(self, failed__retval__runtime, **kwargs):
         """Handler called if the task was successfully processed."""
         failed, retval, runtime = failed__retval__runtime
         if failed:
-            if isinstance(retval.exception, (SystemExit, KeyboardInterrupt)):
-                raise retval.exception
+            exc = retval.exception
+            if isinstance(exc, ExceptionWithTraceback):
+                exc = exc.exc
+            if isinstance(exc, (SystemExit, KeyboardInterrupt)):
+                raise exc
             return self.on_failure(retval, return_ok=True)
         task_ready(self, successful=True)
 
         if self.task.acks_late:
             self.acknowledge()
 
         self.send_event('task-succeeded', result=retval, runtime=runtime)
@@ -531,14 +560,17 @@
                         traceback=safe_str(exc_info.traceback))
 
     def on_failure(self, exc_info, send_failed_event=True, return_ok=False):
         """Handler called if the task raised an exception."""
         task_ready(self)
         exc = exc_info.exception
 
+        if isinstance(exc, ExceptionWithTraceback):
+            exc = exc.exc
+
         is_terminated = isinstance(exc, Terminated)
         if is_terminated:
             # If the task was terminated and the task was not cancelled due
             # to a connection loss, it is revoked.
 
             # We always cancel the tasks inside the master process.
             # If the request was cancelled, it was not revoked and there's
@@ -707,15 +739,15 @@
     if trace is None:
         trace = fast_trace_task if app.use_fast_trace_task else trace_task_ret
 
     class Request(base):
 
         def execute_using_pool(self, pool, **kwargs):
             task_id = self.task_id
-            if (self.expires or task_id in revoked_tasks) and self.revoked():
+            if self.revoked():
                 raise TaskRevokedError(task_id)
 
             time_limit, soft_time_limit = self.time_limits
             result = apply_async(
                 trace,
                 args=(self.type, task_id, self.request_dict, self.body,
                       self.content_type, self.content_encoding),
@@ -731,17 +763,19 @@
             # pylint: disable=attribute-defined-outside-init
             self._apply_result = maybe(ref, result)
             return result
 
         def on_success(self, failed__retval__runtime, **kwargs):
             failed, retval, runtime = failed__retval__runtime
             if failed:
-                if isinstance(retval.exception, (
-                        SystemExit, KeyboardInterrupt)):
-                    raise retval.exception
+                exc = retval.exception
+                if isinstance(exc, ExceptionWithTraceback):
+                    exc = exc.exc
+                if isinstance(exc, (SystemExit, KeyboardInterrupt)):
+                    raise exc
                 return self.on_failure(retval, return_ok=True)
             task_ready(self)
 
             if acks_late:
                 self.acknowledge()
 
             if events:
```

### Comparing `celery-5.3.0b1/celery/worker/state.py` & `celery-5.3.0b2/celery/worker/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,26 +63,30 @@
 
 #: count of all tasks accepted by the worker
 all_total_count = [0]
 
 #: the list of currently revoked tasks.  Persistent if ``statedb`` set.
 revoked = LimitedSet(maxlen=REVOKES_MAX, expires=REVOKE_EXPIRES)
 
+#: Mapping of stamped headers flagged for revoking.
+revoked_headers = {}
+
 should_stop = None
 should_terminate = None
 
 
 def reset_state():
     requests.clear()
     reserved_requests.clear()
     active_requests.clear()
     successful_requests.clear()
     total_count.clear()
     all_total_count[:] = [0]
     revoked.clear()
+    revoked_headers.clear()
 
 
 def maybe_shutdown():
     """Shutdown if flags have been set."""
     if should_terminate is not None and should_terminate is not False:
         raise WorkerTerminate(should_terminate)
     elif should_stop is not None and should_stop is not False:
@@ -95,19 +99,21 @@
     """Update global state when a task has been reserved."""
     add_request(request.id, request)
     add_reserved_request(request)
 
 
 def task_accepted(request,
                   _all_total_count=None,
+                  add_request=requests.__setitem__,
                   add_active_request=active_requests.add,
                   add_to_total_count=total_count.update):
     """Update global state when a task has been accepted."""
     if not _all_total_count:
         _all_total_count = all_total_count
+    add_request(request.id, request)
     add_active_request(request)
     add_to_total_count({request.name: 1})
     all_total_count[0] += 1
 
 
 def task_ready(request,
                successful=False,
```

### Comparing `celery-5.3.0b1/celery/worker/strategy.py` & `celery-5.3.0b2/celery/worker/strategy.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/celery/worker/worker.py` & `celery-5.3.0b2/celery/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from celery.utils.text import str_to_list
 from celery.utils.threads import default_socket_timeout
 
 from . import state
 
 try:
     import resource
-except ImportError:  # pragma: no cover
+except ImportError:
     resource = None
 
 
 __all__ = ('WorkController',)
 
 #: Default socket timeout at shutdown.
 SHUTDOWN_SOCKET_TIMEOUT = 5.0
```

### Comparing `celery-5.3.0b1/celery.egg-info/PKG-INFO` & `celery-5.3.0b2/celery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: celery
-Version: 5.3.0b1
+Version: 5.3.0b2
 Summary: Distributed Task Queue.
 Home-page: https://docs.celeryq.dev/
 Author: Ask Solem
 Author-email: auvipy@gmail.com
-License: BSD
+License: BSD-3-Clause
 Project-URL: Documentation, https://docs.celeryq.dev/en/stable/
 Project-URL: Changelog, https://docs.celeryq.dev/en/stable/changelog.html
 Project-URL: Code, https://github.com/celery/celery
 Project-URL: Tracker, https://github.com/celery/celery/issues
 Project-URL: Funding, https://opencollective.com/celery
 Keywords: task job queue distributed messaging actor
 Platform: any
@@ -25,52 +25,52 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
-Provides-Extra: auth
-Provides-Extra: pyro
-Provides-Extra: solar
-Provides-Extra: cosmosdbsql
-Provides-Extra: sqs
-Provides-Extra: tblib
-Provides-Extra: brotli
-Provides-Extra: yaml
-Provides-Extra: pymemcache
-Provides-Extra: consul
-Provides-Extra: slmq
+Provides-Extra: eventlet
+Provides-Extra: memcache
 Provides-Extra: gevent
-Provides-Extra: s3
-Provides-Extra: arangodb
-Provides-Extra: couchbase
-Provides-Extra: couchdb
-Provides-Extra: sqlalchemy
-Provides-Extra: pytest
 Provides-Extra: mongodb
 Provides-Extra: redis
-Provides-Extra: elasticsearch
-Provides-Extra: zstd
-Provides-Extra: msgpack
+Provides-Extra: sqs
+Provides-Extra: auth
 Provides-Extra: cassandra
-Provides-Extra: memcache
-Provides-Extra: azureblockblob
+Provides-Extra: brotli
+Provides-Extra: s3
+Provides-Extra: couchbase
+Provides-Extra: pyro
+Provides-Extra: slmq
+Provides-Extra: cosmosdbsql
+Provides-Extra: arangodb
 Provides-Extra: zookeeper
+Provides-Extra: pytest
+Provides-Extra: solar
 Provides-Extra: librabbitmq
-Provides-Extra: eventlet
+Provides-Extra: azureblockblob
+Provides-Extra: pymemcache
+Provides-Extra: yaml
 Provides-Extra: django
+Provides-Extra: elasticsearch
 Provides-Extra: dynamodb
+Provides-Extra: zstd
+Provides-Extra: consul
+Provides-Extra: sqlalchemy
+Provides-Extra: couchdb
+Provides-Extra: tblib
+Provides-Extra: msgpack
 License-File: LICENSE
 
 .. image:: https://docs.celeryq.dev/en/latest/_images/celery-banner-small.png
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |ocbackerbadge| |ocsponsorbadge|
 
-:Version: 5.3.0b1 (dawn-chorus)
+:Version: 5.3.0b2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 Donations
@@ -128,19 +128,19 @@
 
 
 This is the version of celery which will support Python 3.7 or newer.
 
 If you're running an older version of Python, you need to be running
 an older version of Celery:
 
+- Python 3.6: Celery 5.1 or earlier.
+- Python 2.7: Celery 4.x series.
 - Python 2.6: Celery series 3.1 or earlier.
 - Python 2.5: Celery series 3.0 or earlier.
 - Python 2.4: Celery series 2.2 or earlier.
-- Python 2.7: Celery 4.x series.
-- Python 3.6: Celery 5.1 or earlier.
 
 Celery is a project with minimal funding,
 so we don't support Microsoft Windows.
 Please don't open any issues related to that platform.
 
 *Celery* is usually used with a message broker to send and receive messages.
 The RabbitMQ, Redis transports are feature complete,
@@ -451,19 +451,19 @@
 
 You can install the latest snapshot of these using the following
 pip commands:
 
 ::
 
 
-    $ pip install https://github.com/celery/celery/zipball/master#egg=celery
-    $ pip install https://github.com/celery/billiard/zipball/master#egg=billiard
-    $ pip install https://github.com/celery/py-amqp/zipball/master#egg=amqp
-    $ pip install https://github.com/celery/kombu/zipball/master#egg=kombu
-    $ pip install https://github.com/celery/vine/zipball/master#egg=vine
+    $ pip install https://github.com/celery/celery/zipball/main#egg=celery
+    $ pip install https://github.com/celery/billiard/zipball/main#egg=billiard
+    $ pip install https://github.com/celery/py-amqp/zipball/main#egg=amqp
+    $ pip install https://github.com/celery/kombu/zipball/main#egg=kombu
+    $ pip install https://github.com/celery/vine/zipball/main#egg=vine
 
 With git
 ~~~~~~~~
 
 Please see the Contributing section.
 
 .. _getting-help:
@@ -521,15 +521,15 @@
 of `celery`. If you don't like GitHub (for some reason) you're welcome
 to send regular patches.
 
 Be sure to also read the `Contributing to Celery`_ section in the
 documentation.
 
 .. _`Contributing to Celery`:
-    https://docs.celeryq.dev/en/master/contributing.html
+    https://docs.celeryq.dev/en/main/contributing.html
 
 |oc-contributors|
 
 .. |oc-contributors| image:: https://opencollective.com/celery/contributors.svg?width=890&button=false
     :target: https://github.com/celery/celery/graphs/contributors
 
 Backers
@@ -567,16 +567,16 @@
 
 .. # vim: syntax=rst expandtab tabstop=4 shiftwidth=4 shiftround
 
 .. |build-status| image:: https://github.com/celery/celery/actions/workflows/python-package.yml/badge.svg
     :alt: Build status
     :target: https://github.com/celery/celery/actions/workflows/python-package.yml
 
-.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/celery?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/celery?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/celery.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
     :alt: Celery can be installed via wheel
```

### Comparing `celery-5.3.0b1/celery.egg-info/SOURCES.txt` & `celery-5.3.0b2/celery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -452,14 +452,20 @@
 examples/next-steps/proj/celery.py
 examples/next-steps/proj/tasks.py
 examples/periodic-tasks/myapp.py
 examples/resultgraph/tasks.py
 examples/security/mysecureapp.py
 examples/security/ssl/worker.key
 examples/security/ssl/worker.pem
+examples/stamping/config.py
+examples/stamping/examples.py
+examples/stamping/myapp.py
+examples/stamping/revoke_example.py
+examples/stamping/tasks.py
+examples/stamping/visitors.py
 examples/tutorial/tasks.py
 extra/bash-completion/celery.bash
 extra/generic-init.d/celerybeat
 extra/generic-init.d/celeryd
 extra/macOS/org.celeryq.beat.plist
 extra/macOS/org.celeryq.worker.plist
 extra/supervisord/celery.sh
@@ -614,14 +620,15 @@
 t/unit/security/test_security.py
 t/unit/security/test_serialization.py
 t/unit/tasks/__init__.py
 t/unit/tasks/test_canvas.py
 t/unit/tasks/test_chord.py
 t/unit/tasks/test_context.py
 t/unit/tasks/test_result.py
+t/unit/tasks/test_stamping.py
 t/unit/tasks/test_states.py
 t/unit/tasks/test_tasks.py
 t/unit/tasks/test_trace.py
 t/unit/tasks/unit_tasks.py
 t/unit/utils/__init__.py
 t/unit/utils/test_collections.py
 t/unit/utils/test_debug.py
```

### Comparing `celery-5.3.0b1/celery.egg-info/requires.txt` & `celery-5.3.0b2/celery.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 pytz>=2021.3
-billiard<5.0,>=3.6.4.0
-kombu<6.0,>=5.3.0b1
+billiard<5.0,>=4.1.0
+kombu<6.0,>=5.3.0b2
 vine<6.0,>=5.0.0
 click<9.0,>=8.1.2
 click-didyoumean>=0.3.0
 click-repl>=0.2.0
 click-plugins>=1.1.1
 
 [:python_version < "3.8"]
-importlib-metadata>=1.4.0
+importlib-metadata>=3.6
 
 [arangodb]
 pyArango>=2.0.1
 
 [auth]
-cryptography~=37.0.1
+cryptography==39.0.0
 
 [azureblockblob]
 azure-storage-blob>=12.11.0
 
 [brotli]
 
 [brotli:platform_python_implementation == "CPython"]
@@ -63,15 +63,15 @@
 
 [librabbitmq]
 librabbitmq>=1.5.0
 
 [memcache]
 
 [memcache:platform_system != "Windows"]
-pylibmc==1.6.1
+pylibmc==1.6.3
 
 [mongodb]
 pymongo[srv]>=4.0.2
 
 [msgpack]
 msgpack==1.0.4
 
@@ -81,29 +81,29 @@
 [pyro]
 pyro4==4.82
 
 [pytest]
 pytest-celery==0.0.0
 
 [redis]
-redis>=4.2.2
+redis<4.4.0,>=4.2.2
 
 [s3]
 boto3>=1.9.125
 
 [slmq]
 softlayer_messaging>=1.0.3
 
 [solar]
 
 [solar:platform_python_implementation != "PyPy"]
 ephem~=4.1.3
 
 [sqlalchemy]
-sqlalchemy~=1.4.34
+sqlalchemy==1.4.45
 
 [sqs]
 kombu[sqs]~=5.2.4
 
 [tblib]
 
 [tblib:python_version < "3.8.0"]
@@ -115,8 +115,8 @@
 [yaml]
 PyYAML>=3.10
 
 [zookeeper]
 kazoo>=1.3.1
 
 [zstd]
-zstandard==0.18.0
+zstandard==0.19.0
```

### Comparing `celery-5.3.0b1/docs/AUTHORS.txt` & `celery-5.3.0b2/docs/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/Makefile` & `celery-5.3.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/_ext/celerydocs.py` & `celery-5.3.0b2/docs/_ext/celerydocs.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/community.rst` & `celery-5.3.0b2/docs/community.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/conf.py` & `celery-5.3.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/copyright.rst` & `celery-5.3.0b2/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/django/first-steps-with-django.rst` & `celery-5.3.0b2/docs/django/first-steps-with-django.rst`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 .. literalinclude:: ../../examples/django/demoapp/tasks.py
 
 
 .. seealso::
 
     You can find the full source code for the Django example project at:
-    https://github.com/celery/celery/tree/master/examples/django/
+    https://github.com/celery/celery/tree/main/examples/django/
 
 Extensions
 ==========
 
 .. _django-celery-results:
 
 ``django-celery-results`` - Using the Django ORM/Cache as a result backend
```

### Comparing `celery-5.3.0b1/docs/faq.rst` & `celery-5.3.0b2/docs/faq.rst`

 * *Files 2% similar despite different names*

```diff
@@ -874,17 +874,18 @@
 
 .. _faq-schedule-at-specific-time:
 
 Can I schedule tasks to execute at a specific time?
 ---------------------------------------------------
 
 **Answer**: Yes. You can use the `eta` argument of :meth:`Task.apply_async`.
+Note that using distant `eta` times is not recommended, and in such case
+:ref:`periodic tasks<guide-beat>` should be preferred.
 
-See also :ref:`guide-beat`.
-
+See :ref:`calling-eta` for more details.
 
 .. _faq-safe-worker-shutdown:
 
 Can I safely shut down the worker?
 ----------------------------------
 
 **Answer**: Yes, use the :sig:`TERM` signal.
```

### Comparing `celery-5.3.0b1/docs/getting-started/backends-and-brokers/index.rst` & `celery-5.3.0b2/docs/getting-started/backends-and-brokers/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/getting-started/backends-and-brokers/rabbitmq.rst` & `celery-5.3.0b2/docs/getting-started/backends-and-brokers/rabbitmq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 Installing the RabbitMQ Server
 ==============================
 
 See `Installing RabbitMQ`_ over at RabbitMQ's website. For macOS
 see `Installing RabbitMQ on macOS`_.
 
-.. _`Installing RabbitMQ`: http://www.rabbitmq.com/install.html
+.. _`Downloading and Installing RabbitMQ`: https://www.rabbitmq.com/download.html
 
 .. note::
 
     If you're getting `nodedown` errors after installing and using
     :command:`rabbitmqctl` then this blog post can help you identify
     the source of the problem:
 
@@ -65,17 +65,17 @@
 
     $ sudo rabbitmqctl set_permissions -p myvhost myuser ".*" ".*" ".*"
 
 Substitute in appropriate values for ``myuser``, ``mypassword`` and ``myvhost`` above.
 
 See the RabbitMQ `Admin Guide`_ for more information about `access control`_.
 
-.. _`Admin Guide`: http://www.rabbitmq.com/admin-guide.html
+.. _`Admin Guide`: https://www.rabbitmq.com/admin-guide.html
 
-.. _`access control`: http://www.rabbitmq.com/admin-guide.html#access-control
+.. _`access control`: https://www.rabbitmq.com/access-control.html
 
 .. _rabbitmq-macOS-installation:
 
 Installing RabbitMQ on macOS
 ----------------------------
 
 The easiest way to install RabbitMQ on macOS is using `Homebrew`_ the new and
```

### Comparing `celery-5.3.0b1/docs/getting-started/backends-and-brokers/redis.rst` & `celery-5.3.0b2/docs/getting-started/backends-and-brokers/redis.rst`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,32 @@
 
 If you are using Sentinel, you should specify the master_name using the :setting:`result_backend_transport_options` setting:
 
 .. code-block:: python
 
     app.conf.result_backend_transport_options = {'master_name': "mymaster"}
 
+.. _redis-result-backend-global-keyprefix:
+
+Global keyprefix
+^^^^^^^^^^^^^^^^
+
+The global key prefix will be prepended to all keys used for the result backend,
+which can be useful when a redis database is shared by different users.
+By default, no prefix is prepended.
+
+To configure the global keyprefix for the Redis result backend, use the ``global_keyprefix`` key under :setting:`result_backend_transport_options`:
+
+
+.. code-block:: python
+
+    app.conf.result_backend_transport_options = {
+        'global_keyprefix': 'my_prefix_'
+    }
+
 .. _redis-result-backend-timeout:
 
 Connection timeouts
 ^^^^^^^^^^^^^^^^^^^
 
 To configure the connection timeouts for the Redis result backend, use the ``retry_policy`` key under :setting:`result_backend_transport_options`:
 
@@ -129,22 +147,24 @@
 If a task isn't acknowledged within the :ref:`redis-visibility_timeout`
 the task will be redelivered to another worker and executed.
 
 This causes problems with ETA/countdown/retry tasks where the
 time to execute exceeds the visibility timeout; in fact if that
 happens it will be executed again, and again in a loop.
 
-So you have to increase the visibility timeout to match
-the time of the longest ETA you're planning to use.
-
-Note that Celery will redeliver messages at worker shutdown,
+To remediate that, you can increase the visibility timeout to match
+the time of the longest ETA you're planning to use. However, this is not
+recommended as it may have negative impact on the reliability.
+Celery will redeliver messages at worker shutdown,
 so having a long visibility timeout will only delay the redelivery
 of 'lost' tasks in the event of a power failure or forcefully terminated
 workers.
 
+Broker is not a database, so if you are in need of scheduling tasks for
+a more distant future, database-backed periodic task might be a better choice.
 Periodic tasks won't be affected by the visibility timeout,
 as this is a concept separate from ETA/countdown.
 
 You can increase this timeout by configuring a transport option
 with the same name:
 
 .. code-block:: python
```

### Comparing `celery-5.3.0b1/docs/getting-started/backends-and-brokers/sqs.rst` & `celery-5.3.0b2/docs/getting-started/backends-and-brokers/sqs.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/getting-started/first-steps-with-celery.rst` & `celery-5.3.0b2/docs/getting-started/first-steps-with-celery.rst`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 .. _celerytut-installation:
 
 Installing Celery
 =================
 
 Celery is on the Python Package Index (PyPI), so it can be installed
-with standard Python tools like ``pip`` or ``easy_install``:
+with standard Python tools like ``pip``:
 
 .. code-block:: console
 
     $ pip install celery
 
 Application
 ===========
```

### Comparing `celery-5.3.0b1/docs/getting-started/introduction.rst` & `celery-5.3.0b2/docs/getting-started/introduction.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/getting-started/next-steps.rst` & `celery-5.3.0b2/docs/getting-started/next-steps.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/glossary.rst` & `celery-5.3.0b2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-1.0.rst` & `celery-5.3.0b2/docs/history/changelog-1.0.rst`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 * AMQP backend: Added timeout support for `result.get()` /
   `result.wait()`.
 
 * New task option: `Task.acks_late` (default: :setting:`CELERY_ACKS_LATE`)
 
     Late ack means the task messages will be acknowledged **after** the task
-    has been executed, not *just before*, which is the default behavior.
+    has been executed, not *right before*, which is the default behavior.
 
     .. note::
 
         This means the tasks may be executed twice if the worker
         crashes in mid-execution. Not acceptable for most
         applications, but desirable for others.
```

### Comparing `celery-5.3.0b1/docs/history/changelog-2.0.rst` & `celery-5.3.0b2/docs/history/changelog-2.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-2.1.rst` & `celery-5.3.0b2/docs/history/changelog-2.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-2.2.rst` & `celery-5.3.0b2/docs/history/changelog-2.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-2.3.rst` & `celery-5.3.0b2/docs/history/changelog-2.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-2.4.rst` & `celery-5.3.0b2/docs/history/changelog-2.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-2.5.rst` & `celery-5.3.0b2/docs/history/changelog-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-3.0.rst` & `celery-5.3.0b2/docs/history/changelog-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-3.1.rst` & `celery-5.3.0b2/docs/history/changelog-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-4.0.rst` & `celery-5.3.0b2/docs/history/changelog-4.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-4.1.rst` & `celery-5.3.0b2/docs/history/changelog-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-4.2.rst` & `celery-5.3.0b2/docs/history/changelog-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-4.3.rst` & `celery-5.3.0b2/docs/history/changelog-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-4.4.rst` & `celery-5.3.0b2/docs/history/changelog-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-5.0.rst` & `celery-5.3.0b2/docs/history/changelog-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/changelog-5.1.rst` & `celery-5.3.0b2/docs/history/changelog-5.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/index.rst` & `celery-5.3.0b2/docs/history/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-2.5.rst` & `celery-5.3.0b2/docs/history/whatsnew-2.5.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-3.0.rst` & `celery-5.3.0b2/docs/history/whatsnew-3.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-3.1.rst` & `celery-5.3.0b2/docs/history/whatsnew-3.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-4.0.rst` & `celery-5.3.0b2/docs/history/whatsnew-4.0.rst`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     related to sending emails.
 
 - ``celery.contrib.batches`` has been removed.
 
     This was an experimental feature, so not covered by our deprecation
     timeline guarantee.
 
-    You can copy and pase the existing batches code for use within your projects:
+    You can copy and pass the existing batches code for use within your projects:
     https://github.com/celery/celery/blob/3.1/celery/contrib/batches.py
 
 Features removed for lack of funding
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 We announced with the 3.1 release that some transports were
 moved to experimental status, and that there'd be no official
@@ -1391,15 +1391,15 @@
 .. # XXX What changed?
 
 New Elasticsearch result backend introduced
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 See :ref:`conf-elasticsearch-result-backend` for more information.
 
-To depend on Celery with Elasticsearch as the result bakend use:
+To depend on Celery with Elasticsearch as the result backend use:
 
 .. code-block:: console
 
     $ pip install celery[elasticsearch]
 
 You can also combine multiple extension requirements,
 please see :ref:`bundles` for more information.
```

### Comparing `celery-5.3.0b1/docs/history/whatsnew-4.1.rst` & `celery-5.3.0b2/docs/history/whatsnew-4.1.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-4.2.rst` & `celery-5.3.0b2/docs/history/whatsnew-4.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-4.3.rst` & `celery-5.3.0b2/docs/history/whatsnew-4.3.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-4.4.rst` & `celery-5.3.0b2/docs/history/whatsnew-4.4.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-5.0.rst` & `celery-5.3.0b2/docs/history/whatsnew-5.0.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/history/whatsnew-5.1.rst` & `celery-5.3.0b2/docs/history/whatsnew-5.1.rst`

 * *Files 4% similar despite different names*

```diff
@@ -204,14 +204,34 @@
 ---------------
 
 Kombu
 ~~~~~
 
 Starting from v5.1, the minimum required version is Kombu 5.1.0.
 
+Py-AMQP
+~~~~~~~
+
+Starting from Celery 5.1, py-amqp will always validate certificates received from the server
+and it is no longer required to manually set ``cert_reqs`` to ``ssl.CERT_REQUIRED``.
+
+The previous default, ``ssl.CERT_NONE`` is insecure and we its usage should be discouraged.
+If you'd like to revert to the previous insecure default set ``cert_reqs`` to ``ssl.CERT_NONE``
+
+.. code-block:: python
+
+    import ssl
+
+    broker_use_ssl = {
+      'keyfile': '/var/ssl/private/worker-key.pem',
+      'certfile': '/var/ssl/amqp-server-cert.pem',
+      'ca_certs': '/var/ssl/myca.pem',
+      'cert_reqs': ssl.CERT_NONE
+    }
+
 Billiard
 ~~~~~~~~
 
 Starting from v5.1, the minimum required version is Billiard 3.6.4.
 
 Important Notes From 5.0
 ------------------------
```

### Comparing `celery-5.3.0b1/docs/images/celery-banner-small.png` & `celery-5.3.0b2/docs/images/celery-banner-small.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/celery-banner.png` & `celery-5.3.0b2/docs/images/celery-banner.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/celery_128.png` & `celery-5.3.0b2/docs/images/celery_128.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/celery_512.png` & `celery-5.3.0b2/docs/images/celery_512.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/celeryevshotsm.jpg` & `celery-5.3.0b2/docs/images/celeryevshotsm.jpg`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/dashboard.png` & `celery-5.3.0b2/docs/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/favicon.ico` & `celery-5.3.0b2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/monitor.png` & `celery-5.3.0b2/docs/images/monitor.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/result_graph.png` & `celery-5.3.0b2/docs/images/result_graph.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/images/worker_graph_full.png` & `celery-5.3.0b2/docs/images/worker_graph_full.png`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/includes/installation.txt` & `celery-5.3.0b2/docs/includes/installation.txt`

 * *Files 2% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 
 You can install the latest snapshot of these using the following
 pip commands:
 
 
 .. code-block:: console
 
-    $ pip install https://github.com/celery/celery/zipball/master#egg=celery
-    $ pip install https://github.com/celery/billiard/zipball/master#egg=billiard
-    $ pip install https://github.com/celery/py-amqp/zipball/master#egg=amqp
-    $ pip install https://github.com/celery/kombu/zipball/master#egg=kombu
-    $ pip install https://github.com/celery/vine/zipball/master#egg=vine
+    $ pip install https://github.com/celery/celery/zipball/main#egg=celery
+    $ pip install https://github.com/celery/billiard/zipball/main#egg=billiard
+    $ pip install https://github.com/celery/py-amqp/zipball/main#egg=amqp
+    $ pip install https://github.com/celery/kombu/zipball/main#egg=kombu
+    $ pip install https://github.com/celery/vine/zipball/main#egg=vine
 
 With git
 ~~~~~~~~
 
 Please see the :ref:`Contributing <contributing>` section.
```

### Comparing `celery-5.3.0b1/docs/includes/introduction.txt` & `celery-5.3.0b2/docs/includes/introduction.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.0b1 (dawn-chorus)
+:Version: 5.3.0b2 (dawn-chorus)
 :Web: https://docs.celeryq.dev/en/stable/index.html
 :Download: https://pypi.org/project/celery/
 :Source: https://github.com/celery/celery/
 :Keywords: task, queue, job, async, rabbitmq, amqp, redis,
   python, distributed, actors
 
 --
```

### Comparing `celery-5.3.0b1/docs/includes/resources.txt` & `celery-5.3.0b2/docs/includes/resources.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 of `celery`. If you don't like GitHub (for some reason) you're welcome
 to send regular patches.
 
 Be sure to also read the `Contributing to Celery`_ section in the
 documentation.
 
 .. _`Contributing to Celery`:
-    https://docs.celeryq.dev/en/master/contributing.html
+    https://docs.celeryq.dev/en/main/contributing.html
 
 .. _license:
 
 License
 =======
 
 This software is licensed under the `New BSD License`. See the :file:`LICENSE`
```

### Comparing `celery-5.3.0b1/docs/index.rst` & `celery-5.3.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/app-overview.rst` & `celery-5.3.0b2/docs/internals/app-overview.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/deprecation.rst` & `celery-5.3.0b2/docs/internals/deprecation.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/guide.rst` & `celery-5.3.0b2/docs/internals/guide.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/protocol.rst` & `celery-5.3.0b2/docs/internals/protocol.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/reference/index.rst` & `celery-5.3.0b2/docs/internals/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/internals/worker.rst` & `celery-5.3.0b2/docs/internals/worker.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/make.bat` & `celery-5.3.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/reference/celery.app.amqp.rst` & `celery-5.3.0b2/docs/reference/celery.app.amqp.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/reference/celery.rst` & `celery-5.3.0b2/docs/reference/celery.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/reference/celery.utils.debug.rst` & `celery-5.3.0b2/docs/reference/celery.utils.debug.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/reference/index.rst` & `celery-5.3.0b2/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/sec/CELERYSA-0001.txt` & `celery-5.3.0b2/docs/sec/CELERYSA-0001.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/sec/CELERYSA-0002.txt` & `celery-5.3.0b2/docs/sec/CELERYSA-0002.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/sec/CELERYSA-0003.txt` & `celery-5.3.0b2/docs/sec/CELERYSA-0003.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/spelling_wordlist.txt` & `celery-5.3.0b2/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/templates/readme.txt` & `celery-5.3.0b2/docs/templates/readme.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 .. include:: ../includes/introduction.txt
 
 .. include:: ../includes/installation.txt
 
 .. include:: ../includes/resources.txt
 
-.. |build-status| image:: https://secure.travis-ci.org/celery/celery.png?branch=master
+.. |build-status| image:: https://secure.travis-ci.org/celery/celery.png?branch=main
     :alt: Build status
     :target: https://travis-ci.org/celery/celery
 
-.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=master
-    :target: https://codecov.io/github/celery/celery?branch=master
+.. |coverage| image:: https://codecov.io/github/celery/celery/coverage.svg?branch=main
+    :target: https://codecov.io/github/celery/celery?branch=main
 
 .. |license| image:: https://img.shields.io/pypi/l/celery.svg
     :alt: BSD License
     :target: https://opensource.org/licenses/BSD-3-Clause
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/celery.svg
     :alt: Celery can be installed via wheel
```

### Comparing `celery-5.3.0b1/docs/tutorials/task-cookbook.rst` & `celery-5.3.0b2/docs/tutorials/task-cookbook.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/application.rst` & `celery-5.3.0b2/docs/userguide/application.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/calling.rst` & `celery-5.3.0b2/docs/userguide/calling.rst`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,17 @@
 
     add.apply_async((2, 2), link=[add.s(16), other_task.s()])
 
 The callbacks/errbacks will then be called in order, and all
 callbacks will be called with the return value of the parent task
 as a partial argument.
 
+In the case of a chord, we can handle errors using multiple handling strategies.
+See :ref:`chord error handling <chord-errors>` for more information.
+
 .. _calling-on-message:
 
 On message
 ==========
 
 Celery supports catching all states changes by setting on_message callback.
 
@@ -250,14 +253,32 @@
     >>> from datetime import datetime, timedelta
 
     >>> tomorrow = datetime.utcnow() + timedelta(days=1)
     >>> add.apply_async((2, 2), eta=tomorrow)
 
 .. warning::
 
+    Tasks with `eta` or `countdown` are immediately fetched by the worker
+    and until the scheduled time passes, they reside in the worker's memory.
+    When using those options to schedule lots of tasks for a distant future,
+    those tasks may accumulate in the worker and make a significant impact on
+    the RAM usage.
+
+    Moreover, tasks are not acknowledged until the worker starts executing
+    them. If using Redis as a broker, task will get redelivered when `countdown`
+    exceeds `visibility_timeout` (see :ref:`redis-caveats`).
+
+    Therefore, using `eta` and `countdown` **is not recommended** for
+    scheduling tasks for a distant future. Ideally, use values no longer
+    than several minutes. For longer durations, consider using
+    database-backed periodic tasks, e.g. with :pypi:`django-celery-beat` if
+    using Django (see :ref:`beat-custom-schedulers`).
+
+.. warning::
+
     When using RabbitMQ as a message broker when specifying a ``countdown``
     over 15 minutes, you may encounter the problem that the worker terminates
     with an :exc:`~amqp.exceptions.PreconditionFailed` error will be raised:
 
     .. code-block:: pycon
 
         amqp.exceptions.PreconditionFailed: (0, 0): (406) PRECONDITION_FAILED - consumer ack timed out on channel
@@ -349,23 +370,49 @@
     delay (float or integer). Default is 0.2.
 
 - `interval_max`
 
     Maximum number of seconds (float or integer) to wait between
     retries. Default is 0.2.
 
+- `retry_errors`
+
+    `retry_errors` is a tuple of exception classes that should be retried.
+    It will be ignored if not specified. Default is None (ignored).
+
+    .. warning::
+
+        If you specify a tuple of exception classes, you must make sure
+        that you also specify the ``max_retries`` option, otherwise
+        you will get an error.
+
+    For example, if you want to retry only tasks that were timed out, you can use
+    :exc:`~kombu.exceptions.TimeoutError`:
+
+    .. code-block:: python
+
+        from kombu.exceptions import TimeoutError
+
+        add.apply_async((2, 2), retry=True, retry_policy={
+            'max_retries': 3,
+            'retry_errors': (TimeoutError, ),
+        })
+
+    .. versionadded:: 5.3
+
 For example, the default policy correlates to:
 
 .. code-block:: python
 
     add.apply_async((2, 2), retry=True, retry_policy={
         'max_retries': 3,
         'interval_start': 0,
         'interval_step': 0.2,
         'interval_max': 0.2,
+        'retry_errors': None,
     })
 
 the maximum time spent retrying will be 0.4 seconds. It's set relatively
 short by default because a connection failure could lead to a retry pile effect
 if the broker connection is down -- For example, many web server processes waiting
 to retry, blocking other incoming requests.
 
@@ -446,16 +493,15 @@
 
     :ref:`Message Serialization <kombu:guide-serialization>` in the Kombu user
     guide.
 
 Each option has its advantages and disadvantages.
 
 json -- JSON is supported in many programming languages, is now
-    a standard part of Python (since 2.6), and is fairly fast to decode
-    using the modern Python libraries, such as :pypi:`simplejson`.
+    a standard part of Python (since 2.6), and is fairly fast to decode.
 
     The primary disadvantage to JSON is that it limits you to the following
     data types: strings, Unicode, floats, Boolean, dictionaries, and lists.
     Decimals and dates are notably missing.
 
     Binary data will be transferred using Base64 encoding,
     increasing the size of the transferred data by 34% compared to an encoding
@@ -491,25 +537,37 @@
 
     However, the Python libraries for YAML are a good bit slower than the
     libraries for JSON.
 
     If you need a more expressive set of data types and need to maintain
     cross-language compatibility, then YAML may be a better fit than the above.
 
+    To use it, install Celery with:
+
+    .. code-block:: console
+
+      $ pip install celery[yaml]
+
     See http://yaml.org/ for more information.
 
 msgpack -- msgpack is a binary serialization format that's closer to JSON
-    in features. It's very young however, and support should be considered
-    experimental at this point.
+    in features. The format compresses better, so is a faster to parse and
+    encode compared to JSON.
+
+    To use it, install Celery with:
+
+    .. code-block:: console
+
+      $ pip install celery[msgpack]
 
     See http://msgpack.org/ for more information.
 
-The encoding used is available as a message header, so the worker knows how to
-deserialize any task. If you use a custom serializer, this serializer must
-be available for the worker.
+To use a custom serializer you need add the content type to
+:setting:`accept_content`. By default, only JSON is accepted,
+and tasks containing other content headers are rejected.
 
 The following order is used to decide the serializer
 used when sending a task:
 
     1. The `serializer` execution option.
     2. The :attr:`@-Task.serializer` attribute
     3. The :setting:`task_serializer` setting.
```

### Comparing `celery-5.3.0b1/docs/userguide/canvas.rst` & `celery-5.3.0b2/docs/userguide/canvas.rst`

 * *Files 11% similar despite different names*

```diff
@@ -793,15 +793,17 @@
 * :meth:`~celery.result.GroupResult.ready`
 
     Return :const:`True` if all of the subtasks
     are ready.
 
 * :meth:`~celery.result.GroupResult.completed_count`
 
-    Return the number of completed subtasks.
+    Return the number of completed subtasks. Note that `complete` means `successful` in
+    this context. In other words, the return value of this method is the number of
+    ``successful`` tasks.
 
 * :meth:`~celery.result.GroupResult.revoke`
 
     Revoke all of the subtasks.
 
 * :meth:`~celery.result.GroupResult.join`
 
@@ -939,14 +941,17 @@
 
 Chords may have callback and errback signatures linked to them, which addresses
 some of the issues with linking signatures to groups.
 Doing so will link the provided signature to the chord's body which can be
 expected to gracefully invoke callbacks just once upon completion of the body,
 or errbacks just once if any task in the chord header or body fails.
 
+This behavior can be manipulated to allow error handling of the chord header using the :ref:`task_allow_error_cb_on_chord_header <task_allow_error_cb_on_chord_header>` flag.
+Enabling this flag will cause the chord header to invoke the errback for the body (default behavior) *and* any task in the chord's header that fails.
+
 .. _chord-important-notes:
 
 Important Notes
 ~~~~~~~~~~~~~~~
 
 Tasks used within a chord must *not* ignore their results. In practice this
 means that you must enable a :const:`result_backend` in order to use
@@ -1150,15 +1155,15 @@
 
 .. code-block:: pycon
 
     >>> sig1 = add.si(2, 2)
     >>> sig1_res = sig1.freeze()
     >>> g = group(sig1, add.si(3, 3))
     >>> g.stamp(stamp='your_custom_stamp')
-    >>> res = g1.apply_async()
+    >>> res = g.apply_async()
     >>> res.get(timeout=TIMEOUT)
     [4, 6]
     >>> sig1_res._get_task_meta()['stamp']
     ['your_custom_stamp']
 
 will initialize a group ``g`` and mark its components with stamp ``your_custom_stamp``.
 
@@ -1194,15 +1199,15 @@
 
 If more complex stamping logic is required, it is possible
 to implement custom stamping behavior based on the Visitor
 pattern. The class that implements this custom logic must
 inherit ``VisitorStamping`` and implement appropriate methods.
 
 For example, the following example ``InGroupVisitor`` will label
-tasks that are in side of some group by lable ``in_group``.
+tasks that are in side of some group by label ``in_group``.
 
 .. code-block:: python
 
     class InGroupVisitor(StampingVisitor):
         def __init__(self):
             self.in_group = False
 
@@ -1214,7 +1219,122 @@
             self.in_group = False
 
         def on_chain_start(self, chain, **headers) -> dict:
             return {"in_group": [self.in_group], "stamped_headers": ["in_group"]}
 
         def on_signature(self, sig, **headers) -> dict:
             return {"in_group": [self.in_group], "stamped_headers": ["in_group"]}
+
+The following example shows another custom stamping visitor, which labels all
+tasks with a custom ``monitoring_id`` which can represent a UUID value of an external monitoring system,
+that can be used to track the task execution by including the id with such a visitor implementation.
+This ``monitoring_id`` can be a randomly generated UUID, or a unique identifier of the span id used by
+the external monitoring system, etc.
+
+.. code-block:: python
+
+    class MonitoringIdStampingVisitor(StampingVisitor):
+        def on_signature(self, sig, **headers) -> dict:
+            return {'monitoring_id': uuid4().hex}
+
+.. note::
+
+    The ``stamped_headers`` key returned in ``on_signature`` is used to specify the headers that will be
+    stamped on the task. If this key is not specified, the stamping visitor will assume all keys in the
+    returned dictionary are the stamped headers from the visitor.
+    This means the following code block will result in the same behavior as the previous example.
+
+.. code-block:: python
+
+    class MonitoringIdStampingVisitor(StampingVisitor):
+        def on_signature(self, sig, **headers) -> dict:
+            return {'monitoring_id': uuid4().hex, 'stamped_headers': ['monitoring_id']}
+
+Next, lets see how to use the ``MonitoringIdStampingVisitor`` example stamping visitor.
+
+.. code-block:: python
+
+    sig_example = signature('t1')
+    sig_example.stamp(visitor=MonitoringIdStampingVisitor())
+
+    group_example = group([signature('t1'), signature('t2')])
+    group_example.stamp(visitor=MonitoringIdStampingVisitor())
+
+    chord_example = chord([signature('t1'), signature('t2')], signature('t3'))
+    chord_example.stamp(visitor=MonitoringIdStampingVisitor())
+
+    chain_example = chain(signature('t1'), group(signature('t2'), signature('t3')), signature('t4'))
+    chain_example.stamp(visitor=MonitoringIdStampingVisitor())
+
+Lastly, it's important to mention that each monitoring id stamp in the example above would be different from each other between tasks.
+
+Callbacks stamping
+------------------
+
+The stamping API also supports stamping callbacks implicitly.
+This means that when a callback is added to a task, the stamping
+visitor will be applied to the callback as well.
+
+.. warning::
+
+    The callback must be linked to the signature before stamping.
+
+For example, lets examine the following custom stamping visitor.
+
+.. code-block:: python
+
+    class CustomStampingVisitor(StampingVisitor):
+        def on_signature(self, sig, **headers) -> dict:
+            return {'header': 'value'}
+
+        def on_callback(self, callback, **header) -> dict:
+            return {'on_callback': True}
+
+        def on_errback(self, errback, **header) -> dict:
+            return {'on_errback': True}
+
+This custom stamping visitor will stamp the signature, callbacks, and errbacks with ``{'header': 'value'}``
+and stamp the callbacks and errbacks with ``{'on_callback': True}`` and ``{'on_errback': True}`` respectively as shown below.
+
+.. code-block:: python
+
+        c = chord([add.s(1, 1), add.s(2, 2)], xsum.s())
+        callback = signature('sig_link')
+        errback = signature('sig_link_error')
+        c.link(callback)
+        c.link_error(errback)
+        c.stamp(visitor=CustomStampingVisitor())
+
+This example will result in the following stamps:
+
+.. code-block:: python
+
+    >>> c.options
+    {'header': 'value', 'stamped_headers': ['header']}
+    >>> c.tasks.tasks[0].options
+    {'header': 'value', 'stamped_headers': ['header']}
+    >>> c.tasks.tasks[1].options
+    {'header': 'value', 'stamped_headers': ['header']}
+    >>> c.body.options
+    {'header': 'value', 'stamped_headers': ['header']}
+    >>> c.body.options['link'][0].options
+    {'header': 'value', 'on_callback': True, 'stamped_headers': ['header', 'on_callback']}
+    >>> c.body.options['link_error'][0].options
+    {'header': 'value', 'on_errback': True, 'stamped_headers': ['header', 'on_errback']}
+
+When calling ``apply_async()`` on ``c``, the group stamping will be applied on top of the above stamps.
+This will result in the following stamps:
+
+.. code-block:: python
+
+    >>> c.options
+    {'header': 'value', 'groups': ['1234'], 'stamped_headers': ['header', 'groups']}
+    >>> c.tasks.tasks[0].options
+    {'header': 'value', 'groups': ['1234'], 'stamped_headers': ['header', 'groups']}
+    >>> c.tasks.tasks[1].options
+    {'header': 'value', 'groups': ['1234'], 'stamped_headers': ['header', 'groups']}
+    >>> c.body.options
+    {'header': 'value', 'groups': [], 'stamped_headers': ['header', 'groups']}
+    >>> c.body.options['link'][0].options
+    {'header': 'value', 'on_callback': True, 'groups': [], 'stamped_headers': ['header', 'on_callback', 'groups']}
+    >>> c.body.options['link_error'][0].options
+    {'header': 'value', 'on_errback': True, 'groups': [], 'stamped_headers': ['header', 'on_errback', 'groups']}
```

### Comparing `celery-5.3.0b1/docs/userguide/concurrency/eventlet.rst` & `celery-5.3.0b2/docs/userguide/concurrency/eventlet.rst`

 * *Files 1% similar despite different names*

```diff
@@ -63,9 +63,9 @@
 .. _`Eventlet`: http://eventlet.net
 .. _`epoll(4)`: http://linux.die.net/man/4/epoll
 .. _`libevent`: http://monkey.org/~provos/libevent/
 .. _`highly scalable non-blocking I/O`:
     https://en.wikipedia.org/wiki/Asynchronous_I/O#Select.28.2Fpoll.29_loops
 .. _`Coroutines`: https://en.wikipedia.org/wiki/Coroutine
 .. _`Eventlet examples`:
-    https://github.com/celery/celery/tree/master/examples/eventlet
+    https://github.com/celery/celery/tree/main/examples/eventlet
```

### Comparing `celery-5.3.0b1/docs/userguide/configuration.rst` & `celery-5.3.0b2/docs/userguide/configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 ``CELERY_ROUTES``                          :setting:`task_routes`
 ``CELERY_SEND_SENT_EVENT``                 :setting:`task_send_sent_event`
 ``CELERY_TASK_SERIALIZER``                 :setting:`task_serializer`
 ``CELERYD_SOFT_TIME_LIMIT``                :setting:`task_soft_time_limit`
 ``CELERY_TASK_TRACK_STARTED``              :setting:`task_track_started`
 ``CELERY_TASK_REJECT_ON_WORKER_LOST``      :setting:`task_reject_on_worker_lost`
 ``CELERYD_TIME_LIMIT``                     :setting:`task_time_limit`
+``CELERY_ALLOW_ERROR_CB_ON_CHORD_HEADER``  :setting:`task_allow_error_cb_on_chord_header`
 ``CELERYD_AGENT``                          :setting:`worker_agent`
 ``CELERYD_AUTOSCALER``                     :setting:`worker_autoscaler`
 ``CELERYD_CONCURRENCY``                    :setting:`worker_concurrency`
 ``CELERYD_CONSUMER``                       :setting:`worker_consumer`
 ``CELERY_WORKER_DIRECT``                   :setting:`worker_direct`
 ``CELERY_DISABLE_RATE_LIMITS``             :setting:`worker_disable_rate_limits`
 ``CELERY_ENABLE_REMOTE_CONTROL``           :setting:`worker_enable_remote_control`
@@ -507,14 +508,65 @@
 ~~~~~~~~~~~~~~~~~~~
 
 Default: No time limit.
 
 Task hard time limit in seconds. The worker processing the task will
 be killed and replaced with a new one when this is exceeded.
 
+.. setting:: task_allow_error_cb_on_chord_header
+
+``task_allow_error_cb_on_chord_header``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.3
+
+Default: Disabled.
+
+Enabling this flag will allow linking an error callback to a chord header,
+which by default will not link when using :code:`link_error()`, and preventing
+from the chord's body to execute if any of the tasks in the header fails.
+
+Consider the following canvas with the flag disabled (default behavior):
+
+.. code-block:: python
+
+    header = group([t1, t2])
+    body = t3
+    c = chord(header, body)
+    c.link_error(error_callback_sig)
+
+If *any* of the header tasks failed (:code:`t1` or :code:`t2`), by default, the chord body (:code:`t3`) would **not execute**, and :code:`error_callback_sig` will be called **once** (for the body).
+
+Enabling this flag will change the above behavior by:
+
+1. :code:`error_callback_sig` will be linked to :code:`t1` and :code:`t2` (as well as :code:`t3`).
+2. If *any* of the header tasks failed, :code:`error_callback_sig` will be called **for each** failed header task **and** the :code:`body` (even if the body didn't run).
+
+Consider now the following canvas with the flag enabled:
+
+.. code-block:: python
+
+    header = group([failingT1, failingT2])
+    body = t3
+    c = chord(header, body)
+    c.link_error(error_callback_sig)
+
+If *all* of the header tasks failed (:code:`failingT1` and :code:`failingT2`), then the chord body (:code:`t3`) would **not execute**, and :code:`error_callback_sig` will be called **3 times** (two times for the header and one time for the body).
+
+Lastly, consider the following canvas with the flag enabled:
+
+.. code-block:: python
+
+    header = group([failingT1, failingT2])
+    body = t3
+    upgraded_chord = chain(header, body)
+    upgraded_chord.link_error(error_callback_sig)
+
+This canvas will behave exactly the same as the previous one, since the :code:`chain` will be upgraded to a :code:`chord` internally.
+
 .. setting:: task_soft_time_limit
 
 ``task_soft_time_limit``
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 Default: No soft time limit.
 
@@ -539,15 +591,15 @@
 
 ``task_acks_late``
 ~~~~~~~~~~~~~~~~~~
 
 Default: Disabled.
 
 Late ack means the task messages will be acknowledged **after** the task
-has been executed, not *just before* (the default behavior).
+has been executed, not *right before* (the default behavior).
 
 .. seealso::
 
     FAQ: :ref:`faq-acks_late-vs-retry`.
 
 .. setting:: task_acks_on_failure_or_timeout
 
@@ -736,14 +788,26 @@
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Default: Inf
 
 This is the maximum of retries in case of recoverable exceptions.
 
 
+.. setting:: result_backend_thread_safe
+
+``result_backend_thread_safe``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Default: False
+
+If True, then the backend object is shared across threads.
+This may be useful for using a shared connection pool instead of creating
+a connection for every thread.
+
+
 .. setting:: result_backend_transport_options
 
 ``result_backend_transport_options``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Default: ``{}`` (empty mapping).
 
@@ -2397,26 +2461,26 @@
 
 Default: Disabled.
 
 This option enables so that every worker has a dedicated queue,
 so that tasks can be routed to specific workers.
 
 The queue name for each worker is automatically generated based on
-the worker hostname and a ``.dq`` suffix, using the ``C.dq`` exchange.
+the worker hostname and a ``.dq`` suffix, using the ``C.dq2`` exchange.
 
 For example the queue name for the worker with node name ``w1@example.com``
 becomes::
 
     w1@example.com.dq
 
 Then you can route the task to the worker by specifying the hostname
-as the routing key and the ``C.dq`` exchange::
+as the routing key and the ``C.dq2`` exchange::
 
     task_routes = {
-        'tasks.add': {'exchange': 'C.dq', 'routing_key': 'w1@example.com'}
+        'tasks.add': {'exchange': 'C.dq2', 'routing_key': 'w1@example.com'}
     }
 
 .. setting:: task_create_missing_queues
 
 ``task_create_missing_queues``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -2642,20 +2706,22 @@
     broker_use_ssl = {
       'keyfile': '/var/ssl/private/worker-key.pem',
       'certfile': '/var/ssl/amqp-server-cert.pem',
       'ca_certs': '/var/ssl/myca.pem',
       'cert_reqs': ssl.CERT_REQUIRED
     }
 
-.. warning::
+.. versionadded:: 5.1
+
+    Starting from Celery 5.1, py-amqp will always validate certificates received from the server
+    and it is no longer required to manually set ``cert_reqs`` to ``ssl.CERT_REQUIRED``.
+
+    The previous default, ``ssl.CERT_NONE`` is insecure and we its usage should be discouraged.
+    If you'd like to revert to the previous insecure default set ``cert_reqs`` to ``ssl.CERT_NONE``
 
-    Be careful using ``broker_use_ssl=True``. It's possible that your default
-    configuration won't validate the server cert at all. Please read Python
-    `ssl module security
-    considerations <https://docs.python.org/3/library/ssl.html#ssl-security>`_.
 
 ``redis``
 _________
 
 
 The setting must be a dict with the following keys:
 
@@ -2748,14 +2814,27 @@
 Default: 100.
 
 Maximum number of retries before we give up re-establishing a connection
 to the AMQP broker.
 
 If this is set to :const:`0` or :const:`None`, we'll retry forever.
 
+``broker_channel_error_retry``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.3
+
+Default: Disabled.
+
+Automatically try to re-establish the connection to the AMQP broker
+if any invalid response has been returned.
+
+The retry count and interval is the same as that of `broker_connection_retry`.
+Also, this option doesn't work when `broker_connection_retry` is `False`.
+
 .. setting:: broker_login_method
 
 ``broker_login_method``
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 Default: ``"AMQPLAIN"``.
 
@@ -3437,7 +3516,20 @@
 but for the :pypi:`django-celery-beat` database scheduler it's 5 seconds
 because the schedule may be changed externally, and so it must take
 changes to the schedule into account.
 
 Also when running Celery beat embedded (:option:`-B <celery worker -B>`)
 on Jython as a thread the max interval is overridden and set to 1 so
 that it's possible to shut down in a timely manner.
+
+.. setting:: beat_cron_starting_deadline
+
+``beat_cron_starting_deadline``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. versionadded:: 5.3
+
+Default: None.
+
+When using cron, the number of seconds :mod:`~celery.bin.beat` can look back
+when deciding whether a cron schedule is due. When set to `None`, cronjobs that
+are past due will always run immediately.
```

### Comparing `celery-5.3.0b1/docs/userguide/daemonizing.rst` & `celery-5.3.0b2/docs/userguide/daemonizing.rst`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 See the `extra/generic-init.d/`_ directory Celery distribution.
 
 This directory contains generic bash init-scripts for the
 :program:`celery worker` program,
 these should run on Linux, FreeBSD, OpenBSD, and other Unix-like platforms.
 
 .. _`extra/generic-init.d/`:
-    https://github.com/celery/celery/tree/master/extra/generic-init.d/
+    https://github.com/celery/celery/tree/main/extra/generic-init.d/
 
 .. _generic-initd-celeryd:
 
 Init-script: ``celeryd``
 ----------------------------------------------------------------------
 
 :Usage: `/etc/init.d/celeryd {start|stop|restart|status}`
@@ -369,15 +369,15 @@
 
 Usage ``systemd``
 ======================================================================
 
 * `extra/systemd/`_
 
 .. _`extra/systemd/`:
-    https://github.com/celery/celery/tree/master/extra/systemd/
+    https://github.com/celery/celery/tree/main/extra/systemd/
 
 .. _generic-systemd-celery:
 
 :Usage: `systemctl {start|stop|restart|status} celery.service`
 :Configuration file: /etc/conf.d/celery
 
 Service file: celery.service
@@ -537,18 +537,18 @@
 
 :pypi:`supervisor`
 ======================================================================
 
 * `extra/supervisord/`_
 
 .. _`extra/supervisord/`:
-    https://github.com/celery/celery/tree/master/extra/supervisord/
+    https://github.com/celery/celery/tree/main/extra/supervisord/
 
 .. _daemon-launchd:
 
 ``launchd`` (macOS)
 ======================================================================
 
 * `extra/macOS`_
 
 .. _`extra/macOS`:
-    https://github.com/celery/celery/tree/master/extra/macOS/
+    https://github.com/celery/celery/tree/main/extra/macOS/
```

### Comparing `celery-5.3.0b1/docs/userguide/debugging.rst` & `celery-5.3.0b2/docs/userguide/debugging.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/extending.rst` & `celery-5.3.0b2/docs/userguide/extending.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/monitoring.rst` & `celery-5.3.0b2/docs/userguide/monitoring.rst`

 * *Files 1% similar despite different names*

```diff
@@ -295,17 +295,17 @@
     $ celery -A proj flower --port=5555
 
 Broker URL can also be passed through the
 :option:`--broker <celery --broker>` argument :
 
 .. code-block:: console
 
-    $ celery flower --broker=amqp://guest:guest@localhost:5672//
+    $ celery --broker=amqp://guest:guest@localhost:5672// flower
     or
-    $ celery flower --broker=redis://guest:guest@localhost:6379/0
+    $ celery --broker=redis://guest:guest@localhost:6379/0 flower
 
 Then, you can visit flower in your web browser :
 
 .. code-block:: console
 
     $ open http://localhost:5555
```

### Comparing `celery-5.3.0b1/docs/userguide/optimizing.rst` & `celery-5.3.0b2/docs/userguide/optimizing.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/periodic-tasks.rst` & `celery-5.3.0b2/docs/userguide/periodic-tasks.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/routing.rst` & `celery-5.3.0b2/docs/userguide/routing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -300,16 +300,16 @@
 
 .. code-block:: python
 
     ['celery', 'celery:1', 'celery:2', 'celery:3', 'celery:4', 'celery:5', 'celery:6', 'celery:7', 'celery:8', 'celery:9']
 
 
 That said, note that this will never be as good as priorities implemented at the
-server level, and may be approximate at best. But it may still be good enough
-for your application.
+broker server level, and may be approximate at best. But it may still be good
+enough for your application.
 
 
 AMQP Primer
 ===========
 
 Messages
 --------
```

### Comparing `celery-5.3.0b1/docs/userguide/security.rst` & `celery-5.3.0b2/docs/userguide/security.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/signals.rst` & `celery-5.3.0b2/docs/userguide/signals.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/docs/userguide/tasks.rst` & `celery-5.3.0b2/docs/userguide/tasks.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1428,17 +1428,19 @@
 ~~~~~~~~~~~~~~
 
 The above can be added to each task like this:
 
 .. code-block:: python
 
 
-    @app.task(base=DatabaseTask)
-    def process_rows():
-        for row in process_rows.db.table.all():
+    from celery.app import task
+
+    @app.task(base=DatabaseTask, bind=True)
+    def process_rows(self: task):
+        for row in self.db.table.all():
             process_row(row)
 
 The ``db`` attribute of the ``process_rows`` task will then
 always stay the same in each process.
 
 .. _custom-task-cls-app-wide:
```

### Comparing `celery-5.3.0b1/docs/userguide/testing.rst` & `celery-5.3.0b2/docs/userguide/testing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,16 @@
 
 .. code-block:: python
 
     def test_create_task(celery_app, celery_worker):
         @celery_app.task
         def mul(x, y):
             return x * y
-
+        
+        celery_worker.reload()
         assert mul.delay(4, 4).get(timeout=10) == 16
 
 ``celery_worker`` - Embed live worker.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 This fixture starts a Celery worker instance that you can use
 for integration tests.  The worker will be started in a *separate thread*
```

### Comparing `celery-5.3.0b1/docs/userguide/workers.rst` & `celery-5.3.0b2/docs/userguide/workers.rst`

 * *Files 5% similar despite different names*

```diff
@@ -464,14 +464,79 @@
 
 See also :ref:`worker-files`
 
 Note that remote control commands must be working for revokes to work.
 Remote control commands are only supported by the RabbitMQ (amqp) and Redis
 at this point.
 
+.. control:: revoke_by_stamped_header
+
+``revoke_by_stamped_header``: Revoking tasks by their stamped headers
+---------------------------------------------------------------------
+:pool support: all, terminate only supported by prefork and eventlet
+:broker support: *amqp, redis*
+:command: :program:`celery -A proj control revoke_by_stamped_header <header=value>`
+
+This command is similar to :meth:`~@control.revoke`, but instead of
+specifying the task id(s), you specify the stamped header(s) as key-value pair(s),
+and each task that has a stamped header matching the key-value pair(s) will be revoked.
+
+.. warning::
+
+    The revoked headers mapping is not persistent across restarts, so if you
+    restart the workers, the revoked headers will be lost and need to be
+    mapped again.
+
+.. warning::
+
+    This command may perform poorly if your worker pool concurrency is high
+    and terminate is enabled, since it will have to iterate over all the running
+    tasks to find the ones with the specified stamped header.
+
+**Example**
+
+.. code-block:: pycon
+
+    >>> app.control.revoke_by_stamped_header({'header': 'value'})
+
+    >>> app.control.revoke_by_stamped_header({'header': 'value'}, terminate=True)
+
+    >>> app.control.revoke_by_stamped_header({'header': 'value'}, terminate=True, signal='SIGKILL')
+
+
+Revoking multiple tasks by stamped headers
+------------------------------------------
+
+.. versionadded:: 5.3
+
+The ``revoke_by_stamped_header`` method also accepts a list argument, where it will revoke
+by several headers or several values.
+
+**Example**
+
+.. code-block:: pycon
+
+    >> app.control.revoke_by_stamped_header({
+    ...    'header_A': 'value_1',
+    ...    'header_B': ['value_2', 'value_3'],
+    })
+
+This will revoke all of the tasks that have a stamped header ``header_A`` with value ``value_1``,
+and all of the tasks that have a stamped header ``header_B`` with values ``value_2`` or ``value_3``.
+
+**CLI Example**
+
+.. code-block:: console
+
+    $ celery -A proj control revoke_by_stamped_header stamped_header_key_A=stamped_header_value_1 stamped_header_key_B=stamped_header_value_2
+
+    $ celery -A proj control revoke_by_stamped_header stamped_header_key_A=stamped_header_value_1 stamped_header_key_B=stamped_header_value_2 --terminate
+
+    $ celery -A proj control revoke_by_stamped_header stamped_header_key_A=stamped_header_value_1 stamped_header_key_B=stamped_header_value_2 --terminate --signal=SIGKILL
+
 .. _worker-time-limits:
 
 Time Limits
 ===========
 
 .. versionadded:: 2.0
```

### Comparing `celery-5.3.0b1/docs/whatsnew-5.2.rst` & `celery-5.3.0b2/docs/whatsnew-5.2.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/app/myapp.py` & `celery-5.3.0b2/examples/app/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/celery_http_gateway/README.rst` & `celery-5.3.0b2/examples/celery_http_gateway/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/celery_http_gateway/settings.py` & `celery-5.3.0b2/examples/celery_http_gateway/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/celery_http_gateway/urls.py` & `celery-5.3.0b2/examples/celery_http_gateway/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/django/README.rst` & `celery-5.3.0b2/examples/django/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/django/proj/celery.py` & `celery-5.3.0b2/examples/django/proj/celery.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/django/proj/settings.py` & `celery-5.3.0b2/examples/django/proj/settings.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/django/proj/urls.py` & `celery-5.3.0b2/examples/django/proj/urls.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/django/proj/wsgi.py` & `celery-5.3.0b2/examples/django/proj/wsgi.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/eventlet/README.rst` & `celery-5.3.0b2/examples/eventlet/README.rst`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/eventlet/bulk_task_producer.py` & `celery-5.3.0b2/examples/eventlet/bulk_task_producer.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/eventlet/webcrawler.py` & `celery-5.3.0b2/examples/eventlet/webcrawler.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/next-steps/setup.py` & `celery-5.3.0b2/examples/next-steps/setup.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/periodic-tasks/myapp.py` & `celery-5.3.0b2/examples/periodic-tasks/myapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/resultgraph/tasks.py` & `celery-5.3.0b2/examples/resultgraph/tasks.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/security/mysecureapp.py` & `celery-5.3.0b2/examples/security/mysecureapp.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/security/ssl/worker.key` & `celery-5.3.0b2/examples/security/ssl/worker.key`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/examples/security/ssl/worker.pem` & `celery-5.3.0b2/examples/security/ssl/worker.pem`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/bash-completion/celery.bash` & `celery-5.3.0b2/extra/bash-completion/celery.bash`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/generic-init.d/celerybeat` & `celery-5.3.0b2/extra/generic-init.d/celerybeat`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/generic-init.d/celeryd` & `celery-5.3.0b2/extra/generic-init.d/celeryd`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     local iwoth=$(ls -ld "$path" | cut -b 9)
 
     if [ "$(id -u $owner)" != "0" ]; then
         echo "Error: Config script '$path' must be owned by root!"
         echo
         echo "Resolution:"
         echo "Review the file carefully, and make sure it hasn't been "
-        echo "modified with mailicious intent.  When sure the "
+        echo "modified with malicious intent.  When sure the "
         echo "script is safe to execute with superuser privileges "
         echo "you can change ownership of the script:"
         echo "    $ sudo chown root '$path'"
         exit 1
     fi
 
     if [ "$iwoth" != "-" ]; then  # S_IWOTH
```

### Comparing `celery-5.3.0b1/extra/macOS/org.celeryq.beat.plist` & `celery-5.3.0b2/extra/macOS/org.celeryq.beat.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/macOS/org.celeryq.worker.plist` & `celery-5.3.0b2/extra/macOS/org.celeryq.worker.plist`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/supervisord/celerybeat.conf` & `celery-5.3.0b2/extra/supervisord/celerybeat.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/supervisord/celeryd.conf` & `celery-5.3.0b2/extra/supervisord/celeryd.conf`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/supervisord/supervisord.conf` & `celery-5.3.0b2/extra/supervisord/supervisord.conf`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 childlogdir=/var/log/supervisord/            ; where child log files will live
 
 
 [rpcinterface:supervisor]
 supervisor.rpcinterface_factory = supervisor.rpcinterface:make_main_rpcinterface
 
 [supervisorctl]
-serverurl=unix:///tmp/supervisor.sock ; use unix:// schem for a unix sockets.
+serverurl=unix:///tmp/supervisor.sock ; use unix:// scheme for a unix sockets.
 
 
 [include]
 
 # Uncomment this line for celeryd for Python
 ;files=celeryd.conf
```

### Comparing `celery-5.3.0b1/extra/systemd/celery.service` & `celery-5.3.0b2/extra/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/extra/zsh-completion/celery.zsh` & `celery-5.3.0b2/extra/zsh-completion/celery.zsh`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/requirements/README.rst` & `celery-5.3.0b2/requirements/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 Index
 =====
 
 * :file:`requirements/default.txt`
 
-    Default requirements for Python 2.7+.
+    Default requirements for Python 3.7+.
 
 * :file:`requirements/jython.txt`
 
     Extra requirements needed to run on Jython 2.5
 
 * :file:`requirements/security.txt`
 
@@ -25,15 +25,15 @@
 
 * :file:`requirements/test-ci-base.txt`
 
     Extra test requirements required by the CI suite (Tox).
 
 * :file:`requirements/test-ci-default.txt`
 
-    Extra test requirements required for Python 2.7 by the CI suite (Tox).
+    Extra test requirements required for Python 3.7 by the CI suite (Tox).
 
 * :file:`requirements/test-integration.txt`
 
     Extra requirements needed when running the integration test suite.
 
 * :file:`requirements/doc.txt`
```

### Comparing `celery-5.3.0b1/requirements/test-ci-default.txt` & `celery-5.3.0b2/requirements/test-ci-default.txt`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/setup.py` & `celery-5.3.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     version=meta['version'],
     description=meta['doc'],
     long_description=long_description(),
     keywords=meta['keywords'],
     author=meta['author'],
     author_email=meta['contact'],
     url=meta['homepage'],
-    license='BSD',
+    license='BSD-3-Clause',
     platforms=['any'],
     install_requires=install_requires(),
     python_requires=">=3.7",
     tests_require=reqs('test.txt'),
     extras_require=extras_require(),
     cmdclass={'test': pytest},
     include_package_data=True,
```

### Comparing `celery-5.3.0b1/t/benchmarks/bench_worker.py` & `celery-5.3.0b2/t/benchmarks/bench_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/integration/conftest.py` & `celery-5.3.0b2/t/integration/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 
 import pytest
 
 # we have to import the pytest plugin fixtures here,
 # in case user did not do the `python setup.py develop` yet,
 # that installs the pytest plugin into the setuptools registry.
@@ -26,25 +27,34 @@
 
 
 def get_active_redis_channels():
     return get_redis_connection().execute_command('PUBSUB CHANNELS')
 
 
 @pytest.fixture(scope='session')
-def celery_config():
-    return {
+def celery_config(request):
+    config = {
         'broker_url': TEST_BROKER,
         'result_backend': TEST_BACKEND,
         'cassandra_servers': ['localhost'],
         'cassandra_keyspace': 'tests',
         'cassandra_table': 'tests',
         'cassandra_read_consistency': 'ONE',
         'cassandra_write_consistency': 'ONE',
         'result_extended': True
     }
+    try:
+        # To override the default configuration, create the integration-tests-config.json file
+        # in Celery's root directory.
+        # The file must contain a dictionary of valid configuration name/value pairs.
+        config_overrides = json.load(open(str(request.config.rootdir / "integration-tests-config.json")))
+        config.update(config_overrides)
+    except OSError:
+        pass
+    return config
 
 
 @pytest.fixture(scope='session')
 def celery_enable_logging():
     return True
```

### Comparing `celery-5.3.0b1/t/integration/tasks.py` & `celery-5.3.0b2/t/integration/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections.abc import Iterable
 from time import sleep
 
 from celery import Signature, Task, chain, chord, group, shared_task
+from celery.canvas import StampingVisitor, signature
 from celery.exceptions import SoftTimeLimitExceeded
 from celery.utils.log import get_task_logger
 
 from .conftest import get_redis_connection
 
 logger = get_task_logger(__name__)
 
@@ -22,14 +23,20 @@
     if z:
         return x + y + z
     else:
         return x + y
 
 
 @shared_task
+def mul(x: int, y: int) -> int:
+    """Multiply two numbers"""
+    return x * y
+
+
+@shared_task
 def write_to_file_and_return_int(file_name, i):
     with open(file_name, mode='a', buffering=1) as file_handle:
         file_handle.write(str(i)+'\n')
 
     return i
 
 
@@ -237,14 +244,20 @@
 @shared_task
 def redis_echo(message, redis_key="redis-echo"):
     """Task that appends the message to a redis list."""
     redis_connection = get_redis_connection()
     redis_connection.rpush(redis_key, message)
 
 
+@shared_task(bind=True)
+def redis_echo_group_id(self, _, redis_key="redis-group-ids"):
+    redis_connection = get_redis_connection()
+    redis_connection.rpush(redis_key, self.request.group)
+
+
 @shared_task
 def redis_count(redis_key="redis-count"):
     """Task that increments a specified or well-known redis key."""
     redis_connection = get_redis_connection()
     redis_connection.incr(redis_key)
 
 
@@ -411,7 +424,34 @@
     return request_id
 
 
 @shared_task
 def errback_new_style(request, exc, tb):
     redis_count(request.id)
     return request.id
+
+
+class StampOnReplace(StampingVisitor):
+    stamp = {'StampOnReplace': 'This is the replaced task'}
+
+    def on_signature(self, sig, **headers) -> dict:
+        return self.stamp
+
+
+class StampedTaskOnReplace(Task):
+    """Custom task for stamping on replace"""
+
+    def on_replace(self, sig):
+        sig.stamp(StampOnReplace())
+        return super().on_replace(sig)
+
+
+@shared_task
+def replaced_with_me():
+    return True
+
+
+@shared_task(bind=True, base=StampedTaskOnReplace)
+def replace_with_stamped_task(self: StampedTaskOnReplace, replace_with=None):
+    if replace_with is None:
+        replace_with = replaced_with_me.s()
+    self.replace(signature(replace_with))
```

### Comparing `celery-5.3.0b1/t/integration/test_backend.py` & `celery-5.3.0b2/t/integration/test_backend.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/integration/test_canvas.py` & `celery-5.3.0b2/t/integration/test_canvas.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 import re
 import tempfile
 import uuid
 from datetime import datetime, timedelta
 from time import monotonic, sleep
 
 import pytest
-import pytest_subtests  # noqa: F401
+import pytest_subtests  # noqa
 
 from celery import chain, chord, group, signature
 from celery.backends.base import BaseKeyValueStoreBackend
+from celery.canvas import StampingVisitor
 from celery.exceptions import ImproperlyConfigured, TimeoutError
 from celery.result import AsyncResult, GroupResult, ResultSet
+from celery.signals import before_task_publish, task_received
 
 from . import tasks
 from .conftest import TEST_BACKEND, get_active_redis_channels, get_redis_connection
-from .tasks import (ExpectedException, add, add_chord_to_chord, add_replaced, add_to_all, add_to_all_to_chord,
-                    build_chain_inside_task, collect_ids, delayed_sum, delayed_sum_with_soft_guard,
-                    errback_new_style, errback_old_style, fail, fail_replaced, identity, ids, print_unicode,
-                    raise_error, redis_count, redis_echo, replace_with_chain, replace_with_chain_which_raises,
-                    replace_with_empty_chain, retry_once, return_exception, return_priority, second_order_replace1,
+from .tasks import (ExpectedException, StampOnReplace, add, add_chord_to_chord, add_replaced, add_to_all,
+                    add_to_all_to_chord, build_chain_inside_task, collect_ids, delayed_sum,
+                    delayed_sum_with_soft_guard, errback_new_style, errback_old_style, fail, fail_replaced, identity,
+                    ids, mul, print_unicode, raise_error, redis_count, redis_echo, redis_echo_group_id,
+                    replace_with_chain, replace_with_chain_which_raises, replace_with_empty_chain,
+                    replace_with_stamped_task, retry_once, return_exception, return_priority, second_order_replace1,
                     tsum, write_to_file_and_return_int, xsum)
 
 RETRYABLE_EXCEPTIONS = (OSError, ConnectionError, TimeoutError)
 
 
 def is_retryable_exception(exc):
     return isinstance(exc, RETRYABLE_EXCEPTIONS)
@@ -58,20 +61,44 @@
         if maybe_key_msg is None:
             raise TimeoutError(
                 "Fetching from {!r} timed out - still awaiting {!r}"
                 .format(redis_key, dict(+expected_msgs))
             )
         retrieved_key, msg = maybe_key_msg
         assert retrieved_key.decode("utf-8") == redis_key
-        expected_msgs[msg] -= 1     # silently accepts unexpected messages
+        expected_msgs[msg] -= 1  # silently accepts unexpected messages
 
     # There should be no more elements - block momentarily
     assert redis_connection.blpop(redis_key, min(1, timeout)) is None
 
 
+def await_redis_list_message_length(expected_length, redis_key="redis-group-ids", timeout=TIMEOUT):
+    """
+    Helper to wait for a specified or well-known redis key to contain a string.
+    """
+    sleep(1)
+    redis_connection = get_redis_connection()
+
+    check_interval = 0.1
+    check_max = int(timeout / check_interval)
+
+    for i in range(check_max + 1):
+        length = redis_connection.llen(redis_key)
+
+        if length == expected_length:
+            break
+
+        sleep(check_interval)
+    else:
+        raise TimeoutError(f'{redis_key!r} has length of {length}, but expected to be of length {expected_length}')
+
+    sleep(min(1, timeout))
+    assert redis_connection.llen(redis_key) == expected_length
+
+
 def await_redis_count(expected_count, redis_key="redis-count", timeout=TIMEOUT):
     """
     Helper to wait for a specified or well-known redis key to count to a value.
     """
     redis_connection = get_redis_connection()
 
     check_interval = 0.1
@@ -91,14 +118,21 @@
         raise TimeoutError(f"{redis_key!r} was never incremented")
 
     # There should be no more increments - block momentarily
     sleep(min(1, timeout))
     assert int(redis_connection.get(redis_key)) == expected_count
 
 
+def compare_group_ids_in_redis(redis_key='redis-group-ids'):
+    redis_connection = get_redis_connection()
+    actual = redis_connection.lrange(redis_key, 0, -1)
+    assert len(actual) >= 2, 'Expected at least 2 group ids in redis'
+    assert actual[0] == actual[1], 'Expected group ids to be equal'
+
+
 class test_link_error:
     @flaky
     def test_link_error_eager(self):
         exception = ExpectedException("Task expected to fail", "test")
         result = fail.apply(args=("test",), link_error=return_exception.s())
         actual = result.get(timeout=TIMEOUT, propagate=False)
         assert actual == exception
@@ -565,14 +599,37 @@
         )
         c.link(redis_echo.s())
         res = c.delay()
 
         assert res.get(timeout=TIMEOUT) == 'Hello world'
         await_redis_echo({link_msg, 'Hello world'})
 
+    def test_chain_flattening_keep_links_of_inner_chain(self, manager):
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+
+        redis_connection = get_redis_connection()
+
+        link_b_msg = 'link_b called'
+        link_b_key = 'echo_link_b'
+        link_b_sig = redis_echo.si(link_b_msg, redis_key=link_b_key)
+
+        def link_chain(sig):
+            sig.link(link_b_sig)
+            sig.link_error(identity.s('link_ab'))
+            return sig
+
+        inner_chain = link_chain(chain(identity.s('a'), add.s('b')))
+        flat_chain = chain(inner_chain, add.s('c'))
+        redis_connection.delete(link_b_key)
+        res = flat_chain.delay()
+
+        assert res.get(timeout=TIMEOUT) == 'abc'
+        await_redis_echo((link_b_msg,), redis_key=link_b_key)
+
     def test_chain_with_eb_replaced_with_chain_with_eb(
         self, manager, subtests
     ):
         if not manager.app.conf.result_backend.startswith('redis'):
             raise pytest.skip('Requires redis result backend.')
 
         redis_connection = get_redis_connection()
@@ -750,77 +807,257 @@
                        reason="Task is timeout instead of returning exception on rpc backend",
                        strict=False)
     def test_chain_child_replaced_with_chain_last(self, manager):
         orig_sig = chain(identity.s(42), replace_with_chain.s())
         res_obj = orig_sig.delay()
         assert res_obj.get(timeout=TIMEOUT) == 42
 
+    @pytest.mark.parametrize('redis_key', ['redis-group-ids'])
+    def test_chord_header_id_duplicated_on_rabbitmq_msg_duplication(self, manager, subtests, celery_session_app,
+                                                                    redis_key):
+        """
+        When a task that predates a chord in a chain was duplicated by Rabbitmq (for whatever reason),
+        the chord header id was not duplicated. This caused the chord header to have a different id.
+        This test ensures that the chord header's id preserves itself in face of such an edge case.
+        To validate the correct behavior is implemented, we collect the original and duplicated chord header ids
+        in redis, to ensure that they are the same.
+        """
 
-class test_result_set:
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
 
-    @flaky
-    def test_result_set(self, manager):
-        assert_ping(manager)
+        if manager.app.conf.broker_url.startswith('redis'):
+            raise pytest.xfail('Redis broker does not duplicate the task (t1)')
 
-        rs = ResultSet([add.delay(1, 1), add.delay(2, 2)])
-        assert rs.get(timeout=TIMEOUT) == [2, 4]
+        # Republish t1 to cause the chain to be executed twice
+        @before_task_publish.connect
+        def before_task_publish_handler(sender=None, body=None, exchange=None, routing_key=None, headers=None,
+                                        properties=None,
+                                        declare=None, retry_policy=None, **kwargs):
+            """ We want to republish t1 to ensure that the chain is executed twice """
+
+            metadata = {
+                'body': body,
+                'exchange': exchange,
+                'routing_key': routing_key,
+                'properties': properties,
+                'headers': headers,
+            }
+
+            with celery_session_app.producer_pool.acquire(block=True) as producer:
+                # Publish t1 to the message broker, just before it's going to be published which causes duplication
+                return producer.publish(
+                    metadata['body'],
+                    exchange=metadata['exchange'],
+                    routing_key=metadata['routing_key'],
+                    retry=None,
+                    retry_policy=retry_policy,
+                    serializer='json',
+                    delivery_mode=None,
+                    headers=headers,
+                    **kwargs
+                )
 
-    @flaky
-    def test_result_set_error(self, manager):
-        assert_ping(manager)
+        # Clean redis key
+        redis_connection = get_redis_connection()
+        if redis_connection.exists(redis_key):
+            redis_connection.delete(redis_key)
 
-        rs = ResultSet([raise_error.delay(), add.delay(1, 1)])
-        rs.get(timeout=TIMEOUT, propagate=False)
+        # Prepare tasks
+        t1, t2, t3, t4 = identity.s(42), redis_echo_group_id.s(), identity.s(), identity.s()
+        c = chain(t1, chord([t2, t3], t4))
 
-        assert rs.results[0].failed()
-        assert rs.results[1].successful()
+        # Delay chain
+        r1 = c.delay()
+        r1.get(timeout=TIMEOUT)
 
+        # Cleanup
+        before_task_publish.disconnect(before_task_publish_handler)
+
+        with subtests.test(msg='Compare group ids via redis list'):
+            await_redis_list_message_length(2, redis_key=redis_key, timeout=15)
+            compare_group_ids_in_redis(redis_key=redis_key)
+
+        # Cleanup
+        redis_connection = get_redis_connection()
+        redis_connection.delete(redis_key)
+
+    def test_chaining_upgraded_chords_pure_groups(self, manager, subtests):
+        """ This test is built to reproduce the github issue https://github.com/celery/celery/issues/5958
+
+        The issue describes a canvas where a chain of groups are executed multiple times instead of once.
+        This test is built to reproduce the issue and to verify that the issue is fixed.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
 
-class test_group:
-    def test_group_stamping(self, manager, subtests):
         if not manager.app.conf.result_backend.startswith('redis'):
             raise pytest.skip('Requires redis result backend.')
 
-        sig1 = add.s(1, 1000)
-        sig1_res = sig1.freeze()
-        g1 = group(sig1, add.s(1, 2000))
-        g1_res = g1.freeze()
-        res = g1.apply_async()
-        res.get(timeout=TIMEOUT)
+        redis_connection = get_redis_connection()
+        redis_key = 'echo_chamber'
 
-        with subtests.test("sig_1 is stamped", groups=[g1_res.id]):
-            assert sig1_res._get_task_meta()["groups"] == [g1_res.id]
+        c = chain(
+            # letting the chain upgrade the chord, reproduces the issue in _chord.__or__
+            group(
+                redis_echo.si('1', redis_key=redis_key),
+                redis_echo.si('2', redis_key=redis_key),
+                redis_echo.si('3', redis_key=redis_key),
+            ),
+            group(
+                redis_echo.si('4', redis_key=redis_key),
+                redis_echo.si('5', redis_key=redis_key),
+                redis_echo.si('6', redis_key=redis_key),
+            ),
+            group(
+                redis_echo.si('7', redis_key=redis_key),
+            ),
+            group(
+                redis_echo.si('8', redis_key=redis_key),
+            ),
+            redis_echo.si('9', redis_key=redis_key),
+            redis_echo.si('Done', redis_key='Done'),
+        )
+
+        with subtests.test(msg='Run the chain and wait for completion'):
+            redis_connection.delete(redis_key, 'Done')
+            c.delay().get(timeout=TIMEOUT)
+            await_redis_list_message_length(1, redis_key='Done', timeout=10)
+
+        with subtests.test(msg='All tasks are executed once'):
+            actual = [sig.decode('utf-8') for sig in redis_connection.lrange(redis_key, 0, -1)]
+            expected = [str(i) for i in range(1, 10)]
+            with subtests.test(msg='All tasks are executed once'):
+                assert sorted(actual) == sorted(expected)
+
+        # Cleanup
+        redis_connection.delete(redis_key, 'Done')
+
+    def test_chaining_upgraded_chords_starting_with_chord(self, manager, subtests):
+        """ This test is built to reproduce the github issue https://github.com/celery/celery/issues/5958
+
+        The issue describes a canvas where a chain of groups are executed multiple times instead of once.
+        This test is built to reproduce the issue and to verify that the issue is fixed.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
 
-    def test_nested_group_stamping(self, manager, subtests):
         if not manager.app.conf.result_backend.startswith('redis'):
             raise pytest.skip('Requires redis result backend.')
 
-        sig1 = add.s(2, 2)
-        sig2 = add.s(2)
+        redis_connection = get_redis_connection()
+        redis_key = 'echo_chamber'
+
+        c = chain(
+            # by manually upgrading the chord to a group, we can reproduce the issue in _chain.__or__
+            chord(group([redis_echo.si('1', redis_key=redis_key),
+                         redis_echo.si('2', redis_key=redis_key),
+                         redis_echo.si('3', redis_key=redis_key)]),
+                  group([redis_echo.si('4', redis_key=redis_key),
+                         redis_echo.si('5', redis_key=redis_key),
+                         redis_echo.si('6', redis_key=redis_key)])),
+            group(
+                redis_echo.si('7', redis_key=redis_key),
+            ),
+            group(
+                redis_echo.si('8', redis_key=redis_key),
+            ),
+            redis_echo.si('9', redis_key=redis_key),
+            redis_echo.si('Done', redis_key='Done'),
+        )
+
+        with subtests.test(msg='Run the chain and wait for completion'):
+            redis_connection.delete(redis_key, 'Done')
+            c.delay().get(timeout=TIMEOUT)
+            await_redis_list_message_length(1, redis_key='Done', timeout=10)
 
-        sig1_res = sig1.freeze()
-        sig2_res = sig2.freeze()
+        with subtests.test(msg='All tasks are executed once'):
+            actual = [sig.decode('utf-8') for sig in redis_connection.lrange(redis_key, 0, -1)]
+            expected = [str(i) for i in range(1, 10)]
+            with subtests.test(msg='All tasks are executed once'):
+                assert sorted(actual) == sorted(expected)
 
-        g2 = group(sig2, chain(add.s(4), add.s(2)))
+        # Cleanup
+        redis_connection.delete(redis_key, 'Done')
 
-        g2_res = g2.freeze()
+    def test_chaining_upgraded_chords_mixed_canvas(self, manager, subtests):
+        """ This test is built to reproduce the github issue https://github.com/celery/celery/issues/5958
 
-        g1 = group(sig1, chain(add.s(1, 1), g2))
+        The issue describes a canvas where a chain of groups are executed multiple times instead of once.
+        This test is built to reproduce the issue and to verify that the issue is fixed.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
 
-        g1_res = g1.freeze()
-        res = g1.apply_async()
-        res.get(timeout=TIMEOUT)
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
 
-        with subtests.test("sig1 is stamped", groups=[g1_res.id]):
-            assert sig1_res._get_task_meta()['groups'] == [g1_res.id]
-        with subtests.test("sig2 is stamped", groups=[g1_res.id, g2_res.id]):
-            assert sig2_res._get_task_meta()['groups'] == \
-                [g1_res.id, g2_res.id]
+        redis_connection = get_redis_connection()
+        redis_key = 'echo_chamber'
+
+        c = chain(
+            chord(group([redis_echo.si('1', redis_key=redis_key),
+                         redis_echo.si('2', redis_key=redis_key),
+                         redis_echo.si('3', redis_key=redis_key)]),
+                  group([redis_echo.si('4', redis_key=redis_key),
+                         redis_echo.si('5', redis_key=redis_key),
+                         redis_echo.si('6', redis_key=redis_key)])),
+            redis_echo.si('7', redis_key=redis_key),
+            group(
+                redis_echo.si('8', redis_key=redis_key),
+            ),
+            redis_echo.si('9', redis_key=redis_key),
+            redis_echo.si('Done', redis_key='Done'),
+        )
+
+        with subtests.test(msg='Run the chain and wait for completion'):
+            redis_connection.delete(redis_key, 'Done')
+            c.delay().get(timeout=TIMEOUT)
+            await_redis_list_message_length(1, redis_key='Done', timeout=10)
+
+        with subtests.test(msg='All tasks are executed once'):
+            actual = [sig.decode('utf-8') for sig in redis_connection.lrange(redis_key, 0, -1)]
+            expected = [str(i) for i in range(1, 10)]
+            with subtests.test(msg='All tasks are executed once'):
+                assert sorted(actual) == sorted(expected)
+
+        # Cleanup
+        redis_connection.delete(redis_key, 'Done')
+
+
+class test_result_set:
 
     @flaky
+    def test_result_set(self, manager):
+        assert_ping(manager)
+
+        rs = ResultSet([add.delay(1, 1), add.delay(2, 2)])
+        assert rs.get(timeout=TIMEOUT) == [2, 4]
+
+    @flaky
+    def test_result_set_error(self, manager):
+        assert_ping(manager)
+
+        rs = ResultSet([raise_error.delay(), add.delay(1, 1)])
+        rs.get(timeout=TIMEOUT, propagate=False)
+
+        assert rs.results[0].failed()
+        assert rs.results[1].successful()
+
+
+class test_group:
+    @flaky
     def test_ready_with_exception(self, manager):
         if not manager.app.conf.result_backend.startswith('redis'):
             raise pytest.skip('Requires redis result backend.')
 
         g = group([add.s(1, 2), raise_error.s()])
         result = g.apply_async()
         while not result.ready():
@@ -1254,51 +1491,14 @@
     ping_result = manager.inspect().ping()
     assert ping_result
     ping_val = list(ping_result.values())[0]
     assert ping_val == {"ok": "pong"}
 
 
 class test_chord:
-    def test_chord_stamping_two_levels(self, manager, subtests):
-        """
-        For a group within a chord, test that group stamps are stored in
-        the correct order.
-        """
-        try:
-            manager.app.backend.ensure_chords_allowed()
-        except NotImplementedError as e:
-            raise pytest.skip(e.args[0])
-
-        sig_1 = add.s(2, 2)
-        sig_2 = add.s(2)
-
-        sig_1_res = sig_1.freeze()
-        sig_2_res = sig_2.freeze()
-
-        g2 = group(
-            sig_2,
-            add.s(4),
-        )
-
-        g2_res = g2.freeze()
-
-        sig_sum = xsum.s()
-        sig_sum.freeze()
-
-        g1 = chord([sig_1, chain(add.s(4, 4), g2)], sig_sum)
-        g1.freeze()
-
-        res = g1.apply_async()
-        res.get(timeout=TIMEOUT)
-
-        with subtests.test("sig_1_res is stamped", groups=[g1.tasks.id]):
-            assert sig_1_res._get_task_meta()['groups'] == [g1.tasks.id]
-        with subtests.test("sig_2_res is stamped", groups=[g1.id]):
-            assert sig_2_res._get_task_meta()['groups'] == [g1.tasks.id, g2_res.id]
-
     @flaky
     def test_simple_chord_with_a_delay_in_group_save(self, manager, monkeypatch):
         try:
             manager.app.backend.ensure_chords_allowed()
         except NotImplementedError as e:
             raise pytest.skip(e.args[0])
 
@@ -2364,35 +2564,32 @@
                 res.get(timeout=TIMEOUT)
         with subtests.test(msg="Errback is called after body group fails"):
             # NOTE: Here we expect the errback to be called once per failing
             # task in the chord body since it is a group
             await_redis_count(fail_task_count, redis_key=redis_key)
         redis_connection.delete(redis_key)
 
-    @pytest.mark.parametrize(
-        "errback_task", [errback_old_style, errback_new_style, ],
-    )
-    def test_mutable_errback_called_by_chord_from_group_fail_multiple(
+    @pytest.mark.parametrize("errback_task", [errback_old_style, errback_new_style])
+    def test_mutable_errback_called_by_chord_from_group_fail_multiple_on_header_failure(
         self, errback_task, manager, subtests
     ):
         if not manager.app.conf.result_backend.startswith("redis"):
             raise pytest.skip("Requires redis result backend.")
         redis_connection = get_redis_connection()
 
         fail_task_count = 42
         # We have to use failing task signatures with unique task IDs to ensure
         # the chord can complete when they are used as part of its header!
         fail_sigs = tuple(
             fail.s() for _ in range(fail_task_count)
         )
-        fail_sig_ids = tuple(s.freeze().id for s in fail_sigs)
         errback = errback_task.s()
         # Include a mix of passing and failing tasks
         child_sig = group(
-            *(identity.si(42) for _ in range(24)),  # arbitrary task count
+            *(identity.si(42) for _ in range(8)),  # arbitrary task count
             *fail_sigs,
         )
 
         chord_sig = chord((child_sig,), identity.s())
         chord_sig.link_error(errback)
         expected_redis_key = chord_sig.body.freeze().id
         redis_connection.delete(expected_redis_key)
@@ -2402,14 +2599,36 @@
             with pytest.raises(ExpectedException):
                 res.get(timeout=TIMEOUT)
         with subtests.test(msg="Errback is called after header group fails"):
             # NOTE: Here we only expect the errback to be called once since it
             # is attached to the chord body which is a single task!
             await_redis_count(1, redis_key=expected_redis_key)
 
+    @pytest.mark.parametrize("errback_task", [errback_old_style, errback_new_style])
+    def test_mutable_errback_called_by_chord_from_group_fail_multiple_on_body_failure(
+        self, errback_task, manager, subtests
+    ):
+        if not manager.app.conf.result_backend.startswith("redis"):
+            raise pytest.skip("Requires redis result backend.")
+        redis_connection = get_redis_connection()
+
+        fail_task_count = 42
+        # We have to use failing task signatures with unique task IDs to ensure
+        # the chord can complete when they are used as part of its header!
+        fail_sigs = tuple(
+            fail.s() for _ in range(fail_task_count)
+        )
+        fail_sig_ids = tuple(s.freeze().id for s in fail_sigs)
+        errback = errback_task.s()
+        # Include a mix of passing and failing tasks
+        child_sig = group(
+            *(identity.si(42) for _ in range(8)),  # arbitrary task count
+            *fail_sigs,
+        )
+
         chord_sig = chord((identity.si(42),), child_sig)
         chord_sig.link_error(errback)
         for fail_sig_id in fail_sig_ids:
             redis_connection.delete(fail_sig_id)
         with subtests.test(msg="Error propagates from body group"):
             res = chord_sig.delay()
             sleep(1)
@@ -2530,14 +2749,212 @@
         orig_sig = chord(
             identity.s(42),
             chain(identity.s(), replace_with_chain.s(), ),
         )
         res_obj = orig_sig.delay()
         assert res_obj.get(timeout=TIMEOUT) == [42]
 
+    def test_enabling_flag_allow_error_cb_on_chord_header(self, manager, subtests):
+        """
+        Test that the flag allow_error_callback_on_chord_header works as
+        expected. To confirm this, we create a chord with a failing header
+        task, and check that the body does not execute when the header task fails.
+        This allows preventing the body from executing when the chord header fails
+        when the flag is turned on. In addition, we make sure the body error callback
+        is also executed when the header fails and the flag is turned on.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+        redis_connection = get_redis_connection()
+
+        manager.app.conf.task_allow_error_cb_on_chord_header = True
+
+        header_errback_msg = 'header errback called'
+        header_errback_key = 'echo_header_errback'
+        header_errback_sig = redis_echo.si(header_errback_msg, redis_key=header_errback_key)
+
+        body_errback_msg = 'body errback called'
+        body_errback_key = 'echo_body_errback'
+        body_errback_sig = redis_echo.si(body_errback_msg, redis_key=body_errback_key)
+
+        body_msg = 'chord body called'
+        body_key = 'echo_body'
+        body_sig = redis_echo.si(body_msg, redis_key=body_key)
+
+        headers = (
+            (fail.si(),),
+            (fail.si(), fail.si(), fail.si()),
+            (fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si()),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42), fail.si()),
+        )
+
+        # for some reason using parametrize breaks the test so we do it manually unfortunately
+        for header in headers:
+            chord_sig = chord(header, body_sig)
+            # link error to chord header ONLY
+            [header_task.link_error(header_errback_sig) for header_task in chord_sig.tasks]
+            # link error to chord body ONLY
+            chord_sig.body.link_error(body_errback_sig)
+            redis_connection.delete(header_errback_key, body_errback_key, body_key)
+
+            with subtests.test(msg='Error propagates from failure in header'):
+                res = chord_sig.delay()
+                with pytest.raises(ExpectedException):
+                    res.get(timeout=TIMEOUT)
+
+            with subtests.test(msg='Confirm the body was not executed'):
+                with pytest.raises(TimeoutError):
+                    # confirm the chord body was not called
+                    await_redis_echo((body_msg,), redis_key=body_key, timeout=10)
+                # Double check
+                assert not redis_connection.exists(body_key), 'Chord body was called when it should have not'
+
+            with subtests.test(msg='Confirm the errback was called for each failed header task + body'):
+                # confirm the errback was called for each task in the chord header
+                failed_header_tasks_count = len(list(filter(lambda f_sig: f_sig == fail.si(), header)))
+                expected_header_errbacks = tuple(header_errback_msg for _ in range(failed_header_tasks_count))
+                await_redis_echo(expected_header_errbacks, redis_key=header_errback_key)
+
+                # confirm the errback was called for the chord body
+                await_redis_echo((body_errback_msg,), redis_key=body_errback_key)
+
+            redis_connection.delete(header_errback_key, body_errback_key)
+
+    def test_disabling_flag_allow_error_cb_on_chord_header(self, manager, subtests):
+        """
+        Confirm that when allow_error_callback_on_chord_header is disabled, the default
+        behavior is kept.
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+        redis_connection = get_redis_connection()
+
+        manager.app.conf.task_allow_error_cb_on_chord_header = False
+
+        errback_msg = 'errback called'
+        errback_key = 'echo_errback'
+        errback_sig = redis_echo.si(errback_msg, redis_key=errback_key)
+
+        body_msg = 'chord body called'
+        body_key = 'echo_body'
+        body_sig = redis_echo.si(body_msg, redis_key=body_key)
+
+        headers = (
+            (fail.si(),),
+            (fail.si(), fail.si(), fail.si()),
+            (fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si()),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42), fail.si()),
+        )
+
+        # for some reason using parametrize breaks the test so we do it manually unfortunately
+        for header in headers:
+            chord_sig = chord(header, body_sig)
+            chord_sig.link_error(errback_sig)
+            redis_connection.delete(errback_key, body_key)
+
+            with subtests.test(msg='Error propagates from failure in header'):
+                res = chord_sig.delay()
+                with pytest.raises(ExpectedException):
+                    res.get(timeout=TIMEOUT)
+
+            with subtests.test(msg='Confirm the body was not executed'):
+                with pytest.raises(TimeoutError):
+                    # confirm the chord body was not called
+                    await_redis_echo((body_msg,), redis_key=body_key, timeout=10)
+                # Double check
+                assert not redis_connection.exists(body_key), 'Chord body was called when it should have not'
+
+            with subtests.test(msg='Confirm only one errback was called'):
+                await_redis_echo((errback_msg,), redis_key=errback_key, timeout=10)
+                with pytest.raises(TimeoutError):
+                    await_redis_echo((errback_msg,), redis_key=errback_key, timeout=10)
+
+            # Cleanup
+            redis_connection.delete(errback_key)
+
+    def test_flag_allow_error_cb_on_chord_header_on_upgraded_chord(self, manager, subtests):
+        """
+        Confirm that allow_error_callback_on_chord_header flag supports upgraded chords
+        """
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        if not manager.app.conf.result_backend.startswith('redis'):
+            raise pytest.skip('Requires redis result backend.')
+        redis_connection = get_redis_connection()
+
+        manager.app.conf.task_allow_error_cb_on_chord_header = True
+
+        errback_msg = 'errback called'
+        errback_key = 'echo_errback'
+        errback_sig = redis_echo.si(errback_msg, redis_key=errback_key)
+
+        body_msg = 'chord body called'
+        body_key = 'echo_body'
+        body_sig = redis_echo.si(body_msg, redis_key=body_key)
+
+        headers = (
+            # (fail.si(),),  <-- this is not supported because it's not a valid chord header (only one task)
+            (fail.si(), fail.si(), fail.si()),
+            (fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si()),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42)),
+            (fail.si(), identity.si(42), fail.si(), identity.si(42), fail.si()),
+        )
+
+        # for some reason using parametrize breaks the test so we do it manually unfortunately
+        for header in headers:
+            implicit_chord_sig = chain(group(list(header)), body_sig)
+            implicit_chord_sig.link_error(errback_sig)
+            redis_connection.delete(errback_key, body_key)
+
+            with subtests.test(msg='Error propagates from failure in header'):
+                res = implicit_chord_sig.delay()
+                with pytest.raises(ExpectedException):
+                    res.get(timeout=TIMEOUT)
+
+            with subtests.test(msg='Confirm the body was not executed'):
+                with pytest.raises(TimeoutError):
+                    # confirm the chord body was not called
+                    await_redis_echo((body_msg,), redis_key=body_key, timeout=10)
+                # Double check
+                assert not redis_connection.exists(body_key), 'Chord body was called when it should have not'
+
+            with subtests.test(msg='Confirm the errback was called for each failed header task + body'):
+                # confirm the errback was called for each task in the chord header
+                failed_header_tasks_count = len(list(filter(lambda f_sig: f_sig.name == fail.si().name, header)))
+                expected_errbacks_count = failed_header_tasks_count + 1  # +1 for the body
+                expected_errbacks = tuple(errback_msg for _ in range(expected_errbacks_count))
+                await_redis_echo(expected_errbacks, redis_key=errback_key)
+
+                # confirm there are not leftovers
+                assert not redis_connection.exists(errback_key)
+
+            # Cleanup
+            redis_connection.delete(errback_key)
+
 
 class test_signature_serialization:
     """
     Confirm nested signatures can be rebuilt after passing through a backend.
 
     These tests are expected to finish and return `None` or raise an exception
     in the error case. The exception indicates that some element of a nested
@@ -2628,7 +3045,360 @@
             raise pytest.skip(e.args[0])
 
         sig = chain(
             tasks.return_nested_signature_chord_chord.s(),
             tasks.rebuild_signature.s()
         )
         sig.delay().get(timeout=TIMEOUT)
+
+
+class test_stamping_mechanism:
+    def test_stamping_workflow(self, manager, subtests):
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        workflow = group(
+            add.s(1, 2) | add.s(3),
+            add.s(4, 5) | add.s(6),
+            identity.si(21),
+        ) | group(
+            xsum.s(),
+            xsum.s(),
+        )
+
+        @task_received.connect
+        def task_received_handler(request=None, **kwargs):
+            nonlocal assertion_result
+            link = None
+            if request._Request__payload[2]["callbacks"]:
+                link = signature(request._Request__payload[2]["callbacks"][0])
+            link_error = None
+            if request._Request__payload[2]["errbacks"]:
+                link_error = signature(request._Request__payload[2]["errbacks"][0])
+
+            assertion_result = all(
+                [
+                    assertion_result,
+                    [stamped_header in request.stamps for stamped_header in request.stamped_headers],
+                    [
+                        stamped_header in link.options
+                        for stamped_header in link.options["stamped_headers"]
+                        if link  # the link itself doensn't have a link
+                    ],
+                    [
+                        stamped_header in link_error.options
+                        for stamped_header in link_error.options["stamped_headers"]
+                        if link_error  # the link_error itself doensn't have a link
+                    ],
+                ]
+            )
+
+        @before_task_publish.connect
+        def before_task_publish_handler(
+            body=None,
+            headers=None,
+            **kwargs,
+        ):
+            nonlocal assertion_result
+
+            assertion_result = all(
+                [stamped_header in headers["stamps"] for stamped_header in headers["stamped_headers"]]
+            )
+
+        class CustomStampingVisitor(StampingVisitor):
+            def on_signature(self, sig, **headers) -> dict:
+                return {"on_signature": 42}
+
+        with subtests.test("Prepare canvas workflow and stamp it"):
+            link_sig = identity.si("link")
+            link_error_sig = identity.si("link_error")
+            canvas_workflow = workflow
+            canvas_workflow.link(link_sig)
+            canvas_workflow.link_error(link_error_sig)
+            canvas_workflow.stamp(visitor=CustomStampingVisitor())
+
+        with subtests.test("Check canvas was executed successfully"):
+            assertion_result = False
+            assert canvas_workflow.apply_async().get() == [42] * 2
+            assert assertion_result
+
+    def test_stamping_example_canvas(self, manager):
+        """Test the stamping example canvas from the examples directory"""
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        c = chain(
+            group(identity.s(i) for i in range(1, 4)) | xsum.s(),
+            chord(group(mul.s(10) for _ in range(1, 4)), xsum.s()),
+        )
+
+        res = c()
+        assert res.get(timeout=TIMEOUT) == 180
+
+    def test_stamp_value_type_defined_by_visitor(self, manager, subtests):
+        """Test that the visitor can define the type of the stamped value"""
+
+        @before_task_publish.connect
+        def before_task_publish_handler(
+            sender=None,
+            body=None,
+            exchange=None,
+            routing_key=None,
+            headers=None,
+            properties=None,
+            declare=None,
+            retry_policy=None,
+            **kwargs,
+        ):
+            nonlocal task_headers
+            task_headers = headers.copy()
+
+        with subtests.test(msg="Test stamping a single value"):
+
+            class CustomStampingVisitor(StampingVisitor):
+                def on_signature(self, sig, **headers) -> dict:
+                    return {"stamp": 42}
+
+            stamped_task = add.si(1, 1)
+            stamped_task.stamp(visitor=CustomStampingVisitor())
+            result = stamped_task.freeze()
+            task_headers = None
+            stamped_task.apply_async()
+            assert task_headers is not None
+            assert result.get() == 2
+            assert "stamps" in task_headers
+            assert "stamp" in task_headers["stamps"]
+            assert not isinstance(task_headers["stamps"]["stamp"], list)
+
+        with subtests.test(msg="Test stamping a list of values"):
+
+            class CustomStampingVisitor(StampingVisitor):
+                def on_signature(self, sig, **headers) -> dict:
+                    return {"stamp": [4, 2]}
+
+            stamped_task = add.si(1, 1)
+            stamped_task.stamp(visitor=CustomStampingVisitor())
+            result = stamped_task.freeze()
+            task_headers = None
+            stamped_task.apply_async()
+            assert task_headers is not None
+            assert result.get() == 2
+            assert "stamps" in task_headers
+            assert "stamp" in task_headers["stamps"]
+            assert isinstance(task_headers["stamps"]["stamp"], list)
+
+    def test_properties_not_affected_from_stamping(self, manager, subtests):
+        """Test that the task properties are not dirty with stamping visitor entries"""
+
+        @before_task_publish.connect
+        def before_task_publish_handler(
+            sender=None,
+            body=None,
+            exchange=None,
+            routing_key=None,
+            headers=None,
+            properties=None,
+            declare=None,
+            retry_policy=None,
+            **kwargs,
+        ):
+            nonlocal task_headers
+            nonlocal task_properties
+            task_headers = headers.copy()
+            task_properties = properties.copy()
+
+        class CustomStampingVisitor(StampingVisitor):
+            def on_signature(self, sig, **headers) -> dict:
+                return {"stamp": 42}
+
+        stamped_task = add.si(1, 1)
+        stamped_task.stamp(visitor=CustomStampingVisitor())
+        result = stamped_task.freeze()
+        task_headers = None
+        task_properties = None
+        stamped_task.apply_async()
+        assert task_properties is not None
+        assert result.get() == 2
+        assert "stamped_headers" in task_headers
+        stamped_headers = task_headers["stamped_headers"]
+
+        with subtests.test(msg="Test that the task properties are not dirty with stamping visitor entries"):
+            assert "stamped_headers" not in task_properties, "stamped_headers key should not be in task properties"
+            for stamp in stamped_headers:
+                assert stamp not in task_properties, f'The stamp "{stamp}" should not be in the task properties'
+
+    def test_task_received_has_access_to_stamps(self, manager):
+        """Make sure that the request has the stamps using the task_received signal"""
+
+        assertion_result = False
+
+        @task_received.connect
+        def task_received_handler(sender=None, request=None, signal=None, **kwargs):
+            nonlocal assertion_result
+            assertion_result = all([stamped_header in request.stamps for stamped_header in request.stamped_headers])
+
+        class CustomStampingVisitor(StampingVisitor):
+            def on_signature(self, sig, **headers) -> dict:
+                return {"stamp": 42}
+
+        stamped_task = add.si(1, 1)
+        stamped_task.stamp(visitor=CustomStampingVisitor())
+        stamped_task.apply_async().get()
+        assert assertion_result
+
+    def test_all_tasks_of_canvas_are_stamped(self, manager, subtests):
+        """Test that complex canvas are stamped correctly"""
+        try:
+            manager.app.backend.ensure_chords_allowed()
+        except NotImplementedError as e:
+            raise pytest.skip(e.args[0])
+
+        @task_received.connect
+        def task_received_handler(**kwargs):
+            request = kwargs["request"]
+            nonlocal assertion_result
+
+            assertion_result = all(
+                [
+                    assertion_result,
+                    all([stamped_header in request.stamps for stamped_header in request.stamped_headers]),
+                    request.stamps["stamp"] == 42,
+                ]
+            )
+
+        # Using a list because pytest.mark.parametrize does not play well
+        canvas = [
+            add.s(1, 1),
+            group(add.s(1, 1), add.s(2, 2)),
+            chain(add.s(1, 1), add.s(2, 2)),
+            chord([add.s(1, 1), add.s(2, 2)], xsum.s()),
+            chain(group(add.s(0, 0)), add.s(-1)),
+            add.s(1, 1) | add.s(10),
+            group(add.s(1, 1) | add.s(10), add.s(2, 2) | add.s(20)),
+            chain(add.s(1, 1) | add.s(10), add.s(2) | add.s(20)),
+            chord([add.s(1, 1) | add.s(10), add.s(2, 2) | add.s(20)], xsum.s()),
+            chain(
+                chain(add.s(1, 1) | add.s(10), add.s(2) | add.s(20)),
+                add.s(3) | add.s(30),
+            ),
+            chord(
+                group(
+                    chain(add.s(1, 1), add.s(2)),
+                    chord([add.s(3, 3), add.s(4, 4)], xsum.s()),
+                ),
+                xsum.s(),
+            ),
+        ]
+
+        for sig in canvas:
+            with subtests.test(msg="Assert all tasks are stamped"):
+
+                class CustomStampingVisitor(StampingVisitor):
+                    def on_signature(self, sig, **headers) -> dict:
+                        return {"stamp": 42}
+
+                stamped_task = sig
+                stamped_task.stamp(visitor=CustomStampingVisitor())
+                assertion_result = True
+                stamped_task.apply_async().get()
+                assert assertion_result
+
+    def test_replace_merge_stamps(self, manager):
+        """Test that replacing a task keeps the previous and new stamps"""
+
+        @task_received.connect
+        def task_received_handler(**kwargs):
+            request = kwargs["request"]
+            nonlocal assertion_result
+            expected_stamp_key = list(StampOnReplace.stamp.keys())[0]
+            expected_stamp_value = list(StampOnReplace.stamp.values())[0]
+
+            assertion_result = all(
+                [
+                    assertion_result,
+                    all([stamped_header in request.stamps for stamped_header in request.stamped_headers]),
+                    request.stamps["stamp"] == 42,
+                    request.stamps[expected_stamp_key] == expected_stamp_value
+                    if "replaced_with_me" in request.task_name
+                    else True,
+                ]
+            )
+
+        class CustomStampingVisitor(StampingVisitor):
+            def on_signature(self, sig, **headers) -> dict:
+                return {"stamp": 42}
+
+        stamped_task = replace_with_stamped_task.s()
+        stamped_task.stamp(visitor=CustomStampingVisitor())
+        assertion_result = False
+        stamped_task.delay()
+        assertion_result = True
+        sleep(1)
+        # stamped_task needs to be stamped with CustomStampingVisitor
+        # and the replaced task with both CustomStampingVisitor and StampOnReplace
+        assert assertion_result, "All of the tasks should have been stamped"
+
+    def test_linking_stamped_sig(self, manager):
+        """Test that linking a callback after stamping will stamp the callback correctly"""
+
+        assertion_result = False
+
+        @task_received.connect
+        def task_received_handler(sender=None, request=None, signal=None, **kwargs):
+            nonlocal assertion_result
+            link = request._Request__payload[2]["callbacks"][0]
+            assertion_result = all(
+                [stamped_header in link["options"] for stamped_header in link["options"]["stamped_headers"]]
+            )
+
+        class FixedMonitoringIdStampingVisitor(StampingVisitor):
+            def __init__(self, msg_id):
+                self.msg_id = msg_id
+
+            def on_signature(self, sig, **headers):
+                mtask_id = self.msg_id
+                return {"mtask_id": mtask_id}
+
+        link_sig = identity.si("link_sig")
+        stamped_pass_sig = identity.si("passing sig")
+        stamped_pass_sig.stamp(visitor=FixedMonitoringIdStampingVisitor(str(uuid.uuid4())))
+        stamped_pass_sig.link(link_sig)
+        stamped_pass_sig.stamp(visitor=FixedMonitoringIdStampingVisitor("1234"))
+        stamped_pass_sig.apply_async().get(timeout=2)
+        assert assertion_result
+
+    def test_err_linking_stamped_sig(self, manager):
+        """Test that linking an error after stamping will stamp the errlink correctly"""
+
+        assertion_result = False
+
+        @task_received.connect
+        def task_received_handler(sender=None, request=None, signal=None, **kwargs):
+            nonlocal assertion_result
+            link_error = request.errbacks[0]
+            assertion_result = all(
+                [
+                    stamped_header in link_error["options"]
+                    for stamped_header in link_error["options"]["stamped_headers"]
+                ]
+            )
+
+        class FixedMonitoringIdStampingVisitor(StampingVisitor):
+            def __init__(self, msg_id):
+                self.msg_id = msg_id
+
+            def on_signature(self, sig, **headers):
+                mtask_id = self.msg_id
+                return {"mtask_id": mtask_id}
+
+        link_error_sig = identity.si("link_error")
+        stamped_fail_sig = fail.si()
+        stamped_fail_sig.stamp(visitor=FixedMonitoringIdStampingVisitor(str(uuid.uuid4())))
+        stamped_fail_sig.link_error(link_error_sig)
+        with pytest.raises(ExpectedException):
+            stamped_fail_sig.stamp(visitor=FixedMonitoringIdStampingVisitor("1234"))
+            stamped_fail_sig.apply_async().get()
+        assert assertion_result
```

### Comparing `celery-5.3.0b1/t/integration/test_inspect.py` & `celery-5.3.0b2/t/integration/test_inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 @pytest.fixture()
 def inspect(manager):
     return manager.app.control.inspect()
 
 
 class test_Inspect:
-    """Integration tests fo app.control.inspect() API"""
+    """Integration tests to app.control.inspect() API"""
 
     @flaky
     def test_ping(self, inspect):
         """Tests pinging the worker"""
         ret = inspect.ping()
         assert len(ret) == 1
         assert ret[NODENAME] == {'ok': 'pong'}
```

### Comparing `celery-5.3.0b1/t/integration/test_security.py` & `celery-5.3.0b2/t/integration/test_security.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/integration/test_tasks.py` & `celery-5.3.0b2/t/unit/backends/test_cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,316 +1,284 @@
-from datetime import datetime, timedelta
-from time import perf_counter, sleep
+import sys
+import types
+from contextlib import contextmanager
+from unittest.mock import Mock, patch
 
 import pytest
+from kombu.utils.encoding import ensure_bytes, str_to_bytes
 
-import celery
-from celery import group
+from celery import signature, states, uuid
+from celery.backends.cache import CacheBackend, DummyClient, backends
+from celery.exceptions import ImproperlyConfigured
+from t.unit import conftest
 
-from .conftest import get_active_redis_channels
-from .tasks import (ClassBasedAutoRetryTask, ExpectedException, add, add_ignore_result, add_not_typed, fail,
-                    print_unicode, retry, retry_once, retry_once_headers, retry_once_priority, return_properties,
-                    sleeping)
-
-TIMEOUT = 10
-
-
-_flaky = pytest.mark.flaky(reruns=5, reruns_delay=2)
-_timeout = pytest.mark.timeout(timeout=300)
-
-
-def flaky(fn):
-    return _timeout(_flaky(fn))
-
-
-class test_class_based_tasks:
-
-    @flaky
-    def test_class_based_task_retried(self, celery_session_app,
-                                      celery_session_worker):
-        task = ClassBasedAutoRetryTask()
-        celery_session_app.register_task(task)
-        res = task.delay()
-        assert res.get(timeout=TIMEOUT) == 1
-
-
-def _producer(j):
-    """Single producer helper function"""
-    results = []
-    for i in range(20):
-        results.append([i + j, add.delay(i, j)])
-    for expected, result in results:
-        value = result.get(timeout=10)
-        assert value == expected
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        assert result.successful() is True
-    return j
-
-
-class test_tasks:
-
-    def test_simple_call(self):
-        """Tests direct simple call of task"""
-        assert add(1, 1) == 2
-        assert add(1, 1, z=1) == 3
-
-    @flaky
-    def test_basic_task(self, manager):
-        """Tests basic task call"""
-        results = []
-        # Tests calling task only with args
-        for i in range(10):
-            results.append([i + i, add.delay(i, i)])
-        for expected, result in results:
-            value = result.get(timeout=10)
-            assert value == expected
-            assert result.status == 'SUCCESS'
-            assert result.ready() is True
-            assert result.successful() is True
-
-        results = []
-        # Tests calling task with args and kwargs
-        for i in range(10):
-            results.append([3*i, add.delay(i, i, z=i)])
-        for expected, result in results:
-            value = result.get(timeout=10)
-            assert value == expected
-            assert result.status == 'SUCCESS'
-            assert result.ready() is True
-            assert result.successful() is True
-
-    @flaky
-    def test_multiprocess_producer(self, manager):
-        """Testing multiple processes calling tasks."""
-        from multiprocessing import Pool
-        pool = Pool(20)
-        ret = pool.map(_producer, range(120))
-        assert list(ret) == list(range(120))
-
-    @flaky
-    def test_multithread_producer(self, manager):
-        """Testing multiple threads calling tasks."""
-        from multiprocessing.pool import ThreadPool
-        pool = ThreadPool(20)
-        ret = pool.map(_producer, range(120))
-        assert list(ret) == list(range(120))
-
-    @flaky
-    def test_ignore_result(self, manager):
-        """Testing calling task with ignoring results."""
-        result = add.apply_async((1, 2), ignore_result=True)
-        assert result.get() is None
-        # We wait since it takes a bit of time for the result to be
-        # persisted in the result backend.
-        sleep(1)
-        assert result.result is None
-
-    @flaky
-    def test_timeout(self, manager):
-        """Testing timeout of getting results from tasks."""
-        result = sleeping.delay(10)
-        with pytest.raises(celery.exceptions.TimeoutError):
-            result.get(timeout=5)
-
-    @flaky
-    def test_expired(self, manager):
-        """Testing expiration of task."""
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            sleeping.delay(2)
-        # Execute task with expiration = 1 sec
-        result = add.apply_async((1, 1), expires=1)
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            result.get()
-        assert result.status == 'REVOKED'
-        assert result.ready() is True
-        assert result.failed() is False
-        assert result.successful() is False
-
-        # Fill the queue with tasks which took > 1 sec to process
-        for _ in range(4):
-            sleeping.delay(2)
-        # Execute task with expiration at now + 1 sec
-        result = add.apply_async((1, 1), expires=datetime.utcnow() + timedelta(seconds=1))
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            result.get()
-        assert result.status == 'REVOKED'
-        assert result.ready() is True
-        assert result.failed() is False
-        assert result.successful() is False
-
-    @flaky
-    def test_eta(self, manager):
-        """Tests tasks scheduled at some point in future."""
-        start = perf_counter()
-        # Schedule task to be executed in 3 seconds
-        result = add.apply_async((1, 1), countdown=3)
-        sleep(1)
-        assert result.status == 'PENDING'
-        assert result.ready() is False
-        assert result.get() == 2
-        end = perf_counter()
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-        start = perf_counter()
-        # Schedule task to be executed at time now + 3 seconds
-        result = add.apply_async((2, 2), eta=datetime.utcnow() + timedelta(seconds=3))
-        sleep(1)
-        assert result.status == 'PENDING'
-        assert result.ready() is False
-        assert result.get() == 4
-        end = perf_counter()
-        assert result.status == 'SUCCESS'
-        assert result.ready() is True
-        # Difference between calling the task and result must be bigger than 3 secs
-        assert (end - start) > 3
-
-    @flaky
-    def test_fail(self, manager):
-        """Tests that the failing task propagates back correct exception."""
-        result = fail.delay()
-        with pytest.raises(ExpectedException):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-        assert result.ready() is True
-        assert result.failed() is True
-        assert result.successful() is False
-
-    @flaky
-    def test_revoked(self, manager):
-        """Testing revoking of task"""
-        # Fill the queue with tasks to fill the queue
-        for _ in range(4):
-            sleeping.delay(2)
-        # Execute task and revoke it
-        result = add.apply_async((1, 1))
-        result.revoke()
-        with pytest.raises(celery.exceptions.TaskRevokedError):
-            result.get()
-        assert result.status == 'REVOKED'
-        assert result.ready() is True
-        assert result.failed() is False
-        assert result.successful() is False
-
-    @flaky
-    def test_wrong_arguments(self, manager):
-        """Tests that proper exceptions are raised when task is called with wrong arguments."""
-        with pytest.raises(TypeError):
-            add(5)
-
-        with pytest.raises(TypeError):
-            add(5, 5, wrong_arg=5)
-
-        with pytest.raises(TypeError):
-            add.delay(5)
-
-        with pytest.raises(TypeError):
-            add.delay(5, wrong_arg=5)
-
-        # Tasks with typing=False are not checked but execution should fail
-        result = add_not_typed.delay(5)
-        with pytest.raises(TypeError):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-
-        result = add_not_typed.delay(5, wrong_arg=5)
-        with pytest.raises(TypeError):
-            result.get(timeout=5)
-        assert result.status == 'FAILURE'
-
-    @pytest.mark.xfail(reason="Retry failed on rpc backend", strict=False)
-    def test_retry(self, manager):
-        """Tests retrying of task."""
-        # Tests when max. retries is reached
-        result = retry.delay()
-        for _ in range(5):
-            status = result.status
-            if status != 'PENDING':
-                break
-            sleep(1)
-        assert status == 'RETRY'
-        with pytest.raises(ExpectedException):
-            result.get()
-        assert result.status == 'FAILURE'
-
-        # Tests when task is retried but after returns correct result
-        result = retry.delay(return_value='bar')
-        for _ in range(5):
-            status = result.status
-            if status != 'PENDING':
-                break
-            sleep(1)
-        assert status == 'RETRY'
-        assert result.get() == 'bar'
-        assert result.status == 'SUCCESS'
-
-    @flaky
-    def test_task_accepted(self, manager, sleep=1):
-        r1 = sleeping.delay(sleep)
-        sleeping.delay(sleep)
-        manager.assert_accepted([r1.id])
-
-    @flaky
-    def test_task_retried_once(self, manager):
-        res = retry_once.delay()
-        assert res.get(timeout=TIMEOUT) == 1  # retried once
-
-    @flaky
-    def test_task_retried_once_with_expires(self, manager):
-        res = retry_once.delay(expires=60)
-        assert res.get(timeout=TIMEOUT) == 1  # retried once
-
-    @flaky
-    def test_task_retried_priority(self, manager):
-        res = retry_once_priority.apply_async(priority=7)
-        assert res.get(timeout=TIMEOUT) == 7  # retried once with priority 7
-
-    @flaky
-    def test_task_retried_headers(self, manager):
-        res = retry_once_headers.apply_async(headers={'x-test-header': 'test-value'})
-        headers = res.get(timeout=TIMEOUT)
-        assert headers is not None  # retried once with headers
-        assert 'x-test-header' in headers  # retry keeps custom headers
-
-    @flaky
-    def test_unicode_task(self, manager):
-        manager.join(
-            group(print_unicode.s() for _ in range(5))(),
-            timeout=TIMEOUT, propagate=True,
+
+class SomeClass:
+
+    def __init__(self, data):
+        self.data = data
+
+
+class test_CacheBackend:
+
+    def setup_method(self):
+        self.app.conf.result_serializer = 'pickle'
+        self.tb = CacheBackend(backend='memory://', app=self.app)
+        self.tid = uuid()
+        self.old_get_best_memcached = backends['memcache']
+        backends['memcache'] = lambda: (DummyClient, ensure_bytes)
+
+    def teardown_method(self):
+        backends['memcache'] = self.old_get_best_memcached
+
+    def test_no_backend(self):
+        self.app.conf.cache_backend = None
+        with pytest.raises(ImproperlyConfigured):
+            CacheBackend(backend=None, app=self.app)
+
+    def test_memory_client_is_shared(self):
+        """This test verifies that memory:// backend state is shared over multiple threads"""
+        from threading import Thread
+        t = Thread(
+            target=lambda: CacheBackend(backend='memory://', app=self.app).set('test', 12345)
+        )
+        t.start()
+        t.join()
+        assert self.tb.client.get('test') == 12345
+
+    def test_mark_as_done(self):
+        assert self.tb.get_state(self.tid) == states.PENDING
+        assert self.tb.get_result(self.tid) is None
+
+        self.tb.mark_as_done(self.tid, 42)
+        assert self.tb.get_state(self.tid) == states.SUCCESS
+        assert self.tb.get_result(self.tid) == 42
+
+    def test_is_pickled(self):
+        result = {'foo': 'baz', 'bar': SomeClass(12345)}
+        self.tb.mark_as_done(self.tid, result)
+        # is serialized properly.
+        rindb = self.tb.get_result(self.tid)
+        assert rindb.get('foo') == 'baz'
+        assert rindb.get('bar').data == 12345
+
+    def test_mark_as_failure(self):
+        try:
+            raise KeyError('foo')
+        except KeyError as exception:
+            self.tb.mark_as_failure(self.tid, exception)
+            assert self.tb.get_state(self.tid) == states.FAILURE
+            assert isinstance(self.tb.get_result(self.tid), KeyError)
+
+    def test_apply_chord(self):
+        tb = CacheBackend(backend='memory://', app=self.app)
+        result_args = (
+            uuid(),
+            [self.app.AsyncResult(uuid()) for _ in range(3)],
         )
+        tb.apply_chord(result_args, None)
+        assert self.app.GroupResult.restore(result_args[0], backend=tb) == self.app.GroupResult(*result_args)
 
-    @flaky
-    def test_properties(self, celery_session_worker):
-        res = return_properties.apply_async(app_id="1234")
-        assert res.get(timeout=TIMEOUT)["app_id"] == "1234"
-
-
-class tests_task_redis_result_backend:
-    def setup(self, manager):
-        if not manager.app.conf.result_backend.startswith('redis'):
-            raise pytest.skip('Requires redis result backend.')
-
-    def test_ignoring_result_no_subscriptions(self):
-        assert get_active_redis_channels() == []
-        result = add_ignore_result.delay(1, 2)
-        assert result.ignored is True
-        assert get_active_redis_channels() == []
-
-    def test_asyncresult_forget_cancels_subscription(self):
-        result = add.delay(1, 2)
-        assert get_active_redis_channels() == [
-            f"celery-task-meta-{result.id}"
-        ]
-        result.forget()
-        assert get_active_redis_channels() == []
-
-    def test_asyncresult_get_cancels_subscription(self):
-        result = add.delay(1, 2)
-        assert get_active_redis_channels() == [
-            f"celery-task-meta-{result.id}"
-        ]
-        assert result.get(timeout=3) == 3
-        assert get_active_redis_channels() == []
+    @patch('celery.result.GroupResult.restore')
+    def test_on_chord_part_return(self, restore):
+        tb = CacheBackend(backend='memory://', app=self.app)
+
+        deps = Mock()
+        deps.__len__ = Mock()
+        deps.__len__.return_value = 2
+        restore.return_value = deps
+        task = Mock()
+        task.name = 'foobarbaz'
+        self.app.tasks['foobarbaz'] = task
+        task.request.chord = signature(task)
+
+        result_args = (
+            uuid(),
+            [self.app.AsyncResult(uuid()) for _ in range(3)],
+        )
+        task.request.group = result_args[0]
+        tb.apply_chord(result_args, None)
+
+        deps.join_native.assert_not_called()
+        tb.on_chord_part_return(task.request, 'SUCCESS', 10)
+        deps.join_native.assert_not_called()
+
+        tb.on_chord_part_return(task.request, 'SUCCESS', 10)
+        deps.join_native.assert_called_with(propagate=True, timeout=3.0)
+        deps.delete.assert_called_with()
+
+    def test_mget(self):
+        self.tb._set_with_state('foo', 1, states.SUCCESS)
+        self.tb._set_with_state('bar', 2, states.SUCCESS)
+
+        assert self.tb.mget(['foo', 'bar']) == {'foo': 1, 'bar': 2}
+
+    def test_forget(self):
+        self.tb.mark_as_done(self.tid, {'foo': 'bar'})
+        x = self.app.AsyncResult(self.tid, backend=self.tb)
+        x.forget()
+        assert x.result is None
+
+    def test_process_cleanup(self):
+        self.tb.process_cleanup()
+
+    def test_expires_as_int(self):
+        tb = CacheBackend(backend='memory://', expires=10, app=self.app)
+        assert tb.expires == 10
+
+    def test_unknown_backend_raises_ImproperlyConfigured(self):
+        with pytest.raises(ImproperlyConfigured):
+            CacheBackend(backend='unknown://', app=self.app)
+
+    def test_as_uri_no_servers(self):
+        assert self.tb.as_uri() == 'memory:///'
+
+    def test_as_uri_one_server(self):
+        backend = 'memcache://127.0.0.1:11211/'
+        b = CacheBackend(backend=backend, app=self.app)
+        assert b.as_uri() == backend
+
+    def test_as_uri_multiple_servers(self):
+        backend = 'memcache://127.0.0.1:11211;127.0.0.2:11211;127.0.0.3/'
+        b = CacheBackend(backend=backend, app=self.app)
+        assert b.as_uri() == backend
+
+    def test_regression_worker_startup_info(self):
+        pytest.importorskip('memcache')
+        self.app.conf.result_backend = (
+            'cache+memcached://127.0.0.1:11211;127.0.0.2:11211;127.0.0.3/'
+        )
+        worker = self.app.Worker()
+        with conftest.stdouts():
+            worker.on_start()
+            assert worker.startup_info()
+
+
+class MyMemcachedStringEncodingError(Exception):
+    pass
+
+
+class MemcachedClient(DummyClient):
+
+    def set(self, key, value, *args, **kwargs):
+        key_t, must_be, not_be, cod = bytes, 'string', 'bytes', 'decode'
+
+        if isinstance(key, key_t):
+            raise MyMemcachedStringEncodingError(
+                f'Keys must be {must_be}, not {not_be}.  Convert your '
+                f'strings using mystring.{cod}(charset)!')
+        return super().set(key, value, *args, **kwargs)
+
+
+class MockCacheMixin:
+
+    @contextmanager
+    def mock_memcache(self):
+        memcache = types.ModuleType('memcache')
+        memcache.Client = MemcachedClient
+        memcache.Client.__module__ = memcache.__name__
+        prev, sys.modules['memcache'] = sys.modules.get('memcache'), memcache
+        try:
+            yield True
+        finally:
+            if prev is not None:
+                sys.modules['memcache'] = prev
+
+    @contextmanager
+    def mock_pylibmc(self):
+        pylibmc = types.ModuleType('pylibmc')
+        pylibmc.Client = MemcachedClient
+        pylibmc.Client.__module__ = pylibmc.__name__
+        prev = sys.modules.get('pylibmc')
+        sys.modules['pylibmc'] = pylibmc
+        try:
+            yield True
+        finally:
+            if prev is not None:
+                sys.modules['pylibmc'] = prev
+
+
+class test_get_best_memcache(MockCacheMixin):
+
+    def test_pylibmc(self):
+        with self.mock_pylibmc():
+            with conftest.reset_modules('celery.backends.cache'):
+                from celery.backends import cache
+                cache._imp = [None]
+                assert cache.get_best_memcache()[0].__module__ == 'pylibmc'
+
+    @pytest.mark.masked_modules('pylibmc')
+    def test_memcache(self, mask_modules):
+        with self.mock_memcache():
+            with conftest.reset_modules('celery.backends.cache'):
+                from celery.backends import cache
+                cache._imp = [None]
+                assert (cache.get_best_memcache()[0]().__module__ ==
+                        'memcache')
+
+    @pytest.mark.masked_modules('pylibmc', 'memcache')
+    def test_no_implementations(self, mask_modules):
+        with conftest.reset_modules('celery.backends.cache'):
+            from celery.backends import cache
+            cache._imp = [None]
+            with pytest.raises(ImproperlyConfigured):
+                cache.get_best_memcache()
+
+    def test_cached(self):
+        with self.mock_pylibmc():
+            with conftest.reset_modules('celery.backends.cache'):
+                from celery.backends import cache
+                cache._imp = [None]
+                cache.get_best_memcache()[0](behaviors={'foo': 'bar'})
+                assert cache._imp[0]
+                cache.get_best_memcache()[0]()
+
+    def test_backends(self):
+        from celery.backends.cache import backends
+        with self.mock_memcache():
+            for name, fun in backends.items():
+                assert fun()
+
+
+class test_memcache_key(MockCacheMixin):
+
+    @pytest.mark.masked_modules('pylibmc')
+    def test_memcache_unicode_key(self, mask_modules):
+        with self.mock_memcache():
+            with conftest.reset_modules('celery.backends.cache'):
+                from celery.backends import cache
+                cache._imp = [None]
+                task_id, result = str(uuid()), 42
+                b = cache.CacheBackend(backend='memcache', app=self.app)
+                b.store_result(task_id, result, state=states.SUCCESS)
+                assert b.get_result(task_id) == result
+
+    @pytest.mark.masked_modules('pylibmc')
+    def test_memcache_bytes_key(self, mask_modules):
+        with self.mock_memcache():
+            with conftest.reset_modules('celery.backends.cache'):
+                from celery.backends import cache
+                cache._imp = [None]
+                task_id, result = str_to_bytes(uuid()), 42
+                b = cache.CacheBackend(backend='memcache', app=self.app)
+                b.store_result(task_id, result, state=states.SUCCESS)
+                assert b.get_result(task_id) == result
+
+    def test_pylibmc_unicode_key(self):
+        with conftest.reset_modules('celery.backends.cache'):
+            with self.mock_pylibmc():
+                from celery.backends import cache
+                cache._imp = [None]
+                task_id, result = str(uuid()), 42
+                b = cache.CacheBackend(backend='memcache', app=self.app)
+                b.store_result(task_id, result, state=states.SUCCESS)
+                assert b.get_result(task_id) == result
+
+    def test_pylibmc_bytes_key(self):
+        with conftest.reset_modules('celery.backends.cache'):
+            with self.mock_pylibmc():
+                from celery.backends import cache
+                cache._imp = [None]
+                task_id, result = str_to_bytes(uuid()), 42
+                b = cache.CacheBackend(backend='memcache', app=self.app)
+                b.store_result(task_id, result, state=states.SUCCESS)
+                assert b.get_result(task_id) == result
```

### Comparing `celery-5.3.0b1/t/integration/test_worker.py` & `celery-5.3.0b2/t/integration/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/app/test_amqp.py` & `celery-5.3.0b2/t/unit/app/test_amqp.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 
     def test_as_task_message_without_utc(self):
         self.app.amqp.utc = False
         self.app.amqp.as_task_v1(uuid(), 'foo', countdown=30, expires=40)
 
 
 class test_AMQP_Base:
-    def setup(self):
+    def setup_method(self):
         self.simple_message = self.app.amqp.as_task_v2(
             uuid(), 'foo', create_sent_event=True,
         )
         self.simple_message_no_sent_event = self.app.amqp.as_task_v2(
             uuid(), 'foo', create_sent_event=False,
         )
```

### Comparing `celery-5.3.0b1/t/unit/app/test_annotations.py` & `celery-5.3.0b2/t/unit/app/test_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class MyAnnotation:
     foo = 65
 
 
 class AnnotationCase:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
         self.add = add
 
         @self.app.task(shared=False)
         def mul(x, y):
```

### Comparing `celery-5.3.0b1/t/unit/app/test_app.py` & `celery-5.3.0b2/t/unit/app/test_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         # set there by that fixture.
         res = _state.orig_task_join_will_block()
         assert res is True
 
 
 class test_App:
 
-    def setup(self):
+    def setup_method(self):
         self.app.add_defaults(deepcopy(self.CELERY_TEST_CONFIG))
 
     def test_now(self):
         timezone_setting_value = 'US/Eastern'
         tz_utc = timezone.get_timezone('UTC')
         tz_us_eastern = timezone.get_timezone(timezone_setting_value)
 
@@ -738,15 +738,15 @@
     def test_get_active_apps(self):
         assert list(_state._get_active_apps())
 
         app1 = self.Celery()
         appid = id(app1)
         assert app1 in _state._get_active_apps()
         app1.close()
-        del(app1)
+        del (app1)
 
         gc.collect()
 
         # weakref removed from list when app goes out of scope.
         with pytest.raises(StopIteration):
             next(app for app in _state._get_active_apps() if id(app) == appid)
 
@@ -1019,23 +1019,23 @@
         oid1 = self.app.thread_oid
         oid2 = self.app.thread_oid
         uuid.UUID(oid1)
         uuid.UUID(oid2)
         assert oid1 == oid2
 
     def test_backend(self):
-        # Test that app.bakend returns the same backend in single thread
+        # Test that app.backend returns the same backend in single thread
         backend1 = self.app.backend
         backend2 = self.app.backend
         assert isinstance(backend1, Backend)
         assert isinstance(backend2, Backend)
         assert backend1 is backend2
 
     def test_thread_backend(self):
-        # Test that app.bakend returns the new backend for each thread
+        # Test that app.backend returns the new backend for each thread
         main_backend = self.app.backend
         from concurrent.futures import ThreadPoolExecutor
         with ThreadPoolExecutor(max_workers=1) as executor:
             future = executor.submit(lambda: self.app.backend)
         thread_backend = future.result()
         assert isinstance(main_backend, Backend)
         assert isinstance(thread_backend, Backend)
@@ -1048,14 +1048,29 @@
         from concurrent.futures import ThreadPoolExecutor
         with ThreadPoolExecutor(max_workers=1) as executor:
             future = executor.submit(lambda: self.app.thread_oid)
         thread_oid = future.result()
         uuid.UUID(thread_oid)
         assert main_oid != thread_oid
 
+    def test_thread_backend_thread_safe(self):
+        # Should share the backend object across threads
+        from concurrent.futures import ThreadPoolExecutor
+
+        with self.Celery() as app:
+            app.conf.update(result_backend_thread_safe=True)
+            main_backend = app.backend
+            with ThreadPoolExecutor(max_workers=1) as executor:
+                future = executor.submit(lambda: app.backend)
+
+            thread_backend = future.result()
+            assert isinstance(main_backend, Backend)
+            assert isinstance(thread_backend, Backend)
+            assert main_backend is thread_backend
+
 
 class test_defaults:
 
     def test_strtobool(self):
         for s in ('false', 'no', '0'):
             assert not defaults.strtobool(s)
         for s in ('true', 'yes', '1'):
```

### Comparing `celery-5.3.0b1/t/unit/app/test_backends.py` & `celery-5.3.0b2/t/unit/app/test_backends.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/app/test_beat.py` & `celery-5.3.0b2/t/unit/app/test_beat.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,24 +692,27 @@
                 minute='*/13', nowfun=now_func), 'task': 'non_missed'}
         }
         shelve['entries'] = {
             'first_missed': beat.ScheduleEntry(
                 'first_missed', 'first_missed',
                 last_run_at=now_func() - timedelta(minutes=2),
                 total_run_count=10,
+                app=self.app,
                 schedule=app_schedule['first_missed']['schedule']),
             'second_missed': beat.ScheduleEntry(
                 'second_missed', 'second_missed',
                 last_run_at=now_func() - timedelta(minutes=2),
                 total_run_count=10,
+                app=self.app,
                 schedule=app_schedule['second_missed']['schedule']),
             'non_missed': beat.ScheduleEntry(
                 'non_missed', 'non_missed',
                 last_run_at=now_func() - timedelta(minutes=2),
                 total_run_count=10,
+                app=self.app,
                 schedule=app_schedule['non_missed']['schedule']),
         }
 
         self.app.conf.beat_schedule = app_schedule
 
         scheduler = scheduler_class(self.app)
```

### Comparing `celery-5.3.0b1/t/unit/app/test_builtins.py` & `celery-5.3.0b2/t/unit/app/test_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from celery.app import builtins
 from celery.contrib.testing.mocks import ContextMock
 from celery.utils.functional import pass1
 
 
 class BuiltinsCase:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def xsum(x):
             return sum(x)
         self.xsum = xsum
 
         @self.app.task(shared=False)
         def add(x, y):
@@ -30,15 +30,15 @@
         cleanup_task = builtins.add_backend_cleanup_task(self.app)
         cleanup_task()
         self.app.backend.cleanup.assert_called()
 
 
 class test_accumulate(BuiltinsCase):
 
-    def setup(self):
+    def setup_method(self):
         self.accumulate = self.app.tasks['celery.accumulate']
 
     def test_with_index(self):
         assert self.accumulate(1, 2, 3, 4, index=0) == 1
 
     def test_no_index(self):
         assert self.accumulate(1, 2, 3, 4), (1, 2, 3 == 4)
@@ -85,24 +85,24 @@
             chunks_mul, [(2, 2), (4, 4), (8, 8)], 1,
         )
         apply_chunks.assert_called()
 
 
 class test_group(BuiltinsCase):
 
-    def setup(self):
+    def setup_method(self):
         self.maybe_signature = self.patching('celery.canvas.maybe_signature')
         self.maybe_signature.side_effect = pass1
         self.app.producer_or_acquire = Mock()
         self.app.producer_or_acquire.attach_mock(
             ContextMock(serializer='json'), 'return_value'
         )
         self.app.conf.task_always_eager = True
         self.task = builtins.add_group_task(self.app)
-        super().setup()
+        super().setup_method()
 
     def test_apply_async_eager(self):
         self.task.apply = Mock(name='apply')
         self.task.apply_async((1, 2, 3, 4, 5))
         self.task.apply.assert_called()
 
     def mock_group(self, *tasks):
@@ -128,28 +128,28 @@
         g, result = self.mock_group(self.add.s(2, 2), self.add.s(4, 4))
         self.task(g.tasks, result, result.id, None, add_to_parent=False)
         current_worker_task.add_trail.assert_not_called()
 
 
 class test_chain(BuiltinsCase):
 
-    def setup(self):
-        super().setup()
+    def setup_method(self):
+        super().setup_method()
         self.task = builtins.add_chain_task(self.app)
 
     def test_not_implemented(self):
         with pytest.raises(NotImplementedError):
             self.task()
 
 
 class test_chord(BuiltinsCase):
 
-    def setup(self):
+    def setup_method(self):
         self.task = builtins.add_chord_task(self.app)
-        super().setup()
+        super().setup_method()
 
     def test_apply_async(self):
         x = chord([self.add.s(i, i) for i in range(10)], body=self.xsum.s())
         r = x.apply_async()
         assert r
         assert r.parent
```

### Comparing `celery-5.3.0b1/t/unit/app/test_control.py` & `celery-5.3.0b2/t/unit/app/test_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             next(iter(reply[0]))) in str(w[0].message.args[0])
         assert 'foo@example.com' in nodes
         assert 'bar@example.com' in nodes
 
 
 class test_inspect:
 
-    def setup(self):
+    def setup_method(self):
         self.app.control.broadcast = Mock(name='broadcast')
         self.app.control.broadcast.return_value = {}
         self.inspect = self.app.control.inspect()
 
     def test_prepare_reply(self):
         reply = self.inspect._prepare([
             {'w1': {'ok': 1}},
@@ -203,15 +203,15 @@
     def test_report(self):
         self.inspect.report()
         self.assert_broadcast_called('report')
 
 
 class test_Control_broadcast:
 
-    def setup(self):
+    def setup_method(self):
         self.app.control.mailbox = Mock(name='mailbox')
 
     def test_broadcast(self):
         self.app.control.broadcast('foobarbaz', arguments={'foo': 2})
         self.app.control.mailbox.assert_called()
         self.app.control.mailbox()._broadcast.assert_called_with(
             'foobarbaz', {'foo': 2}, None, False, 1.0, None, None,
@@ -227,15 +227,15 @@
             'foobarbaz1', {}, [1, 2, 3], False, 1.0, None, None,
             channel=None,
         )
 
 
 class test_Control:
 
-    def setup(self):
+    def setup_method(self):
         self.app.control.broadcast = Mock(name='broadcast')
         self.app.control.broadcast.return_value = {}
 
         @self.app.task(shared=False)
         def mytask():
             pass
         self.mytask = mytask
@@ -420,14 +420,24 @@
             'revoke',
             destination=None,
             task_id='foozbaaz',
             signal=control.TERM_SIGNAME,
             terminate=False,
         )
 
+    def test_revoke_by_stamped_headers(self):
+        self.app.control.revoke_by_stamped_headers({'foo': 'bar'})
+        self.assert_control_called_with_args(
+            'revoke_by_stamped_headers',
+            destination=None,
+            headers={'foo': 'bar'},
+            signal=control.TERM_SIGNAME,
+            terminate=False,
+        )
+
     def test_revoke__with_options(self):
         self.app.control.revoke(
             'foozbaaz',
             destination='a@q.com',
             terminate=True,
             signal='KILL',
             limit=404,
@@ -437,14 +447,31 @@
             destination='a@q.com',
             task_id='foozbaaz',
             signal='KILL',
             terminate=True,
             _options={'limit': 404},
         )
 
+    def test_revoke_by_stamped_headers__with_options(self):
+        self.app.control.revoke_by_stamped_headers(
+            {'foo': 'bar'},
+            destination='a@q.com',
+            terminate=True,
+            signal='KILL',
+            limit=404,
+        )
+        self.assert_control_called_with_args(
+            'revoke_by_stamped_headers',
+            destination='a@q.com',
+            headers={'foo': 'bar'},
+            signal='KILL',
+            terminate=True,
+            _options={'limit': 404},
+        )
+
     def test_election(self):
         self.app.control.election('some_id', 'topic', 'action')
         self.assert_control_called_with_args(
             'election',
             destination=None,
             topic='topic',
             action='action',
@@ -495,14 +522,22 @@
         self.app.control.revoke = Mock(name='revoke')
         self.app.AsyncResult('foozbazzbar').revoke()
         self.app.control.revoke.assert_called_with(
             'foozbazzbar',
             connection=None, reply=False, signal=None,
             terminate=False, timeout=None)
 
+    def test_revoke_by_stamped_headers_from_result(self):
+        self.app.control.revoke_by_stamped_headers = Mock(name='revoke_by_stamped_headers')
+        self.app.AsyncResult('foozbazzbar').revoke_by_stamped_headers({'foo': 'bar'})
+        self.app.control.revoke_by_stamped_headers.assert_called_with(
+            {'foo': 'bar'},
+            connection=None, reply=False, signal=None,
+            terminate=False, timeout=None)
+
     def test_revoke_from_resultset(self):
         self.app.control.revoke = Mock(name='revoke')
         uuids = [uuid() for _ in range(10)]
         r = self.app.GroupResult(
             uuid(), [self.app.AsyncResult(x) for x in uuids])
         r.revoke()
         self.app.control.revoke.assert_called_with(
```

### Comparing `celery-5.3.0b1/t/unit/app/test_defaults.py` & `celery-5.3.0b2/t/unit/app/test_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 from celery.app.defaults import (_OLD_DEFAULTS, _OLD_SETTING_KEYS, _TO_NEW_KEY, _TO_OLD_KEY, DEFAULTS, NAMESPACES,
                                  SETTING_KEYS)
 
 
 class test_defaults:
 
-    def setup(self):
+    def setup_method(self):
         self._prev = sys.modules.pop('celery.app.defaults', None)
 
-    def teardown(self):
+    def teardown_method(self):
         if self._prev:
             sys.modules['celery.app.defaults'] = self._prev
 
     def test_option_repr(self):
         assert repr(NAMESPACES['broker']['url'])
 
     def test_any(self):
```

### Comparing `celery-5.3.0b1/t/unit/app/test_exceptions.py` & `celery-5.3.0b2/t/unit/app/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/app/test_loaders.py` & `celery-5.3.0b2/t/unit/app/test_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                        'to': 'y@x.com'}
     server_options = {'host': 'smtp.x.com',
                       'port': 1234,
                       'user': 'x',
                       'password': 'qwerty',
                       'timeout': 3}
 
-    def setup(self):
+    def setup_method(self):
         self.loader = DummyLoader(app=self.app)
 
     def test_handlers_pass(self):
         self.loader.on_task_init('foo.task', 'feedface-cafebabe')
         self.loader.on_worker_init()
 
     def test_now(self):
@@ -208,15 +208,15 @@
             assert not l.configured
             context_executed[0] = True
         assert context_executed[0]
 
 
 class test_AppLoader:
 
-    def setup(self):
+    def setup_method(self):
         self.loader = AppLoader(app=self.app)
 
     def test_on_worker_init(self):
         self.app.conf.imports = ('subprocess',)
         sys.modules.pop('subprocess', None)
         self.loader.init_worker()
         assert 'subprocess' in sys.modules
```

### Comparing `celery-5.3.0b1/t/unit/app/test_log.py` & `celery-5.3.0b2/t/unit/app/test_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 class test_default_logger:
 
     def setup_logger(self, *args, **kwargs):
         self.app.log.setup_logging_subsystem(*args, **kwargs)
 
         return logging.root
 
-    def setup(self):
+    def setup_method(self):
         self.get_logger = lambda n=None: get_logger(n) if n else logging.root
         signals.setup_logging.receivers[:] = []
         self.app.log.already_setup = False
 
     def test_get_logger_sets_parent(self):
         logger = get_logger('celery.test_get_logger')
         assert logger.parent.name == base_logger.name
@@ -308,29 +308,29 @@
             assert p.write('FOOFO') == 0
         finally:
             p._thread.recurse_protection = False
 
 
 class test_task_logger(test_default_logger):
 
-    def setup(self):
+    def setup_method(self):
         logger = self.logger = get_logger('celery.task')
         logger.handlers = []
         logging.root.manager.loggerDict.pop(logger.name, None)
         self.uid = uuid()
 
         @self.app.task(shared=False)
         def test_task():
             pass
         self.get_logger().handlers = []
         self.task = test_task
         from celery._state import _task_stack
         _task_stack.push(test_task)
 
-    def teardown(self):
+    def teardown_method(self):
         from celery._state import _task_stack
         _task_stack.pop()
 
     def setup_logger(self, *args, **kwargs):
         return self.app.log.setup_task_loggers(*args, **kwargs)
 
     def get_logger(self, *args, **kwargs):
```

### Comparing `celery-5.3.0b1/t/unit/app/test_registry.py` & `celery-5.3.0b2/t/unit/app/test_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         app.tasks['txfoo1'] = 'bar1'
         assert _unpickle_task_v2('txfoo1') == 'bar1'
         assert _unpickle_task_v2('txfoo1', module='celery') == 'bar1'
 
 
 class test_TaskRegistry:
 
-    def setup(self):
+    def setup_method(self):
         self.mytask = self.app.task(name='A', shared=False)(returns)
         self.missing_name_task = self.app.task(
             name=None, shared=False)(returns)
         self.missing_name_task.name = None  # name is overridden with path
         self.myperiodic = self.app.task(
             name='B', shared=False, type='periodic',
         )(returns)
```

### Comparing `celery-5.3.0b1/t/unit/app/test_routes.py` & `celery-5.3.0b2/t/unit/app/test_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def set_queues(app, **queues):
     app.conf.task_queues = queues
     app.amqp.queues = app.amqp.Queues(queues)
 
 
 class RouteCase:
 
-    def setup(self):
+    def setup_method(self):
         self.a_queue = {
             'exchange': 'fooexchange',
             'exchange_type': 'fanout',
             'routing_key': 'xuzzy',
         }
         self.b_queue = {
             'exchange': 'barexchange',
```

### Comparing `celery-5.3.0b1/t/unit/app/test_schedules.py` & `celery-5.3.0b2/t/unit/app/test_schedules.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         yield
     finally:
         cls.nowfun = prev_nowfun
 
 
 class test_solar:
 
-    def setup(self):
-        pytest.importorskip('ephem0')
+    def setup_method(self):
+        pytest.importorskip('ephem')
         self.s = solar('sunrise', 60, 30, app=self.app)
 
     def test_reduce(self):
         fun, args = self.s.__reduce__()
         assert fun(*args) == self.s
 
     def test_eq(self):
@@ -468,18 +468,38 @@
         now = tz.localize(datetime(2017, 3, 26, 7, 0))
         crontab.nowfun = lambda: now
         next = now + crontab.remaining_estimate(last_run_at)
 
         assert next.utcoffset().seconds == 7200
         assert next == tz.localize(datetime(2017, 3, 26, 9, 0))
 
+    def test_negative_utc_timezone_with_day_of_month(self):
+        # UTC-8
+        tzname = "America/Los_Angeles"
+        self.app.timezone = tzname
+        tz = pytz.timezone(tzname)
+
+        # set day_of_month to test on _delta_to_next
+        crontab = self.crontab(minute=0, day_of_month='27-31')
+
+        # last_run_at: '2023/01/28T23:00:00-08:00'
+        last_run_at = tz.localize(datetime(2023, 1, 28, 23, 0))
+
+        # now: '2023/01/29T00:00:00-08:00'
+        now = tz.localize(datetime(2023, 1, 29, 0, 0))
+
+        crontab.nowfun = lambda: now
+        next = now + crontab.remaining_estimate(last_run_at)
+
+        assert next == tz.localize(datetime(2023, 1, 29, 0, 0))
+
 
 class test_crontab_is_due:
 
-    def setup(self):
+    def setup_method(self):
         self.now = self.app.now()
         self.next_minute = 60 - self.now.second - 1e-6 * self.now.microsecond
         self.every_minute = self.crontab()
         self.quarterly = self.crontab(minute='*/15')
         self.hourly = self.crontab(minute=30)
         self.daily = self.crontab(hour=7, minute=30)
         self.weekly = self.crontab(hour=7, minute=30, day_of_week='thursday')
@@ -796,7 +816,159 @@
             assert remaining == 364 * 24 * 60 * 60
 
     def test_yearly_execution_is_not_due(self):
         with patch_crontab_nowfun(self.yearly, datetime(2010, 3, 7, 10, 30)):
             due, remaining = self.yearly.is_due(datetime(2009, 3, 12, 7, 30))
             assert not due
             assert remaining == 4 * 24 * 60 * 60 - 3 * 60 * 60
+
+    def test_execution_not_due_if_task_not_run_at_last_feasible_time_outside_deadline(
+            self):
+        """If the crontab schedule was added after the task was due, don't
+        immediately fire the task again"""
+        # could have feasibly been run on 12/5 at 7:30, but wasn't.
+        self.app.conf.beat_cron_starting_deadline = 3600
+        last_run = datetime(2022, 12, 4, 10, 30)
+        now = datetime(2022, 12, 5, 10, 30)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert not due
+
+    def test_execution_not_due_if_task_not_run_at_last_feasible_time_no_deadline_set(
+            self):
+        """Same as above test except there's no deadline set, so it should be
+         due"""
+        last_run = datetime(2022, 12, 4, 10, 30)
+        now = datetime(2022, 12, 5, 10, 30)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert due
+
+    def test_execution_due_if_task_not_run_at_last_feasible_time_within_deadline(
+            self):
+        # Could have feasibly been run on 12/5 at 7:30, but wasn't. We are
+        # still within a 1 hour deadline from the
+        # last feasible run, so the task should still be due.
+        self.app.conf.beat_cron_starting_deadline = 3600
+        last_run = datetime(2022, 12, 4, 10, 30)
+        now = datetime(2022, 12, 5, 8, 0)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert due
+
+    def test_execution_due_if_task_not_run_at_any_feasible_time_within_deadline(
+            self):
+        # Could have feasibly been run on 12/4 at 7:30, or 12/5 at 7:30,
+        # but wasn't. We are still within a 1 hour
+        # deadline from the last feasible run (12/5), so the task should
+        # still be due.
+        self.app.conf.beat_cron_starting_deadline = 3600
+        last_run = datetime(2022, 12, 3, 10, 30)
+        now = datetime(2022, 12, 5, 8, 0)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert due
+
+    def test_execution_not_due_if_task_not_run_at_any_feasible_time_outside_deadline(
+            self):
+        """Verifies that remaining is still the time to the next
+        feasible run date even though the original feasible date
+        was passed over in favor of a newer one."""
+        # Could have feasibly been run on 12/4 or 12/5 at 7:30,
+        # but wasn't.
+        self.app.conf.beat_cron_starting_deadline = 3600
+        last_run = datetime(2022, 12, 3, 10, 30)
+        now = datetime(2022, 12, 5, 11, 0)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert not due
+
+    def test_execution_not_due_if_last_run_in_future(self):
+        # Should not run if the last_run hasn't happened yet.
+        last_run = datetime(2022, 12, 6, 7, 30)
+        now = datetime(2022, 12, 5, 10, 30)
+        expected_next_execution_time = datetime(2022, 12, 7, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert not due
+            assert remaining == expected_remaining
+
+    def test_execution_not_due_if_last_run_at_last_feasible_time(self):
+        # Last feasible time is 12/5 at 7:30
+        last_run = datetime(2022, 12, 5, 7, 30)
+        now = datetime(2022, 12, 5, 10, 30)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert not due
+
+    def test_execution_not_due_if_last_run_past_last_feasible_time(self):
+        # Last feasible time is 12/5 at 7:30
+        last_run = datetime(2022, 12, 5, 8, 30)
+        now = datetime(2022, 12, 5, 10, 30)
+        expected_next_execution_time = datetime(2022, 12, 6, 7, 30)
+        expected_remaining = (
+                    expected_next_execution_time - now).total_seconds()
+
+        # Run the daily (7:30) crontab with the current date
+        with patch_crontab_nowfun(self.daily, now):
+            due, remaining = self.daily.is_due(last_run)
+            assert remaining == expected_remaining
+            assert not due
+
+    def test_execution_due_for_negative_utc_timezone_with_day_of_month(self):
+        # UTC-8
+        tzname = "America/Los_Angeles"
+        self.app.timezone = tzname
+        tz = pytz.timezone(tzname)
+
+        # set day_of_month to test on _delta_to_next
+        crontab = self.crontab(minute=0, day_of_month='27-31')
+
+        # last_run_at: '2023/01/28T23:00:00-08:00'
+        last_run_at = tz.localize(datetime(2023, 1, 28, 23, 0))
+
+        # now: '2023/01/29T00:00:00-08:00'
+        now = tz.localize(datetime(2023, 1, 29, 0, 0))
+
+        with patch_crontab_nowfun(crontab, now):
+            due, remaining = crontab.is_due(last_run_at)
+            assert (due, remaining) == (True, 3600)
```

### Comparing `celery-5.3.0b1/t/unit/app/test_utils.py` & `celery-5.3.0b2/t/unit/app/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/apps/test_multi.py` & `celery-5.3.0b2/t/unit/apps/test_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         p.options = {'x': 'y'}
         r = p.optmerge('foo')
         assert r['x'] == 'y'
 
 
 class test_Node:
 
-    def setup(self):
+    def setup_method(self):
         self.p = Mock(name='p')
         self.p.options = {
             '--executable': 'python',
             '--logfile': '/var/log/celery/foo.log',
         }
         self.p.namespaces = {}
         with patch('celery.apps.multi.os.mkdir'):
@@ -304,15 +304,15 @@
 
         mock_exists.assert_any_call('/var/run/demo/celery')
         mock_dirs.assert_any_call('/var/run/demo/celery')
 
 
 class test_Cluster:
 
-    def setup(self):
+    def setup_method(self):
         self.Popen = self.patching('celery.apps.multi.Popen')
         self.kill = self.patching('os.kill')
         self.gethostname = self.patching('celery.apps.multi.gethostname')
         self.gethostname.return_value = 'example.com'
         self.Pidfile = self.patching('celery.apps.multi.Pidfile')
         with patch('celery.apps.multi.os.mkdir'):
             self.cluster = Cluster(
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_arangodb.py` & `celery-5.3.0b2/t/unit/backends/test_arangodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     pyArango = None
 
 pytest.importorskip('pyArango')
 
 
 class test_ArangoDbBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.backend = ArangoDbBackend(app=self.app)
 
     def test_init_no_arangodb(self):
         prev, module.py_arango_connection = module.py_arango_connection, None
         try:
             with pytest.raises(ImproperlyConfigured):
                 ArangoDbBackend(app=self.app)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_asynchronous.py` & `celery-5.3.0b2/t/unit/backends/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/backends/test_azureblockblob.py` & `celery-5.3.0b2/t/unit/backends/test_azureblockblob.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 MODULE_TO_MOCK = "celery.backends.azureblockblob"
 
 pytest.importorskip('azure.storage.blob')
 pytest.importorskip('azure.core.exceptions')
 
 
 class test_AzureBlockBlobBackend:
-    def setup(self):
+    def setup_method(self):
         self.url = (
             "azureblockblob://"
             "DefaultEndpointsProtocol=protocol;"
             "AccountName=name;"
             "AccountKey=key;"
             "EndpointSuffix=suffix")
 
@@ -164,15 +164,15 @@
             app=self.app,
             url=self.url
         )
         assert backend.base_path == ''
 
 
 class test_as_uri:
-    def setup(self):
+    def setup_method(self):
         self.url = (
             "azureblockblob://"
             "DefaultEndpointsProtocol=protocol;"
             "AccountName=name;"
             "AccountKey=account_key;"
             "EndpointSuffix=suffix"
         )
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_base.py` & `celery-5.3.0b2/t/unit/backends/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import copy
 import re
 from contextlib import contextmanager
 from unittest.mock import ANY, MagicMock, Mock, call, patch, sentinel
 
 import pytest
 from kombu.serialization import prepare_accept_content
-from kombu.utils.encoding import ensure_bytes
+from kombu.utils.encoding import bytes_to_str, ensure_bytes
 
 import celery
 from celery import chord, group, signature, states, uuid
 from celery.app.task import Context, Task
 from celery.backends.base import BaseBackend, DisabledBackend, KeyValueStoreBackend, _nulldict
 from celery.exceptions import BackendGetMetaError, BackendStoreError, ChordError, SecurityError, TimeoutError
 from celery.result import result_from_tuple
@@ -64,15 +65,15 @@
     def test_create_exception_cls(self):
         assert serialization.create_exception_cls('FooError', 'm')
         assert serialization.create_exception_cls('FooError', 'm', KeyError)
 
 
 class test_Backend_interface:
 
-    def setup(self):
+    def setup_method(self):
         self.app.conf.accept_content = ['json']
 
     def test_accept_precedence(self):
 
         # default is app.conf.accept_content
         accept_content = self.app.conf.accept_content
         b1 = BaseBackend(self.app)
@@ -162,15 +163,15 @@
         assert meta['args'] == args
         assert meta['kwargs'] == kwargs
         assert meta['queue'] == 'celery'
 
 
 class test_BaseBackend_interface:
 
-    def setup(self):
+    def setup_method(self):
         self.b = BaseBackend(self.app)
 
         @self.app.task(shared=False)
         def callback(result):
             pass
 
         self.callback = callback
@@ -256,15 +257,15 @@
     def test_unpickleable(self):
         assert isinstance(fnpe(Unpickleable()), KeyError)
         assert fnpe(Impossible()) is None
 
 
 class test_prepare_exception:
 
-    def setup(self):
+    def setup_method(self):
         self.b = BaseBackend(self.app)
 
     def test_unpickleable(self):
         self.b.serializer = 'pickle'
         x = self.b.prepare_exception(Unpickleable(1, 2, 'foo'))
         assert isinstance(x, KeyError)
         y = self.b.exception_to_python(x)
@@ -354,15 +355,15 @@
 
     def _delete_group(self, group_id):
         self._data.pop(group_id, None)
 
 
 class test_BaseBackend_dict:
 
-    def setup(self):
+    def setup_method(self):
         self.b = DictBackend(app=self.app)
 
         @self.app.task(shared=False, bind=True)
         def bound_errback(self, result):
             pass
 
         @self.app.task(shared=False)
@@ -645,15 +646,15 @@
         assert b.get_children('id') is None
         b._get_task_meta_for.return_value = {'children': 3}
         assert b.get_children('id') == 3
 
 
 class test_KeyValueStoreBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.b = KVBackend(app=self.app)
 
     def test_on_chord_part_return(self):
         assert not self.b.implements_incr
         self.b.on_chord_part_return(None, None, None)
 
     def test_get_store_delete_result(self):
@@ -718,14 +719,30 @@
             self.b.get_key_for_group(None)
 
     def test_strip_prefix(self):
         x = self.b.get_key_for_task('x1b34')
         assert self.b._strip_prefix(x) == 'x1b34'
         assert self.b._strip_prefix('x1b34') == 'x1b34'
 
+    def test_global_keyprefix(self):
+        global_keyprefix = "test_global_keyprefix_"
+        app = copy.deepcopy(self.app)
+        app.conf.get('result_backend_transport_options', {}).update({"global_keyprefix": global_keyprefix})
+        b = KVBackend(app=app)
+        tid = uuid()
+        assert bytes_to_str(b.get_key_for_task(tid)) == f"{global_keyprefix}_celery-task-meta-{tid}"
+        assert bytes_to_str(b.get_key_for_group(tid)) == f"{global_keyprefix}_celery-taskset-meta-{tid}"
+        assert bytes_to_str(b.get_key_for_chord(tid)) == f"{global_keyprefix}_chord-unlock-{tid}"
+
+    def test_global_keyprefix_missing(self):
+        tid = uuid()
+        assert bytes_to_str(self.b.get_key_for_task(tid)) == f"celery-task-meta-{tid}"
+        assert bytes_to_str(self.b.get_key_for_group(tid)) == f"celery-taskset-meta-{tid}"
+        assert bytes_to_str(self.b.get_key_for_chord(tid)) == f"chord-unlock-{tid}"
+
     def test_get_many(self):
         for is_dict in True, False:
             self.b.mget_returns_dict = is_dict
             ids = {uuid(): i for i in range(10)}
             for id, i in ids.items():
                 self.b.mark_as_done(id, i)
             it = self.b.get_many(list(ids), interval=0.01)
@@ -1010,15 +1027,15 @@
             (self.add.s(2, 2) |
              group(self.add.s(2, 2),
                    self.add.s(5, 6)) | self.add.s()).delay()
 
 
 class test_as_uri:
 
-    def setup(self):
+    def setup_method(self):
         self.b = BaseBackend(
             app=self.app,
             url='sch://uuuu:pwpw@hostname.dom'
         )
 
     def test_as_uri_include_password(self):
         assert self.b.as_uri(True) == self.b.url
@@ -1198,7 +1215,19 @@
                 b.store_result(sentinel.task_id, 42, states.SUCCESS)
                 assert False
             except BackendStoreError:
                 assert b._sleep.call_count == 0
         finally:
             self.app.conf.result_backend_always_retry = prev
             self.app.conf.result_backend_max_retries = prev_max_retries
+
+    def test_result_backend_thread_safe(self):
+        # Should identify the backend as thread safe
+        self.app.conf.result_backend_thread_safe = True
+        b = BaseBackend(app=self.app)
+        assert b.thread_safe is True
+
+    def test_result_backend_not_thread_safe(self):
+        # Should identify the backend as not being thread safe
+        self.app.conf.result_backend_thread_safe = False
+        b = BaseBackend(app=self.app)
+        assert b.thread_safe is False
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_cassandra.py` & `celery-5.3.0b2/t/unit/backends/test_cassandra.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     'cassandra.cluster',
     'cassandra.query',
 ]
 
 
 class test_CassandraBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.app.conf.update(
             cassandra_servers=['example.com'],
             cassandra_keyspace='celery',
             cassandra_table='task_results',
         )
 
     @pytest.mark.patched_module(*CASSANDRA_MODULES)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_consul.py` & `celery-5.3.0b2/t/unit/backends/test_consul.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from celery.backends.consul import ConsulBackend
 
 pytest.importorskip('consul')
 
 
 class test_ConsulBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.backend = ConsulBackend(
             app=self.app, url='consul://localhost:800')
 
     def test_supports_autoexpire(self):
         assert self.backend.supports_autoexpire
 
     def test_consul_consistency(self):
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_cosmosdbsql.py` & `celery-5.3.0b2/t/unit/backends/test_cosmosdbsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 MODULE_TO_MOCK = "celery.backends.cosmosdbsql"
 
 pytest.importorskip('pydocumentdb')
 
 
 class test_DocumentDBBackend:
-    def setup(self):
+    def setup_method(self):
         self.url = "cosmosdbsql://:key@endpoint"
         self.backend = CosmosDBSQLBackend(app=self.app, url=self.url)
 
     def test_missing_third_party_sdk(self):
         pydocumentdb = cosmosdbsql.pydocumentdb
         try:
             cosmosdbsql.pydocumentdb = None
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_couchbase.py` & `celery-5.3.0b2/t/unit/backends/test_couchbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 COUCHBASE_BUCKET = 'celery_bucket'
 
 pytest.importorskip('couchbase')
 
 
 class test_CouchbaseBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.backend = CouchbaseBackend(app=self.app)
 
     def test_init_no_couchbase(self):
         prev, module.Cluster = module.Cluster, None
         try:
             with pytest.raises(ImproperlyConfigured):
                 CouchbaseBackend(app=self.app)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_couchdb.py` & `celery-5.3.0b2/t/unit/backends/test_couchdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 COUCHDB_CONTAINER = 'celery_container'
 
 pytest.importorskip('pycouchdb')
 
 
 class test_CouchBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.Server = self.patching('pycouchdb.Server')
         self.backend = CouchBackend(app=self.app)
 
     def test_init_no_pycouchdb(self):
         """test init no pycouchdb raises"""
         prev, module.pycouchdb = module.pycouchdb, None
         try:
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_database.py` & `celery-5.3.0b2/t/unit/backends/test_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         session.rollback.assert_called_with()
         session.close.assert_called_with()
 
 
 @skip.if_pypy
 class test_DatabaseBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.uri = 'sqlite:///test.db'
         self.app.conf.result_serializer = 'pickle'
 
     def test_retry_helper(self):
         from celery.backends.database import DatabaseError
 
         calls = [0]
@@ -215,15 +215,15 @@
 
     def test_TaskSet__repr__(self):
         assert 'foo', repr(TaskSet('foo' in None))
 
 
 @skip.if_pypy
 class test_DatabaseBackend_result_extended():
-    def setup(self):
+    def setup_method(self):
         self.uri = 'sqlite:///test.db'
         self.app.conf.result_serializer = 'pickle'
         self.app.conf.result_extended = True
 
     @pytest.mark.parametrize(
         'result_serializer, args, kwargs',
         [
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_dynamodb.py` & `celery-5.3.0b2/t/unit/backends/test_dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from celery.backends.dynamodb import DynamoDBBackend
 from celery.exceptions import ImproperlyConfigured
 
 pytest.importorskip('boto3')
 
 
 class test_DynamoDBBackend:
-    def setup(self):
+    def setup_method(self):
         self._static_timestamp = Decimal(1483425566.52)
         self.app.conf.result_backend = 'dynamodb://'
 
     @property
     def backend(self):
         """:rtype: DynamoDBBackend"""
         return self.app.backend
@@ -117,60 +117,56 @@
         )
         backend._get_client()
 
         mock_validate_ttl_methods.assert_called_once()
         mock_set_table_ttl.assert_called_once()
 
     def test_get_or_create_table_not_exists(self):
+        from botocore.exceptions import ClientError
+
         self.backend._client = MagicMock()
         mock_create_table = self.backend._client.create_table = MagicMock()
+        client_error = ClientError(
+            {
+                'Error': {
+                    'Code': 'ResourceNotFoundException'
+                }
+            },
+            'DescribeTable'
+        )
         mock_describe_table = self.backend._client.describe_table = \
             MagicMock()
-
-        mock_describe_table.return_value = {
-            'Table': {
-                'TableStatus': 'ACTIVE'
-            }
-        }
+        mock_describe_table.side_effect = client_error
+        self.backend._wait_for_table_status = MagicMock()
 
         self.backend._get_or_create_table()
+        mock_describe_table.assert_called_once_with(
+            TableName=self.backend.table_name
+        )
         mock_create_table.assert_called_once_with(
             **self.backend._get_table_schema()
         )
 
     def test_get_or_create_table_already_exists(self):
-        from botocore.exceptions import ClientError
-
         self.backend._client = MagicMock()
         mock_create_table = self.backend._client.create_table = MagicMock()
-        client_error = ClientError(
-            {
-                'Error': {
-                    'Code': 'ResourceInUseException',
-                    'Message': 'Table already exists: {}'.format(
-                        self.backend.table_name
-                    )
-                }
-            },
-            'CreateTable'
-        )
-        mock_create_table.side_effect = client_error
         mock_describe_table = self.backend._client.describe_table = \
             MagicMock()
 
         mock_describe_table.return_value = {
             'Table': {
                 'TableStatus': 'ACTIVE'
             }
         }
 
         self.backend._get_or_create_table()
         mock_describe_table.assert_called_once_with(
             TableName=self.backend.table_name
         )
+        mock_create_table.assert_not_called()
 
     def test_wait_for_table_status(self):
         self.backend._client = MagicMock()
         mock_describe_table = self.backend._client.describe_table = \
             MagicMock()
         mock_describe_table.side_effect = [
             {'Table': {
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_elasticsearch.py` & `celery-5.3.0b2/t/unit/backends/test_elasticsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 
 pytest.importorskip('elasticsearch')
 
 
 class test_ElasticsearchBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.backend = ElasticsearchBackend(app=self.app)
 
     def test_init_no_elasticsearch(self):
         prev, module.elasticsearch = module.elasticsearch, None
         try:
             with pytest.raises(ImproperlyConfigured):
                 ElasticsearchBackend(app=self.app)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_filesystem.py` & `celery-5.3.0b2/t/unit/backends/test_filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from celery.backends.filesystem import FilesystemBackend
 from celery.exceptions import ImproperlyConfigured
 
 
 @t.skip.if_win32
 class test_FilesystemBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.directory = tempfile.mkdtemp()
         self.url = 'file://' + self.directory
         self.path = self.directory.encode('ascii')
 
     def test_a_path_is_required(self):
         with pytest.raises(ImproperlyConfigured):
             FilesystemBackend(app=self.app)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_mongodb.py` & `celery-5.3.0b2/t/unit/backends/test_mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     )
     sanitized_default_url = 'mongodb://uuuu:**@hostname.dom/database'
     sanitized_replica_set_url = (
         'mongodb://uuuu:**@hostname.dom/,'
         'hostname.dom/database?replicaSet=rs'
     )
 
-    def setup(self):
+    def setup_method(self):
         self.patching('celery.backends.mongodb.MongoBackend.encode')
         self.patching('celery.backends.mongodb.MongoBackend.decode')
         self.patching('celery.backends.mongodb.Binary')
         self.backend = MongoBackend(app=self.app, url=self.default_url)
 
     def test_init_no_mongodb(self, patching):
         patching('celery.backends.mongodb.pymongo', None)
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_redis.py` & `celery-5.3.0b2/t/unit/backends/test_redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
             ]
             callback = ms.return_value = Signature('add')
             callback.id = 'id1'
             self.b.set_chord_size(group_id, size)
             callback.delay = Mock(name='callback.delay')
             yield tasks, request, callback
 
-    def setup(self):
+    def setup_method(self):
         self.Backend = self.get_backend()
         self.E_LOST = self.get_E_LOST()
         self.b = self.Backend(app=self.app)
 
 
 class test_RedisBackend(basetest_RedisBackend):
     @pytest.mark.usefixtures('depends_on_current_app')
@@ -1189,15 +1189,15 @@
 
         return _SentinelBackend
 
     def get_E_LOST(self):
         from celery.backends.redis import E_LOST
         return E_LOST
 
-    def setup(self):
+    def setup_method(self):
         self.Backend = self.get_backend()
         self.E_LOST = self.get_E_LOST()
         self.b = self.Backend(app=self.app)
 
     @pytest.mark.usefixtures('depends_on_current_app')
     def test_reduce(self):
         pytest.importorskip('redis')
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_rpc.py` & `celery-5.3.0b2/t/unit/backends/test_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         consumer = self.get_consumer()
         # drain_events shouldn't crash when called before start
         consumer.drain_events(0.001)
 
 
 class test_RPCBackend:
 
-    def setup(self):
+    def setup_method(self):
         self.b = RPCBackend(app=self.app)
 
     def test_oid(self):
         oid = self.b.oid
         oid2 = self.b.oid
         assert uuid.UUID(oid)
         assert oid == oid2
```

### Comparing `celery-5.3.0b1/t/unit/backends/test_s3.py` & `celery-5.3.0b2/t/unit/backends/test_s3.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/bin/test_beat.py` & `celery-5.3.0b2/t/unit/bin/test_beat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/bin/test_worker.py` & `celery-5.3.0b2/t/unit/bin/test_worker.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_concurrency.py` & `celery-5.3.0b2/t/unit/concurrency/test_concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         BasePool(10).on_stop()
 
     def test_interface_on_apply(self):
         BasePool(10).on_apply()
 
     def test_interface_info(self):
         assert BasePool(10).info == {
+            'implementation': 'celery.concurrency.base:BasePool',
             'max-concurrency': 10,
         }
 
     def test_interface_flush(self):
         assert BasePool(10).flush() is None
 
     def test_active(self):
@@ -162,24 +163,26 @@
     def test_no_concurrent_futures__returns_no_threads_pool_name(self):
         expected_pool_names = (
             'prefork',
             'eventlet',
             'gevent',
             'solo',
             'processes',
+            'custom',
         )
         with patch.dict(sys.modules, {'concurrent.futures': None}):
             importlib.reload(concurrency)
             assert concurrency.get_available_pool_names() == expected_pool_names
 
     def test_concurrent_futures__returns_threads_pool_name(self):
         expected_pool_names = (
             'prefork',
             'eventlet',
             'gevent',
             'solo',
             'processes',
             'threads',
+            'custom',
         )
         with patch.dict(sys.modules, {'concurrent.futures': Mock()}):
             importlib.reload(concurrency)
             assert concurrency.get_available_pool_names() == expected_pool_names
```

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_eventlet.py` & `celery-5.3.0b2/t/unit/concurrency/test_eventlet.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     'greenlet',
 )
 
 
 @t.skip.if_pypy
 class EventletCase:
 
-    def setup(self):
+    def setup_method(self):
         self.patching.modules(*eventlet_modules)
 
-    def teardown(self):
+    def teardown_method(self):
         for mod in [mod for mod in sys.modules
                     if mod.startswith('eventlet')]:
             try:
-                del(sys.modules[mod])
+                del (sys.modules[mod])
             except KeyError:
                 pass
 
 
 class test_aaa_eventlet_patch(EventletCase):
 
     def test_aaa_is_patched(self):
@@ -125,14 +125,15 @@
         assert x.limit == 8
         x._pool.resize.assert_called_with(8)
 
     def test_get_info(self):
         x = TaskPool(10)
         x._pool = Mock(name='_pool')
         assert x._get_info() == {
+            'implementation': 'celery.concurrency.eventlet:TaskPool',
             'max-concurrency': 10,
             'free-threads': x._pool.free(),
             'running-threads': x._pool.running(),
         }
 
     def test_terminate_job(self):
         func = Mock()
```

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_gevent.py` & `celery-5.3.0b2/t/unit/concurrency/test_gevent.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from celery import maybe_patch_concurrency
         maybe_patch_concurrency(['x', '-P', 'gevent'])
         patch_all.assert_called()
 
 
 class test_Timer:
 
-    def setup(self):
+    def setup_method(self):
         self.patching.modules(*gevent_modules)
         self.greenlet = self.patching('gevent.greenlet')
         self.GreenletExit = self.patching('gevent.greenlet.GreenletExit')
 
     def test_sched(self):
         self.greenlet.Greenlet = object
         x = Timer()
@@ -53,15 +53,15 @@
 
         g = x._Greenlet()
         g.cancel()
 
 
 class test_TaskPool:
 
-    def setup(self):
+    def setup_method(self):
         self.patching.modules(*gevent_modules)
         self.spawn_raw = self.patching('gevent.spawn_raw')
         self.Pool = self.patching('gevent.pool.Pool')
 
     def test_pool(self):
         x = TaskPool()
         x.on_start()
```

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_pool.py` & `celery-5.3.0b2/t/unit/concurrency/test_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         raise KeyError('FOO EXCEPTION')
     except KeyError:
         return ExceptionInfo()
 
 
 class test_TaskPool:
 
-    def setup(self):
+    def setup_method(self):
         from celery.concurrency.prefork import TaskPool
         self.TaskPool = TaskPool
 
     def test_attrs(self):
         p = self.TaskPool(2)
         assert p.limit == 2
         assert p._pool is None
```

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_prefork.py` & `celery-5.3.0b2/t/unit/concurrency/test_prefork.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 class ExeMockTaskPool(mp.TaskPool):
     Pool = BlockingPool = ExeMockPool
 
 
 @t.skip.if_win32
 class test_AsynPool:
 
-    def setup(self):
+    def setup_method(self):
         pytest.importorskip('multiprocessing')
 
     def test_gen_not_started(self):
 
         def gen():
             yield 1
             assert not asynpool.gen_not_started(g)
@@ -365,15 +365,15 @@
         pool.register_with_event_loop(hub)
         hub.on_tick.add.assert_called_once()
 
 
 @t.skip.if_win32
 class test_ResultHandler:
 
-    def setup(self):
+    def setup_method(self):
         pytest.importorskip('multiprocessing')
 
     def test_process_result(self):
         x = asynpool.ResultHandler(
             Mock(), Mock(), {}, Mock(),
             Mock(), Mock(), Mock(), Mock(),
             fileno_to_outq={},
```

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_solo.py` & `celery-5.3.0b2/t/unit/concurrency/test_solo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/concurrency/test_thread.py` & `celery-5.3.0b2/t/unit/concurrency/test_thread.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/conftest.py` & `celery-5.3.0b2/t/unit/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
         yield mods
     finally:
         for name in names:
             try:
                 sys.modules[name] = prev[name]
             except KeyError:
                 try:
-                    del(sys.modules[name])
+                    del (sys.modules[name])
                 except KeyError:
                     pass
 
 
 class _patching:
 
     def __init__(self, monkeypatch, request):
```

### Comparing `celery-5.3.0b1/t/unit/contrib/test_abortable.py` & `celery-5.3.0b2/t/unit/contrib/test_abortable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from celery.contrib.abortable import AbortableAsyncResult, AbortableTask
 
 
 class test_AbortableTask:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(base=AbortableTask, shared=False)
         def abortable():
             return True
         self.abortable = abortable
 
     def test_async_result_is_abortable(self):
         result = self.abortable.apply_async()
```

### Comparing `celery-5.3.0b1/t/unit/contrib/test_migrate.py` & `celery-5.3.0b2/t/unit/contrib/test_migrate.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/contrib/test_pytest.py` & `celery-5.3.0b2/t/unit/contrib/test_pytest.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/contrib/test_rdb.py` & `celery-5.3.0b2/t/unit/contrib/test_rdb.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/contrib/test_sphinx.py` & `celery-5.3.0b2/t/unit/contrib/test_sphinx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import pytest
 
 try:
-    from sphinx.application import Sphinx  # noqa: F401
+    from sphinx.application import Sphinx  # noqa
     from sphinx_testing import TestApp
     sphinx_installed = True
 except ImportError:
     sphinx_installed = False
 
 
 SRCDIR = os.path.join(os.path.dirname(__file__), 'proj')
```

### Comparing `celery-5.3.0b1/t/unit/contrib/test_worker.py` & `celery-5.3.0b2/t/unit/contrib/test_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 # this import adds a @shared_task, which uses connect_on_app_finalize
 # to install the celery.ping task that the test lib uses
-import celery.contrib.testing.tasks  # noqa: F401
+import celery.contrib.testing.tasks  # noqa
 from celery import Celery
 from celery.contrib.testing.worker import start_worker
 
 
 class test_worker:
-    def setup(self):
+    def setup_method(self):
         self.app = Celery('celerytest', backend='cache+memory://', broker='memory://',)
 
         @self.app.task
         def add(x, y):
             return x + y
 
         self.add = add
```

### Comparing `celery-5.3.0b1/t/unit/events/test_cursesmon.py` & `celery-5.3.0b2/t/unit/events/test_cursesmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     def getmaxyx(self):
         return self.y, self.x
 
 
 class test_CursesDisplay:
 
-    def setup(self):
+    def setup_method(self):
         from celery.events import cursesmon
         self.monitor = cursesmon.CursesMonitor(object(), app=self.app)
         self.win = MockWindow()
         self.monitor.win = self.win
 
     def test_format_row_with_default_widths(self):
         self.win.x, self.win.y = 91, 24
```

### Comparing `celery-5.3.0b1/t/unit/events/test_events.py` & `celery-5.3.0b2/t/unit/events/test_events.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/events/test_snapshot.py` & `celery-5.3.0b2/t/unit/events/test_snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 timer = MockTimer()
 
 
 class test_Polaroid:
 
-    def setup(self):
+    def setup_method(self):
         self.state = self.app.events.State()
 
     def test_constructor(self):
         x = Polaroid(self.state, app=self.app)
         assert x.app is self.app
         assert x.state is self.state
         assert x.freq
@@ -97,15 +97,15 @@
                 raise KeyboardInterrupt()
 
     class MockEvents(Events):
 
         def Receiver(self, *args, **kwargs):
             return test_evcam.MockReceiver()
 
-    def setup(self):
+    def setup_method(self):
         self.app.events = self.MockEvents()
         self.app.events.app = self.app
 
     def test_evcam(self, restore_logging):
         evcam(Polaroid, timer=timer, app=self.app)
         evcam(Polaroid, timer=timer, loglevel='CRITICAL', app=self.app)
         self.MockReceiver.raise_keyboard_interrupt = True
```

### Comparing `celery-5.3.0b1/t/unit/events/test_state.py` & `celery-5.3.0b2/t/unit/events/test_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             QTEV('started', tA, 'w1', name='tA', clock=offset + 3),
             QTEV('received', tC, 'w2', name='tC', clock=offset + 3),
             QTEV('started', tB, 'w2', name='tB', clock=offset + 5),
             QTEV('retried', tA, 'w1', name='tA', clock=offset + 7),
             QTEV('succeeded', tB, 'w2', name='tB', clock=offset + 9),
             QTEV('started', tC, 'w2', name='tC', clock=offset + 10),
             QTEV('received', tA, 'w3', name='tA', clock=offset + 13),
-            QTEV('succeded', tC, 'w2', name='tC', clock=offset + 12),
+            QTEV('succeeded', tC, 'w2', name='tC', clock=offset + 12),
             QTEV('started', tA, 'w3', name='tA', clock=offset + 14),
             QTEV('succeeded', tA, 'w3', name='TA', clock=offset + 16),
         ]
 
     def rewind_with_offset(self, offset, uids=None):
         self.offset = offset
         self.uids = self.setuids(uids or self.uids)
```

### Comparing `celery-5.3.0b1/t/unit/fixups/test_django.py` & `celery-5.3.0b2/t/unit/fixups/test_django.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,18 +259,28 @@
                                 'django.core.cache', 'django.conf',
                                 'django.db.utils')
     def test_validate_models(self, patching, module):
         f = self.Fixup(self.app)
         f.django_setup = Mock(name='django.setup')
         patching.modules('django.core.checks')
         from django.core.checks import run_checks
+
         f.validate_models()
         f.django_setup.assert_called_with()
         run_checks.assert_called_with()
 
+        # test --skip-checks flag
+        f.django_setup.reset_mock()
+        run_checks.reset_mock()
+
+        patching.setenv('CELERY_SKIP_CHECKS', True)
+        f.validate_models()
+        f.django_setup.assert_called_with()
+        run_checks.assert_not_called()
+
     def test_django_setup(self, patching):
         patching('celery.fixups.django.symbol_by_name')
         patching('celery.fixups.django.import_module')
         django, = patching.modules('django')
         f = self.Fixup(self.app)
         f.django_setup()
         django.setup.assert_called_with()
```

### Comparing `celery-5.3.0b1/t/unit/security/__init__.py` & `celery-5.3.0b2/t/unit/security/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -101,7 +101,37 @@
 /G/QJkk/QAQ5kE0Ng1jHQ5iuWF2beACGPNSHLE0P3HDNAn8FxD/bXZGMLXMTAlnQ
 EsGOaXzMvbxadIcq0UDEjX7qMQIDjbjVj8kKCL2N2V0Xuq0voW/yzePr3Y1/qMZm
 IkNh5kgfa4dm3qROgsPkSya+bF16vsWSfgS7ebUCAwEAATANBgkqhkiG9w0BAQUF
 AAOBgQBzaZ5vBkzksPhnWb2oobuy6Ne/LMEtdQ//qeVY4sKl2tOJUCSdWRen9fqP
 e+zYdEdkFCd8rp568Eiwkq/553uy4rlE927/AEqs/+KGYmAtibk/9vmi+/+iZXyS
 WWZybzzDZFncq1/N1C3Y/hrCBNDFO4TsnTLAhWtZ4c0vDAiacw==
 -----END CERTIFICATE-----"""
+
+CERT_ECDSA = """-----BEGIN CERTIFICATE-----
+MIIDTTCCATWgAwIBAgIBCTANBgkqhkiG9w0BAQsFADANMQswCQYDVQQGEwJGSTAe
+Fw0yMjA4MDQwOTA5MDlaFw0yNTA0MzAwOTA5MDlaMCMxCzAJBgNVBAYTAkZJMRQw
+EgYDVQQDDAtUZXN0IFNlcnZlcjBZMBMGByqGSM49AgEGCCqGSM49AwEHA0IABIZV
+GFM0uPbXehT55s2yq3Zd7tCvN6GMGpE2+KSZqTtDP5c7x23QvBYF6q/T8MLNWCSB
+TxaERpvt8XL+ksOZ8vSjbTBrMB0GA1UdDgQWBBRiY7qDBo7KAYJIn3qTMGAkPimO
+6TAyBgNVHSMEKzApoRGkDzANMQswCQYDVQQGEwJGSYIUN/TljutVzZQ8GAMSX8yl
+Fy9dO/8wCQYDVR0TBAIwADALBgNVHQ8EBAMCBaAwDQYJKoZIhvcNAQELBQADggIB
+AKADv8zZvq8TWtvEZSmf476u+sdxs1hROqqSSJ0M3ePJq2lJ+MGI60eeU/0AyDRt
+Q5XAjr2g9wGY3sbA9uYmsIc2kaF+urrUbeoGB1JstALoxviGuM0EzEf+wK5/EbyA
+DDMg9j7b51CBMb3FjkiUQgOjM/u5neYpFxF0awXm4khThdOKTFd0FLVX+mcaKPZ4
+dkLcM/0NL25896DBPN982ObHOVqQjtY3sunXVuyeky8rhKmDvpasYu9xRkzSJBp7
+sCPnY6nsCexVICbuI+Q9oNT98YjHipDHQU0U/k/MvK7K/UCY2esKAnxzcOqoMQhi
+UjsKddXQ29GUEA9Btn9QB1sp39cR75S8/mFN2f2k/LhNm8j6QeHB4MhZ5L2H68f3
+K2wjzQHMZUrKXf3UM00VbT8E9j0FQ7qjYa7ZnQScvhTqsak2e0um8tqcPyk4WD6l
+/gRrLpk8l4x/Qg6F16hdj1p5xOsCUcVDkhIdKf8q3ZXjU2OECYPCFVOwiDQ2ngTf
+Se/bcjxgYXBQ99rkEf0vxk47KqC2ZBJy5enUxqUeVbbqho46vJagMzJoAmzp7yFP
+c1g8aazOWLD2kUxcqkUn8nv2HqApfycddz2O7OJ5Hl8e4vf+nVliuauGzImo0fiK
+VOL9+/r5Kek0fATRWdL4xtbB7zlk+EuoP9T5ZoTYlf14
+-----END CERTIFICATE-----"""
+
+KEY_ECDSA = """-----BEGIN EC PARAMETERS-----
+BggqhkjOPQMBBw==
+-----END EC PARAMETERS-----
+-----BEGIN EC PRIVATE KEY-----
+MHcCAQEEIOj98rAhc4ToQkHby+Iegvhm3UBx+3TwpfNza+2Vn8d7oAoGCCqGSM49
+AwEHoUQDQgAEhlUYUzS49td6FPnmzbKrdl3u0K83oYwakTb4pJmpO0M/lzvHbdC8
+FgXqr9Pwws1YJIFPFoRGm+3xcv6Sw5ny9A==
+-----END EC PRIVATE KEY-----"""
```

### Comparing `celery-5.3.0b1/t/unit/security/test_certificate.py` & `celery-5.3.0b2/t/unit/security/test_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pytest
 
 from celery.exceptions import SecurityError
 from celery.security.certificate import Certificate, CertStore, FSCertStore
 from t.unit import conftest
 
-from . import CERT1, CERT2, KEY1
+from . import CERT1, CERT2, CERT_ECDSA, KEY1
 from .case import SecurityCase
 
 
 class test_Certificate(SecurityCase):
 
     def test_valid_certificate(self):
         Certificate(CERT1)
@@ -25,14 +25,16 @@
             Certificate('')
         with pytest.raises(SecurityError):
             Certificate('foo')
         with pytest.raises(SecurityError):
             Certificate(CERT1[:20] + CERT1[21:])
         with pytest.raises(SecurityError):
             Certificate(KEY1)
+        with pytest.raises(SecurityError):
+            Certificate(CERT_ECDSA)
 
     @pytest.mark.skip('TODO: cert expired')
     def test_has_expired(self):
         assert not Certificate(CERT1).has_expired()
 
     def test_has_expired_mock(self):
         x = Certificate(CERT1)
```

### Comparing `celery-5.3.0b1/t/unit/security/test_key.py` & `celery-5.3.0b2/t/unit/security/test_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from kombu.utils.encoding import ensure_bytes
 
 from celery.exceptions import SecurityError
 from celery.security.key import PrivateKey
 from celery.security.utils import get_digest_algorithm
 
-from . import CERT1, ENCKEY1, ENCKEY2, KEY1, KEY2, KEYPASSWORD
+from . import CERT1, ENCKEY1, ENCKEY2, KEY1, KEY2, KEY_ECDSA, KEYPASSWORD
 from .case import SecurityCase
 
 
 class test_PrivateKey(SecurityCase):
 
     def test_valid_private_key(self):
         PrivateKey(KEY1)
@@ -28,13 +28,18 @@
             PrivateKey(KEY1[:20] + KEY1[21:])
         with pytest.raises(SecurityError):
             PrivateKey(ENCKEY1, KEYPASSWORD+b"wrong")
         with pytest.raises(SecurityError):
             PrivateKey(ENCKEY2, KEYPASSWORD+b"wrong")
         with pytest.raises(SecurityError):
             PrivateKey(CERT1)
+        with pytest.raises(SecurityError):
+            PrivateKey(KEY_ECDSA)
 
     def test_sign(self):
         pkey = PrivateKey(KEY1)
         pkey.sign(ensure_bytes('test'), get_digest_algorithm())
         with pytest.raises(AttributeError):
             pkey.sign(ensure_bytes('test'), get_digest_algorithm('unknown'))
+
+        # pkey = PrivateKey(KEY_ECDSA)
+        # pkey.sign(ensure_bytes('test'), get_digest_algorithm())
```

### Comparing `celery-5.3.0b1/t/unit/security/test_security.py` & `celery-5.3.0b2/t/unit/security/test_security.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from . import CERT1, ENCKEY1, KEY1, KEYPASSWORD
 from .case import SecurityCase
 
 
 class test_security(SecurityCase):
 
-    def teardown(self):
+    def teardown_method(self):
         registry._disabled_content_types.clear()
         registry._set_default_serializer('json')
         try:
             registry.unregister('auth')
         except SerializerNotInstalled:
             pass
```

### Comparing `celery-5.3.0b1/t/unit/security/test_serialization.py` & `celery-5.3.0b2/t/unit/security/test_serialization.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/tasks/test_chord.py` & `celery-5.3.0b2/t/unit/tasks/test_chord.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class AnySignatureWithTask(Signature):
     def __eq__(self, other):
         return self.task == other.task
 
 
 class ChordCase:
 
-    def setup(self):
+    def setup_method(self):
 
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
         self.add = add
 
 
@@ -73,15 +73,15 @@
 
         class AlwaysReady(TSR):
             is_ready = True
             value = [2, 4, 8, 6]
 
         with self._chord_context(AlwaysReady) as (cb, retry, _):
             cb.type.apply_async.assert_called_with(
-                ([2, 4, 8, 6],), {}, task_id=cb.id, stamped_headers=['groups'], groups=[]
+                ([2, 4, 8, 6],), {}, task_id=cb.id,
             )
             # didn't retry
             assert not retry.call_count
 
     def test_deps_ready_fails(self):
         GroupResult = Mock(name='GroupResult')
         GroupResult.return_value.ready.side_effect = KeyError('foo')
@@ -230,16 +230,14 @@
             run.assert_called_once_with(
                 AnySignatureWithTask(g),
                 mul.s(),
                 (),
                 task_id=None,
                 kwargs={},
                 interval=10,
-                groups=[ch.tasks.id],
-                stamped_headers=['groups']
             )
 
     def test_unlock_with_chord_params_and_task_id(self):
         @self.app.task(shared=False)
         def mul(x, y):
             return x * y
 
@@ -254,16 +252,14 @@
             run.assert_called_once_with(
                 AnySignatureWithTask(g),
                 mul.s(),
                 (),
                 task_id=sentinel.task_id,
                 kwargs={},
                 interval=10,
-                groups=[ch.tasks.id],
-                stamped_headers=['groups']
             )
 
 
 class test_chord(ChordCase):
 
     def test_eager(self):
         from celery import chord
@@ -319,15 +315,15 @@
         # (#6810)
         assert x.kwargs['kwargs'] == {}
         assert pickle.loads(pickle.dumps(x)).kwargs == x.kwargs
 
 
 class test_add_to_chord:
 
-    def setup(self):
+    def setup_method(self):
 
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
         self.add = add
 
         @self.app.task(shared=False, bind=True)
```

### Comparing `celery-5.3.0b1/t/unit/tasks/test_context.py` & `celery-5.3.0b2/t/unit/tasks/test_context.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/tasks/test_result.py` & `celery-5.3.0b2/t/unit/tasks/test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     def remove_pending_result(self, *args, **kwargs):
         return True
 
 
 class test_AsyncResult:
 
-    def setup(self):
+    def setup_method(self):
         self.app.conf.result_cache_max = 100
         self.app.conf.result_serializer = 'pickle'
         self.app.conf.result_extended = True
         self.task1 = mock_task('task1', states.SUCCESS, 'the')
         self.task2 = mock_task('task2', states.SUCCESS, 'quick')
         self.task3 = mock_task('task3', states.FAILURE, KeyError('brown'))
         self.task4 = mock_task('task3', states.RETRY, KeyError('red'))
@@ -546,17 +546,17 @@
         x.add(self.app.AsyncResult(2))
         assert len(x) == 2
 
     @contextmanager
     def dummy_copy(self):
         with patch('celery.result.copy') as copy:
 
-            def passt(arg):
+            def pass_value(arg):
                 return arg
-            copy.side_effect = passt
+            copy.side_effect = pass_value
 
             yield
 
     def test_add_discard(self):
         x = self.app.ResultSet([])
         x.add(self.app.AsyncResult('1'))
         assert self.app.AsyncResult('1') in x.results
@@ -624,15 +624,15 @@
     def get_many(self, *args, **kwargs):
         return ((id, {'result': i, 'status': states.SUCCESS})
                 for i, id in enumerate(self.ids))
 
 
 class test_GroupResult:
 
-    def setup(self):
+    def setup_method(self):
         self.size = 10
         self.ts = self.app.GroupResult(
             uuid(), make_mock_group(self.app, self.size),
         )
 
     @pytest.mark.usefixtures('depends_on_current_app')
     def test_is_pickleable(self):
@@ -878,15 +878,15 @@
     def test_result(self, app):
         res = app.AsyncResult(uuid())
         assert res.result is None
 
 
 class test_failed_AsyncResult:
 
-    def setup(self):
+    def setup_method(self):
         self.size = 11
         self.app.conf.result_serializer = 'pickle'
         results = make_mock_group(self.app, 10)
         failed = mock_task('ts11', states.FAILURE, KeyError('Baz'))
         save_result(self.app, failed)
         failed_res = self.app.AsyncResult(failed['id'])
         self.ts = self.app.GroupResult(uuid(), results + [failed_res])
@@ -903,15 +903,15 @@
 
     def test_failed(self):
         assert self.ts.failed()
 
 
 class test_pending_Group:
 
-    def setup(self):
+    def setup_method(self):
         self.ts = self.app.GroupResult(
             uuid(), [self.app.AsyncResult(uuid()),
                      self.app.AsyncResult(uuid())])
 
     def test_completed_count(self):
         assert self.ts.completed_count() == 0
 
@@ -928,15 +928,15 @@
     def test_join_longer(self):
         with pytest.raises(TimeoutError):
             self.ts.join(timeout=1)
 
 
 class test_EagerResult:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def raising(x, y):
             raise KeyError(x, y)
         self.raising = raising
 
     def test_wait_raises(self):
         res = self.raising.apply(args=[3, 3])
```

### Comparing `celery-5.3.0b1/t/unit/tasks/test_states.py` & `celery-5.3.0b2/t/unit/tasks/test_states.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/tasks/test_tasks.py` & `celery-5.3.0b2/t/unit/tasks/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 import pytest
 from kombu import Queue
 from kombu.exceptions import EncodeError
 
 from celery import Task, group, uuid
 from celery.app.task import _reprtask
+from celery.canvas import StampingVisitor, signature
 from celery.contrib.testing.mocks import ContextMock
 from celery.exceptions import Ignore, ImproperlyConfigured, Retry
 from celery.result import AsyncResult, EagerResult
 from celery.utils.time import parse_iso8601
 
 try:
     from urllib.error import HTTPError
-except ImportError:  # pragma: no cover
+except ImportError:
     from urllib2 import HTTPError
 
 
 def return_True(*args, **kwargs):
     # Task run functions can't be closures/lambdas, as they're pickled.
     return True
 
@@ -55,15 +56,15 @@
     retry_backoff = True
     retry_backoff_max = 700
     retry_jitter = False
 
 
 class TasksCase:
 
-    def setup(self):
+    def setup_method(self):
         self.mytask = self.app.task(shared=False)(return_True)
 
         @self.app.task(bind=True, count=0, shared=False)
         def increment_counter(self, increment_by=1):
             self.count += increment_by or 1
             return self.count
 
@@ -1055,14 +1056,32 @@
         mytask.app.events.attach_mock(ContextMock(), 'default_dispatcher')
         mytask.request.id = 'fb'
         mytask.send_event('task-foo', id=3122)
         mytask.app.events.default_dispatcher().send.assert_called_with(
             'task-foo', uuid='fb', id=3122,
             retry=True, retry_policy=self.app.conf.task_publish_retry_policy)
 
+    @pytest.mark.usefixtures('depends_on_current_app')
+    def test_on_replace(self):
+        class CustomStampingVisitor(StampingVisitor):
+            def on_signature(self, sig, **headers) -> dict:
+                return {'header': 'value'}
+
+        class MyTask(Task):
+            def on_replace(self, sig):
+                sig.stamp(CustomStampingVisitor())
+                return super().on_replace(sig)
+
+        mytask = self.app.task(shared=False, base=MyTask)(return_True)
+
+        sig1 = signature('sig1')
+        with pytest.raises(Ignore):
+            mytask.replace(sig1)
+        assert sig1.options['header'] == 'value'
+
     def test_replace(self):
         sig1 = MagicMock(name='sig1')
         sig1.options = {}
         self.mytask.request.id = sentinel.request_id
         with pytest.raises(Ignore):
             self.mytask.replace(sig1)
         sig1.freeze.assert_called_once_with(self.mytask.request.id)
```

### Comparing `celery-5.3.0b1/t/unit/tasks/test_trace.py` & `celery-5.3.0b2/t/unit/tasks/test_trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ):
     t = build_tracer(task.name, task, eager=eager, propagate=propagate, app=app, **opts)
     ret = t(task_id, args, kwargs, request)
     return ret.retval, ret.info
 
 
 class TraceCase:
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
 
         self.add = add
 
         @self.app.task(shared=False, ignore_result=True)
@@ -358,18 +358,18 @@
     def test_callbacks__sigs(self, group_, maybe_signature):
         sig1 = Mock(name='sig')
         sig2 = Mock(name='sig2')
         sig3 = group([Mock(name='g1'), Mock(name='g2')], app=self.app)
         sig3.apply_async = Mock(name='gapply')
         request = {'callbacks': [sig1, sig3, sig2], 'root_id': 'root'}
 
-        def passt(s, *args, **kwargs):
+        def pass_value(s, *args, **kwargs):
             return s
 
-        maybe_signature.side_effect = passt
+        maybe_signature.side_effect = pass_value
         retval, _ = self.trace(self.add, (2, 2), {}, request=request)
         group_.assert_called_with((4,), parent_id='id-1', root_id='root', priority=None)
         sig3.apply_async.assert_called_with(
             (4,), parent_id='id-1', root_id='root', priority=None
         )
 
     @patch('celery.canvas.maybe_signature')
@@ -377,18 +377,18 @@
     def test_callbacks__only_groups(self, group_, maybe_signature):
         sig1 = group([Mock(name='g1'), Mock(name='g2')], app=self.app)
         sig2 = group([Mock(name='g3'), Mock(name='g4')], app=self.app)
         sig1.apply_async = Mock(name='gapply')
         sig2.apply_async = Mock(name='gapply')
         request = {'callbacks': [sig1, sig2], 'root_id': 'root'}
 
-        def passt(s, *args, **kwargs):
+        def pass_value(s, *args, **kwargs):
             return s
 
-        maybe_signature.side_effect = passt
+        maybe_signature.side_effect = pass_value
         retval, _ = self.trace(self.add, (2, 2), {}, request=request)
         sig1.apply_async.assert_called_with(
             (4,), parent_id='id-1', root_id='root', priority=None
         )
         sig2.apply_async.assert_called_with(
             (4,), parent_id='id-1', root_id='root', priority=None
         )
```

### Comparing `celery-5.3.0b1/t/unit/test_canvas.py` & `celery-5.3.0b2/t/unit/test_canvas.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_collections.py` & `celery-5.3.0b2/t/unit/utils/test_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         x['attr2'] = 2
         assert x['attr1'] == 1
         assert x['attr2'] == 2
 
 
 class test_ConfigurationView:
 
-    def setup(self):
+    def setup_method(self):
         self.view = ConfigurationView(
             {'changed_key': 1, 'both': 2},
             [
                 {'default_key': 1, 'both': 1},
             ],
         )
 
@@ -141,16 +141,16 @@
     def test_exception_info(self):
 
         try:
             raise LookupError('The quick brown fox jumps...')
         except Exception:
             einfo = ExceptionInfo()
             assert str(einfo) == einfo.traceback
-            assert isinstance(einfo.exception, LookupError)
-            assert einfo.exception.args == ('The quick brown fox jumps...',)
+            assert isinstance(einfo.exception.exc, LookupError)
+            assert einfo.exception.exc.args == ('The quick brown fox jumps...',)
             assert einfo.traceback
 
             assert repr(einfo)
 
 
 @t.skip.if_win32
 class test_LimitedSet:
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_debug.py` & `celery-5.3.0b2/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_deprecated.py` & `celery-5.3.0b2/t/unit/utils/test_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         warn.reset_mock()
         assert x.foo == 10
         warn.assert_called_with(
             stacklevel=3, deprecation='1.2', alternative=None,
             description='foo', removal=None,
         )
         warn.reset_mock()
-        del(x.foo)
+        del (x.foo)
         warn.assert_called_with(
             stacklevel=3, deprecation='1.2', alternative=None,
             description='foo', removal=None,
         )
         assert x._foo is None
 
     def test_deprecated_no_setter_or_deleter(self):
@@ -53,15 +53,15 @@
             def foo(self):
                 pass
         assert X.foo
         x = X()
         with pytest.raises(AttributeError):
             x.foo = 10
         with pytest.raises(AttributeError):
-            del(x.foo)
+            del (x.foo)
 
 
 class test_warn:
 
     @patch('warnings.warn')
     def test_warn_deprecated(self, warn):
         deprecated.warn('Foo')
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_dispatcher.py` & `celery-5.3.0b2/t/unit/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_functional.py` & `celery-5.3.0b2/t/unit/utils/test_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import collections
 
 import pytest
-import pytest_subtests  # noqa: F401
+import pytest_subtests  # noqa
 from kombu.utils.functional import lazy
 
 from celery.utils.functional import (DummyContext, first, firstmethod, fun_accepts_kwargs, fun_takes_argument,
                                      head_from_fun, is_numeric_value, lookahead, maybe_list, mlazy, padlist, regen,
                                      seq_concat_item, seq_concat_seq)
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_graph.py` & `celery-5.3.0b2/t/unit/utils/test_graph.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_imports.py` & `celery-5.3.0b2/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_local.py` & `celery-5.3.0b2/t/unit/utils/test_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+from importlib.util import find_spec
 from unittest.mock import Mock
 
 import pytest
 
 from celery.local import PromiseProxy, Proxy, maybe_evaluate, try_import
 
 
@@ -106,45 +108,45 @@
         assert x.a == 1
         assert x.b == 2
         assert x.c == 3
 
         setattr(x, 'a', 10)
         assert x.a == 10
 
-        del(x.a)
+        del (x.a)
         assert x.a == 1
 
     def test_dictproxy(self):
         v = {}
         x = Proxy(lambda: v)
         x['foo'] = 42
         assert x['foo'] == 42
         assert len(x) == 1
         assert 'foo' in x
-        del(x['foo'])
+        del (x['foo'])
         with pytest.raises(KeyError):
             x['foo']
         assert iter(x)
 
     def test_listproxy(self):
         v = []
         x = Proxy(lambda: v)
         x.append(1)
         x.extend([2, 3, 4])
         assert x[0] == 1
         assert x[:-1] == [1, 2, 3]
-        del(x[-1])
+        del (x[-1])
         assert x[:-1] == [1, 2]
         x[0] = 10
         assert x[0] == 10
         assert 10 in x
         assert len(x) == 3
         assert iter(x)
         x[0:2] = [1, 2]
-        del(x[0:2])
+        del (x[0:2])
         assert str(x)
 
     def test_complex_cast(self):
 
         class O:
 
             def __complex__(self):
@@ -335,7 +337,19 @@
         x = PromiseProxy(lambda: 30)
         assert not x.__evaluated__()
         assert maybe_evaluate(x) == 30
         assert maybe_evaluate(x) == 30
 
         assert maybe_evaluate(30) == 30
         assert x.__evaluated__()
+
+
+class test_celery_import:
+    def test_import_celery(self, monkeypatch):
+        monkeypatch.delitem(sys.modules, "celery", raising=False)
+        spec = find_spec("celery")
+        assert spec
+
+        import celery
+
+        assert celery.__spec__ == spec
+        assert find_spec("celery") == spec
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_pickle.py` & `celery-5.3.0b2/t/unit/utils/test_pickle.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_platforms.py` & `celery-5.3.0b2/t/unit/utils/test_platforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,33 +9,26 @@
 import pytest
 
 import t.skip
 from celery import _find_option_with_arg, platforms
 from celery.exceptions import SecurityError, SecurityWarning
 from celery.platforms import (ASSUMING_ROOT, ROOT_DISALLOWED, ROOT_DISCOURAGED, DaemonContext, LockFailed, Pidfile,
                               _setgroups_hack, check_privileges, close_open_fds, create_pidlock, detached,
-                              fd_by_path, get_fdmax, ignore_errno, initgroups, isatty, maybe_drop_privileges,
-                              parse_gid, parse_uid, set_mp_process_title, set_pdeathsig, set_process_title, setgid,
-                              setgroups, setuid, signals)
+                              fd_by_path, get_fdmax, ignore_errno, initgroups, maybe_drop_privileges, parse_gid,
+                              parse_uid, set_mp_process_title, set_pdeathsig, set_process_title, setgid, setgroups,
+                              setuid, signals)
 from celery.utils.text import WhateverIO
 from t.unit import conftest
 
 try:
     import resource
-except ImportError:  # pragma: no cover
+except ImportError:
     resource = None
 
 
-def test_isatty():
-    fh = Mock(name='fh')
-    assert isatty(fh) is fh.isatty()
-    fh.isatty.side_effect = AttributeError()
-    assert not isatty(fh)
-
-
 class test_find_option_with_arg:
 
     def test_long_opt(self):
         assert _find_option_with_arg(
             ['--foo=bar'], long_opts=['--foo']) == 'bar'
 
     def test_short_opt(self):
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_saferepr.py` & `celery-5.3.0b2/t/unit/utils/test_saferepr.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_serialization.py` & `celery-5.3.0b2/t/unit/utils/test_serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,18 +92,15 @@
 
     @pytest.mark.parametrize('s,b',
                              STRTOBOOL_DEFAULT_TABLE.items())
     def test_default_table(self, s, b):
         assert strtobool(s) == b
 
     def test_unknown_value(self):
-        with pytest.raises(TypeError,
-                           # todo replace below when dropping python 2.7
-                           # match="Cannot coerce 'foo' to type bool"):
-                           match=r"Cannot coerce u?'foo' to type bool"):
+        with pytest.raises(TypeError, match="Cannot coerce 'foo' to type bool"):
             strtobool('foo')
 
     def test_no_op(self):
         assert strtobool(1) == 1
 
     def test_custom_table(self):
         custom_table = {
```

### Comparing `celery-5.3.0b1/t/unit/utils/test_sysinfo.py` & `celery-5.3.0b2/t/unit/utils/test_sysinfo.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_term.py` & `celery-5.3.0b2/t/unit/utils/test_term.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_text.py` & `celery-5.3.0b2/t/unit/utils/test_text.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_threads.py` & `celery-5.3.0b2/t/unit/utils/test_threads.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_time.py` & `celery-5.3.0b2/t/unit/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_timer2.py` & `celery-5.3.0b2/t/unit/utils/test_timer2.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/utils/test_utils.py` & `celery-5.3.0b2/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/worker/test_autoscale.py` & `celery-5.3.0b2/t/unit/worker/test_autoscale.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         info = w.info(parent)
         assert 'autoscaler' in info
         assert parent.autoscaler_cls().info.called
 
 
 class test_Autoscaler:
 
-    def setup(self):
+    def setup_method(self):
         self.pool = MockPool(3)
 
     def test_stop(self):
 
         class Scaler(autoscale.Autoscaler):
             alive = True
             joined = False
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_bootsteps.py` & `celery-5.3.0b2/t/unit/worker/test_bootsteps.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 class test_Step:
 
     class Def(bootsteps.StartStopStep):
         name = 'test_Step.Def'
 
-    def setup(self):
+    def setup_method(self):
         self.steps = []
 
     def test_blueprint_name(self, bp='test_blueprint_name'):
 
         class X(bootsteps.Step):
             blueprint = bp
             name = 'X'
@@ -158,15 +158,15 @@
 
 
 class test_StartStopStep:
 
     class Def(bootsteps.StartStopStep):
         name = 'test_StartStopStep.Def'
 
-    def setup(self):
+    def setup_method(self):
         self.steps = []
 
     def test_start__stop(self):
         x = self.Def(self)
         x.create = Mock()
 
         # include creates the underlying object and sets
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_components.py` & `celery-5.3.0b2/t/unit/worker/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         w.use_eventloop = True
         Timer(w).create(w)
         assert not w.timer.queue
 
 
 class test_Hub:
 
-    def setup(self):
+    def setup_method(self):
         self.w = Mock(name='w')
         self.hub = Hub(self.w)
         self.w.hub = Mock(name='w.hub')
 
     @patch('celery.worker.components.set_event_loop')
     @patch('celery.worker.components.get_event_loop')
     def test_create(self, get_event_loop, set_event_loop):
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_consumer.py` & `celery-5.3.0b2/t/unit/worker/test_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import errno
 import socket
 from collections import deque
 from unittest.mock import MagicMock, Mock, call, patch
 
 import pytest
+from amqp import ChannelError
 from billiard.exceptions import RestartFreqExceeded
 
 from celery import bootsteps
 from celery.contrib.testing.mocks import ContextMock
 from celery.exceptions import WorkerShutdown, WorkerTerminate
 from celery.utils.collections import LimitedSet
 from celery.worker.consumer.agent import Agent
@@ -37,15 +38,15 @@
         consumer.connection = _amqp_connection()
         consumer.connection_errors = (socket.error, OSError,)
         consumer.conninfo = consumer.connection
         return consumer
 
 
 class test_Consumer(ConsumerTestCase):
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
         self.add = add
 
     def test_repr(self):
         assert repr(self.get_consumer())
@@ -65,20 +66,20 @@
         with patch('celery.worker.consumer.consumer._detect_environment') as d:
             d.return_value = 'gevent'
             self.app.conf.broker_connection_timeout = 33.33
             self.get_consumer()
             assert self.app.conf.broker_connection_timeout is None
 
     def test_limit_moved_to_pool(self):
-        with patch('celery.worker.consumer.consumer.task_reserved') as reserv:
+        with patch('celery.worker.consumer.consumer.task_reserved') as task_reserved:
             c = self.get_consumer()
             c.on_task_request = Mock(name='on_task_request')
             request = Mock(name='request')
             c._limit_move_to_pool(request)
-            reserv.assert_called_with(request)
+            task_reserved.assert_called_with(request)
             c.on_task_request.assert_called_with(request)
 
     def test_update_prefetch_count(self):
         c = self.get_consumer()
         c._update_qos_eventually = Mock(name='update_qos')
         c.initial_prefetch_count = None
         c.pool.num_processes = None
@@ -180,19 +181,19 @@
         request = Mock()
         bucket.pop = lambda: bucket.contents.popleft()
         bucket.can_consume.return_value = True
         bucket.contents = deque()
 
         with patch(
             'celery.worker.consumer.consumer.Consumer._limit_move_to_pool'
-        ) as reserv:
+        ) as task_reserved:
             bucket.contents.append((request, 3))
             c._schedule_bucket_request(bucket)
             bucket.can_consume.assert_called_with(3)
-            reserv.assert_called_with(request)
+            task_reserved.assert_called_with(request)
 
         bucket.can_consume.return_value = False
         bucket.contents = deque()
         bucket.expected_time.return_value = 3.33
         bucket.contents.append((request, 4))
         limit_order = c._limit_order
         c._schedule_bucket_request(bucket)
@@ -213,32 +214,32 @@
     def test_limit_task(self):
         c = self.get_consumer()
         bucket = Mock()
         request = Mock()
 
         with patch(
             'celery.worker.consumer.consumer.Consumer._schedule_bucket_request'
-        ) as reserv:
+        ) as task_reserved:
             c._limit_task(request, bucket, 1)
             bucket.add.assert_called_with((request, 1))
-            reserv.assert_called_with(bucket)
+            task_reserved.assert_called_with(bucket)
 
     def test_post_eta(self):
         c = self.get_consumer()
         c.qos = Mock()
         bucket = Mock()
         request = Mock()
 
         with patch(
             'celery.worker.consumer.consumer.Consumer._schedule_bucket_request'
-        ) as reserv:
+        ) as task_reserved:
             c._limit_post_eta(request, bucket, 1)
             c.qos.decrement_eventually.assert_called_with()
             bucket.add.assert_called_with((request, 1))
-            reserv.assert_called_with(bucket)
+            task_reserved.assert_called_with(bucket)
 
     def test_max_restarts_exceeded(self):
         c = self.get_consumer()
 
         def se(*args, **kwargs):
             c.blueprint.state = CLOSE
             raise RestartFreqExceeded()
@@ -306,14 +307,39 @@
 
         # stops test from running indefinitely in the while loop
         c.blueprint.restart.side_effect = self._closer(c)
 
         c.start()
         c.blueprint.restart.assert_called_once()
 
+    @pytest.mark.parametrize("broker_channel_error_retry", [True, False])
+    def test_blueprint_restart_for_channel_errors(self, broker_channel_error_retry):
+        c = self.get_consumer()
+
+        # ensure that WorkerShutdown is not raised
+        c.app.conf['broker_connection_retry'] = True
+        c.app.conf['broker_connection_retry_on_startup'] = True
+        c.app.conf['broker_channel_error_retry'] = broker_channel_error_retry
+        c.restart_count = -1
+
+        # ensure that blueprint state is not in stop conditions
+        c.blueprint.state = bootsteps.RUN
+        c.blueprint.start.side_effect = ChannelError()
+
+        # stops test from running indefinitely in the while loop
+        c.blueprint.restart.side_effect = self._closer(c)
+
+        # restarted only when broker_channel_error_retry is True
+        if broker_channel_error_retry:
+            c.start()
+            c.blueprint.restart.assert_called_once()
+        else:
+            with pytest.raises(ChannelError):
+                c.start()
+
     def test_collects_at_restart(self):
         c = self.get_consumer()
         c.connection.collect.side_effect = MemoryError()
         c.blueprint.start.side_effect = socket.error()
         c.blueprint.restart.side_effect = self._closer(c)
         c.start()
         c.connection.collect.assert_called_with()
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_control.py` & `celery-5.3.0b2/t/unit/worker/test_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from celery.utils.collections import AttributeDict
 from celery.utils.timer2 import Timer
 from celery.worker import WorkController as _WC
 from celery.worker import consumer, control
 from celery.worker import state as worker_state
 from celery.worker.pidbox import Pidbox, gPidbox
 from celery.worker.request import Request
-from celery.worker.state import REVOKE_EXPIRES, revoked
+from celery.worker.state import REVOKE_EXPIRES, revoked, revoked_headers
 
 hostname = socket.gethostname()
 
 
 class WorkController:
     autoscaler = None
 
@@ -112,15 +112,15 @@
         g.loop(parent)
 
         assert do_reset.call_count == 4
 
 
 class test_ControlPanel:
 
-    def setup(self):
+    def setup_method(self):
         self.panel = self.create_panel(consumer=Consumer(self.app))
 
         @self.app.task(name='c.unittest.mytask', rate_limit=200, shared=False)
         def mytask():
             pass
         self.mytask = mytask
 
@@ -540,14 +540,32 @@
             assert 'terminate:' in r['ok']
             # unknown task id only revokes
             r = control.revoke(state, uuid(), terminate=True)
             assert 'tasks unknown' in r['ok']
         finally:
             worker_state.task_ready(request)
 
+    def test_revoke_by_stamped_headers_terminate(self):
+        request = Mock()
+        request.id = uuid()
+        request.options = stamped_header = {'stamp': 'foo'}
+        request.options['stamped_headers'] = ['stamp']
+        state = self.create_state()
+        state.consumer = Mock()
+        worker_state.task_reserved(request)
+        try:
+            r = control.revoke_by_stamped_headers(state, stamped_header, terminate=True)
+            assert stamped_header == revoked_headers
+            assert 'terminate:' in r['ok']
+            # unknown task id only revokes
+            r = control.revoke_by_stamped_headers(state, stamped_header, terminate=True)
+            assert 'tasks unknown' in r['ok']
+        finally:
+            worker_state.task_ready(request)
+
     def test_autoscale(self):
         self.panel.state.consumer = Mock()
         self.panel.state.consumer.controller = Mock()
         sc = self.panel.state.consumer.controller.autoscaler = Mock()
         sc.update.return_value = 10, 2
         m = {'method': 'autoscale',
              'destination': hostname,
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_heartbeat.py` & `celery-5.3.0b2/t/unit/worker/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `celery-5.3.0b1/t/unit/worker/test_loops.py` & `celery-5.3.0b2/t/unit/worker/test_loops.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     x.blueprint.state = CLOSE
     asynloop(*x.args)
     return x, x.consumer.on_message
 
 
 class test_asynloop:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
         self.add = add
 
     def test_drain_after_consume(self):
         x, _ = get_task_callback(self.app, transport_driver_type='amqp')
@@ -525,15 +525,15 @@
         synloop(*x.args)
 
         x.obj.timer.call_repeatedly.assert_not_called()
 
 
 class test_quick_drain:
 
-    def setup(self):
+    def setup_method(self):
         self.connection = Mock(name='connection')
 
     def test_drain(self):
         _quick_drain(self.connection, timeout=33.3)
         self.connection.drain_events.assert_called_with(timeout=33.3)
 
     def test_drain_error(self):
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_request.py` & `celery-5.3.0b2/t/unit/worker/test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from celery.worker.request import Request, create_request_cls
 from celery.worker.request import logger as req_logger
 from celery.worker.state import revoked
 
 
 class RequestCase:
 
-    def setup(self):
+    def setup_method(self):
         self.app.conf.result_serializer = 'pickle'
 
         @self.app.task(shared=False)
         def add(x, y, **kw_):
             return x + y
 
         self.add = add
@@ -381,24 +381,24 @@
         req.delivery_info['redelivered'] = True
         req.task.backend = Mock()
 
         with self.assert_signal_called(
             task_failure,
             sender=req.task,
             task_id=req.id,
-            exception=einfo.exception,
+            exception=einfo.exception.exc,
             args=req.args,
             kwargs=req.kwargs,
             traceback=einfo.traceback,
             einfo=einfo
         ):
             req.on_failure(einfo)
 
         req.task.backend.mark_as_failure.assert_called_once_with(req.id,
-                                                                 einfo.exception,
+                                                                 einfo.exception.exc,
                                                                  request=req._context,
                                                                  store_result=True)
 
     def test_tzlocal_is_cached(self):
         req = self.get_request(self.add.s(2, 2))
         req._tzlocal = 'foo'
         assert req.tzlocal == 'foo'
@@ -803,15 +803,15 @@
         job.on_failure(exc_info)
         assert not job.eventer.send.called
 
     def test_from_message_invalid_kwargs(self):
         m = self.TaskMessage(self.mytask.name, args=(), kwargs='foo')
         req = Request(m, app=self.app)
         with pytest.raises(InvalidTaskError):
-            raise req.execute().exception
+            raise req.execute().exception.exc
 
     def test_on_hard_timeout_acks_late(self, patching):
         error = patching('celery.worker.request.error')
 
         job = self.xRequest()
         job.acknowledge = Mock(name='ack')
         job.task.acks_late = True
@@ -1169,19 +1169,19 @@
         group_index = 42
         job = self.xRequest(id=uuid(), group_index=group_index)
         assert job.group_index == group_index
 
 
 class test_create_request_class(RequestCase):
 
-    def setup(self):
+    def setup_method(self):
         self.task = Mock(name='task')
         self.pool = Mock(name='pool')
         self.eventer = Mock(name='eventer')
-        super().setup()
+        super().setup_method()
 
     def create_request_cls(self, **kwargs):
         return create_request_cls(
             Request, self.task, self.pool, 'foo', self.eventer, app=self.app,
             **kwargs
         )
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_state.py` & `celery-5.3.0b2/t/unit/worker/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 @pytest.fixture
 def reset_state():
     yield
     state.active_requests.clear()
     state.revoked.clear()
+    state.revoked_headers.clear()
     state.total_count.clear()
 
 
 class MockShelve(dict):
     filename = None
     in_sync = False
     closed = False
@@ -40,15 +41,15 @@
 
 class MyPersistent(state.Persistent):
     storage = MockShelve()
 
 
 class test_maybe_shutdown:
 
-    def teardown(self):
+    def teardown_method(self):
         state.should_stop = None
         state.should_terminate = None
 
     def test_should_stop(self):
         state.should_stop = True
         with pytest.raises(WorkerShutdown):
             state.maybe_shutdown()
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_strategy.py` & `celery-5.3.0b2/t/unit/worker/test_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from celery.worker.request import Request
 from celery.worker.strategy import default as default_strategy
 from celery.worker.strategy import hybrid_to_proto2, proto1_to_proto2
 
 
 class test_proto1_to_proto2:
 
-    def setup(self):
+    def setup_method(self):
         self.message = Mock(name='message')
         self.body = {
             'args': (1,),
             'kwargs': {'foo': 'baz'},
             'utc': False,
             'taskset': '123',
         }
@@ -54,15 +54,15 @@
         assert headers == dict(self.body, group='123')
         assert decoded
         assert not utc
 
 
 class test_default_strategy_proto2:
 
-    def setup(self):
+    def setup_method(self):
         @self.app.task(shared=False)
         def add(x, y):
             return x + y
 
         self.add = add
 
     def get_message_class(self):
@@ -297,15 +297,15 @@
             )
             task_message_handler(C.message, None, None, None, None)
             _MyRequest.assert_called()
 
 
 class test_hybrid_to_proto2:
 
-    def setup(self):
+    def setup_method(self):
         self.message = Mock(name='message', headers={"custom": "header"})
         self.body = {
             'args': (1,),
             'kwargs': {'foo': 'baz'},
             'utc': False,
             'taskset': '123',
         }
```

### Comparing `celery-5.3.0b1/t/unit/worker/test_worker.py` & `celery-5.3.0b2/t/unit/worker/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,24 +73,24 @@
         m.channel = channel
         m.delivery_info = {'consumer_tag': 'mock'}
         return m
 
 
 class test_Consumer(ConsumerCase):
 
-    def setup(self):
+    def setup_method(self):
         self.buffer = FastQueue()
         self.timer = Timer()
 
         @self.app.task(shared=False)
         def foo_task(x, y, z):
             return x * y * z
         self.foo_task = foo_task
 
-    def teardown(self):
+    def teardown_method(self):
         self.timer.stop()
 
     def LoopConsumer(self, buffer=None, controller=None, timer=None, app=None,
                      without_mingle=True, without_gossip=True,
                      without_heartbeat=True, **kwargs):
         if controller is None:
             controller = Mock(name='.controller')
@@ -216,16 +216,16 @@
         c = self.LoopConsumer()
         c.blueprint.state = RUN
         c.steps.pop()
         m = self.create_task_message(
             Mock(), self.foo_task.name,
             args=(1, 2), kwargs='foobarbaz', id=1)
         c.update_strategies()
-        strat = c.strategies[self.foo_task.name] = Mock(name='strategy')
-        strat.side_effect = InvalidTaskError()
+        strategy = c.strategies[self.foo_task.name] = Mock(name='strategy')
+        strategy.side_effect = InvalidTaskError()
 
         callback = self._get_on_message(c)
         callback(m)
         error.assert_called()
         assert 'Received invalid task message' in error.call_args[0][0]
 
     @patch('celery.worker.consumer.consumer.crit')
@@ -693,27 +693,27 @@
         c = self.NoopConsumer()
         c.steps.pop()
         c.blueprint.start(c)
 
 
 class test_WorkController(ConsumerCase):
 
-    def setup(self):
+    def setup_method(self):
         self.worker = self.create_worker()
         self._logger = worker_module.logger
         self._comp_logger = components.logger
         self.logger = worker_module.logger = Mock()
         self.comp_logger = components.logger = Mock()
 
         @self.app.task(shared=False)
         def foo_task(x, y, z):
             return x * y * z
         self.foo_task = foo_task
 
-    def teardown(self):
+    def teardown_method(self):
         worker_module.logger = self._logger
         components.logger = self._comp_logger
 
     def create_worker(self, **kw):
         worker = self.app.WorkController(concurrency=1, loglevel=0, **kw)
         worker.blueprint.shutdown_complete.set()
         return worker
```

