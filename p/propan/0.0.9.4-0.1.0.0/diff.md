# Comparing `tmp/propan-0.0.9.4.tar.gz` & `tmp/propan-0.1.0.0.tar.gz`

## Comparing `propan-0.0.9.4.tar` & `propan-0.1.0.0.tar`

### file list

```diff
@@ -1,90 +1,95 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.4/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__about__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__main__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/annotations.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    10868 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/__init__.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/app.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/main.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/parser.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/logging.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/test/__init__.py
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/test/rabbit.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/classes.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/main.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/test.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 propan-0.0.9.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.4/LICENSE
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 propan-0.0.9.4/README.md
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 propan-0.0.9.4/pyproject.toml
--rw-r--r--   0        0        0    14468 2020-02-02 00:00:00.000000 propan-0.0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.0.0/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.1.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 propan-0.1.0.0/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__about__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/__main__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/py.typed
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/app.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/main.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/log/logging.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/test/__init__.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/test/rabbit.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.0.0/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.0.0/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.0.0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.0.0/LICENSE
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 propan-0.1.0.0/README.md
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 propan-0.1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 propan-0.1.0.0/PKG-INFO
```

### Comparing `propan-0.0.9.4/CONTRIBUTING.md` & `propan-0.1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/SECURITY.md` & `propan-0.1.0.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/.github/workflows/documentation.yml` & `propan-0.1.0.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/.github/workflows/publish_coverage.yml` & `propan-0.1.0.0/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/.github/workflows/publish_pypi.yml` & `propan-0.1.0.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/.github/workflows/tests.yml` & `propan-0.1.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/3_lifespan_events.py` & `propan-0.1.0.0/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/4_cli_attributes_promotion.py` & `propan-0.1.0.0/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/5_publishing.py` & `propan-0.1.0.0/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/6_arguments_casting.py` & `propan-0.1.0.0/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/7_handler_errors_processing.py` & `propan-0.1.0.0/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/1_dependency_injection.py` & `propan-0.1.0.0/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.0.0/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.0.0/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.0.0/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.0.0/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/dependencies/7_annotated.py` & `propan-0.1.0.0/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/quart.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.0.0/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/__init__.py` & `propan-0.1.0.0/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/annotations.py` & `propan-0.1.0.0/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/types.py` & `propan-0.1.0.0/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/push_back_watcher.py` & `propan-0.1.0.0/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/model/broker_usecase.py` & `propan-0.1.0.0/propan/brokers/model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     SendableMessage,
     Wrapper,
 )
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
 T = TypeVar("T")
+Cls = TypeVar("Cls", bound="BrokerUsecase")
 
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: List[Any]
     _connection: Any
@@ -64,15 +65,15 @@
         context.set_global("broker", self)
 
     async def connect(self, *args: Any, **kwargs: Any) -> Any:
         if self._connection is None:
             _args = args or self._connection_args
             _kwargs = kwargs or self._connection_kwargs
             self._connection = await self._connect(*_args, **_kwargs)
-            return self._connection
+        return self._connection
 
     @abstractmethod
     async def _connect(self, *args: Any, **kwargs: Any) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
     async def publish(
@@ -96,15 +97,17 @@
 
     @abstractmethod
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
     ) -> Callable[[PropanMessage], T]:
         raise NotImplementedError()
 
-    def _get_log_context(self, message: PropanMessage) -> Dict[str, Any]:
+    def _get_log_context(
+        self, message: PropanMessage, **kwargs: Dict[str, str]
+    ) -> Dict[str, Any]:
         return {
             "message_id": message.message_id[:10] if message else "",
         }
 
     @abstractmethod
     def handle(
         self,
@@ -134,15 +137,15 @@
         return self._fmt
 
     async def start(self) -> None:
         if self.logger is not None:
             change_logger_handlers(self.logger, self.fmt)
         await self.connect()
 
-    async def __aenter__(self) -> "BrokerUsecase":
+    async def __aenter__(self: Cls) -> Cls:
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.close()
 
     def _wrap_handler(
```

### Comparing `propan-0.0.9.4/propan/brokers/model/schemas.py` & `propan-0.1.0.0/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/model/utils.py` & `propan-0.1.0.0/propan/brokers/model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/nats/nats_broker.py` & `propan-0.1.0.0/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.0.0/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.0.0/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/nats/schemas.py` & `propan-0.1.0.0/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
 import aio_pika
 import aiormq
+from aio_pika.abc import DeliveryMode
 
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, SendableMessage, Wrapper
 from propan.utils.context import context as global_context
@@ -39,66 +40,53 @@
 
         self._channel = None
         self.handlers = []
 
         self.__max_queue_len = 4
         self.__max_exchange_len = 4
 
-    async def __aenter__(self) -> "RabbitBroker":
-        await self.connect()
-        await self._init_channel()
-        return self
-
     async def close(self) -> None:
+        if self._channel is not None:
+            await self._channel.close()
+            self._channel = None
+
         if self._connection is not None:
             await self._connection.close()
+            self._connection = None
 
     async def _connect(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> aio_pika.Connection:
-        return await aio_pika.connect_robust(
+        connection = await aio_pika.connect_robust(
             *args, **kwargs, loop=asyncio.get_event_loop()
         )
 
-    async def _init_channel(
-        self,
-        max_consumers: Optional[int] = None,
-    ) -> None:
-        if self._channel is None:
-            if self._connection is None:
-                raise ValueError("RabbitBroker not connected yet")
-
-            max_consumers = max_consumers or self._max_consumers
-            self._channel = await self._connection.channel()
+        if self._channel is None:  # pragma: no branch
+            max_consumers = self._max_consumers
+            self._channel = await connection.channel()
 
             if max_consumers:
                 self._log(f"Set max consumers to {max_consumers}", logging.INFO)
-                await self._channel.set_qos(prefetch_count=int(max_consumers))
+                await self._channel.set_qos(prefetch_count=int(self._max_consumers))
+
+        return connection
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         **original_kwargs,
     ) -> Wrapper:
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
         self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
-            for handler in self.handlers:
-                if handler.exchange == exchange and handler.queue == queue:
-                    raise ValueError(
-                        f"`{func.__name__}` uses already "
-                        f"using `{queue.name}` queue to listen "
-                        f"`{exchange.name if exchange else 'default'}` exchange"
-                    )
-
             func = self._wrap_handler(
                 func,
                 queue=queue,
                 exchange=exchange,
                 **original_kwargs,
             )
             handler = Handler(callback=func, queue=queue, exchange=exchange)
@@ -106,15 +94,14 @@
 
             return func
 
         return wrapper
 
     async def start(self) -> None:
         await super().start()
-        await self._init_channel()
 
         for handler in self.handlers:
             queue = await self._init_handler(handler)
 
             func = handler.callback
 
             if self.logger is not None:
@@ -133,14 +120,15 @@
         routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
         timeout: TimeoutType = None,
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
+        persist: bool = False,
         **message_kwargs,
     ) -> Union[aiormq.abc.ConfirmationFrameType, Dict, str, bytes, None]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
@@ -150,59 +138,81 @@
             callback_queue = None
 
         if exchange is None:
             exchange_obj = self._channel.default_exchange
         else:
             exchange_obj = await self._init_exchange(exchange)
 
-        message = self._validate_message(message, callback_queue, **message_kwargs)
+        message = self._validate_message(
+            message=message,
+            callback_queue=callback_queue,
+            persist=persist,
+            **message_kwargs,
+        )
 
         r = await exchange_obj.publish(
             message=message,
-            routing_key=routing_key or queue.name,
+            routing_key=routing_key or queue.routing or "",
             mandatory=mandatory,
             immediate=immediate,
             timeout=timeout,
         )
-
         if callback_queue is None:
             return r
 
         else:
+            iter = callback_queue.iterator()
+            await iter.consume()
             try:
-                async with callback_queue.iterator(
-                    timeout=callback_timeout
-                ) as queue_iterator:
-                    async for m in queue_iterator:  # pragma: no branch
-                        return await self._decode_message(m)
+                msg = await asyncio.wait_for(iter._queue.get(), callback_timeout)
             except asyncio.TimeoutError as e:
                 if raise_timeout is True:  # pragma: no branch
                     raise e
+            else:
+                return await self._decode_message(msg)
 
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self._init_queue(handler.queue)
         if handler.exchange is not None and handler.exchange.name != "default":
             exchange = await self._init_exchange(handler.exchange)
-            await queue.bind(exchange, handler.queue.routing_key or handler.queue.name)
+            await queue.bind(
+                exchange,
+                routing_key=handler.queue.routing,
+                arguments=handler.queue.bind_arguments,
+            )
         return queue
 
     async def _init_queue(
         self,
         queue: RabbitQueue,
     ) -> aio_pika.abc.AbstractRobustQueue:
         return await self._channel.declare_queue(**queue.dict())
 
     async def _init_exchange(
         self,
         exchange: RabbitExchange,
     ) -> aio_pika.abc.AbstractRobustExchange:
-        return await self._channel.declare_exchange(**exchange.dict())
+        original = await self._channel.declare_exchange(**exchange.dict())
+
+        current = exchange
+        current_exch = original
+        while current.bind_to is not None:
+            parent_exch = await self._channel.declare_exchange(**current.bind_to.dict())
+            await current_exch.bind(
+                exchange=parent_exch,
+                routing_key=current.routing_key,
+                arguments=current.bind_arguments,
+            )
+            current = current.bind_to
+            current_exch = parent_exch
+
+        return original
 
     def _get_log_context(
         self,
         message: Optional[PropanMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
     ) -> Dict[str, Any]:
@@ -252,36 +262,42 @@
                     on_max=pika_message.reject,
                 )
 
             async with context:
                 r = await func(message)
                 if message.raw_message.reply_to:
                     await self.publish(
-                        r,
+                        message=r,
                         routing_key=pika_message.reply_to,
                         correlation_id=pika_message.correlation_id,
                     )
 
                 return r
 
         return wrapper
 
     @classmethod
     def _validate_message(
         cls: Type["RabbitBroker"],
         message: PikaSendableMessage,
+        persist: bool = False,
         callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
         **message_kwargs: Dict[str, Any],
     ) -> aio_pika.Message:
         if not isinstance(message, aio_pika.message.Message):
             message, content_type = super()._encode_message(message)
 
+            delivery_mode = (
+                DeliveryMode.PERSISTENT if persist else DeliveryMode.NOT_PERSISTENT
+            )
+
             message = aio_pika.Message(
                 message,
                 **{
+                    "delivery_mode": delivery_mode,
                     "content_type": content_type,
                     "reply_to": callback_queue,
                     "correlation_id": str(uuid4()),
                     **message_kwargs,
                 },
             )
```

### Comparing `propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.0.0/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         callback: bool = False,
         callback_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
         # message kwargs
         headers: Optional[aio_pika.abc.HeadersType] = None,
         content_type: Optional[str] = None,
         content_encoding: Optional[str] = None,
-        delivery_mode: Union[aio_pika.abc.DeliveryMode, int, None] = None,
+        persist: bool = False,
         priority: Optional[int] = None,
         correlation_id: Optional[str] = None,
         reply_to: Optional[str] = None,
         expiration: Optional[aio_pika.abc.DateType] = None,
         message_id: Optional[str] = None,
         timestamp: Optional[aio_pika.abc.DateType] = None,
         type: Optional[str] = None,
@@ -165,18 +165,14 @@
     ) -> Callable[[PropanMessage], T]: ...
     def _get_log_context(  # type: ignore[override]
         self,
         message: Optional[PropanMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
     ) -> Dict[str, Any]: ...
-    async def _init_channel(
-        self,
-        max_consumers: Optional[int] = None,
-    ) -> None: ...
     async def _init_handler(
         self,
         handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue: ...
     async def _init_queue(
         self,
         queue: RabbitQueue,
```

### Comparing `propan-0.0.9.4/propan/brokers/rabbit/schemas.py` & `propan-0.1.0.0/propan/brokers/rabbit/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,33 +11,43 @@
     "RabbitExchange",
     "Handler",
     "ExchangeType",
 )
 
 
 class RabbitQueue(Queue):
+    name: str = ""
     durable: bool = False
     exclusive: bool = False
     passive: bool = False
     auto_delete: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
 
-    routing_key: str = Field(default="", exclude=True)
+    bind_arguments: Optional[Dict[str, Any]] = Field(None, exclude=True)
+    routing_key: str = Field("", exclude=True)
+
+    @property
+    def routing(self) -> Optional[str]:
+        return self.routing_key or self.name or None
 
 
 class RabbitExchange(NameRequired):
     type: ExchangeType = ExchangeType.DIRECT
     durable: bool = False
     auto_delete: bool = False
     internal: bool = False
     passive: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
 
+    bind_to: Optional["RabbitExchange"] = Field(None, exclude=True)
+    bind_arguments: Optional[Dict[str, Any]] = Field(None, exclude=True)
+    routing_key: str = Field("", exclude=True)
+
 
 class Handler(BaseModel):
     callback: DecoratedCallable
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = None
```

### Comparing `propan-0.0.9.4/propan/cli/app.py` & `propan-0.1.0.0/propan/cli/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 import asyncio
 import logging
 from typing import Dict, List, Optional
 
 from anyio import create_memory_object_stream, create_task_group
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+from typing_extensions import Protocol
 
-from propan.brokers.model.broker_usecase import BrokerUsecase
 from propan.cli.supervisors.utils import set_exit
 from propan.cli.utils.parser import SettingField
 from propan.log import logger
-from propan.types import AsyncFunc, DecoratedCallableNone, NoneCallable
+from propan.types import AnyCallable, AsyncFunc, DecoratedCallableNone
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
 
+class Runnable(Protocol):
+    async def start(self) -> None:
+        ...
+
+    async def close(self) -> None:
+        ...
+
+
 class PropanApp:
     _on_startup_calling: List[AsyncFunc]
     _on_shutdown_calling: List[AsyncFunc]
 
     _stop_stream: Optional[MemoryObjectSendStream[bool]]
     _receive_stream: Optional[MemoryObjectReceiveStream[bool]]
 
     def __init__(
         self,
-        broker: Optional[BrokerUsecase] = None,
+        broker: Optional[Runnable] = None,
         logger: Optional[logging.Logger] = logger,
     ):
         self.broker = broker
         self.logger = logger
         self.context = context
         context.set_global("app", self)
 
         self._on_startup_calling = []
         self._on_shutdown_calling = []
         self._stop_stream = None
         self._receive_stream = None
         self._command_line_options: Dict[str, SettingField] = {}
 
-    def set_broker(self, broker: BrokerUsecase) -> None:
+    def set_broker(self, broker: Runnable) -> None:
         self.broker = broker
 
-    def on_startup(self, func: NoneCallable) -> DecoratedCallableNone:
+    def on_startup(self, func: AnyCallable) -> DecoratedCallableNone:
         f: AsyncFunc = apply_types(to_async(func))
         self._on_startup_calling.append(f)
         return func
 
-    def on_shutdown(self, func: NoneCallable) -> DecoratedCallableNone:
+    def on_shutdown(self, func: AnyCallable) -> DecoratedCallableNone:
         f: AsyncFunc = apply_types(to_async(func))
         self._on_shutdown_calling.append(f)
         return func
 
     async def run(self, log_level: int = logging.INFO) -> None:
         self._init_async_cycle()
         async with create_task_group() as tg:
```

### Comparing `propan-0.0.9.4/propan/cli/main.py` & `propan-0.1.0.0/propan/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Optional
 
 import typer
 
 from propan.__about__ import __version__
 from propan.cli.app import PropanApp
 from propan.cli.utils.imports import get_app_path, import_object
-from propan.cli.utils.logs import LogLevels, set_log_level
+from propan.cli.utils.logs import LogLevels, get_log_level, set_log_level
 from propan.cli.utils.parser import SettingField, parse_cli_args
 from propan.log import logger
 
 cli = typer.Typer()
 
 
 def version_callback(version: bool) -> None:
@@ -73,66 +73,68 @@
     ),
     reload: bool = typer.Option(
         False, "--reload", is_flag=True, help="Restart app at directory files changes"
     ),
 ) -> None:
     """Run [MODULE:APP] Propan application"""
     app, extra = parse_cli_args(app, *ctx.args)
+    casted_log_level = get_log_level(log_level)
 
     module, app = get_app_path(app)
 
     app_dir = module.parent
     sys.path.insert(0, str(app_dir))
 
-    args = (module, app, extra)
+    args = (module, app, extra, casted_log_level)
 
     if reload and workers > 1:
         raise ValueError("You can't use reload option with multiprocessing")
 
-    set_log_level(log_level)
-
     if reload is True:
         from propan.cli.supervisors.watchfiles import WatchReloader
 
         WatchReloader(target=_run, args=args, reload_dirs=(app_dir,)).run()
 
     elif workers > 1:
         from propan.cli.supervisors.multiprocess import Multiprocess
 
         Multiprocess(target=_run, args=(*args, logging.DEBUG), workers=workers).run()
 
     else:
-        _run(module=module, app=app, extra_options=extra)
+        _run(module=module, app=app, extra_options=extra, log_level=casted_log_level)
 
 
 def _run(
     module: Path,
     app: str,
     extra_options: Dict[str, SettingField],
     log_level: int = logging.INFO,
+    app_level: int = logging.INFO,
 ) -> None:
     try:
         propan_app = import_object(module, app)
 
         if not isinstance(propan_app, PropanApp):
             raise ValueError(f"{propan_app} is not a PropanApp")
 
     except (ValueError, FileNotFoundError, AttributeError) as e:
         logger.error(e)
         logger.error("Please, input module like [python_file:propan_app_name]")
         exit()
 
     else:
+        set_log_level(log_level, propan_app)
+
         propan_app._command_line_options = extra_options
 
         if sys.platform not in ("win32", "cygwin", "cli"):
             import uvloop
 
             if sys.version_info >= (3, 11):
                 with asyncio.Runner(loop_factory=uvloop.new_event_loop) as runner:
-                    runner.run(propan_app.run(log_level))
+                    runner.run(propan_app.run(log_level=app_level))
                     return
 
             else:
                 uvloop.install()
 
-        asyncio.run(propan_app.run(log_level))
+        asyncio.run(propan_app.run(log_level=app_level))
```

### Comparing `propan-0.0.9.4/propan/cli/startproject.py` & `propan-0.1.0.0/propan/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/supervisors/basereload.py` & `propan-0.1.0.0/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/supervisors/multiprocess.py` & `propan-0.1.0.0/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/supervisors/utils.py` & `propan-0.1.0.0/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/supervisors/watchfiles.py` & `propan-0.1.0.0/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/utils/imports.py` & `propan-0.1.0.0/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/cli/utils/parser.py` & `propan-0.1.0.0/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/fastapi/core/route.py` & `propan-0.1.0.0/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/fastapi/core/router.py` & `propan-0.1.0.0/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.pyi` & `propan-0.1.0.0/propan/fastapi/rabbit/rabbit_router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/log/formatter.py` & `propan-0.1.0.0/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/log/logging.py` & `propan-0.1.0.0/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/test/rabbit.py` & `propan-0.1.0.0/propan/test/rabbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,10 +143,9 @@
             if callback:
                 return r
 
 
 def TestRabbitBroker(broker: RabbitBroker) -> RabbitBroker:
     broker._channel = AsyncMock()
     broker.connect = AsyncMock()  # type: ignore
-    broker._init_channel = AsyncMock()  # type: ignore
     broker.publish = MethodType(publish, broker)  # type: ignore
     return broker
```

### Comparing `propan-0.0.9.4/propan/utils/context/main.py` & `propan-0.1.0.0/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/propan/utils/context/types.py` & `propan-0.1.0.0/propan/utils/context/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from fast_depends.library import CustomField
 
 from propan.types import AnyDict
 from propan.utils.context import context
 
 
-class Context(CustomField):
+class Context(CustomField):  # type: ignore
     def __init__(
         self, real_name: str = "", *, cast: bool = False, default: Any = _empty
     ):
         self.name = real_name
         self.default = default
         super().__init__(cast=cast, required=(default is _empty))
```

### Comparing `propan-0.0.9.4/LICENSE` & `propan-0.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.4/README.md` & `propan-0.1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
+**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
@@ -76,15 +76,15 @@
 
 ---
 
 ## Declarative?
 
 With declarative tools you should define **what you need to get**. With traditional imperative tools you should write **what you need to do**.
 
-Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc. 
+Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc.
 
 This is the **Quickstart** with the *aio-pika*:
 
 ```python
 import asyncio
 import aio_pika
```

### Comparing `propan-0.0.9.4/pyproject.toml` & `propan-0.1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 homepage = "https://github.com/Lancetnik/Propan"
 keywords = ["rabbitmq", "framework", "message brokers"]
 
 requires-python = ">=3.7"
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -41,15 +41,15 @@
     "Environment :: Web Environment",
     "Framework :: AsyncIO",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "fast-depends>=1.1.1",
+    "fast-depends>=1.1.3",
     "watchfiles",
     "typer",
     "uvloop>=0.14.0,!=0.15.0,!=0.15.1; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')",
 ]
 
 dynamic = ["version"]
```

### Comparing `propan-0.0.9.4/PKG-INFO` & `propan-0.1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.9.4
+Version: 0.1.0.0
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: framework,message brokers,rabbitmq
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -32,15 +32,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: fast-depends>=1.1.1
+Requires-Dist: fast-depends>=1.1.3
 Requires-Dist: typer
 Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles
 Provides-Extra: async-nats
 Requires-Dist: nats-py>=2; extra == 'async-nats'
 Provides-Extra: async-rabbit
 Requires-Dist: aio-pika>=9; extra == 'async-rabbit'
@@ -95,15 +95,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
+**Propan** - just *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
@@ -147,15 +147,15 @@
 
 ---
 
 ## Declarative?
 
 With declarative tools you should define **what you need to get**. With traditional imperative tools you should write **what you need to do**.
 
-Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc. 
+Take a look at classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py), etc.
 
 This is the **Quickstart** with the *aio-pika*:
 
 ```python
 import asyncio
 import aio_pika
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: propan Version: 0.0.9.4 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.0.0 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
-framework,message brokers,rabbitmq Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment Classifier: Framework :: AsyncIO
-Classifier: Framework :: Pydantic Classifier: Framework :: Pydantic :: 1
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Topic :: Internet Classifier:
-Topic :: Software Development Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Typing :: Typed Requires-Python: >=3.7 Requires-Dist: fast-
-depends>=1.1.1 Requires-Dist: typer Requires-Dist:
+framework,message brokers,rabbitmq Classifier: Development Status :: 5 -
+Production/Stable Classifier: Environment :: Web Environment Classifier:
+Framework :: AsyncIO Classifier: Framework :: Pydantic Classifier: Framework ::
+Pydantic :: 1 Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Information Technology Classifier: Intended Audience :: System
+Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Topic :: Internet
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Application Frameworks Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7
+Requires-Dist: fast-depends>=1.1.3 Requires-Dist: typer Requires-Dist:
 uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32' and (sys_platform !=
 'cygwin' and platform_python_implementation != 'PyPy') Requires-Dist:
 watchfiles Provides-Extra: async-nats Requires-Dist: nats-py>=2; extra ==
 'async-nats' Provides-Extra: async-rabbit Requires-Dist: aio-pika>=9; extra ==
 'async-rabbit' Provides-Extra: dev Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev' Requires-Dist: mypy==1.1.1; extra ==
 'dev' Requires-Dist: propan[doc]; extra == 'dev' Requires-Dist: propan[test];
@@ -41,15 +41,15 @@
 'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan
 [async-rabbit]; extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra ==
 'test' Requires-Dist: pytest-xdist[psutil]; extra == 'test' Requires-Dist:
 pytest>=7; extra == 'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
-# Propan **Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ
+# Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development
 toolkit, which existed only in HTTP-frameworks world until now. It's designed
 to create reactive microservices around Messaging_Architecture. It is a modern,
 high-level framework on top of popular specific Python brokers libraries, based
 on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://
 fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/
```

