# Comparing `tmp/volttron-10.0.3a9.tar.gz` & `tmp/volttron-10.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron-10.0.3a9.tar", max compression
+gzip compressed data, was "volttron-10.0.4rc0.tar", max compression
```

## Comparing `volttron-10.0.3a9.tar` & `volttron-10.0.4rc0.tar`

### file list

```diff
@@ -1,101 +1,100 @@
--rw-r--r--   0        0        0    11928 2023-05-01 21:23:45.340246 volttron-10.0.3a9/LICENSE
--rw-r--r--   0        0        0     1775 2023-05-01 21:23:45.340246 volttron-10.0.3a9/README.md
--rw-r--r--   0        0        0     1924 2023-05-01 21:26:01.562345 volttron-10.0.3a9/pyproject.toml
--rw-r--r--   0        0        0     4187 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/__init__.py
--rw-r--r--   0        0        0     6396 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/commands/__init__.py
--rw-r--r--   0        0        0     4469 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/commands/config.py
--rw-r--r--   0        0        0     2547 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/commands/connection.py
--rw-r--r--   0        0        0   112374 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/commands/control.py
--rw-r--r--   0        0        0    19307 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/commands/install_agents.py
--rw-r--r--   0        0        0     2172 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/known_identities.py
--rw-r--r--   0        0        0      953 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/__init__.py
--rw-r--r--   0        0        0     3192 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/headers.py
--rw-r--r--   0        0        0     5103 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/health.py
--rw-r--r--   0        0        0     4427 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/socket.py
--rw-r--r--   0        0        0     8062 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/topics.py
--rw-r--r--   0        0        0     7414 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/messaging/utils.py
--rw-r--r--   0        0        0     1895 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/__init__.py
--rw-r--r--   0        0        0     7993 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/__init__.py
--rw-r--r--   0        0        0     7762 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/connection.py
--rw-r--r--   0        0        0    42650 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/core.py
--rw-r--r--   0        0        0     4821 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/decorators.py
--rw-r--r--   0        0        0     1750 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/dispatch.py
--rw-r--r--   0        0        0     2056 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/errors.py
--rw-r--r--   0        0        0     3607 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/example.py
--rw-r--r--   0        0        0     2545 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/results.py
--rw-r--r--   0        0        0     1908 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/__init__.py
--rw-r--r--   0        0        0    17299 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/auth.py
--rw-r--r--   0        0        0      969 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/base.py
--rw-r--r--   0        0        0     5906 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/channel.py
--rw-r--r--   0        0        0    18124 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/configstore.py
--rw-r--r--   0        0        0     5771 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/health.py
--rw-r--r--   0        0        0     4342 2023-05-01 21:23:45.340246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/heartbeat.py
--rw-r--r--   0        0        0     3955 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/hello.py
--rw-r--r--   0        0        0     5352 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/peerlist.py
--rw-r--r--   0        0        0     2704 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/ping.py
--rw-r--r--   0        0        0    23787 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/pubsub.py
--rw-r--r--   0        0        0     2436 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/query.py
--rw-r--r--   0        0        0    24879 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/rpc.py
--rw-r--r--   0        0        0     8137 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/web.py
--rw-r--r--   0        0        0     2508 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/agent/utils.py
--rw-r--r--   0        0        0     2435 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/green.py
--rw-r--r--   0        0        0     3662 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/client/vip/zmq_connection.py
--rw-r--r--   0        0        0      929 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/__init__.py
--rw-r--r--   0        0        0    29564 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/__main__.py
--rw-r--r--   0        0        0    53671 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/aip.py
--rw-r--r--   0        0        0     3792 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/async_.py
--rw-r--r--   0        0        0     5249 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/log_actions.py
--rw-r--r--   0        0        0     1739 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/monitor.py
--rw-r--r--   0        0        0     1023 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/router/__init__.py
--rw-r--r--   0        0        0    14104 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/router/base_router.py
--rw-r--r--   0        0        0     3080 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/router/green_router.py
--rw-r--r--   0        0        0    14582 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/router/router.py
--rw-r--r--   0        0        0     2428 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/router/servicepeer.py
--rw-r--r--   0        0        0    13088 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/scheduling.py
--rw-r--r--   0        0        0    23122 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/server_argparser.py
--rw-r--r--   0        0        0    23260 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/server_ui.py
--rw-r--r--   0        0        0     7203 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/serviceloader.py
--rw-r--r--   0        0        0     3485 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/tracking.py
--rw-r--r--   0        0        0    17046 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/server/wheel_wrap.py
--rw-r--r--   0        0        0     1074 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/auth/__init__.py
--rw-r--r--   0        0        0    61866 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/auth/auth_service.py
--rw-r--r--   0        0        0      967 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/config_store/__init__.py
--rw-r--r--   0        0        0    19031 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/config_store/config_store_service.py
--rw-r--r--   0        0        0      975 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/control/__init__.py
--rw-r--r--   0        0        0    25084 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/control/control_service.py
--rw-r--r--   0        0        0      961 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/health/__init__.py
--rw-r--r--   0        0        0     4510 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/health/health_service.py
--rw-r--r--   0        0        0     1182 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/routing/__init__.py
--rw-r--r--   0        0        0     5710 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/routing/external_rpc_service.py
--rw-r--r--   0        0        0    37252 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/routing/pubsub_service.py
--rw-r--r--   0        0        0    18407 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/routing/routing_service.py
--rw-r--r--   0        0        0    14318 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/services/routing/zmq_proxy_router.py
--rw-r--r--   0        0        0     1803 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/types/__init__.py
--rw-r--r--   0        0        0     2427 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/types/peer.py
--rw-r--r--   0        0        0     8756 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/types/server_config.py
--rw-r--r--   0        0        0     4195 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/utils/__init__.py
--rw-r--r--   0        0        0    23141 2023-05-01 21:23:45.344246 volttron-10.0.3a9/src/volttron/utils/argparser.py
--rw-r--r--   0        0        0    42623 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/certs.py
--rw-r--r--   0        0        0     8457 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/commands.py
--rw-r--r--   0        0        0     6586 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/context.py
--rw-r--r--   0        0        0     4343 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/dynamic_helper.py
--rw-r--r--   0        0        0     1973 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/file_access.py
--rw-r--r--   0        0        0     4230 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/filewatch.py
--rw-r--r--   0        0        0     3224 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/frame_serialization.py
--rw-r--r--   0        0        0     1555 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/frozendict.py
--rw-r--r--   0        0        0     1899 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/identities.py
--rw-r--r--   0        0        0     2028 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/jsonapi.py
--rw-r--r--   0        0        0    16313 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/jsonrpc.py
--rw-r--r--   0        0        0     8980 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/keystore.py
--rw-r--r--   0        0        0     4780 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/logs.py
--rw-r--r--   0        0        0     2111 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/math_utils.py
--rw-r--r--   0        0        0     2619 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/messagebus.py
--rw-r--r--   0        0        0     3799 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/network.py
--rw-r--r--   0        0        0     4754 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/persistance.py
--rw-r--r--   0        0        0    13422 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/scheduling.py
--rw-r--r--   0        0        0    21221 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/socket.py
--rw-r--r--   0        0        0     3078 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/storeutils.py
--rw-r--r--   0        0        0     6690 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/time.py
--rw-r--r--   0        0        0     2223 2023-05-01 21:23:45.348246 volttron-10.0.3a9/src/volttron/utils/version.py
--rw-r--r--   0        0        0     3817 1970-01-01 00:00:00.000000 volttron-10.0.3a9/setup.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 volttron-10.0.3a9/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/LICENSE
+-rw-r--r--   0        0        0     3124 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/README.md
+-rw-r--r--   0        0        0     2047 2023-05-11 14:34:09.118894 volttron-10.0.4rc0/pyproject.toml
+-rw-r--r--   0        0        0     4187 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/__init__.py
+-rw-r--r--   0        0        0     6396 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/commands/__init__.py
+-rw-r--r--   0        0        0     4469 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/commands/config.py
+-rw-r--r--   0        0        0     2547 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/commands/connection.py
+-rw-r--r--   0        0        0   112374 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/commands/control.py
+-rw-r--r--   0        0        0    19307 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/commands/install_agents.py
+-rw-r--r--   0        0        0     2172 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/known_identities.py
+-rw-r--r--   0        0        0      953 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/messaging/__init__.py
+-rw-r--r--   0        0        0     3192 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/messaging/headers.py
+-rw-r--r--   0        0        0     5103 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/messaging/health.py
+-rw-r--r--   0        0        0     4427 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/messaging/socket.py
+-rw-r--r--   0        0        0     8062 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/messaging/topics.py
+-rw-r--r--   0        0        0     7414 2023-05-11 14:32:59.494194 volttron-10.0.4rc0/src/volttron/client/messaging/utils.py
+-rw-r--r--   0        0        0     1895 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/vip/__init__.py
+-rw-r--r--   0        0        0     7993 2023-05-11 14:34:05.174855 volttron-10.0.4rc0/src/volttron/client/vip/agent/__init__.py
+-rw-r--r--   0        0        0     7762 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/connection.py
+-rw-r--r--   0        0        0    42650 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/core.py
+-rw-r--r--   0        0        0     4821 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/decorators.py
+-rw-r--r--   0        0        0     1750 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/dispatch.py
+-rw-r--r--   0        0        0     2056 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/errors.py
+-rw-r--r--   0        0        0     3607 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/example.py
+-rw-r--r--   0        0        0     2545 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/results.py
+-rw-r--r--   0        0        0     1908 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/__init__.py
+-rw-r--r--   0        0        0    17299 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/auth.py
+-rw-r--r--   0        0        0      969 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/base.py
+-rw-r--r--   0        0        0     5906 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/channel.py
+-rw-r--r--   0        0        0    18124 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/configstore.py
+-rw-r--r--   0        0        0     5771 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/health.py
+-rw-r--r--   0        0        0     4342 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/heartbeat.py
+-rw-r--r--   0        0        0     3955 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/hello.py
+-rw-r--r--   0        0        0     5352 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/peerlist.py
+-rw-r--r--   0        0        0     2704 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/ping.py
+-rw-r--r--   0        0        0    23787 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/pubsub.py
+-rw-r--r--   0        0        0     2436 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/query.py
+-rw-r--r--   0        0        0    24879 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/rpc.py
+-rw-r--r--   0        0        0     8137 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/web.py
+-rw-r--r--   0        0        0     2508 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/agent/utils.py
+-rw-r--r--   0        0        0     2435 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/green.py
+-rw-r--r--   0        0        0     3662 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/client/vip/zmq_connection.py
+-rw-r--r--   0        0        0      929 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/__init__.py
+-rw-r--r--   0        0        0    29564 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/__main__.py
+-rw-r--r--   0        0        0    53671 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/aip.py
+-rw-r--r--   0        0        0     3792 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/async_.py
+-rw-r--r--   0        0        0     5249 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/log_actions.py
+-rw-r--r--   0        0        0     1739 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/monitor.py
+-rw-r--r--   0        0        0     1023 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/router/__init__.py
+-rw-r--r--   0        0        0    14104 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/router/base_router.py
+-rw-r--r--   0        0        0     3080 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/router/green_router.py
+-rw-r--r--   0        0        0    14582 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/router/router.py
+-rw-r--r--   0        0        0     2428 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/router/servicepeer.py
+-rw-r--r--   0        0        0    13088 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/scheduling.py
+-rw-r--r--   0        0        0    23122 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/server_argparser.py
+-rw-r--r--   0        0        0    23260 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/server_ui.py
+-rw-r--r--   0        0        0     7203 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/serviceloader.py
+-rw-r--r--   0        0        0     3485 2023-05-11 14:34:05.178855 volttron-10.0.4rc0/src/volttron/server/tracking.py
+-rw-r--r--   0        0        0    17046 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/server/wheel_wrap.py
+-rw-r--r--   0        0        0     1074 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/auth/__init__.py
+-rw-r--r--   0        0        0    61866 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/auth/auth_service.py
+-rw-r--r--   0        0        0      967 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/config_store/__init__.py
+-rw-r--r--   0        0        0    19031 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/config_store/config_store_service.py
+-rw-r--r--   0        0        0      975 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/control/__init__.py
+-rw-r--r--   0        0        0    25084 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/control/control_service.py
+-rw-r--r--   0        0        0      961 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/health/__init__.py
+-rw-r--r--   0        0        0     4510 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/health/health_service.py
+-rw-r--r--   0        0        0     1182 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/routing/__init__.py
+-rw-r--r--   0        0        0     5710 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/routing/external_rpc_service.py
+-rw-r--r--   0        0        0    37252 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/routing/pubsub_service.py
+-rw-r--r--   0        0        0    18407 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/routing/routing_service.py
+-rw-r--r--   0        0        0    14318 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/services/routing/zmq_proxy_router.py
+-rw-r--r--   0        0        0     1803 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/types/__init__.py
+-rw-r--r--   0        0        0     2427 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/types/peer.py
+-rw-r--r--   0        0        0     8756 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/types/server_config.py
+-rw-r--r--   0        0        0     4195 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/__init__.py
+-rw-r--r--   0        0        0    23141 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/argparser.py
+-rw-r--r--   0        0        0    42623 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/certs.py
+-rw-r--r--   0        0        0     8457 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/commands.py
+-rw-r--r--   0        0        0     6586 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/context.py
+-rw-r--r--   0        0        0     4343 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/dynamic_helper.py
+-rw-r--r--   0        0        0     1973 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/file_access.py
+-rw-r--r--   0        0        0     4230 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/filewatch.py
+-rw-r--r--   0        0        0     3224 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/frame_serialization.py
+-rw-r--r--   0        0        0     1555 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/frozendict.py
+-rw-r--r--   0        0        0     1899 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/identities.py
+-rw-r--r--   0        0        0     2028 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/jsonapi.py
+-rw-r--r--   0        0        0    16313 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/jsonrpc.py
+-rw-r--r--   0        0        0     8980 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/keystore.py
+-rw-r--r--   0        0        0     4780 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/logs.py
+-rw-r--r--   0        0        0     2111 2023-05-11 14:34:05.182855 volttron-10.0.4rc0/src/volttron/utils/math_utils.py
+-rw-r--r--   0        0        0     2619 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/messagebus.py
+-rw-r--r--   0        0        0     3799 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/network.py
+-rw-r--r--   0        0        0     4754 2023-05-11 14:32:59.502195 volttron-10.0.4rc0/src/volttron/utils/persistance.py
+-rw-r--r--   0        0        0    13422 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/scheduling.py
+-rw-r--r--   0        0        0    21221 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/socket.py
+-rw-r--r--   0        0        0     3078 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/storeutils.py
+-rw-r--r--   0        0        0     6690 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/time.py
+-rw-r--r--   0        0        0     2223 2023-05-11 14:34:05.186855 volttron-10.0.4rc0/src/volttron/utils/version.py
+-rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 volttron-10.0.4rc0/PKG-INFO
```

### Comparing `volttron-10.0.3a9/LICENSE` & `volttron-10.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/pyproject.toml` & `volttron-10.0.4rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron"
-version = "10.0.3a9"
+version = "10.0.4rc0"
 description = "VOLTTRON™ is an open source platform for distributed sensing and control. The platform provides services for collecting and storing data from buildings and devices and provides an environment for developing applications which interact with that data."
 authors = ["volttron <volttron@pnnl.gov>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://volttron.org"
 repository = "https://github.com/eclipse-volttron/volttron-core"
 documentation = "https://volttron.readthedocs.org"
@@ -31,24 +31,26 @@
 toml = "^0.10.2"
 dateutils = "^0.6.12"
 tzlocal = "^4.1"
 psutil = "^5.9.0"
 cryptography = "^36.0.1"
 watchdog-gevent = "^0.1.1"
 pip = "22.2.2"
+pytest-timeout = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
+mypy = "^1.2.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 volttron = 'volttron.server.__main__:main'
 vcfg = 'volttron.client.commands.config:main'
 volttron-cfg = 'volttron.client.commands.config:main'
 vctl = 'volttron.client.commands.control:main'
@@ -63,7 +65,12 @@
 ]
 
 [tool.yapf]
 based_on_style = "pep8"
 spaces_before_comment = 4
 column_limit = 99
 split_before_logical_operator = true
+
+[tool.mypy]
+show_error_context = true
+pretty = true
+show_column_numbers = true
```

### Comparing `volttron-10.0.3a9/src/volttron/client/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/commands/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/commands/config.py` & `volttron-10.0.4rc0/src/volttron/client/commands/config.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/commands/connection.py` & `volttron-10.0.4rc0/src/volttron/client/commands/connection.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/commands/control.py` & `volttron-10.0.4rc0/src/volttron/client/commands/control.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/commands/install_agents.py` & `volttron-10.0.4rc0/src/volttron/client/commands/install_agents.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/known_identities.py` & `volttron-10.0.4rc0/src/volttron/client/known_identities.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/headers.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/headers.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/health.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/health.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/socket.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/socket.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/topics.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/topics.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/messaging/utils.py` & `volttron-10.0.4rc0/src/volttron/client/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/vip/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/connection.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/connection.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/core.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/core.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/decorators.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/decorators.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/dispatch.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/dispatch.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/errors.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/errors.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/example.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/example.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/results.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/results.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/__init__.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/auth.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/auth.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/base.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/base.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/channel.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/channel.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/configstore.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/configstore.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/health.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/health.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/heartbeat.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/heartbeat.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/hello.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/hello.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/peerlist.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/peerlist.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/ping.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/ping.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/pubsub.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/pubsub.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/query.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/query.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/rpc.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/rpc.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/subsystems/web.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/subsystems/web.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/agent/utils.py` & `volttron-10.0.4rc0/src/volttron/client/vip/agent/utils.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/green.py` & `volttron-10.0.4rc0/src/volttron/client/vip/green.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/client/vip/zmq_connection.py` & `volttron-10.0.4rc0/src/volttron/client/vip/zmq_connection.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/__init__.py` & `volttron-10.0.4rc0/src/volttron/server/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/__main__.py` & `volttron-10.0.4rc0/src/volttron/server/__main__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/aip.py` & `volttron-10.0.4rc0/src/volttron/server/aip.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/async_.py` & `volttron-10.0.4rc0/src/volttron/server/async_.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/log_actions.py` & `volttron-10.0.4rc0/src/volttron/server/log_actions.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/monitor.py` & `volttron-10.0.4rc0/src/volttron/server/monitor.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/router/__init__.py` & `volttron-10.0.4rc0/src/volttron/server/router/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/router/base_router.py` & `volttron-10.0.4rc0/src/volttron/server/router/base_router.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/router/green_router.py` & `volttron-10.0.4rc0/src/volttron/server/router/green_router.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/router/router.py` & `volttron-10.0.4rc0/src/volttron/server/router/router.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/router/servicepeer.py` & `volttron-10.0.4rc0/src/volttron/server/router/servicepeer.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/scheduling.py` & `volttron-10.0.4rc0/src/volttron/server/scheduling.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/server_argparser.py` & `volttron-10.0.4rc0/src/volttron/server/server_argparser.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/server_ui.py` & `volttron-10.0.4rc0/src/volttron/server/server_ui.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/serviceloader.py` & `volttron-10.0.4rc0/src/volttron/server/serviceloader.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/tracking.py` & `volttron-10.0.4rc0/src/volttron/server/tracking.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/server/wheel_wrap.py` & `volttron-10.0.4rc0/src/volttron/server/wheel_wrap.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/auth/__init__.py` & `volttron-10.0.4rc0/src/volttron/services/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/auth/auth_service.py` & `volttron-10.0.4rc0/src/volttron/services/auth/auth_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/config_store/__init__.py` & `volttron-10.0.4rc0/src/volttron/services/config_store/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/config_store/config_store_service.py` & `volttron-10.0.4rc0/src/volttron/services/config_store/config_store_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/control/__init__.py` & `volttron-10.0.4rc0/src/volttron/services/control/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/control/control_service.py` & `volttron-10.0.4rc0/src/volttron/services/control/control_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/health/__init__.py` & `volttron-10.0.4rc0/src/volttron/services/health/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/health/health_service.py` & `volttron-10.0.4rc0/src/volttron/services/health/health_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/routing/__init__.py` & `volttron-10.0.4rc0/src/volttron/services/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/routing/external_rpc_service.py` & `volttron-10.0.4rc0/src/volttron/services/routing/external_rpc_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/routing/pubsub_service.py` & `volttron-10.0.4rc0/src/volttron/services/routing/pubsub_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/routing/routing_service.py` & `volttron-10.0.4rc0/src/volttron/services/routing/routing_service.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/services/routing/zmq_proxy_router.py` & `volttron-10.0.4rc0/src/volttron/services/routing/zmq_proxy_router.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/types/__init__.py` & `volttron-10.0.4rc0/src/volttron/types/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/types/peer.py` & `volttron-10.0.4rc0/src/volttron/types/peer.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/types/server_config.py` & `volttron-10.0.4rc0/src/volttron/types/server_config.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/__init__.py` & `volttron-10.0.4rc0/src/volttron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/argparser.py` & `volttron-10.0.4rc0/src/volttron/utils/argparser.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/certs.py` & `volttron-10.0.4rc0/src/volttron/utils/certs.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/commands.py` & `volttron-10.0.4rc0/src/volttron/utils/commands.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/context.py` & `volttron-10.0.4rc0/src/volttron/utils/context.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/dynamic_helper.py` & `volttron-10.0.4rc0/src/volttron/utils/dynamic_helper.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/file_access.py` & `volttron-10.0.4rc0/src/volttron/utils/file_access.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/filewatch.py` & `volttron-10.0.4rc0/src/volttron/utils/filewatch.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/frame_serialization.py` & `volttron-10.0.4rc0/src/volttron/utils/frame_serialization.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/frozendict.py` & `volttron-10.0.4rc0/src/volttron/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/identities.py` & `volttron-10.0.4rc0/src/volttron/utils/identities.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/jsonapi.py` & `volttron-10.0.4rc0/src/volttron/utils/jsonapi.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/jsonrpc.py` & `volttron-10.0.4rc0/src/volttron/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/keystore.py` & `volttron-10.0.4rc0/src/volttron/utils/keystore.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/logs.py` & `volttron-10.0.4rc0/src/volttron/utils/logs.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/math_utils.py` & `volttron-10.0.4rc0/src/volttron/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/messagebus.py` & `volttron-10.0.4rc0/src/volttron/utils/messagebus.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/network.py` & `volttron-10.0.4rc0/src/volttron/utils/network.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/persistance.py` & `volttron-10.0.4rc0/src/volttron/utils/persistance.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/scheduling.py` & `volttron-10.0.4rc0/src/volttron/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/socket.py` & `volttron-10.0.4rc0/src/volttron/utils/socket.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/storeutils.py` & `volttron-10.0.4rc0/src/volttron/utils/storeutils.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/time.py` & `volttron-10.0.4rc0/src/volttron/utils/time.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/src/volttron/utils/version.py` & `volttron-10.0.4rc0/src/volttron/utils/version.py`

 * *Files identical despite different names*

### Comparing `volttron-10.0.3a9/PKG-INFO` & `volttron-10.0.4rc0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,12 @@
-Metadata-Version: 2.1
-Name: volttron
-Version: 10.0.3a9
-Summary: VOLTTRON™ is an open source platform for distributed sensing and control. The platform provides services for collecting and storing data from buildings and devices and provides an environment for developing applications which interact with that data.
-Home-page: https://volttron.org
-License: Apache-2.0
-Author: volttron
-Author-email: volttron@pnnl.gov
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: cryptography (>=36.0.1,<37.0.0)
-Requires-Dist: dateutils (>=0.6.12,<0.7.0)
-Requires-Dist: gevent (>=22.10.2,<23.0.0)
-Requires-Dist: pip (==22.2.2)
-Requires-Dist: poetry (>=1.2.2,<2.0.0)
-Requires-Dist: psutil (>=5.9.0,<6.0.0)
-Requires-Dist: pyzmq (>=25.0.2,<26.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: tzlocal (>=4.1,<5.0)
-Requires-Dist: watchdog-gevent (>=0.1.1,<0.2.0)
-Project-URL: Documentation, https://volttron.readthedocs.org
-Project-URL: Repository, https://github.com/eclipse-volttron/volttron-core
-Description-Content-Type: text/markdown
-
-VOLTTRON™ is an open source platform for distributed sensing and control. The platform provides services for collecting and storing data from buildings and devices and provides an environment for developing applications which interact with that data.
+Eclipse VOLTTRON™ (VOLTTRON/volttron) is an open source platform for distributed sensing and control. The platform provides services for collecting and storing data from buildings and devices and provides an environment for developing applications which interact with that data.
 
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 [![Pytests](https://github.com/eclipse-volttron/volttron-core/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-core/actions/workflows/run-tests.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron.svg)](https://pypi.org/project/volttron/)
 
 ## Installation
 
 It is recommended to use a virtual environment for installing volttron.
 
@@ -52,33 +21,50 @@
 
  1. Setup VOLTTRON_HOME environment variable: export VOLTTRON_HOME=/path/to/volttron_home/dir 
  
     **NOTE** This is madatory if you have/had in the past, a monolithic    VOLTTRON version that used the default VOLTTRON_HOME $HOME/.volttron. This modular version of VOLTTRON cannot work with volttron_home used by monolithic version of VOLTTRON(version 8.3 or earlier)
  
  2. Start the platform
     ```bash
-    > volttron -vv -l volttron.log &>/dev/null &
+    volttron -vv -l volttron.log &>/dev/null &
     ```
 
  3. Install listener agent
     ```bash
-    > vctl install volttron-listener --start
+    vctl install volttron-listener --start
     ```
 
  4. View status of platform
     ```bash
-    > vctl status
+    vctl status
     ```
 
  5. Shutdown the platform
     ```bash
-    > vctl shutdown --platform
+    vctl shutdown --platform
     ```
 
 Full VOLTTRON documentation available at [VOLTTRON Readthedocs](https://volttron.readthedocs.io)
 
 ## Contributing to VOLTTRON
 
 Please see the [contributing.md](CONTRIBUTING.md) document before contributing to this repository.
 
 Please see [developing_on_modular.md](DEVELOPING_ON_MODULAR.md) document for developing your agents against volttron.
 
+# Disclaimer Notice
+
+This material was prepared as an account of work sponsored by an agency of the
+United States Government.  Neither the United States Government nor the United
+States Department of Energy, nor Battelle, nor any of their employees, nor any
+jurisdiction or organization that has cooperated in the development of these
+materials, makes any warranty, express or implied, or assumes any legal
+liability or responsibility for the accuracy, completeness, or usefulness or any
+information, apparatus, product, software, or process disclosed, or represents
+that its use would not infringe privately owned rights.
+
+Reference herein to any specific commercial product, process, or service by
+trade name, trademark, manufacturer, or otherwise does not necessarily
+constitute or imply its endorsement, recommendation, or favoring by the United
+States Government or any agency thereof, or Battelle Memorial Institute. The
+views and opinions of authors expressed herein do not necessarily state or
+reflect those of the United States Government or any agency thereof.
```

