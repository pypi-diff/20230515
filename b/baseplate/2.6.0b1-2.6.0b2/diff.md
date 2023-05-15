# Comparing `tmp/baseplate-2.6.0b1.tar.gz` & `tmp/baseplate-2.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseplate-2.6.0b1.tar", last modified: Wed Nov 30 18:22:02 2022, max compression
+gzip compressed data, was "baseplate-2.6.0b2.tar", last modified: Tue Dec  6 18:10:20 2022, max compression
```

## Comparing `baseplate-2.6.0b1.tar` & `baseplate-2.6.0b2.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.460934 baseplate-2.6.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.416933 baseplate-2.6.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      507 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26307 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-11-30 18:22:02.460934 baseplate-2.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/
--rw-r--r--   0 runner    (1001) docker     (123)    26319 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16083 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/kombu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/clients/memcache/
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/memcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/memcache/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    22207 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    17076 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/clients/thrift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/frameworks/pyramid/
--rw-r--r--   0 runner    (1001) docker     (123)    16124 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/pyramid/csrf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24586 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    18750 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/kombu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate/frameworks/thrift/
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/frameworks/thrift/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/edgecontext.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/file_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/lib/live_data/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/live_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/live_data/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/live_data/zookeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/message_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19944 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/prometheus_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/lib/ratelimit/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/ratelimit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/memcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/ratelimit/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18670 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/service_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lib/thrift_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/lint/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lint/db_query_string_format_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/lint/example_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.440933 baseplate-2.6.0b1/baseplate/observers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/metrics_tagged.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/sentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    22594 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/observers/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/baseplate/server/
--rw-r--r--   0 runner    (1001) docker     (123)    18493 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/einhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/monkey.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12755 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/queue_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/reloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/runtime_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/thrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/baseplate/sidecars/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/sidecars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/sidecars/event_publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/sidecars/live_data_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/sidecars/secrets_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/sidecars/trace_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/baseplate/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/baseplate/testing/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/testing/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/testing/lib/file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/testing/lib/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/baseplate/thrift/
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/BaseplateService.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/BaseplateServiceV2.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/baseplate.thrift
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/baseplate/thrift/ttypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.436933 baseplate-2.6.0b1/baseplate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-11-30 18:22:02.000000 baseplate-2.6.0b1/baseplate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/bin/baseplate-healthcheck
--rwxr-xr-x   0 runner    (1001) docker     (123)      466 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/bin/baseplate-script
--rwxr-xr-x   0 runner    (1001) docker     (123)      474 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/bin/baseplate-serve
--rwxr-xr-x   0 runner    (1001) docker     (123)      464 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/bin/baseplate-shell
--rwxr-xr-x   0 runner    (1001) docker     (123)      567 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/bin/baseplate-tshell
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/docs/api/baseplate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.444934 baseplate-2.6.0b1/docs/api/baseplate/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/kombu.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/memcache.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/redis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/redis_cluster.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/sqlalchemy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/clients/thrift.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/api/baseplate/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/pyramid.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/kombu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/frameworks/thrift.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/api/baseplate/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/crypto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/datetime.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/edgecontext.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/file_watcher.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/live_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/message_queue.rst
--rw-r--r--   0 runner    (1001) docker     (123)      503 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/random.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/ratelimit.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/retry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/secrets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/service_discovery.rst
--rw-r--r--   0 runner    (1001) docker     (123)      260 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/lib/thrift_pool.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/api/baseplate/observers/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/sentry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/tagged_statsd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/timeout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/baseplate/observers/tracing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/library.rst
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/api/observability-framework.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/cli/healthcheck.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/cli/script.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/cli/serve.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/cli/shell.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/config_dictof_example.ini
--rw-r--r--   0 runner    (1001) docker     (123)      360 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/config_dictof_spec_example.ini
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/config_example.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/guide/startup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    96286 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/images/baseplate.png
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/lint/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/lint/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/secrets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.448934 baseplate-2.6.0b1/docs/tutorial/chapter1/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter1/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/docs/tutorial/chapter2/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter2/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (123)      410 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter2/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/docs/tutorial/chapter3/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter3/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (123)      649 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter3/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter3/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/docs/tutorial/chapter4/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter4/helloworld.ini
--rw-r--r--   0 runner    (1001) docker     (123)      848 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter4/helloworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/chapter4/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/docs/watched_file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/pylint_baseplate_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2022-11-30 18:22:02.460934 baseplate-2.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/data/file_watcher_tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/cassandra_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/integration/live_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/live_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/live_data/writer_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/live_data/zookeeper_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/memcache_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/message_queue_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/pyramid_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/ratelimit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/redis_cluster_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/redis_testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/redis_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/requests_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/sqlalchemy_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/test.thrift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/integration/test_thrift/
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/test_thrift/TestService.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/test_thrift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/test_thrift/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/test_thrift/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    23297 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/thrift_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/timeout_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/integration/tracing_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.452934 baseplate-2.6.0b1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/cassandra_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/kombu_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18814 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/memcache_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/redis_cluster_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/redis_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/requests_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/sqlalchemy_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/clients/thrift_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/core_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/frameworks/pyramid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/pyramid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/pyramid/csrf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/pyramid/http_server_prom_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28081 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/kafka_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/kombu_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/frameworks/thrift_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/crypto_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/datetime_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/events/publisher_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/events/queue_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/file_watcher_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/log_formatter_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/metrics_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/random_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/ratelimit_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/retry_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/lib/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/secrets/store_directory_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/secrets/store_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/service_discovery_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lib/thrift_pool_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lint/db_query_string_format_plugin_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/lint/example_plugin_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/observers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/metrics_tagged_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/metrics_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/sentry_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/observers/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/tracing/publisher_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/observers/tracing_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.456934 baseplate-2.6.0b1/tests/unit/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/server/einhorn_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/server/monkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/server/queue_consumer_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/server/server_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 18:22:02.460934 baseplate-2.6.0b1/tests/unit/sidecars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/sidecars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/sidecars/live_data_watcher_loader_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2022-11-30 18:21:50.000000 baseplate-2.6.0b1/tests/unit/sidecars/live_data_watcher_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.688331 baseplate-2.6.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.656331 baseplate-2.6.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26307 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-12-06 18:10:20.688331 baseplate-2.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26319 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16083 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/kombu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/clients/memcache/
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/memcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/memcache/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22207 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17076 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/clients/thrift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/frameworks/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (123)    16124 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/pyramid/csrf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24586 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18750 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/kombu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate/frameworks/thrift/
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/frameworks/thrift/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/edgecontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/file_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/lib/live_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/live_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/live_data/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/live_data/zookeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/message_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19944 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/prometheus_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/lib/ratelimit/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/ratelimit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/ratelimit/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18670 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/service_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lib/thrift_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lint/db_query_string_format_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/lint/example_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.668331 baseplate-2.6.0b2/baseplate/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/metrics_tagged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22594 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/observers/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/baseplate/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    18493 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/einhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/monkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/queue_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/reloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/runtime_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/thrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/baseplate/sidecars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/sidecars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/sidecars/event_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/sidecars/live_data_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/sidecars/secrets_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/sidecars/trace_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/baseplate/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/baseplate/testing/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/testing/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/testing/lib/file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/testing/lib/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/baseplate/thrift/
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/BaseplateService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/BaseplateServiceV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/baseplate.thrift
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/baseplate/thrift/ttypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.664331 baseplate-2.6.0b2/baseplate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-06 18:10:20.000000 baseplate-2.6.0b2/baseplate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/bin/baseplate-healthcheck
+-rwxr-xr-x   0 runner    (1001) docker     (123)      466 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/bin/baseplate-script
+-rwxr-xr-x   0 runner    (1001) docker     (123)      474 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/bin/baseplate-serve
+-rwxr-xr-x   0 runner    (1001) docker     (123)      464 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/bin/baseplate-shell
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/bin/baseplate-tshell
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/docs/api/baseplate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.672331 baseplate-2.6.0b2/docs/api/baseplate/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/kombu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/memcache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/redis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/redis_cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/requests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/sqlalchemy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/clients/thrift.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/api/baseplate/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/pyramid.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/kombu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/frameworks/thrift.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/api/baseplate/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/crypto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/datetime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/edgecontext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/file_watcher.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/live_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/message_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/random.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/ratelimit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/retry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/secrets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/service_discovery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/lib/thrift_pool.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/api/baseplate/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/sentry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/tagged_statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/timeout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/baseplate/observers/tracing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/library.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/api/observability-framework.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/cli/healthcheck.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/cli/script.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/cli/serve.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/cli/shell.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/config_dictof_example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/config_dictof_spec_example.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/config_example.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/guide/startup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    96286 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/images/baseplate.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/lint/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/secrets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.676331 baseplate-2.6.0b2/docs/tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/docs/tutorial/chapter1/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter1/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/docs/tutorial/chapter2/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter2/helloworld.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter2/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/docs/tutorial/chapter3/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter3/helloworld.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter3/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter3/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/docs/tutorial/chapter4/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter4/helloworld.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter4/helloworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/chapter4/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/docs/watched_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/pylint_baseplate_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2022-12-06 18:10:20.688331 baseplate-2.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/data/file_watcher_tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/cassandra_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/integration/live_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/live_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/live_data/writer_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/live_data/zookeeper_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/memcache_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/message_queue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/pyramid_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/ratelimit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/redis_cluster_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/redis_testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/redis_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/requests_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/sqlalchemy_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/test.thrift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/integration/test_thrift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/test_thrift/TestService.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/test_thrift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/test_thrift/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/test_thrift/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23297 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/thrift_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/timeout_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/integration/tracing_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.680331 baseplate-2.6.0b2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/cassandra_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/kombu_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18814 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/memcache_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/redis_cluster_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/redis_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/requests_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/sqlalchemy_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/clients/thrift_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/core_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/frameworks/pyramid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/pyramid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/pyramid/csrf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/pyramid/http_server_prom_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28081 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/kafka_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/kombu_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/frameworks/thrift_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/crypto_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/datetime_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/events/publisher_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/events/queue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/file_watcher_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/log_formatter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/metrics_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/random_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/ratelimit_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/retry_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/lib/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/secrets/store_directory_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/secrets/store_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/service_discovery_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lib/thrift_pool_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lint/db_query_string_format_plugin_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/lint/example_plugin_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/observers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/metrics_tagged_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/metrics_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/sentry_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.684331 baseplate-2.6.0b2/tests/unit/observers/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/tracing/publisher_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/observers/tracing_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.688331 baseplate-2.6.0b2/tests/unit/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/server/einhorn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/server/monkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/server/queue_consumer_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/server/server_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:20.688331 baseplate-2.6.0b2/tests/unit/sidecars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/sidecars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/sidecars/live_data_watcher_loader_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2022-12-06 18:10:06.000000 baseplate-2.6.0b2/tests/unit/sidecars/live_data_watcher_tests.py
```

### Comparing `baseplate-2.6.0b1/.github/workflows/python-package.yaml` & `baseplate-2.6.0b2/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/.github/workflows/python-publish.yaml` & `baseplate-2.6.0b2/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/CONTRIBUTING.md` & `baseplate-2.6.0b2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/COPYRIGHT` & `baseplate-2.6.0b2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/LICENSE` & `baseplate-2.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/Makefile` & `baseplate-2.6.0b2/Makefile`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/PKG-INFO` & `baseplate-2.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseplate
-Version: 2.6.0b1
+Version: 2.6.0b2
 Summary: reddit's python service framework
 Home-page: https://github.com/reddit/baseplate.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://baseplate.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/reddit/baseplate.py
 Description: # baseplate.py
```

### Comparing `baseplate-2.6.0b1/README.md` & `baseplate-2.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/__init__.py` & `baseplate-2.6.0b2/baseplate/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/__init__.py` & `baseplate-2.6.0b2/baseplate/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/cassandra.py` & `baseplate-2.6.0b2/baseplate/clients/cassandra.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/kombu.py` & `baseplate-2.6.0b2/baseplate/clients/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/memcache/__init__.py` & `baseplate-2.6.0b2/baseplate/clients/memcache/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/memcache/lib.py` & `baseplate-2.6.0b2/baseplate/clients/memcache/lib.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/redis.py` & `baseplate-2.6.0b2/baseplate/clients/redis.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/redis_cluster.py` & `baseplate-2.6.0b2/baseplate/clients/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/requests.py` & `baseplate-2.6.0b2/baseplate/clients/requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/sqlalchemy.py` & `baseplate-2.6.0b2/baseplate/clients/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/clients/thrift.py` & `baseplate-2.6.0b2/baseplate/clients/thrift.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/pyramid/__init__.py` & `baseplate-2.6.0b2/baseplate/frameworks/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/pyramid/csrf.py` & `baseplate-2.6.0b2/baseplate/frameworks/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/kafka.py` & `baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/kafka.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/queue_consumer/kombu.py` & `baseplate-2.6.0b2/baseplate/frameworks/queue_consumer/kombu.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/thrift/__init__.py` & `baseplate-2.6.0b2/baseplate/frameworks/thrift/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/frameworks/thrift/command.py` & `baseplate-2.6.0b2/baseplate/frameworks/thrift/command.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/__init__.py` & `baseplate-2.6.0b2/baseplate/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/_requests.py` & `baseplate-2.6.0b2/baseplate/lib/_requests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/config.py` & `baseplate-2.6.0b2/baseplate/lib/config.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/crypto.py` & `baseplate-2.6.0b2/baseplate/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/datetime.py` & `baseplate-2.6.0b2/baseplate/lib/datetime.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/events.py` & `baseplate-2.6.0b2/baseplate/lib/events.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/file_watcher.py` & `baseplate-2.6.0b2/baseplate/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/live_data/writer.py` & `baseplate-2.6.0b2/baseplate/lib/live_data/writer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/live_data/zookeeper.py` & `baseplate-2.6.0b2/baseplate/lib/live_data/zookeeper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,17 @@
 """Helpers for interacting with ZooKeeper."""
 from typing import Optional
 
 from kazoo.client import KazooClient
-from kazoo.client import KazooState
 from kazoo.handlers.gevent import SequentialGeventHandler
-from prometheus_client import Counter
 
 from baseplate.lib import config
 from baseplate.lib.secrets import SecretsStore
 from baseplate.server.monkey import gevent_is_patched
 
-SESSION_LOST_TOTAL = Counter(
-    "live_data_fetcher_lost_sessions_total",
-    "The number of times a Zookeeper client has had a session be lost.",
-)
-
-SESSION_SUSPENDED_TOTAL = Counter(
-    "live_data_fetcher_suspended_sessions_total",
-    "The number of times a Zookeeper client has had a session be suspended.",
-)
-
-SESSION_SUCCESSFUL_TOTAL = Counter(
-    "live_data_fetcher_connected_sessions_total",
-    "The number of times a Zookeeper client has successfully established a session.",
-)
-
-
-class SessionStatsListener:
-    """A Kazoo listener that monitors changes in connection state.
-    Increments an event counter whenever connection state changes in a
-    Zookeeper connection.
-    """
-
-    def __call__(self, state: KazooState) -> None:
-        if state == KazooState.LOST:
-            SESSION_LOST_TOTAL.inc()
-        elif state == KazooState.SUSPENDED:
-            SESSION_SUSPENDED_TOTAL.inc()
-        else:
-            SESSION_SUCCESSFUL_TOTAL.inc()
-
 
 def zookeeper_client_from_config(
     secrets: SecretsStore, app_config: config.RawConfig, read_only: Optional[bool] = None
 ) -> KazooClient:
     """Configure and return a ZooKeeper client.
 
     There are several configuration options:
@@ -89,15 +57,15 @@
 
     # Kazoo needs to use a different handler with gevent.
     if gevent_is_patched():
         handler = SequentialGeventHandler()
     else:
         handler = None
 
-    client = KazooClient(
+    return KazooClient(
         cfg.hosts,
         timeout=cfg.timeout.total_seconds(),
         auth_data=auth_data,
         read_only=read_only,
         handler=handler,
         # this retry policy tells Kazoo how often it should attempt connections
         # to ZooKeeper from its worker thread/greenlet. when the connection is
@@ -118,12 +86,7 @@
             max_tries=-1,  # keep reconnecting forever
             delay=0.1,  # initial delay
             backoff=2,  # exponential backoff
             max_jitter=1,  # maximum amount to jitter sleeptimes
             max_delay=60,  # never wait longer than this
         ),
     )
-
-    listener = SessionStatsListener()
-    client.add_listener(listener)
-
-    return client
```

### Comparing `baseplate-2.6.0b1/baseplate/lib/log_formatter.py` & `baseplate-2.6.0b2/baseplate/lib/log_formatter.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/message_queue.py` & `baseplate-2.6.0b2/baseplate/lib/message_queue.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/metrics.py` & `baseplate-2.6.0b2/baseplate/lib/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/prometheus_metrics.py` & `baseplate-2.6.0b2/baseplate/lib/prometheus_metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/random.py` & `baseplate-2.6.0b2/baseplate/lib/random.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/__init__.py` & `baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/memcache.py` & `baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/memcache.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/ratelimit/backends/redis.py` & `baseplate-2.6.0b2/baseplate/lib/ratelimit/backends/redis.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/ratelimit/ratelimit.py` & `baseplate-2.6.0b2/baseplate/lib/ratelimit/ratelimit.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/retry.py` & `baseplate-2.6.0b2/baseplate/lib/retry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/secrets.py` & `baseplate-2.6.0b2/baseplate/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/service_discovery.py` & `baseplate-2.6.0b2/baseplate/lib/service_discovery.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lib/thrift_pool.py` & `baseplate-2.6.0b2/baseplate/lib/thrift_pool.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lint/db_query_string_format_plugin.py` & `baseplate-2.6.0b2/baseplate/lint/db_query_string_format_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/lint/example_plugin.py` & `baseplate-2.6.0b2/baseplate/lint/example_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/logging.py` & `baseplate-2.6.0b2/baseplate/observers/logging.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/metrics.py` & `baseplate-2.6.0b2/baseplate/observers/metrics.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/metrics_tagged.py` & `baseplate-2.6.0b2/baseplate/observers/metrics_tagged.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/sentry.py` & `baseplate-2.6.0b2/baseplate/observers/sentry.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/timeout.py` & `baseplate-2.6.0b2/baseplate/observers/timeout.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/observers/tracing.py` & `baseplate-2.6.0b2/baseplate/observers/tracing.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/__init__.py` & `baseplate-2.6.0b2/baseplate/server/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/einhorn.py` & `baseplate-2.6.0b2/baseplate/server/einhorn.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/healthcheck.py` & `baseplate-2.6.0b2/baseplate/server/healthcheck.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/monkey.py` & `baseplate-2.6.0b2/baseplate/server/monkey.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/net.py` & `baseplate-2.6.0b2/baseplate/server/net.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/prometheus.py` & `baseplate-2.6.0b2/baseplate/server/prometheus.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/queue_consumer.py` & `baseplate-2.6.0b2/baseplate/server/queue_consumer.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/reloader.py` & `baseplate-2.6.0b2/baseplate/server/reloader.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/runtime_monitor.py` & `baseplate-2.6.0b2/baseplate/server/runtime_monitor.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/thrift.py` & `baseplate-2.6.0b2/baseplate/server/thrift.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/server/wsgi.py` & `baseplate-2.6.0b2/baseplate/server/wsgi.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/sidecars/__init__.py` & `baseplate-2.6.0b2/baseplate/sidecars/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/sidecars/event_publisher.py` & `baseplate-2.6.0b2/baseplate/sidecars/event_publisher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,31 @@
-# pylint: disable=wrong-import-position,wrong-import-order
-from gevent.monkey import patch_all
-
-from baseplate.server.monkey import patch_stdlib_queues
-
-# In order to allow Prometheus to scrape metrics, we need to concurrently
-# handle requests to '/metrics' along with the sidecar's execution.
-# Monkey patching is used to replace the stdlib sequential versions of functions
-# with concurrent versions. It must happen as soon as possible, before the
-# sequential versions are imported.
-patch_all()
-patch_stdlib_queues()
-
 import argparse
 import configparser
 import email.utils
 import gzip
 import hashlib
 import hmac
 import logging
 
 from typing import Any
 from typing import List
 from typing import Optional
 
-import gevent
 import requests
 
-from prometheus_client import Counter
-
-from baseplate import Baseplate
-from baseplate.clients.requests import ExternalRequestsClient
+from baseplate import __version__ as baseplate_version
 from baseplate.lib import config
 from baseplate.lib import metrics
 from baseplate.lib.events import MAX_EVENT_SIZE
 from baseplate.lib.events import MAX_QUEUE_SIZE
 from baseplate.lib.message_queue import MessageQueue
 from baseplate.lib.message_queue import TimedOutError
 from baseplate.lib.metrics import metrics_client_from_config
 from baseplate.lib.retry import RetryPolicy
 from baseplate.server import EnvironmentInterpolation
-from baseplate.server.prometheus import start_prometheus_exporter_for_sidecar
 from baseplate.sidecars import Batch
 from baseplate.sidecars import BatchFull
 from baseplate.sidecars import SerializedBatch
 from baseplate.sidecars import TimeLimitedBatch
 
 
 logger = logging.getLogger(__name__)
@@ -57,16 +39,14 @@
 MAX_RETRY_TIME = 5 * 60
 # maximum time (seconds) an event can sit around while we wait for more
 # messages to batch
 MAX_BATCH_AGE = 1
 # maximum size (in bytes) of a batch of events
 MAX_BATCH_SIZE = 500 * 1024
 
-PUBLISHES_COUNT_TOTAL = Counter("eventv2_publishes_total", "total count of published events")
-
 
 class MaxRetriesError(Exception):
     pass
 
 
 class V2Batch(Batch):
     # V2 batches are a struct with a single field of list<Event> type. because
@@ -115,20 +95,23 @@
 
     def serialize(self) -> SerializedBatch:
         serialized = self._header.encode() + b",".join(self._items) + self._end
         return SerializedBatch(item_count=len(self._items), serialized=serialized)
 
 
 class BatchPublisher:
-    def __init__(self, bp: Baseplate, metrics_client: metrics.Client, cfg: Any):
-        self.baseplate = bp
+    def __init__(self, metrics_client: metrics.Client, cfg: Any):
         self.metrics = metrics_client
         self.url = f"{cfg.collector.scheme}://{cfg.collector.hostname}/v{cfg.collector.version}"
         self.key_name = cfg.key.name
         self.key_secret = cfg.key.secret
+        self.session = requests.Session()
+        self.session.headers[
+            "User-Agent"
+        ] = f"baseplate.py-{self.__class__.__name__}/{baseplate_version}"
 
     def _sign_payload(self, payload: bytes) -> str:
         digest = hmac.new(self.key_secret, payload, hashlib.sha256).hexdigest()
         return f"key={self.key_name}, mac={digest}"
 
     def publish(self, payload: SerializedBatch) -> None:
         if not payload.item_count:
@@ -142,22 +125,23 @@
             "Content-Type": "application/json",
             "X-Signature": self._sign_payload(payload.serialized),
             "Content-Encoding": "gzip",
         }
 
         for _ in RetryPolicy.new(budget=MAX_RETRY_TIME, backoff=RETRY_BACKOFF):
             try:
-                with self.baseplate.server_context("post") as context:
-                    with self.metrics.timer("post"):
-                        response = context.http_client.post(
-                            self.url,
-                            headers=headers,
-                            data=compressed_payload,
-                            timeout=POST_TIMEOUT,
-                        )
+                with self.metrics.timer("post"):
+                    response = self.session.post(
+                        self.url,
+                        headers=headers,
+                        data=compressed_payload,
+                        timeout=POST_TIMEOUT,
+                        # http://docs.python-requests.org/en/latest/user/advanced/#keep-alive
+                        stream=False,
+                    )
                 response.raise_for_status()
             except requests.HTTPError as exc:
                 self.metrics.counter("error.http").increment()
 
                 # we should crash if it's our fault
                 response = getattr(exc, "response", None)
                 if response is not None and response.status_code < 500:
@@ -167,15 +151,14 @@
                         raise
                 else:
                     logger.exception("HTTP Request failed.")
             except OSError:
                 self.metrics.counter("error.io").increment()
                 logger.exception("HTTP Request failed")
             else:
-                PUBLISHES_COUNT_TOTAL.inc(payload.item_count)
                 self.metrics.counter("sent").increment(payload.item_count)
                 return
 
         raise MaxRetriesError("could not sent batch")
 
 
 SERIALIZER_BY_VERSION = {"2": V2Batch, "2j": V2JBatch}
@@ -222,29 +205,20 @@
 
     event_queue = MessageQueue(
         "/events-" + args.queue_name,
         max_messages=cfg.max_queue_size,
         max_message_size=MAX_EVENT_SIZE,
     )
 
-    bp = Baseplate()
-    bp.configure_context(
-        {
-            "http_client": ExternalRequestsClient("event_collector"),
-        }
-    )
-
     # pylint: disable=maybe-no-member
     serializer = SERIALIZER_BY_VERSION[cfg.collector.version]()
     batcher = TimeLimitedBatch(serializer, MAX_BATCH_AGE)
-    publisher = BatchPublisher(bp, metrics_client, cfg)
+    publisher = BatchPublisher(metrics_client, cfg)
 
     while True:
-        # allow other routines to execute (specifically handling requests to /metrics)
-        gevent.sleep(0)
         message: Optional[bytes]
 
         try:
             message = event_queue.get(timeout=0.2)
         except TimedOutError:
             message = None
 
@@ -260,9 +234,8 @@
         except Exception:
             logger.exception("Events publishing failed.")
         batcher.reset()
         batcher.add(message)
 
 
 if __name__ == "__main__":
-    start_prometheus_exporter_for_sidecar()
     publish_events()
```

### Comparing `baseplate-2.6.0b1/baseplate/sidecars/live_data_watcher.py` & `baseplate-2.6.0b2/baseplate/sidecars/live_data_watcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 """Watch nodes in ZooKeeper and sync their contents to disk on change."""
-# pylint: disable=wrong-import-position,wrong-import-order
-from gevent.monkey import patch_all
-
-from baseplate.server.monkey import patch_stdlib_queues
-
-# In order to allow Prometheus to scrape metrics, we need to concurrently
-# handle requests to '/metrics' along with the sidecar's execution.
-# Monkey patching is used to replace the stdlib sequential versions of functions
-# with concurrent versions. It must happen as soon as possible, before the
-# sequential versions are imported.
-patch_all()
-patch_stdlib_queues()
-
 import argparse
 import configparser
 import json
 import logging
 import os
 import sys
+import time
 
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import NoReturn
 from typing import Optional
 
 import boto3  # type: ignore
-import gevent
 
 from botocore import UNSIGNED  # type: ignore
 from botocore.client import ClientError  # type: ignore
 from botocore.client import Config
 from botocore.exceptions import EndpointConnectionError  # type: ignore
 from kazoo.client import KazooClient
 from kazoo.protocol.states import ZnodeStat
 
 from baseplate.lib import config
 from baseplate.lib.live_data.zookeeper import zookeeper_client_from_config
 from baseplate.lib.secrets import secrets_store_from_config
 from baseplate.server import EnvironmentInterpolation
-from baseplate.server.prometheus import start_prometheus_exporter_for_sidecar
 
 
 logger = logging.getLogger(__name__)
 
 
 HEARTBEAT_INTERVAL = 300
 
@@ -197,15 +183,15 @@
     for node in nodes:
         watcher = NodeWatcher(node.dest, node.owner, node.group, node.mode)
         zookeeper.DataWatch(node.source, watcher.on_change)
 
     # all the interesting stuff is now happening in the Kazoo worker thread
     # and so we'll just spin and periodically heartbeat to prove we're alive.
     while True:
-        gevent.sleep(HEARTBEAT_INTERVAL)
+        time.sleep(HEARTBEAT_INTERVAL)
 
         # see the comment in baseplate.live_data.zookeeper for explanation of
         # how reconnects work with the background thread.
         if zookeeper.connected:
             for node in nodes:
                 try:
                     logger.debug("Heartbeating %s", node.dest)
@@ -268,9 +254,8 @@
     try:
         watch_zookeeper_nodes(zookeeper, nodes)
     finally:
         zookeeper.stop()
 
 
 if __name__ == "__main__":
-    start_prometheus_exporter_for_sidecar()
     main()
```

### Comparing `baseplate-2.6.0b1/baseplate/sidecars/secrets_fetcher.py` & `baseplate-2.6.0b2/baseplate/sidecars/secrets_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,51 +56,37 @@
 
 Some applications require a specific format for their secrets. The `callback` option may
 be provided if a different format is needed. This script will be invoked as a subprocess
 with the JSON file as its first and only argument. This allows you to read in the secrets,
 write to a new file in whatever format needed, and restart other services if necessary.
 
 """
-# pylint: disable=wrong-import-position,wrong-import-order
-from gevent.monkey import patch_all
-
-from baseplate.server.monkey import patch_stdlib_queues
-
-# In order to allow Prometheus to scrape metrics, we need to concurrently
-# handle requests to '/metrics' along with the sidecar's execution.
-# Monkey patching is used to replace the stdlib sequential versions of functions
-# with concurrent versions. It must happen as soon as possible, before the
-# sequential versions are imported.
-patch_all()
-patch_stdlib_queues()
-
 import argparse
 import configparser
 import datetime
 import json
 import logging
 import os
 import posixpath
 import subprocess
+import time
 import urllib.parse
 import uuid
 
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Tuple
 
-import gevent
 import requests
 
 from baseplate import __version__ as baseplate_version
 from baseplate.lib import config
 from baseplate.server import EnvironmentInterpolation
-from baseplate.server.prometheus import start_prometheus_exporter_for_sidecar
 
 
 logger = logging.getLogger(__name__)
 
 
 K8S_SERVICE_ACCOUNT_TOKEN_FILE = "/var/run/secrets/kubernetes.io/serviceaccount/token"
 NONCE_FILENAME = "/var/local/vault.nonce"
@@ -437,13 +423,12 @@
         logger.info("Running secret fetcher as a daemon")
         last_proc = None
         while True:
             soonest_expiration = fetch_secrets(cfg, client_factory)
             last_proc = trigger_callback(cfg.callback, cfg.output.path, last_proc)
             time_til_expiration = soonest_expiration - datetime.datetime.utcnow()
             time_to_sleep = time_til_expiration - VAULT_TOKEN_PREFETCH_TIME
-            gevent.sleep(max(int(time_to_sleep.total_seconds()), 1))
+            time.sleep(max(int(time_to_sleep.total_seconds()), 1))
 
 
 if __name__ == "__main__":
-    start_prometheus_exporter_for_sidecar()
     main()
```

### Comparing `baseplate-2.6.0b1/baseplate/sidecars/trace_publisher.py` & `baseplate-2.6.0b2/baseplate/sidecars/trace_publisher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,26 @@
-# pylint: disable=wrong-import-position,wrong-import-order
-from gevent.monkey import patch_all
-
-from baseplate.server.monkey import patch_stdlib_queues
-
-# In order to allow Prometheus to scrape metrics, we need to concurrently
-# handle requests to '/metrics' along with the sidecar's execution.
-# Monkey patching is used to replace the stdlib sequential versions of functions
-# with concurrent versions. It must happen as soon as possible, before the
-# sequential versions are imported.
-patch_all()
-patch_stdlib_queues()
-
 import argparse
 import configparser
 import logging
+import urllib.parse
 
 from typing import Optional
 
-import gevent
 import requests
 
-from prometheus_client import Counter
-
-from baseplate import Baseplate
-from baseplate.clients.requests import InternalRequestsClient
+from baseplate import __version__ as baseplate_version
 from baseplate.lib import config
 from baseplate.lib import metrics
 from baseplate.lib.message_queue import MessageQueue
 from baseplate.lib.message_queue import TimedOutError
 from baseplate.lib.metrics import metrics_client_from_config
 from baseplate.lib.retry import RetryPolicy
 from baseplate.observers.tracing import MAX_QUEUE_SIZE
 from baseplate.observers.tracing import MAX_SPAN_SIZE
 from baseplate.server import EnvironmentInterpolation
-from baseplate.server.prometheus import start_prometheus_exporter_for_sidecar
 from baseplate.sidecars import BatchFull
 from baseplate.sidecars import RawJSONBatch
 from baseplate.sidecars import SerializedBatch
 from baseplate.sidecars import TimeLimitedBatch
 
 
 logger = logging.getLogger(__name__)
@@ -47,22 +30,17 @@
 
 # maximum size (in bytes) of a batch of traces
 MAX_BATCH_SIZE_DEFAULT = 500 * 1024
 # maximum time (seconds) a traces can sit around while we wait for more
 # messages to batch
 MAX_BATCH_AGE = 1
 
-# max number of connections to Zipkin server
-MAX_NUM_CONNS = 5
-
 # maximum number of retries when publishing traces
 RETRY_LIMIT_DEFAULT = 10
 
-PUBLISHES_COUNT_TOTAL = Counter("zipkin_trace_publishes_total", "total count of published traces")
-
 
 class MaxRetriesError(Exception):
     pass
 
 
 class TraceBatch(RawJSONBatch):
     def __init__(self, max_size: int = MAX_BATCH_SIZE_DEFAULT):
@@ -70,21 +48,28 @@
 
 
 class ZipkinPublisher:
     """Zipkin trace publisher."""
 
     def __init__(
         self,
-        bp: Baseplate,
         zipkin_api_url: str,
         metrics_client: metrics.Client,
         post_timeout: int = POST_TIMEOUT_DEFAULT,
         retry_limit: int = RETRY_LIMIT_DEFAULT,
+        num_conns: int = 5,
     ):
-        self.baseplate = bp
+
+        adapter = requests.adapters.HTTPAdapter(pool_connections=num_conns, pool_maxsize=num_conns)
+        parsed_url = urllib.parse.urlparse(zipkin_api_url)
+        self.session = requests.Session()
+        self.session.headers[
+            "User-Agent"
+        ] = f"baseplate.py-{self.__class__.__name__}/{baseplate_version}"
+        self.session.mount(f"{parsed_url.scheme}://", adapter)
         self.endpoint = f"{zipkin_api_url}/spans"
         self.metrics = metrics_client
         self.post_timeout = post_timeout
         self.retry_limit = retry_limit
 
     def publish(self, payload: SerializedBatch) -> None:
         """Publish spans to Zipkin API.
@@ -97,22 +82,22 @@
         logger.info("Sending batch of %d traces", payload.item_count)
         headers = {
             "User-Agent": "baseplate-trace-publisher/1.0",
             "Content-Type": "application/json",
         }
         for _ in RetryPolicy.new(attempts=self.retry_limit):
             try:
-                with self.baseplate.server_context("post") as context:
-                    with self.metrics.timer("post"):
-                        response = context.http_client.post(
-                            self.endpoint,
-                            data=payload.serialized,
-                            headers=headers,
-                            timeout=self.post_timeout,
-                        )
+                with self.metrics.timer("post"):
+                    response = self.session.post(
+                        self.endpoint,
+                        data=payload.serialized,
+                        headers=headers,
+                        timeout=self.post_timeout,
+                        stream=False,
+                    )
                 response.raise_for_status()
             except requests.HTTPError as exc:
                 self.metrics.counter("error.http").increment()
                 response = getattr(exc, "response", None)
                 if response is not None:
                     logger.exception("HTTP Request failed. Error: %s", response.text)
                     # If client error, skip retries
@@ -121,15 +106,14 @@
                         return
                 else:
                     logger.exception("HTTP Request failed. Response not available")
             except OSError:
                 self.metrics.counter("error.io").increment()
                 logger.exception("HTTP Request failed")
             else:
-                PUBLISHES_COUNT_TOTAL.inc(payload.item_count)
                 self.metrics.counter("sent").increment(payload.item_count)
                 return
 
         raise MaxRetriesError(
             f"ZipkinPublisher exhausted allowance of {self.retry_limit:d} retries."
         )
 
@@ -178,55 +162,36 @@
 
     trace_queue = MessageQueue(
         "/traces-" + args.queue_name,
         max_messages=publisher_cfg.max_queue_size,
         max_message_size=MAX_SPAN_SIZE,
     )
 
-    bp = Baseplate()
-    bp.configure_context(
-        {
-            "http_client": InternalRequestsClient(
-                "trace_collector", pool_connections=MAX_NUM_CONNS, pool_maxsize=MAX_NUM_CONNS
-            ),
-        }
-    )
-
     # pylint: disable=maybe-no-member
     inner_batch = TraceBatch(max_size=publisher_cfg.max_batch_size)
     batcher = TimeLimitedBatch(inner_batch, MAX_BATCH_AGE)
     metrics_client = metrics_client_from_config(publisher_raw_cfg)
     publisher = ZipkinPublisher(
-        bp,
         publisher_cfg.zipkin_api_url.address,
         metrics_client,
         post_timeout=publisher_cfg.post_timeout,
     )
 
     while True:
-        # allow other routines to execute (specifically handling requests to /metrics)
-        gevent.sleep(0)
         message: Optional[bytes]
 
         try:
             message = trace_queue.get(timeout=0.2)
         except TimedOutError:
             message = None
 
         try:
             batcher.add(message)
-            continue
         except BatchFull:
-            pass
-
-        serialized = batcher.serialize()
-        try:
+            serialized = batcher.serialize()
             publisher.publish(serialized)
-        except Exception:
-            logger.exception("Traces publishing failed.")
-        batcher.reset()
-        batcher.add(message)
+            batcher.reset()
+            batcher.add(message)
 
 
 if __name__ == "__main__":
-    start_prometheus_exporter_for_sidecar()
     publish_traces()
```

### Comparing `baseplate-2.6.0b1/baseplate/testing/lib/file_watcher.py` & `baseplate-2.6.0b2/baseplate/testing/lib/file_watcher.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/testing/lib/secrets.py` & `baseplate-2.6.0b2/baseplate/testing/lib/secrets.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/thrift/BaseplateService.py` & `baseplate-2.6.0b2/baseplate/thrift/BaseplateService.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/thrift/BaseplateServiceV2.py` & `baseplate-2.6.0b2/baseplate/thrift/BaseplateServiceV2.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/thrift/baseplate.thrift` & `baseplate-2.6.0b2/baseplate/thrift/baseplate.thrift`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate/thrift/ttypes.py` & `baseplate-2.6.0b2/baseplate/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate.egg-info/PKG-INFO` & `baseplate-2.6.0b2/baseplate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseplate
-Version: 2.6.0b1
+Version: 2.6.0b2
 Summary: reddit's python service framework
 Home-page: https://github.com/reddit/baseplate.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://baseplate.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/reddit/baseplate.py
 Description: # baseplate.py
```

### Comparing `baseplate-2.6.0b1/baseplate.egg-info/SOURCES.txt` & `baseplate-2.6.0b2/baseplate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/baseplate.egg-info/requires.txt` & `baseplate-2.6.0b2/baseplate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/bin/baseplate-tshell` & `baseplate-2.6.0b2/bin/baseplate-tshell`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docker-compose.yml` & `baseplate-2.6.0b2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/cassandra.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/cassandra.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/index.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/kombu.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/kombu.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/memcache.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/memcache.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/redis.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/redis.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/redis_cluster.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/redis_cluster.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/requests.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/requests.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/sqlalchemy.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/clients/thrift.rst` & `baseplate-2.6.0b2/docs/api/baseplate/clients/thrift.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/frameworks/index.rst` & `baseplate-2.6.0b2/docs/api/baseplate/frameworks/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/frameworks/pyramid.rst` & `baseplate-2.6.0b2/docs/api/baseplate/frameworks/pyramid.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/kafka.rst` & `baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/kafka.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/frameworks/queue_consumer/kombu.rst` & `baseplate-2.6.0b2/docs/api/baseplate/frameworks/queue_consumer/kombu.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/frameworks/thrift.rst` & `baseplate-2.6.0b2/docs/api/baseplate/frameworks/thrift.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/index.rst` & `baseplate-2.6.0b2/docs/api/baseplate/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/config.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/config.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/edgecontext.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/edgecontext.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/events.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/events.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/live_data.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/live_data.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/message_queue.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/message_queue.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/ratelimit.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/ratelimit.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/lib/secrets.rst` & `baseplate-2.6.0b2/docs/api/baseplate/lib/secrets.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/index.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/logging.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/logging.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/sentry.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/sentry.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/statsd.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/statsd.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/tagged_statsd.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/tagged_statsd.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/timeout.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/timeout.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/baseplate/observers/tracing.rst` & `baseplate-2.6.0b2/docs/api/baseplate/observers/tracing.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/library.rst` & `baseplate-2.6.0b2/docs/api/library.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/api/observability-framework.rst` & `baseplate-2.6.0b2/docs/api/observability-framework.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/cli/healthcheck.rst` & `baseplate-2.6.0b2/docs/cli/healthcheck.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/cli/script.rst` & `baseplate-2.6.0b2/docs/cli/script.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/cli/serve.rst` & `baseplate-2.6.0b2/docs/cli/serve.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/cli/shell.rst` & `baseplate-2.6.0b2/docs/cli/shell.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/conf.py` & `baseplate-2.6.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/guide/faq.rst` & `baseplate-2.6.0b2/docs/guide/faq.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/guide/startup.rst` & `baseplate-2.6.0b2/docs/guide/startup.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/images/baseplate.png` & `baseplate-2.6.0b2/docs/images/baseplate.png`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/images/favicon.png` & `baseplate-2.6.0b2/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/index.rst` & `baseplate-2.6.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/lint/index.rst` & `baseplate-2.6.0b2/docs/lint/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter1/helloworld.py` & `baseplate-2.6.0b2/docs/tutorial/chapter1/helloworld.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter1/index.rst` & `baseplate-2.6.0b2/docs/tutorial/chapter1/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter2/index.rst` & `baseplate-2.6.0b2/docs/tutorial/chapter2/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter3/helloworld.py` & `baseplate-2.6.0b2/docs/tutorial/chapter3/helloworld.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter3/index.rst` & `baseplate-2.6.0b2/docs/tutorial/chapter3/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter4/helloworld.py` & `baseplate-2.6.0b2/docs/tutorial/chapter4/helloworld.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/docs/tutorial/chapter4/index.rst` & `baseplate-2.6.0b2/docs/tutorial/chapter4/index.rst`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/pylint_baseplate_plugin.py` & `baseplate-2.6.0b2/pylint_baseplate_plugin.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/pylintrc` & `baseplate-2.6.0b2/pylintrc`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/requirements-transitive.txt` & `baseplate-2.6.0b2/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/requirements.txt` & `baseplate-2.6.0b2/requirements.txt`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/setup.cfg` & `baseplate-2.6.0b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/setup.py` & `baseplate-2.6.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/__init__.py` & `baseplate-2.6.0b2/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/cassandra_tests.py` & `baseplate-2.6.0b2/tests/integration/cassandra_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/live_data/writer_tests.py` & `baseplate-2.6.0b2/tests/integration/live_data/writer_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/live_data/zookeeper_tests.py` & `baseplate-2.6.0b2/tests/integration/live_data/zookeeper_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/memcache_tests.py` & `baseplate-2.6.0b2/tests/integration/memcache_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/message_queue_tests.py` & `baseplate-2.6.0b2/tests/integration/message_queue_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/pyramid_tests.py` & `baseplate-2.6.0b2/tests/integration/pyramid_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/ratelimit_tests.py` & `baseplate-2.6.0b2/tests/integration/ratelimit_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/redis_cluster_tests.py` & `baseplate-2.6.0b2/tests/integration/redis_cluster_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/redis_testcase.py` & `baseplate-2.6.0b2/tests/integration/redis_testcase.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/redis_tests.py` & `baseplate-2.6.0b2/tests/integration/redis_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/requests_tests.py` & `baseplate-2.6.0b2/tests/integration/requests_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/sqlalchemy_tests.py` & `baseplate-2.6.0b2/tests/integration/sqlalchemy_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/test_thrift/TestService.py` & `baseplate-2.6.0b2/tests/integration/test_thrift/TestService.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/test_thrift/ttypes.py` & `baseplate-2.6.0b2/tests/integration/test_thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/thrift_tests.py` & `baseplate-2.6.0b2/tests/integration/thrift_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/timeout_tests.py` & `baseplate-2.6.0b2/tests/integration/timeout_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/integration/tracing_tests.py` & `baseplate-2.6.0b2/tests/integration/tracing_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/cassandra_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/cassandra_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/kombu_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/kombu_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/memcache_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/memcache_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/redis_cluster_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/redis_cluster_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/redis_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/redis_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/requests_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/requests_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/sqlalchemy_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/sqlalchemy_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/clients/thrift_tests.py` & `baseplate-2.6.0b2/tests/unit/clients/thrift_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/core_tests.py` & `baseplate-2.6.0b2/tests/unit/core_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/frameworks/pyramid/csrf_tests.py` & `baseplate-2.6.0b2/tests/unit/frameworks/pyramid/csrf_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/frameworks/pyramid/http_server_prom_tests.py` & `baseplate-2.6.0b2/tests/unit/frameworks/pyramid/http_server_prom_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/kafka_tests.py` & `baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/kafka_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/frameworks/queue_consumer/kombu_tests.py` & `baseplate-2.6.0b2/tests/unit/frameworks/queue_consumer/kombu_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/frameworks/thrift_tests.py` & `baseplate-2.6.0b2/tests/unit/frameworks/thrift_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/config_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/config_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/crypto_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/crypto_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/datetime_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/datetime_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/events/publisher_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/events/publisher_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,35 +72,31 @@
 
         batch.reset()
         result = batch.serialize()
         self.assertEqual(result.item_count, 0)
 
 
 class PublisherTests(unittest.TestCase):
-    @mock.patch("baseplate.clients.requests.BaseplateSession", autospec=True)
-    @mock.patch("baseplate.RequestContext", autospec=True)
-    @mock.patch("baseplate.Baseplate", autospec=True)
-    def setUp(self, bp, context, session):
+    @mock.patch("requests.Session", autospec=True)
+    def setUp(self, Session):
         self.config = config.ConfigNamespace()
         self.config.collector = config.ConfigNamespace()
         self.config.collector.hostname = "test.local"
         self.config.collector.version = 1
         self.config.collector.scheme = "https"
         self.config.key = config.ConfigNamespace()
         self.config.key.name = "TestKey"
         self.config.key.secret = b"hunter2"
 
-        bp.server_context.return_value.__enter__.return_value = context
-        context.http_client = session
-        self.baseplate = bp
-        self.session = session
+        self.session = Session.return_value
+        self.session.headers = {}
 
         self.metrics_client = mock.MagicMock(autospec=metrics.Client)
 
-        self.publisher = event_publisher.BatchPublisher(bp, self.metrics_client, self.config)
+        self.publisher = event_publisher.BatchPublisher(self.metrics_client, self.config)
 
     def test_empty_batch(self):
         self.publisher.publish(SerializedBatch(item_count=0, serialized=b""))
         self.assertEqual(self.session.post.call_count, 0)
 
     def test_publish_success(self):
         events = b'[{"example": "value"}]'
@@ -114,15 +110,15 @@
         self.assertEqual(args[0], "https://test.local/v1")
         self.assertEqual(headers["Content-Type"], "application/json")
         self.assertEqual(
             headers["X-Signature"],
             "key=TestKey, mac=7c46d56b99cd4cb05e08238c1d4c10a2f330795e9d7327f17cc66fd206bf1179",
         )
 
-    @mock.patch("gevent.sleep")
+    @mock.patch("time.sleep")
     def test_fail_on_client_error(self, mock_sleep):
         self.session.post.side_effect = [
             requests.HTTPError(400, response=mock.Mock(status_code=400))
         ]
         events = b'[{"example": "value"}]'
 
         with self.assertRaises(requests.HTTPError):
```

### Comparing `baseplate-2.6.0b1/tests/unit/lib/events/queue_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/events/queue_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/file_watcher_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/file_watcher_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/log_formatter_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/log_formatter_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/metrics_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/metrics_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/random_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/random_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/ratelimit_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/ratelimit_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/retry_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/retry_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/secrets/store_directory_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/secrets/store_directory_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/secrets/store_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/secrets/store_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/service_discovery_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/service_discovery_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lib/thrift_pool_tests.py` & `baseplate-2.6.0b2/tests/unit/lib/thrift_pool_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lint/db_query_string_format_plugin_tests.py` & `baseplate-2.6.0b2/tests/unit/lint/db_query_string_format_plugin_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/lint/example_plugin_tests.py` & `baseplate-2.6.0b2/tests/unit/lint/example_plugin_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/observers/metrics_tagged_tests.py` & `baseplate-2.6.0b2/tests/unit/observers/metrics_tagged_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/observers/metrics_tests.py` & `baseplate-2.6.0b2/tests/unit/observers/metrics_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/observers/sentry_tests.py` & `baseplate-2.6.0b2/tests/unit/observers/sentry_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/observers/tracing/publisher_tests.py` & `baseplate-2.6.0b2/tests/unit/observers/tracing/publisher_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,25 @@
 
 from baseplate.lib import metrics
 from baseplate.sidecars import SerializedBatch
 from baseplate.sidecars import trace_publisher
 
 
 class ZipkinPublisherTest(unittest.TestCase):
-    @mock.patch("baseplate.clients.requests.BaseplateSession", autospec=True)
-    @mock.patch("baseplate.RequestContext", autospec=True)
-    @mock.patch("baseplate.Baseplate", autospec=True)
-    def setUp(self, bp, context, session):
+    @mock.patch("requests.Session", autospec=True)
+    def setUp(self, mock_Session):
+        self.session = mock_Session.return_value
+        self.session.headers = {}
         self.metrics_client = mock.MagicMock(autospec=metrics.Client)
         self.zipkin_api_url = "http://test.local/api/v2"
-
-        bp.server_context.return_value.__enter__.return_value = context
-        context.http_client = session
-        self.baseplate = bp
-        self.session = session
-
-        self.publisher = trace_publisher.ZipkinPublisher(
-            bp, self.zipkin_api_url, self.metrics_client
-        )
+        self.publisher = trace_publisher.ZipkinPublisher(self.zipkin_api_url, self.metrics_client)
 
     def test_initialization(self):
         self.assertEqual(self.publisher.endpoint, f"{self.zipkin_api_url}/spans")
+        self.publisher.session.mount.assert_called_with("http://", mock.ANY)
 
     def test_empty_batch(self):
         self.publisher.publish(SerializedBatch(item_count=0, serialized=b""))
         self.assertEqual(self.session.post.call_count, 0)
 
     def test_publish_retry(self):
         # raise two errors and then return a mock response
```

### Comparing `baseplate-2.6.0b1/tests/unit/observers/tracing_tests.py` & `baseplate-2.6.0b2/tests/unit/observers/tracing_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/server/einhorn_tests.py` & `baseplate-2.6.0b2/tests/unit/server/einhorn_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/server/monkey_tests.py` & `baseplate-2.6.0b2/tests/unit/server/monkey_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/server/queue_consumer_tests.py` & `baseplate-2.6.0b2/tests/unit/server/queue_consumer_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/server/server_tests.py` & `baseplate-2.6.0b2/tests/unit/server/server_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/sidecars/live_data_watcher_loader_tests.py` & `baseplate-2.6.0b2/tests/unit/sidecars/live_data_watcher_loader_tests.py`

 * *Files identical despite different names*

### Comparing `baseplate-2.6.0b1/tests/unit/sidecars/live_data_watcher_tests.py` & `baseplate-2.6.0b2/tests/unit/sidecars/live_data_watcher_tests.py`

 * *Files identical despite different names*

