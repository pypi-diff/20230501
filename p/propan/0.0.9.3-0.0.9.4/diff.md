# Comparing `tmp/propan-0.0.9.3.tar.gz` & `tmp/propan-0.0.9.4.tar.gz`

## Comparing `propan-0.0.9.3.tar` & `propan-0.0.9.4.tar`

### file list

```diff
@@ -1,87 +1,90 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.3/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__about__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__main__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/annotations.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/__init__.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/app.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/main.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/parser.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/rabbit_router.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/rabbit_router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/logging.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/classes.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/main.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/test.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 propan-0.0.9.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.3/LICENSE
--rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 propan-0.0.9.3/README.md
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 propan-0.0.9.3/pyproject.toml
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 propan-0.0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.4/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.0.9.4/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__about__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/__main__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/annotations.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/model/utils.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    10868 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/app.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/main.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/log/logging.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/test/__init__.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/test/rabbit.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/classes.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/main.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.9.4/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.4/scripts/test.sh
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 propan-0.0.9.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.4/LICENSE
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 propan-0.0.9.4/README.md
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 propan-0.0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    14468 2020-02-02 00:00:00.000000 propan-0.0.9.4/PKG-INFO
```

### Comparing `propan-0.0.9.3/CONTRIBUTING.md` & `propan-0.0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/SECURITY.md` & `propan-0.0.9.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/.github/workflows/documentation.yml` & `propan-0.0.9.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/.github/workflows/publish_coverage.yml` & `propan-0.0.9.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/.github/workflows/publish_pypi.yml` & `propan-0.0.9.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/.github/workflows/tests.yml` & `propan-0.0.9.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/3_lifespan_events.py` & `propan-0.0.9.4/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/4_cli_attributes_promotion.py` & `propan-0.0.9.4/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/5_publishing.py` & `propan-0.0.9.4/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/6_arguments_casting.py` & `propan-0.0.9.4/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/7_handler_errors_processing.py` & `propan-0.0.9.4/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/1_dependency_injection.py` & `propan-0.0.9.4/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/2_dependency_declaration.py` & `propan-0.0.9.4/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.9.4/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/5_dependency_nesting.py` & `propan-0.0.9.4/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.9.4/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/dependencies/7_annotated.py` & `propan-0.0.9.4/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/quart.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/examples/http_frameworks_integrations/tornado.py` & `propan-0.0.9.4/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/__init__.py` & `propan-0.0.9.4/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/annotations.py` & `propan-0.0.9.4/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/brokers/push_back_watcher.py` & `propan-0.0.9.4/propan/brokers/push_back_watcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from abc import ABC, abstractmethod
 from collections import Counter
 from logging import Logger
 from types import TracebackType
 from typing import Callable, Optional, Type
 
+from typing_extensions import Counter as CounterType
+
 from propan.utils.functions import call_or_await
 
 
 class BaseWatcher(ABC):
     max_tries: int
 
-    def __init__(self, max_tries: int = 0, logger: Optional[Logger] = None):
+    def __init__(
+        self,
+        max_tries: int = 0,
+        logger: Optional[Logger] = None,
+    ):
         self.logger = logger
         self.max_tries = max_tries
 
     @abstractmethod
     def add(self, message_id: str) -> None:
         raise NotImplementedError()
 
@@ -35,17 +41,21 @@
         return False
 
     def remove(self, message_id: str) -> None:
         pass
 
 
 class PushBackWatcher(BaseWatcher):
-    memory: "Counter[str]"
+    memory: CounterType[str]
 
-    def __init__(self, max_tries: int = 3, logger: Optional[Logger] = None):
+    def __init__(
+        self,
+        max_tries: int = 3,
+        logger: Optional[Logger] = None,
+    ):
         super().__init__(logger=logger, max_tries=max_tries)
         self.memory = Counter()
 
     def add(self, message_id: str) -> None:
         self.memory[message_id] += 1
 
     def is_max(self, message_id: str) -> bool:
```

### Comparing `propan-0.0.9.3/propan/brokers/model/broker_usecase.py` & `propan-0.0.9.4/propan/brokers/model/broker_usecase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,41 @@
+import json
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
-from time import perf_counter
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
-from propan.brokers.push_back_watcher import (
-    BaseWatcher,
-    FakePushBackWatcher,
-    PushBackWatcher,
+from propan.brokers.model.schemas import (
+    ContentType,
+    ContentTypes,
+    PropanMessage,
+    SendableModel,
 )
+from propan.brokers.model.utils import (
+    change_logger_handlers,
+    get_watcher,
+    set_message_context,
+    suppress_decor,
+)
+from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import (
     AnyCallable,
     DecodedMessage,
     DecoratedAsync,
     DecoratedCallable,
+    HandlerWrapper,
+    SendableMessage,
     Wrapper,
 )
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
+T = TypeVar("T")
+
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: List[Any]
     _connection: Any
     _fmt: str
@@ -61,162 +73,153 @@
     @abstractmethod
     async def _connect(self, *args: Any, **kwargs: Any) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
     async def publish(
         self,
-        message: Any,
+        message: SendableMessage,
         *args: Any,
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
         **kwargs: Any,
     ) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
     async def close(self) -> None:
         raise NotImplementedError()
 
     @abstractmethod
-    async def _decode_message(self, message: Any) -> DecodedMessage:
+    async def _parse_message(self, message: Any) -> PropanMessage:
         raise NotImplementedError()
 
     @abstractmethod
     def _process_message(
-        self, func: DecoratedCallable, watcher: Optional[BaseWatcher]
-    ) -> Wrapper:
+        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
+    ) -> Callable[[PropanMessage], T]:
         raise NotImplementedError()
 
-    async def start(self) -> None:
-        if self.logger is not None:
-            self._init_logger(self.logger)
-        await self.connect()
-
-    def _get_log_context(self, **kwargs: Any) -> Dict[str, Any]:
-        return {}
+    def _get_log_context(self, message: PropanMessage) -> Dict[str, Any]:
+        return {
+            "message_id": message.message_id[:10] if message else "",
+        }
 
     @abstractmethod
     def handle(
         self,
         *broker_args: Any,
         retry: Union[bool, int] = False,
         **broker_kwargs: Any,
-    ) -> Wrapper:
+    ) -> HandlerWrapper:
         raise NotImplementedError()
 
+    @staticmethod
+    async def _decode_message(message: PropanMessage) -> DecodedMessage:
+        body = message.body
+        m: DecodedMessage = body
+        if message.content_type is not None:
+            if ContentTypes.text.value in message.content_type:
+                m = body.decode()
+            elif ContentTypes.json.value in message.content_type:  # pragma: no branch
+                m = json.loads(body.decode())
+        return m
+
+    @staticmethod
+    def _encode_message(msg: SendableMessage) -> Tuple[bytes, Optional[ContentType]]:
+        return SendableModel.to_send(msg)
+
     @property
-    def fmt(self) -> str:
+    def fmt(self) -> str:  # pragma: no cover
         return self._fmt
 
-    def _init_logger(self, logger: logging.Logger) -> None:
-        for handler in logger.handlers:
-            formatter = handler.formatter
-            if formatter is not None:
-                use_colors = getattr(formatter, "use_colors", None)
-                if use_colors is not None:
-                    kwargs = {"use_colors": use_colors}
-                else:
-                    kwargs = {}
-                handler.setFormatter(type(formatter)(self.fmt, **kwargs))
+    async def start(self) -> None:
+        if self.logger is not None:
+            change_logger_handlers(self.logger, self.fmt)
+        await self.connect()
 
     async def __aenter__(self) -> "BrokerUsecase":
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.close()
 
     def _wrap_handler(
-        self, func: AnyCallable, retry: Union[bool, int], **broker_args: Any
+        self,
+        func: AnyCallable,
+        retry: Union[bool, int] = False,
+        **broker_args: Any,
     ) -> DecoratedAsync:
-        func = to_async(func)
+        f = to_async(func)
 
         if self._is_apply_types is True:
-            func = apply_types(func)
+            f = apply_types(f)
 
         if self.logger is not None:
-            func = self._log_execution(self.logger, **broker_args)(func)
+            f = self._log_execution(**broker_args)(f)
 
-        func = self._wrap_decode_message(func)
+        f = self._wrap_decode_message(f)
 
-        func = self._process_message(func, _get_watcher(self.logger, retry))
+        f = self._process_message(f, get_watcher(self.logger, retry))
 
-        func = _set_message_context(func)
+        f = self._wrap_parse_message(f)
 
-        func = suppress(func)
+        f = set_message_context(f)
 
-        return func
+        f = suppress_decor(f)
 
-    def _wrap_decode_message(self, func: AnyCallable) -> DecoratedCallable:
+        return f
+
+    def _wrap_decode_message(
+        self, func: Callable[..., Awaitable[T]]
+    ) -> Callable[[PropanMessage], Awaitable[T]]:
         @wraps(func)
-        async def wrapper(message: Any) -> Any:
+        async def wrapper(message: PropanMessage) -> T:
             return await func(await self._decode_message(message))
 
         return wrapper
 
-    def _log_execution(self, logger: logging.Logger, **broker_args: Any) -> Wrapper:
+    def _wrap_parse_message(
+        self, func: Callable[[PropanMessage], Awaitable[T]]
+    ) -> Callable[[Any], Awaitable[T]]:
+        @wraps(func)
+        async def wrapper(message: Any) -> T:
+            return await func(await self._parse_message(message))
+
+        return wrapper
+
+    def _log_execution(
+        self,
+        **broker_args: Any,
+    ) -> Wrapper:
         def decor(func: AnyCallable) -> DecoratedCallable:
             @wraps(func)
             async def wrapper(*args: Any, **kwargs: Any) -> Any:
                 message = context.get("message")
 
-                start = perf_counter()
-
                 log_context = self._get_log_context(message=message, **broker_args)
 
                 with context.scope("log_context", log_context):
-                    logger.log(self.log_level, "Received")
+                    self._log("Received")
 
                     try:
                         r = await func(*args, **kwargs)
                     except Exception as e:
-                        logger.error(repr(e))
+                        self._log(repr(e), logging.ERROR)
                         raise e
                     else:
-                        logger.log(
-                            self.log_level,
-                            f"Processed by {(perf_counter() - start):.4f}",
-                        )
+                        self._log("Processed")
                         return r
 
             return wrapper
 
         return decor
 
-    def _log(self, message: str, log_level: Optional[int] = None) -> None:
+    def _log(
+        self,
+        message: str,
+        log_level: Optional[int] = None,
+    ) -> None:
         if self.logger is not None:
             self.logger.log(level=(log_level or self.log_level), msg=message)
-
-
-def _get_watcher(
-    logger: Optional[logging.Logger], try_number: Union[bool, int] = True
-) -> Optional[BaseWatcher]:
-    watcher: Optional[BaseWatcher]
-    if try_number is True:
-        watcher = FakePushBackWatcher()
-    elif try_number is False:
-        watcher = None
-    else:
-        watcher = PushBackWatcher(logger=logger, max_tries=try_number)
-    return watcher
-
-
-def _set_message_context(func: AnyCallable) -> DecoratedCallable:
-    @wraps(func)
-    async def wrapper(message: Any) -> Any:
-        with context.scope("message", message):
-            return await func(message)
-
-    return wrapper
-
-
-def suppress(func: AnyCallable) -> DecoratedCallable:
-    @wraps(func)
-    async def wrapper(message: Any) -> Any:
-        try:
-            return await func(message)
-        except Exception:
-            pass
-
-    return wrapper
```

### Comparing `propan-0.0.9.3/propan/brokers/nats/nats_broker.py` & `propan-0.0.9.4/propan/brokers/nats/nats_broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import json
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Union
-from uuid import uuid4
+from typing import Any, Callable, Dict, List, Optional, TypeVar
 
 import nats
 from nats.aio.client import Client
 from nats.aio.msg import Msg
 
-from propan.brokers.model import BrokerUsecase, ContentTypes
+from propan.brokers.model import BrokerUsecase
+from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.types import AnyDict, DecoratedCallable
+from propan.types import AnyDict, DecoratedCallable, SendableMessage
+
+T = TypeVar("T")
 
 
 class NatsBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[Client]
 
     __max_queue_len: int
@@ -28,36 +29,39 @@
         self.__max_queue_len = 0
         self.__max_subject_len = 4
 
     async def _connect(self, *args: Any, **kwargs: Any) -> Client:
         return await nats.connect(*args, **kwargs)
 
     def handle(
-        self, subject: str, queue: str = "", *, retry: Union[bool, int] = False
+        self,
+        subject: str,
+        queue: str = "",
+        **original_kwargs,
     ) -> Callable[[DecoratedCallable], None]:
         i = len(subject)
         if i > self.__max_subject_len:
             self.__max_subject_len = i
 
         i = len(queue)
         if i > self.__max_queue_len:
             self.__max_queue_len = i
 
-        parent = super()
-
         def wrapper(func: DecoratedCallable) -> None:
             for handler in self.handlers:
                 if handler.subject == subject and handler.queue == queue:
                     raise ValueError(
                         f"`{func.__name__}` uses already "
                         f"using `{subject}` subject with "
                         f"`{queue}` queue"
                     )
 
-            func = parent._wrap_handler(func, retry, queue=queue, subject=subject)
+            func = self._wrap_handler(
+                func, queue=queue, subject=subject, **original_kwargs
+            )
             handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
@@ -71,80 +75,73 @@
                 self._get_log_context(None, handler.subject, handler.queue)
                 self.logger.info(f"`{func.__name__}` waiting for messages")
 
             sub = await self._connection.subscribe(handler.subject, cb=func)
             handler.subscription = sub
 
     async def publish(
-        self, message: Union[str, Dict[str, Any]], subject: str, **publish_args: Any
+        self,
+        message: SendableMessage,
+        subject: str,
+        **publish_args: Any,
     ) -> None:
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
-        if isinstance(message, dict):
-            message = json.dumps(message)
-            headers = {
-                **publish_args.pop("headers", {}),
-                "content-type": ContentTypes.json.value,
-            }
-        else:
-            headers = {
-                **publish_args.pop("headers", {}),
-                "content-type": ContentTypes.text.value,
-            }
+        msg, content_type = super()._encode_message(message)
 
         return await self._connection.publish(
-            subject, message.encode(), headers=headers, **publish_args
+            subject,
+            msg,
+            headers={
+                **publish_args.pop("headers", {}),
+                "content-type": content_type,
+            },
+            **publish_args,
         )
 
     async def close(self) -> None:
         for h in self.handlers:
             await h.subscription.unsubscribe()
 
         if self._connection:
             await self._connection.drain()
 
     def _get_log_context(
-        self, message: Optional[Msg], subject: str, queue: str = "", **kwargs
+        self,
+        message: Optional[PropanMessage],
+        subject: str,
+        queue: str = "",
     ) -> Dict[str, Any]:
-        if message is not None:
-            message_id = message.reply or uuid4().hex
-            message.message_id = message_id
-
         context = {
             "subject": subject,
             "queue": queue,
-            "message_id": message.message_id[:10] if message else "",
+            **super()._get_log_context(message),
         }
-
         return context
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(subject)-{self.__max_subject_len}s | "
             + (f"%(queue)-{self.__max_queue_len}s | " if self.__max_queue_len else "")
             + "%(message_id)-10s "
             "- %(message)s"
         )
 
-    @staticmethod
-    async def _decode_message(message: Msg) -> Union[str, dict, bytes]:
-        body = message.data
-        if message.header:
-            content_type = message.header.get("content-type", "")
-            if ContentTypes.json.value in content_type:
-                body = json.loads(body.decode())
-            elif ContentTypes.text.value in content_type:
-                body = body.decode()
-        return body
+    async def _parse_message(self, message: Msg) -> PropanMessage:
+        return PropanMessage(
+            body=message.dat,
+            content_type=message.header.get("content-type", ""),
+            headers=message.header,
+            raw_message=message,
+        )
 
-    @staticmethod
     def _process_message(
-        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> Callable[[Msg], Any]:
+        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher] = None
+    ) -> Callable[[PropanMessage], T]:
         @wraps(func)
-        async def wrapper(message: Msg):
+        async def wrapper(message: PropanMessage) -> T:
             return await func(message)
 
         return wrapper
```

### Comparing `propan-0.0.9.3/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.9.4/propan/brokers/nats/nats_broker.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import ssl
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
 
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
     DEFAULT_DRAIN_TIMEOUT,
     DEFAULT_INBOX_PREFIX,
     DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
     DEFAULT_MAX_OUTSTANDING_PINGS,
@@ -18,23 +18,26 @@
     ErrorCallback,
     JWTCallback,
     SignatureCallback,
 )
 from nats.aio.msg import Msg
 
 from propan.brokers.model import BrokerUsecase
+from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
-from propan.types import AnyDict, DecodedMessage, DecoratedCallable, Wrapper
+from propan.types import HandlerWrapper, SendableMessage
+
+T = TypeVar("T")
 
 class NatsBroker(BrokerUsecase):
     logger: logging.Logger
-    handlers: List[Handler] = []
-    _connection: Optional[Client] = None
+    handlers: List[Handler]
+    _connection: Optional[Client]
 
     def __init__(
         self,
         servers: Union[str, List[str]] = ["nats://localhost:4222"],  # noqa: B006
         error_cb: Optional[ErrorCallback] = None,
         disconnected_cb: Optional[Callback] = None,
         closed_cb: Optional[Callback] = None,
@@ -103,27 +106,35 @@
         nkeys_seed: Optional[str] = None,
         inbox_prefix: Union[str, bytes] = DEFAULT_INBOX_PREFIX,
         pending_size: int = DEFAULT_PENDING_SIZE,
         flush_timeout: Optional[float] = None,
     ) -> Client: ...
     async def publish(  # type: ignore[override]
         self,
-        message: Union[str, Dict[str, Any]],
+        message: SendableMessage,
         subject: str,
         reply: str = "",
         headers: Optional[Dict[str, str]] = None,
     ) -> None: ...
     def handle(  # type: ignore[override]
-        self, subject: str, queue: str = "", *, retry: Union[bool, int] = False
-    ) -> Wrapper: ...
+        self,
+        subject: str,
+        queue: str = "",
+        *,
+        retry: Union[bool, int] = False,
+    ) -> HandlerWrapper: ...
     async def __aenter__(self) -> "NatsBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
     async def close(self) -> None: ...
     def _get_log_context(  # type: ignore[override]
-        self, message: Optional[Msg], subject: str, queue: str = "", **kwargs: AnyDict
+        self,
+        message: Optional[PropanMessage],
+        subject: str,
+        queue: str = "",
     ) -> Dict[str, Any]: ...
-    @staticmethod
-    async def _decode_message(message: Msg) -> DecodedMessage: ...
-    @staticmethod
     def _process_message(
-        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> Wrapper: ...
+        self,
+        func: Callable[[PropanMessage], T],
+        watcher: Optional[BaseWatcher],
+    ) -> Callable[[PropanMessage], T]: ...
+    @staticmethod
+    async def _parse_message(message: Msg) -> PropanMessage: ...
```

### Comparing `propan-0.0.9.3/propan/brokers/nats/nats_js_broker.py` & `propan-0.0.9.4/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/brokers/nats/schemas.py` & `propan-0.0.9.4/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import asyncio
-import json
 import logging
 from functools import wraps
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
 import aio_pika
 import aiormq
-from pydantic import BaseModel
 
-from propan.brokers.model import BrokerUsecase, ContentTypes
+from propan.brokers.model import BrokerUsecase
+from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
-from propan.types import AnyDict, DecodedMessage, DecoratedCallable, Wrapper
-from propan.utils.functions import async_partial
+from propan.types import AnyDict, DecoratedCallable, SendableMessage, Wrapper
+from propan.utils.context import context as global_context
 
 TimeoutType = Optional[Union[int, float]]
+PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
+T = TypeVar("T")
 
 
 class RabbitBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
 
@@ -43,20 +44,31 @@
         self.__max_exchange_len = 4
 
     async def __aenter__(self) -> "RabbitBroker":
         await self.connect()
         await self._init_channel()
         return self
 
-    async def _connect(self, *args: Any, **kwargs: Any) -> aio_pika.Connection:
+    async def close(self) -> None:
+        if self._connection is not None:
+            await self._connection.close()
+
+    async def _connect(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> aio_pika.Connection:
         return await aio_pika.connect_robust(
             *args, **kwargs, loop=asyncio.get_event_loop()
         )
 
-    async def _init_channel(self, max_consumers: Optional[int] = None) -> None:
+    async def _init_channel(
+        self,
+        max_consumers: Optional[int] = None,
+    ) -> None:
         if self._channel is None:
             if self._connection is None:
                 raise ValueError("RabbitBroker not connected yet")
 
             max_consumers = max_consumers or self._max_consumers
             self._channel = await self._connection.channel()
 
@@ -64,38 +76,35 @@
                 self._log(f"Set max consumers to {max_consumers}", logging.INFO)
                 await self._channel.set_qos(prefetch_count=int(max_consumers))
 
     def handle(
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
-        *,
-        retry: Union[bool, int] = False,
+        **original_kwargs,
     ) -> Wrapper:
         queue, exchange = _validate_queue(queue), _validate_exchange(exchange)
 
-        if exchange:
-            i = len(exchange.name)
-            if i > self.__max_exchange_len:  # pragma: no branch
-                self.__max_exchange_len = i
-
-        i = len(queue.name)
-        if i > self.__max_queue_len:  # pragma: no branch
-            self.__max_queue_len = i
+        self.__setup_log_context(queue, exchange)
 
         def wrapper(func: DecoratedCallable) -> Any:
             for handler in self.handlers:
                 if handler.exchange == exchange and handler.queue == queue:
                     raise ValueError(
                         f"`{func.__name__}` uses already "
                         f"using `{queue.name}` queue to listen "
                         f"`{exchange.name if exchange else 'default'}` exchange"
                     )
 
-            func = self._wrap_handler(func, retry, queue=queue, exchange=exchange)
+            func = self._wrap_handler(
+                func,
+                queue=queue,
+                exchange=exchange,
+                **original_kwargs,
+            )
             handler = Handler(callback=func, queue=queue, exchange=exchange)
             self.handlers.append(handler)
 
             return func
 
         return wrapper
 
@@ -105,22 +114,23 @@
 
         for handler in self.handlers:
             queue = await self._init_handler(handler)
 
             func = handler.callback
 
             if self.logger is not None:
-                self._get_log_context(None, handler.queue, handler.exchange)
+                context = self._get_log_context(None, handler.queue, handler.exchange)
+                global_context.set_local("log_context", context)
                 self.logger.info(f"`{func.__name__}` waiting for messages")
 
             await queue.consume(func)
 
     async def publish(
         self,
-        message: Union[aio_pika.Message, str, Dict[str, Any], BaseModel] = "",
+        message: PikaSendableMessage = "",
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
         *,
         routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
         timeout: TimeoutType = None,
@@ -140,178 +150,180 @@
             callback_queue = None
 
         if exchange is None:
             exchange_obj = self._channel.default_exchange
         else:
             exchange_obj = await self._init_exchange(exchange)
 
-        message = _validate_message(message, callback_queue, **message_kwargs)
+        message = self._validate_message(message, callback_queue, **message_kwargs)
 
         r = await exchange_obj.publish(
             message=message,
             routing_key=routing_key or queue.name,
             mandatory=mandatory,
             immediate=immediate,
             timeout=timeout,
         )
 
         if callback_queue is None:
             return r
 
         else:
-            async with callback_queue.iterator() as queue_iterator:
-                try:
-                    message = await asyncio.wait_for(
-                        anext(queue_iterator), timeout=callback_timeout
-                    )
-                except asyncio.TimeoutError as e:
-                    if raise_timeout is True:
-                        raise e
-                else:
-                    return await self._decode_message(message)
+            try:
+                async with callback_queue.iterator(
+                    timeout=callback_timeout
+                ) as queue_iterator:
+                    async for m in queue_iterator:  # pragma: no branch
+                        return await self._decode_message(m)
+            except asyncio.TimeoutError as e:
+                if raise_timeout is True:  # pragma: no branch
+                    raise e
 
-    async def close(self) -> None:
-        if self._connection is not None:
-            await self._connection.close()
-
-    async def _init_handler(self, handler: Handler) -> aio_pika.abc.AbstractRobustQueue:
+    async def _init_handler(
+        self,
+        handler: Handler,
+    ) -> aio_pika.abc.AbstractRobustQueue:
         queue = await self._init_queue(handler.queue)
         if handler.exchange is not None and handler.exchange.name != "default":
             exchange = await self._init_exchange(handler.exchange)
             await queue.bind(exchange, handler.queue.routing_key or handler.queue.name)
         return queue
 
-    async def _init_queue(self, queue: RabbitQueue) -> aio_pika.abc.AbstractRobustQueue:
-        if queue.declare is True:
-            return await self._channel.declare_queue(**queue.dict())
-        else:
-            return await self._channel.get_queue(queue.name, ensure=False)
+    async def _init_queue(
+        self,
+        queue: RabbitQueue,
+    ) -> aio_pika.abc.AbstractRobustQueue:
+        return await self._channel.declare_queue(**queue.dict())
 
     async def _init_exchange(
-        self, exchange: RabbitExchange
+        self,
+        exchange: RabbitExchange,
     ) -> aio_pika.abc.AbstractRobustExchange:
-        if exchange.declare is True:
-            return await self._channel.declare_exchange(**exchange.dict())
-        else:
-            return await self._channel.get_exchange(exchange.name, ensure=False)
+        return await self._channel.declare_exchange(**exchange.dict())
 
     def _get_log_context(
         self,
-        message: Optional[aio_pika.Message],
+        message: Optional[PropanMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
-        **kwrags,
     ) -> Dict[str, Any]:
-        exchange_name = exchange.name if exchange else "default"
         context = {
-            "exchange": exchange_name,
             "queue": queue.name,
-            "message_id": message.message_id[:10] if message else "",
+            "exchange": exchange.name if exchange else "default",
+            **super()._get_log_context(message),
         }
-
         return context
 
     @property
     def fmt(self) -> str:
-        return self._fmt or (
+        return super().fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(exchange)-{self.__max_exchange_len}s | "
             f"%(queue)-{self.__max_queue_len}s | "
             f"%(message_id)-10s "
             "- %(message)s"
         )
 
     @staticmethod
-    async def _decode_message(
-        message: aio_pika.IncomingMessage,
-    ) -> DecodedMessage:
-        body = message.body
-        if message.content_type is not None:
-            if ContentTypes.text.value in message.content_type:
-                body = body.decode()
-            elif ContentTypes.json.value in message.content_type:  # pragma: no branch
-                body = json.loads(body.decode())
-        return body
+    async def _parse_message(
+        message: aio_pika.message.IncomingMessage,
+    ) -> PropanMessage:
+        return PropanMessage(
+            body=message.body,
+            headers=message.headers,
+            message_id=message.message_id,
+            content_type=message.content_type or "",
+            raw_message=message,
+        )
 
     def _process_message(
-        self, func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> DecoratedCallable:
+        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
+    ) -> Callable[[PropanMessage], T]:
         @wraps(func)
-        async def wrapper(message: aio_pika.IncomingMessage):
+        async def wrapper(message: PropanMessage) -> T:
+            pika_message = message.raw_message
             if watcher is None:
-                context = message.process()
+                context = pika_message.process()
             else:
                 context = WatcherContext(
                     watcher,
                     message.message_id,
-                    on_success=message.ack,
-                    on_error=async_partial(message.reject, True),
-                    on_max=async_partial(message.reject, False),
+                    on_success=pika_message.ack,
+                    on_error=pika_message.nack,
+                    on_max=pika_message.reject,
                 )
 
             async with context:
                 r = await func(message)
-                if message.reply_to:
+                if message.raw_message.reply_to:
                     await self.publish(
                         r,
-                        routing_key=message.reply_to,
-                        correlation_id=message.correlation_id,
+                        routing_key=pika_message.reply_to,
+                        correlation_id=pika_message.correlation_id,
                     )
 
                 return r
 
         return wrapper
 
+    @classmethod
+    def _validate_message(
+        cls: Type["RabbitBroker"],
+        message: PikaSendableMessage,
+        callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
+        **message_kwargs: Dict[str, Any],
+    ) -> aio_pika.Message:
+        if not isinstance(message, aio_pika.message.Message):
+            message, content_type = super()._encode_message(message)
+
+            message = aio_pika.Message(
+                message,
+                **{
+                    "content_type": content_type,
+                    "reply_to": callback_queue,
+                    "correlation_id": str(uuid4()),
+                    **message_kwargs,
+                },
+            )
+
+        return message
+
+    def __setup_log_context(
+        self,
+        queue: Optional[RabbitQueue] = None,
+        exchange: Optional[RabbitExchange] = None,
+    ) -> None:
+        if exchange is not None:
+            i = len(exchange.name)
+            if i > self.__max_exchange_len:  # pragma: no branch
+                self.__max_exchange_len = i
+
+        if queue is not None:  # pragma: no branch
+            i = len(queue.name)
+            if i > self.__max_queue_len:  # pragma: no branch
+                self.__max_queue_len = i
+
 
 def _validate_exchange(
     exchange: Union[str, RabbitExchange, None] = None,
 ) -> Optional[RabbitExchange]:
     if exchange is not None:  # pragma: no branch
         if isinstance(exchange, str):
             exchange = RabbitExchange(name=exchange)
         elif not isinstance(exchange, RabbitExchange):
             raise ValueError(
                 f"Exchange '{exchange}' should be 'str' | 'RabbitExchange' instance"
             )
-
     return exchange
 
 
 def _validate_queue(
     queue: Union[str, RabbitQueue, None] = None
 ) -> Optional[RabbitQueue]:
     if queue is not None:  # pragma: no branch
         if isinstance(queue, str):
             queue = RabbitQueue(name=queue)
         elif not isinstance(queue, RabbitQueue):
             raise ValueError(
                 f"Queue '{queue}' should be 'str' | 'RabbitQueue' instance"
             )
     return queue
-
-
-def _validate_message(
-    message: Union[aio_pika.Message, str, Dict[str, Any], BaseModel],
-    callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
-    **message_kwargs: Dict[str, Any],
-) -> aio_pika.Message:
-    if not isinstance(message, aio_pika.message.Message):
-        if isinstance(message, BaseModel):
-            message = message.json()
-            content_type = ContentTypes.json.value
-        elif isinstance(message, dict):
-            message = json.dumps(message)
-            content_type = ContentTypes.json.value
-        else:
-            content_type = ContentTypes.text.value
-
-        message = aio_pika.Message(
-            message.encode(),
-            **{
-                "content_type": content_type,
-                "reply_to": callback_queue,
-                "correlation_id": str(uuid4()),
-                **message_kwargs,
-            },
-        )
-
-    return message
```

### Comparing `propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.9.4/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import logging
 from ssl import SSLContext
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Type, TypeVar, Union
 
 import aio_pika
 import aiormq
 from pamqp.common import FieldTable
-from pydantic import BaseModel
+from typing_extensions import ParamSpec
 from yarl import URL
 
 from propan.brokers.model import BrokerUsecase
+from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
-from propan.types import AnyDict, DecodedMessage, DecoratedCallable, Wrapper
+from propan.types import SendableMessage
+
+P = ParamSpec("P")
+T = TypeVar("T")
+PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 
 class RabbitBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
 
     __max_queue_len: int
@@ -98,15 +103,15 @@
 
         .. _RFC3986: https://goo.gl/MzgYAs
         .. _official Python documentation: https://goo.gl/pty9xA
         """
         ...
     async def publish(  # type: ignore[override]
         self,
-        message: Union[aio_pika.Message, str, Dict[str, Any], BaseModel] = "",
+        message: PikaSendableMessage = "",
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
         *,
         # publish kwargs
         routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
@@ -132,41 +137,63 @@
     ) -> Optional[aiormq.abc.ConfirmationFrameType]: ...
     def handle(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         retry: Union[bool, int] = False,
-    ) -> Wrapper:
+    ) -> Callable[
+        [
+            Callable[
+                P, Union[PikaSendableMessage, Coroutine[Any, Any, PikaSendableMessage]]
+            ]
+        ],
+        Callable[P, PikaSendableMessage],
+    ]:
         """
         retry: Union[bool, int] - at exeption message will returns to queue `int` times or endless if `True`
         """
         ...
     async def __aenter__(self) -> "RabbitBroker": ...
-    async def _connect(self, *args: Any, **kwargs: Any) -> aio_pika.Connection: ...
+    async def _connect(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> aio_pika.Connection: ...
     async def close(self) -> None: ...
-    @staticmethod
-    async def _decode_message(
-        message: aio_pika.IncomingMessage,
-    ) -> DecodedMessage: ...
-    @staticmethod
     def _process_message(
-        func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> DecoratedCallable: ...
+        self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
+    ) -> Callable[[PropanMessage], T]: ...
     def _get_log_context(  # type: ignore[override]
         self,
-        message: Optional[aio_pika.Message],
+        message: Optional[PropanMessage],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
-        **kwrags: AnyDict,
     ) -> Dict[str, Any]: ...
-    async def _init_channel(self, max_consumers: Optional[int] = None) -> None: ...
+    async def _init_channel(
+        self,
+        max_consumers: Optional[int] = None,
+    ) -> None: ...
     async def _init_handler(
-        self, handler: Handler
+        self,
+        handler: Handler,
     ) -> aio_pika.abc.AbstractRobustQueue: ...
     async def _init_queue(
-        self, queue: RabbitQueue
+        self,
+        queue: RabbitQueue,
     ) -> aio_pika.abc.AbstractRobustQueue: ...
     async def _init_exchange(
-        self, exchange: RabbitExchange
+        self,
+        exchange: RabbitExchange,
     ) -> aio_pika.abc.AbstractRobustExchange: ...
     async def start(self) -> None: ...
+    @classmethod
+    def _validate_message(
+        cls: Type["RabbitBroker"],
+        message: PikaSendableMessage,
+        callback_queue: Optional[aio_pika.abc.AbstractRobustQueue] = None,
+        **message_kwargs: Dict[str, Any],
+    ) -> aio_pika.Message: ...
+    @staticmethod
+    async def _parse_message(
+        message: aio_pika.message.IncomingMessage,
+    ) -> PropanMessage: ...
```

### Comparing `propan-0.0.9.3/propan/brokers/rabbit/schemas.py` & `propan-0.0.9.4/propan/brokers/rabbit/schemas.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 from aio_pika.abc import ExchangeType, TimeoutType
 from pydantic import BaseModel, Field
 
 from propan.brokers.model.schemas import NameRequired, Queue
 from propan.types import DecoratedCallable
 
@@ -19,28 +19,25 @@
     exclusive: bool = False
     passive: bool = False
     auto_delete: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
 
-    declare: bool = Field(default=True, exclude=True)
     routing_key: str = Field(default="", exclude=True)
 
 
 class RabbitExchange(NameRequired):
-    type: Union[ExchangeType, str] = ExchangeType.DIRECT
+    type: ExchangeType = ExchangeType.DIRECT
     durable: bool = False
     auto_delete: bool = False
     internal: bool = False
     passive: bool = False
     arguments: Optional[Dict[str, Any]] = None
     timeout: TimeoutType = None
     robust: bool = True
 
-    declare: bool = Field(default=True, exclude=True)
-
 
 class Handler(BaseModel):
     callback: DecoratedCallable
     queue: RabbitQueue
     exchange: Optional[RabbitExchange] = None
```

### Comparing `propan-0.0.9.3/propan/cli/app.py` & `propan-0.0.9.4/propan/cli/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,9 +92,9 @@
         ):
             await self.broker.close()
 
         for func in self._on_shutdown_calling:
             await func()
 
     async def __exit(self, flag: bool) -> None:
-        if self._stop_stream is not None:
+        if self._stop_stream is not None:  # pragma: no branch
             await self._stop_stream.send(flag)
```

### Comparing `propan-0.0.9.3/propan/cli/main.py` & `propan-0.0.9.4/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/startproject.py` & `propan-0.0.9.4/propan/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/supervisors/basereload.py` & `propan-0.0.9.4/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/supervisors/multiprocess.py` & `propan-0.0.9.4/propan/cli/supervisors/multiprocess.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from propan.cli.supervisors.basereload import BaseReload
 from propan.log import logger
 from propan.types import DecoratedCallable
 
 
 class Multiprocess(BaseReload):
     def __init__(
-        self, target: DecoratedCallable, args: Tuple[Any, ...], workers: int
+        self,
+        target: DecoratedCallable,
+        args: Tuple[Any, ...],
+        workers: int,
     ) -> None:
         super().__init__(target, args, None)
 
         self.workers = workers
         self.processes: List[SpawnProcess] = []
 
     def startup(self) -> None:
```

### Comparing `propan-0.0.9.3/propan/cli/supervisors/utils.py` & `propan-0.0.9.4/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/supervisors/watchfiles.py` & `propan-0.0.9.4/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/utils/imports.py` & `propan-0.0.9.4/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/cli/utils/logs.py` & `propan-0.0.9.4/propan/cli/utils/logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from collections import defaultdict
 from enum import Enum
-from typing import Union
+from typing import DefaultDict, Union
 
 from propan.log import access_logger, logger
 
 
 class LogLevels(str, Enum):
     critical = "critical"
     error = "error"
     warning = "warning"
     info = "info"
     debug = "debug"
 
 
-LOG_LEVELS: "defaultdict[str, int]" = defaultdict(
+LOG_LEVELS: DefaultDict[str, int] = defaultdict(
     lambda: logging.INFO,
     **{
         "critical": logging.CRITICAL,
         "error": logging.ERROR,
         "warning": logging.WARNING,
         "info": logging.INFO,
         "debug": logging.DEBUG,
```

### Comparing `propan-0.0.9.3/propan/cli/utils/parser.py` & `propan-0.0.9.4/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/fastapi/core/route.py` & `propan-0.0.9.4/propan/fastapi/core/route.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,88 +4,95 @@
 from typing import Any, Callable, Coroutine, Optional, Union
 
 from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_dependant, solve_dependencies
 from fastapi.routing import run_endpoint_function
 from pydantic import ValidationError, create_model
 from starlette.requests import Request
-from starlette.routing import BaseRoute, get_name
+from starlette.routing import BaseRoute
 
 from propan.brokers.model import BrokerUsecase
 from propan.types import AnyDict
 
 NativeMessage = Union[str, AnyDict, bytes]
 
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
         broker: BrokerUsecase,
         *,
-        name: Optional[str] = None,
         dependency_overrides_provider: Optional[Any] = None,
         **hanle_kwargs: AnyDict,
     ) -> None:
-        self.broker = broker
         self.path = path
-        self.endpoint = endpoint
-        self.name = name if name else get_name(endpoint)
-        self.dependant = get_dependant(path=path, call=self.endpoint)
+        self.broker = broker
+        self.dependant = get_dependant(path=path, call=endpoint)
 
-        broker.handle(path, **hanle_kwargs)(  # type: ignore
-            PropanMessage.get_session(self.dependant, dependency_overrides_provider)
+        handler = PropanMessage.get_session(
+            self.dependant, dependency_overrides_provider
         )
+        broker.handle(path, **hanle_kwargs)(handler)  # type: ignore
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
-    _headers: AnyDict
-    _body: AnyDict
-    _query_params: AnyDict
+    _headers: AnyDict  # type: ignore
+    _body: AnyDict  # type: ignore
+    _query_params: AnyDict  # type: ignore
 
-    def __init__(self, body: AnyDict, headers: Optional[AnyDict] = None):
+    def __init__(
+        self,
+        body: Optional[AnyDict] = None,
+        headers: Optional[AnyDict] = None,
+    ):
         self.scope = {}
         self._cookies = {}
         self._headers = headers or {}
-        self._body = body
+        self._body = body or {}
         self._query_params = self._body
 
     @classmethod
     def get_session(
-        connection_class,
+        cls,
         dependant: Dependant,
         dependency_overrides_provider: Optional[Any] = None,
     ) -> Callable[[NativeMessage], Any]:
         assert dependant.call
         func = get_app(dependant, dependency_overrides_provider)
 
         dependencies_names = tuple(i.name for i in dependant.dependencies)
 
         first_arg = next(
             dropwhile(
                 lambda i: i in dependencies_names,
                 inspect.signature(dependant.call).parameters,
-            )
+            ),
+            None,
         )
 
         async def app(message: NativeMessage) -> Any:
-            if not isinstance(message, dict):
-                message = {first_arg: message}
-
-            session = connection_class(message)
+            if first_arg is not None:
+                if not isinstance(message, dict):  # pragma: no branch
+                    message = {first_arg: message}
+
+                session = cls(message)
+            else:
+                session = cls()
             return await func(session)
 
         return app
 
 
 def get_app(
-    dependant: Dependant, dependency_overrides_provider: Optional[Any] = None
+    dependant: Dependant,
+    dependency_overrides_provider: Optional[Any] = None,
 ) -> Callable[[PropanMessage], Coroutine[Any, Any, Any]]:
     async def app(request: PropanMessage) -> Any:
         solved_result = await solve_dependencies(
             request=request,
             body=request._body,
             dependant=dependant,
             dependency_overrides_provider=dependency_overrides_provider,
```

### Comparing `propan-0.0.9.3/propan/fastapi/core/router.py` & `propan-0.0.9.4/propan/fastapi/core/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 
 class PropanRouter(APIRouter):
     broker_class: ClassVar[Type[BrokerUsecase]]
     broker: BrokerUsecase
 
     @property
     def mq_routes(self) -> Tuple[PropanRoute, ...]:
-        return tuple(filter(lambda x: isinstance(x, PropanRoute), self.routes))
+        return tuple(
+            filter(lambda x: isinstance(x, PropanRoute), self.routes)  # type: ignore
+        )
 
     async def _connect(self) -> None:
         await self.broker.start()
 
     async def _close(self) -> None:
         await self.broker.close()
 
@@ -84,33 +86,32 @@
         )
 
     def add_api_mq_route(
         self,
         path: str,
         *,
         endpoint: Callable[..., Any],
-        name: Optional[str] = None,
         **broker_kwargs: AnyDict,
     ) -> None:
         route = PropanRoute(
             path,
             endpoint=endpoint,
-            name=name,
             dependency_overrides_provider=self.dependency_overrides_provider,
             broker=self.broker,
             **broker_kwargs,
         )
         self.routes.append(route)
 
     def event(
-        self, path: str, *, name: Optional[str] = None, **broker_kwargs: Dict[str, Any]
+        self,
+        path: str,
+        **broker_kwargs: Dict[str, Any],
     ) -> Callable[[DecoratedCallable], DecoratedCallable]:
         def decorator(func: DecoratedCallable) -> DecoratedCallable:
             self.add_api_mq_route(
                 path,
                 endpoint=func,
-                name=name,
                 **broker_kwargs,
             )
             return func
 
         return decorator
```

### Comparing `propan-0.0.9.3/propan/fastapi/rabbit/rabbit_router.pyi` & `propan-0.0.9.4/propan/fastapi/rabbit/rabbit_router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/log/formatter.py` & `propan-0.0.9.4/propan/log/formatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import sys
 from collections import defaultdict
-from typing import Callable, Optional
-from typing_extensions import Literal
+from typing import Callable, DefaultDict, Optional
 
 import click
+from typing_extensions import Literal
 
 from propan.utils.context.main import context
 
 
 class ColourizedFormatter(logging.Formatter):
-    level_name_colors: "defaultdict[str, Callable[[str], str]]" = defaultdict(
+    level_name_colors: DefaultDict[str, Callable[[str], str]] = defaultdict(
         lambda: str,
         **{
             str(logging.DEBUG): lambda level_name: click.style(
                 str(level_name), fg="cyan"
             ),
             str(logging.INFO): lambda level_name: click.style(
                 str(level_name), fg="green"
```

### Comparing `propan-0.0.9.3/propan/log/logging.py` & `propan-0.0.9.4/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/propan/utils/context/main.py` & `propan-0.0.9.4/propan/utils/context/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return context_var.set(value)
 
     def reset_local(self, key: str, tag: "Token[Any]") -> None:
         self._scope_context[key].reset(tag)
 
     def get_local(self, key: str) -> Any:
         context_var = self._scope_context.get(key)
-        if context_var is not None:
+        if context_var is not None:  # pragma: no branch
             return context_var.get()
 
     def clear(self) -> None:
         self._global_context = {}
         self._scope_context = {}
 
     def get(self, key: str) -> Any:
```

### Comparing `propan-0.0.9.3/propan/utils/context/types.py` & `propan-0.0.9.4/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/LICENSE` & `propan-0.0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.3/README.md` & `propan-0.0.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *<s>an another one HTTP</s>* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
+**Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
@@ -44,20 +44,21 @@
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
-    * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
-    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
-* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
+  * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
+  * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
+* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/5_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Greate to develop**](#cli-power): CLI tool provides great development experience:
-    * framework-independent way to rule application environment
-    * application code hot reloading
+  * framework-independent way to rule application environment
+  * application code hot reloading
+* [**Testability**](https://lancetnik.github.io/Propan/2_getting_started/7_testing): **Propan** allows you to test your app without external dependencies: you shouldn't suit up a Message Broker, use a virtual one!
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Nats**     | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**   | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
@@ -190,50 +191,55 @@
 ## Dependencies
 
 **Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
 Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existing field, raises *pydantic.error_wrappers.ValidationError* value.
+If you call not existing field, raises *pydantic.ValidationError* value.
 
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
-from logging import Logger
-
 import aio_pika
-from propan import PropanApp, Context, RabbitBroker
+from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
+async def dependency(body: dict) -> bool:
+    return True
+
 @rabbit_broker.handle("test")
 async def base_handler(body: dict,
+                       dep: bool = Depends(dependency),
                        broker: RabbitBroker = Context()):
+    assert dep is True
     assert broker is rabbit_broker
 ```
 
 ---
 
 ## CLI power
 
 **Propan** has its own CLI tool that provided the following features:
+
 * project generation
 * multiprocessing workers
 * project hot reloading
 * custom command line arguments passing
 
 ### Context passing
 
 For example: pass your current *.env* project setting to context
+
 ```bash
-$ propan run serve:app --env=.env.dev
+propan run serve:app --env=.env.dev
 ```
 
 ```python
 from propan import PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
 from pydantic import BaseSettings
 
@@ -243,35 +249,35 @@
 
 class Settings(BaseSettings):
     ...
 
 @app.on_startup
 async def setup(env: str, context: ContextRepo):
     settings = Settings(_env_file=env)
-    context.set_context("settings", settings)
+    context.set_global("settings", settings)
 ```
 
 ### Project template
 
 Also, **Propan CLI** is able to generate a production-ready application template:
 
-```shell
-$ propan create [projectname]
+```bash
+propan create [projectname]
 ```
 
 *Notice: project template require* `pydantic[dotenv]` *installation.*
 
 Run the created project:
 
-```shell
+```bash
 # Run rabbimq first
-$ docker compose --file [projectname]/docker-compose.yaml up -d
+docker compose --file [projectname]/docker-compose.yaml up -d
 
 # Run project
-$ propan run [projectname].app.serve:app --env=.env --reload
+propan run [projectname].app.serve:app --env=.env --reload
 ```
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
```

### Comparing `propan-0.0.9.3/pyproject.toml` & `propan-0.0.9.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     "propan[async-nats]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
     "pytest-xdist[psutil]",
 
+    "fastapi",
+
     "asyncmock; python_version < '3.8'",
 ]
 
 doc = [
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
@@ -147,39 +149,53 @@
 run-all = "pytest -v -m 'all'"
 cov = "bash ./scripts/test-cov.sh -v -m 'all'"
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
 disallow_subclassing_any = true
+python_version = "3.7"
 
 [tool.isort]
 profile = "black"
 known_first_party = ["propan"]
 
+[tool.black]
+line-length = 88
+target-version = ['py37']
+include = '\.pyi?$'
+
 [tool.ruff]
+fix = true
+line-length = 88
+target-version = "py37"
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
+    "Q",  # flake8-quotes
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "C901",  # too complex
 ]
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = [
     "propan.Depends", "propan.Context",
     "propan.utils.Depends", "propan.utils.Context",
     "propan.utils.context.Depends", "propan.utils.context.Context",
-    "typer.Argument", "typer.Option", "fastapi.Depends",
+    "typer.Argument", "typer.Option",
+    "fastapi.Depends", "fastapi.datastructures.Default",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q -m 'not slow'"
 testpaths = [
     "tests",
@@ -226,8 +242,9 @@
     "pass",
     '\.\.\.',
 ]
 omit = [
     '*/__about__.py',
     '*/__main__.py',
     '*/__init__.py',
+    '*/annotations.py',
 ]
```

### Comparing `propan-0.0.9.3/PKG-INFO` & `propan-0.0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.9.3
+Version: 0.0.9.4
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -57,14 +57,15 @@
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'doc'
 Requires-Dist: typer[all]; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
+Requires-Dist: fastapi; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest-xdist[psutil]; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -94,15 +95,15 @@
     <a href="https://github.com/Lancetnik/Propan/blob/main/LICENSE" target="_blank">
         <img alt="GitHub" src="https://img.shields.io/github/license/Lancetnik/Propan?color=%23007ec6">
     </a>
 </p>
 
 # Propan
 
-**Propan** - just *<s>an another one HTTP</s>* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
+**Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development toolkit, which existed only in HTTP-frameworks world until now.
 
 It's designed to create reactive microservices around <a href="https://microservices.io/patterns/communication-style/messaging.html" target="_blank">Messaging Architecture</a>.
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
@@ -114,20 +115,21 @@
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
-    * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
-    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
-* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
+  * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
+  * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
+* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/5_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Greate to develop**](#cli-power): CLI tool provides great development experience:
-    * framework-independent way to rule application environment
-    * application code hot reloading
+  * framework-independent way to rule application environment
+  * application code hot reloading
+* [**Testability**](https://lancetnik.github.io/Propan/2_getting_started/7_testing): **Propan** allows you to test your app without external dependencies: you shouldn't suit up a Message Broker, use a virtual one!
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Nats**     | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**   | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
@@ -260,50 +262,55 @@
 ## Dependencies
 
 **Propan** a has dependencies management policy close to `pytest fixtures`.
 You can specify in functions arguments which dependencies
 you would to use. Framework passes them from the global Context object.
 
 Already existed context fields are: *app*, *broker*, *context* (itself), *logger* and *message*.
-If you call not existing field, raises *pydantic.error_wrappers.ValidationError* value.
+If you call not existing field, raises *pydantic.ValidationError* value.
 
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
-from logging import Logger
-
 import aio_pika
-from propan import PropanApp, Context, RabbitBroker
+from propan import PropanApp, RabbitBroker, Context, Depends
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
+async def dependency(body: dict) -> bool:
+    return True
+
 @rabbit_broker.handle("test")
 async def base_handler(body: dict,
+                       dep: bool = Depends(dependency),
                        broker: RabbitBroker = Context()):
+    assert dep is True
     assert broker is rabbit_broker
 ```
 
 ---
 
 ## CLI power
 
 **Propan** has its own CLI tool that provided the following features:
+
 * project generation
 * multiprocessing workers
 * project hot reloading
 * custom command line arguments passing
 
 ### Context passing
 
 For example: pass your current *.env* project setting to context
+
 ```bash
-$ propan run serve:app --env=.env.dev
+propan run serve:app --env=.env.dev
 ```
 
 ```python
 from propan import PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
 from pydantic import BaseSettings
 
@@ -313,35 +320,35 @@
 
 class Settings(BaseSettings):
     ...
 
 @app.on_startup
 async def setup(env: str, context: ContextRepo):
     settings = Settings(_env_file=env)
-    context.set_context("settings", settings)
+    context.set_global("settings", settings)
 ```
 
 ### Project template
 
 Also, **Propan CLI** is able to generate a production-ready application template:
 
-```shell
-$ propan create [projectname]
+```bash
+propan create [projectname]
 ```
 
 *Notice: project template require* `pydantic[dotenv]` *installation.*
 
 Run the created project:
 
-```shell
+```bash
 # Run rabbimq first
-$ docker compose --file [projectname]/docker-compose.yaml up -d
+docker compose --file [projectname]/docker-compose.yaml up -d
 
 # Run project
-$ propan run [projectname].app.serve:app --env=.env --reload
+propan run [projectname].app.serve:app --env=.env --reload
 ```
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.0.9.3 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.0.9.4 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 4 - Beta
@@ -33,23 +33,23 @@
 extra == 'dev' Requires-Dist: ruff==0.0.261; extra == 'dev' Requires-Dist:
 typer[all]; extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-
 include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist: mkdocs-markdownextradata-
 plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-Dist: mkdocs-
 material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs-static-i18n; extra
 == 'doc' Requires-Dist: typer[all]; extra == 'doc' Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test' Requires-
-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist: propan[async-nats];
-extra == 'test' Requires-Dist: propan[async-rabbit]; extra == 'test' Requires-
-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest-xdist
-[psutil]; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
-Description-Content-Type: text/markdown
+Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist: fastapi; extra ==
+'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-Dist: propan
+[async-rabbit]; extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra ==
+'test' Requires-Dist: pytest-xdist[psutil]; extra == 'test' Requires-Dist:
+pytest>=7; extra == 'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
-# Propan **Propan** - just *an another one HTTP* a **declarative Python MQ
+# Propan **Propan** - dsd *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development
 toolkit, which existed only in HTTP-frameworks world until now. It's designed
 to create reactive microservices around Messaging_Architecture. It is a modern,
 high-level framework on top of popular specific Python brokers libraries, based
 on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://
 fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/
@@ -60,92 +60,95 @@
 Multiple features from each argument and parameter declaration. *
 [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use
 in pair with [any HTTP framework](https://lancetnik.github.io/Propan/
 5_integrations/1_integrations-index/) you want * **MQ independent**: Single
 interface to popular MQ: * **NATS** (based on [nats-py](https://github.com/
 nats-io/nats.py)) * **RabbitMQ** (based on [aio-pika](https://aio-
 pika.readthedocs.io/en/latest/)) * [**RPC**](https://lancetnik.github.io/
-Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests
+Propan/2_getting_started/4_broker/5_rpc/): The framework supports RPC requests
 over MQ, which will allow performing long operations on remote services
 asynchronously. * [**Greate to develop**](#cli-power): CLI tool provides great
 development experience: * framework-independent way to rule application
-environment * application code hot reloading ### Supported MQ brokers | | async
-| sync | |--------------|:-----------------------------------------------------
---:|:--------------------:| | **RabbitMQ** | :heavy_check_mark: **stable** :
-heavy_check_mark: | :mag: planning :mag: | | **Nats** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in
-progress** :hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag:
-planning :mag: | :mag: planning :mag: | | **REDIS** | :mag: planning :mag: | :
-mag: planning :mag: | | **Kafka** | :mag: planning :mag: | :mag: planning :mag:
-| | **SQS** | :mag: planning :mag: | :mag: planning :mag: | ### Community If
-you are interested in this project, please give me feedback by star or/and
-watch repository. If you have any questions or ideas about features to
-implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
-discussions) or public [telegram group](https://t.me/propan_python). --- ##
-Declarative? With declarative tools you should define **what you need to get**.
-With traditional imperative tools you should write **what you need to do**.
-Take a look at classic imperative tools, such as [aio-pika](https://aio-
-pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/
-), [nats-py](https://github.com/nats-io/nats.py), etc. This is the
-**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
-async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
-guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
-await connection.channel() queue = await channel.declare_queue(queue_name)
-async with queue.iterator() as queue_iter: async for message in queue_iter:
-async with message.process(): print(message.body) asyncio.run(main()) ```
-**aio-pika** is a really great tool with a really easy learning curve. But it's
-still imperative. You need to *connect*, declare *channel*, *queues*,
-*exchanges* by yourself. Also, you need to manage *connection*, *message*,
-*queue* context to avoid any troubles. It is not a bad way, but it can be easy.
-```python from propan import PropanApp, RabbitBroker broker = RabbitBroker
-("amqp://guest:guest@localhost:5672/") app = PropanApp(broker) @broker.handle
-("test_queue") async def base_handler(body): print(body) ``` This is the
-**Propan** declarative way to write the same code. That is so much easier,
-isn't it? --- ## Quickstart Install using `pip`: ```shell $ pip install "propan
-[async-rabbit]" # or $ pip install "propan[async-nats]" ``` ### Basic usage
-Create an application with the following code at `serve.py`: ```python from
-propan import PropanApp from propan import RabbitBroker # from propan import
-NatsBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker
-= NatsBroker("nats://localhost:4222") app = PropanApp(broker) @broker.handle
-("test") async def base_handler(body): '''Handle all default exchange messages
-with `test` routing key''' print(body) ``` And just run it: ```shell $ propan
-run serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
-function arguments to types according to their annotation. ```python from
-pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
-def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
--- ## Dependencies **Propan** a has dependencies management policy close to
-`pytest fixtures`. You can specify in functions arguments which dependencies
-you would to use. Framework passes them from the global Context object. Already
-existed context fields are: *app*, *broker*, *context* (itself), *logger* and
-*message*. If you call not existing field, raises
-*pydantic.error_wrappers.ValidationError* value. But you can specify your own
+environment * application code hot reloading * [**Testability**](https://
+lancetnik.github.io/Propan/2_getting_started/7_testing): **Propan** allows you
+to test your app without external dependencies: you shouldn't suit up a Message
+Broker, use a virtual one! ### Supported MQ brokers | | async | sync | |-------
+-------|:-------------------------------------------------------:|:------------
+--------:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: |
+:mag: planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag:
+planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
+hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
+:mag: planning :mag: | | **REDIS** | :mag: planning :mag: | :mag: planning :
+mag: | | **Kafka** | :mag: planning :mag: | :mag: planning :mag: | | **SQS** |
+:mag: planning :mag: | :mag: planning :mag: | ### Community If you are
+interested in this project, please give me feedback by star or/and watch
+repository. If you have any questions or ideas about features to implement,
+welcome to [discussions](https://github.com/Lancetnik/Propan/discussions) or
+public [telegram group](https://t.me/propan_python). --- ## Declarative? With
+declarative tools you should define **what you need to get**. With traditional
+imperative tools you should write **what you need to do**. Take a look at
+classic imperative tools, such as [aio-pika](https://aio-pika.readthedocs.io/
+en/latest/), [pika](https://pika.readthedocs.io/en/stable/), [nats-py](https://
+github.com/nats-io/nats.py), etc. This is the **Quickstart** with the *aio-
+pika*: ```python import asyncio import aio_pika async def main(): connection =
+await aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
+"test_queue" async with connection: channel = await connection.channel() queue
+= await channel.declare_queue(queue_name) async with queue.iterator() as
+queue_iter: async for message in queue_iter: async with message.process():
+print(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool
+with a really easy learning curve. But it's still imperative. You need to
+*connect*, declare *channel*, *queues*, *exchanges* by yourself. Also, you need
+to manage *connection*, *message*, *queue* context to avoid any troubles. It is
+not a bad way, but it can be easy. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
+nats]" ``` ### Basic usage Create an application with the following code at
+`serve.py`: ```python from propan import PropanApp from propan import
+RabbitBroker # from propan import NatsBroker broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222")
+app = PropanApp(broker) @broker.handle("test") async def base_handler(body):
+'''Handle all default exchange messages with `test` routing key''' print(body)
+``` And just run it: ```shell $ propan run serve:app ``` --- ## Type casting
+Propan uses `pydantic` to cast incoming function arguments to types according
+to their annotation. ```python from pydantic import BaseModel from propan
+import PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage(BaseModel):
+key: int @broker.handle("test2") async def second_handler(body: SimpleMessage):
+assert isinstance(body.key, int) ``` --- ## Dependencies **Propan** a has
+dependencies management policy close to `pytest fixtures`. You can specify in
+functions arguments which dependencies you would to use. Framework passes them
+from the global Context object. Already existed context fields are: *app*,
+*broker*, *context* (itself), *logger* and *message*. If you call not existing
+field, raises *pydantic.ValidationError* value. But you can specify your own
 dependencies, call dependencies functions (like `Fastapi Depends`) and [more]
 (https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
-```python from logging import Logger import aio_pika from propan import
-PropanApp, Context, RabbitBroker rabbit_broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(rabbit_broker) @rabbit_broker.handle
-("test") async def base_handler(body: dict, broker: RabbitBroker = Context()):
+```python import aio_pika from propan import PropanApp, RabbitBroker, Context,
+Depends rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app
+= PropanApp(rabbit_broker) async def dependency(body: dict) -> bool: return
+True @rabbit_broker.handle("test") async def base_handler(body: dict, dep: bool
+= Depends(dependency), broker: RabbitBroker = Context()): assert dep is True
 assert broker is rabbit_broker ``` --- ## CLI power **Propan** has its own CLI
 tool that provided the following features: * project generation *
 multiprocessing workers * project hot reloading * custom command line arguments
 passing ### Context passing For example: pass your current *.env* project
-setting to context ```bash $ propan run serve:app --env=.env.dev ``` ```python
+setting to context ```bash propan run serve:app --env=.env.dev ``` ```python
 from propan import PropanApp, RabbitBroker from propan.annotations import
 ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
 guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
 (BaseSettings): ... @app.on_startup async def setup(env: str, context:
-ContextRepo): settings = Settings(_env_file=env) context.set_context
-("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
-generate a production-ready application template: ```shell $ propan create
-[projectname] ``` *Notice: project template require* `pydantic[dotenv]`
-*installation.* Run the created project: ```shell # Run rabbimq first $ docker
-compose --file [projectname]/docker-compose.yaml up -d # Run project $ propan
-run [projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+ContextRepo): settings = Settings(_env_file=env) context.set_global("settings",
+settings) ``` ### Project template Also, **Propan CLI** is able to generate a
+production-ready application template: ```bash propan create [projectname] ```
+*Notice: project template require* `pydantic[dotenv]` *installation.* Run the
+created project: ```bash # Run rabbimq first docker compose --file
+[projectname]/docker-compose.yaml up -d # Run project propan run
+[projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
 development experience! --- ## HTTP Frameworks integrations ### Any Framework
 You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
 them according to your application lifespan. ```python from propan import
 NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
 NatsBroker("nats://localhost:4222") @broker.handle("test") async def
 base_handler(body): print(body) @app.after_server_start async def start_broker
 (app, loop): await broker.start() @app.after_server_stop async def stop_broker
```

