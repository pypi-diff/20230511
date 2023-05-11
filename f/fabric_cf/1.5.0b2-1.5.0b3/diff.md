# Comparing `tmp/fabric_cf-1.5.0b2.tar.gz` & `tmp/fabric_cf-1.5.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_cf-1.5.0b2.tar", last modified: Mon Apr  3 14:59:48 2023, max compression
+gzip compressed data, was "fabric_cf-1.5.0b3.tar", last modified: Thu May 11 16:37:50 2023, max compression
```

## Comparing `fabric_cf-1.5.0b2.tar` & `fabric_cf-1.5.0b3.tar`

### file list

```diff
@@ -1,523 +1,517 @@
--rw-r--r--   0        0        0     1926 2023-04-03 14:50:53.534276 fabric_cf-1.5.0b2/.gitignore
--rw-r--r--   0        0        0      889 2023-04-03 14:52:00.091972 fabric_cf-1.5.0b2/Dockerfile-auth
--rw-r--r--   0        0        0      807 2023-04-03 14:50:53.534621 fabric_cf-1.5.0b2/Dockerfile-broker
--rw-r--r--   0        0        0      908 2023-04-03 14:50:53.534765 fabric_cf-1.5.0b2/Dockerfile-cf
--rw-r--r--   0        0        0      825 2023-04-03 14:50:53.534888 fabric_cf-1.5.0b2/Dockerfile-orchestrator
--rw-r--r--   0        0        0     1071 2023-04-03 14:50:53.535054 fabric_cf-1.5.0b2/LICENSE
--rw-r--r--   0        0        0     2046 2023-04-03 14:50:53.535620 fabric_cf-1.5.0b2/README.md
--rwxr-xr-x   0        0        0       74 2023-04-03 14:50:53.535840 fabric_cf-1.5.0b2/authority.sh
--rwxr-xr-x   0        0        0       79 2023-04-03 14:50:53.535996 fabric_cf-1.5.0b2/broker.sh
--rw-r--r--   0        0        0      947 2023-04-03 14:50:53.536169 fabric_cf-1.5.0b2/cleanup_old_schema_from_schema_registry.sh
--rw-r--r--   0        0        0     2861 2023-04-03 14:50:53.536428 fabric_cf-1.5.0b2/docker-compose-kafka.yaml
--rw-r--r--   0        0        0     1560 2023-04-03 14:50:53.536634 fabric_cf-1.5.0b2/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0    11977 2023-04-03 14:50:53.536840 fabric_cf-1.5.0b2/docker-compose-test.yaml
--rwxr-xr-x   0        0        0       45 2023-04-03 14:50:53.536998 fabric_cf-1.5.0b2/docker-entrypoint.sh
--rw-r--r--   0        0        0      350 2023-04-03 14:50:53.537353 fabric_cf-1.5.0b2/env.template
--rw-r--r--   0        0        0      795 2023-04-03 14:50:53.537557 fabric_cf-1.5.0b2/env.template.test
--rw-r--r--   0        0        0    16609 2023-04-03 14:50:53.537818 fabric_cf-1.5.0b2/fabricNo.AnyActorNoPolicy.xml
--rw-r--r--   0        0        0     6343 2023-04-03 14:50:53.538166 fabric_cf-1.5.0b2/fabric_cf/Design.md
--rw-r--r--   0        0        0       24 2023-04-03 14:51:45.747247 fabric_cf-1.5.0b2/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538462 fabric_cf-1.5.0b2/fabric_cf/actor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538776 fabric_cf-1.5.0b2/fabric_cf/actor/boot/__init__.py
--rw-r--r--   0        0        0    15281 2023-04-03 14:50:53.539116 fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration.py
--rw-r--r--   0        0        0     1268 2023-04-03 14:50:53.539529 fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_exception.py
--rw-r--r--   0        0        0     2509 2023-04-03 14:50:53.539906 fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_loader.py
--rw-r--r--   0        0        0    23086 2023-04-03 14:50:53.540212 fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540419 fabric_cf-1.5.0b2/fabric_cf/actor/boot/inventory/__init__.py
--rw-r--r--   0        0        0     4969 2023-04-03 14:50:53.540687 fabric_cf-1.5.0b2/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540852 fabric_cf-1.5.0b2/fabric_cf/actor/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.541039 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/__init__.py
--rw-r--r--   0        0        0     4907 2023-04-03 14:50:53.541250 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_container.py
--rw-r--r--   0        0        0     1530 2023-04-03 14:50:53.541590 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_event.py
--rw-r--r--   0        0        0     2176 2023-04-03 14:50:53.541925 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_identity.py
--rw-r--r--   0        0        0     1991 2023-04-03 14:50:53.542388 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_management_object.py
--rw-r--r--   0        0        0    21765 2023-04-03 14:50:53.542778 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_mixin.py
--rw-r--r--   0        0        0     1918 2023-04-03 14:50:53.543106 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_proxy.py
--rw-r--r--   0        0        0     1323 2023-04-03 14:50:53.543429 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_runnable.py
--rw-r--r--   0        0        0     4497 2023-04-03 14:50:53.543679 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority.py
--rw-r--r--   0        0        0     8736 2023-04-03 14:50:53.543930 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_policy.py
--rw-r--r--   0        0        0     3299 2023-04-03 14:50:53.544153 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_proxy.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.545583 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_reservation.py
--rw-r--r--   0        0        0     6071 2023-04-03 14:50:53.545879 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_base_plugin.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.546104 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_mixin.py
--rw-r--r--   0        0        0     1492 2023-04-03 14:50:53.546359 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
--rw-r--r--   0        0        0     3690 2023-04-03 14:50:53.546566 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_proxy.py
--rw-r--r--   0        0        0     4012 2023-04-03 14:50:53.546780 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_reservation.py
--rw-r--r--   0        0        0     2442 2023-04-03 14:50:53.547038 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_callback_proxy.py
--rw-r--r--   0        0        0     9216 2023-04-03 14:50:53.547299 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_actor.py
--rw-r--r--   0        0        0     6215 2023-04-03 14:50:53.547712 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
--rw-r--r--   0        0        0     2640 2023-04-03 14:50:53.547942 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
--rw-r--r--   0        0        0     5802 2023-04-03 14:50:53.548385 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_policy.py
--rw-r--r--   0        0        0     7724 2023-04-03 14:50:53.548730 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_reservation.py
--rw-r--r--   0        0        0     1936 2023-04-03 14:50:53.548982 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_component.py
--rw-r--r--   0        0        0     9833 2023-04-03 14:50:53.549228 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_concrete_set.py
--rw-r--r--   0        0        0     2729 2023-04-03 14:50:53.549801 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_container_clock.py
--rw-r--r--   0        0        0     3976 2023-04-03 14:50:53.550228 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_container_database.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.550497 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller.py
--rw-r--r--   0        0        0     2423 2023-04-03 14:50:53.550710 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
--rw-r--r--   0        0        0     2787 2023-04-03 14:50:53.550900 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_policy.py
--rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.551118 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_reservation.py
--rw-r--r--   0        0        0    10301 2023-04-03 14:50:53.551323 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_database.py
--rw-r--r--   0        0        0    11026 2023-04-03 14:50:53.551566 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_delegation.py
--rw-r--r--   0        0        0     1867 2023-04-03 14:50:53.551767 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_event.py
--rw-r--r--   0        0        0     1943 2023-04-03 14:50:53.552014 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_management_object.py
--rw-r--r--   0        0        0     9044 2023-04-03 14:50:53.552250 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_actor.py
--rw-r--r--   0        0        0     2534 2023-04-03 14:50:53.552486 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_authority.py
--rw-r--r--   0        0        0     1452 2023-04-03 14:50:53.552674 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
--rw-r--r--   0        0        0     6191 2023-04-03 14:50:53.552834 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
--rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.553039 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_container.py
--rw-r--r--   0        0        0     2317 2023-04-03 14:50:53.553242 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
--rw-r--r--   0        0        0     5014 2023-04-03 14:50:53.553457 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
--rw-r--r--   0        0        0    11147 2023-04-03 14:50:53.553629 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_policy.py
--rw-r--r--   0        0        0     2304 2023-04-03 14:50:53.553847 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_proxy.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.554059 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_proxy_factory.py
--rw-r--r--   0        0        0     1658 2023-04-03 14:50:53.554593 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_query_response_handler.py
--rw-r--r--   0        0        0    14096 2023-04-03 14:50:53.554880 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_mixin.py
--rw-r--r--   0        0        0     9388 2023-04-03 14:50:53.555129 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_resources.py
--rw-r--r--   0        0        0     5581 2023-04-03 14:50:53.555376 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_status.py
--rw-r--r--   0        0        0     8963 2023-04-03 14:50:53.555582 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_resource_control.py
--rw-r--r--   0        0        0     1336 2023-04-03 14:50:53.555785 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_response_handler.py
--rw-r--r--   0        0        0     2246 2023-04-03 14:50:53.556014 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_rpc_request_state.py
--rw-r--r--   0        0        0     5634 2023-04-03 14:50:53.556345 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_actor.py
--rw-r--r--   0        0        0     6415 2023-04-03 14:50:53.556589 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_policy.py
--rw-r--r--   0        0        0     4846 2023-04-03 14:50:53.556782 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_reservation.py
--rw-r--r--   0        0        0    13280 2023-04-03 14:50:53.557016 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_slice.py
--rw-r--r--   0        0        0     3227 2023-04-03 14:50:53.557270 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_substrate.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.557477 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_substrate_database.py
--rw-r--r--   0        0        0     2943 2023-04-03 14:50:53.557727 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_tick.py
--rw-r--r--   0        0        0     6121 2023-04-03 14:50:53.557931 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_ticker.py
--rw-r--r--   0        0        0     1590 2023-04-03 14:50:53.558112 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_timer_queue.py
--rw-r--r--   0        0        0     1387 2023-04-03 14:50:53.558344 fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_timer_task.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.558543 fabric_cf-1.5.0b2/fabric_cf/actor/core/common/__init__.py
--rw-r--r--   0        0        0    12749 2023-04-03 14:50:53.558881 fabric_cf-1.5.0b2/fabric_cf/actor/core/common/constants.py
--rw-r--r--   0        0        0     3254 2023-04-03 14:50:53.559144 fabric_cf-1.5.0b2/fabric_cf/actor/core/common/event_logger.py
--rw-r--r--   0        0        0     5517 2023-04-03 14:50:53.559364 fabric_cf-1.5.0b2/fabric_cf/actor/core/common/exceptions.py
--rw-r--r--   0        0        0     6108 2023-04-03 14:50:53.559599 fabric_cf-1.5.0b2/fabric_cf/actor/core/common/resource_config.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.559841 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/__init__.py
--rw-r--r--   0        0        0    24564 2023-04-03 14:50:53.560251 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/container.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.560471 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/db/__init__.py
--rw-r--r--   0        0        0     8629 2023-04-03 14:50:53.560683 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/db/container_database.py
--rw-r--r--   0        0        0    19263 2023-04-03 14:50:53.561010 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/globals.py
--rw-r--r--   0        0        0     7053 2023-04-03 14:50:53.561272 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/maintenance.py
--rw-r--r--   0        0        0     5472 2023-04-03 14:50:53.561525 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/message_service.py
--rw-r--r--   0        0        0     1508 2023-04-03 14:50:53.561724 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/protocol_descriptor.py
--rw-r--r--   0        0        0    13005 2023-04-03 14:50:53.562081 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/remote_actor_cache.py
--rw-r--r--   0        0        0     8040 2023-04-03 14:50:53.562299 fabric_cf-1.5.0b2/fabric_cf/actor/core/container/rpc_producer.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.562481 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/__init__.py
--rw-r--r--   0        0        0    35190 2023-04-03 14:50:53.563062 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/actor.py
--rw-r--r--   0        0        0     1975 2023-04-03 14:50:53.563319 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/actor_identity.py
--rw-r--r--   0        0        0    14656 2023-04-03 14:50:53.563570 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/authority.py
--rw-r--r--   0        0        0     4845 2023-04-03 14:50:53.563854 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/authority_policy.py
--rw-r--r--   0        0        0    20313 2023-04-03 14:50:53.564180 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/broker.py
--rw-r--r--   0        0        0     5914 2023-04-03 14:50:53.565067 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/broker_policy.py
--rw-r--r--   0        0        0    18186 2023-04-03 14:50:53.565344 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/controller.py
--rw-r--r--   0        0        0     8542 2023-04-03 14:50:53.565615 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/event_processor.py
--rw-r--r--   0        0        0     5467 2023-04-03 14:50:53.565861 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/inventory_slice_manager.py
--rw-r--r--   0        0        0     6171 2023-04-03 14:50:53.566145 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/policy.py
--rw-r--r--   0        0        0     2042 2023-04-03 14:50:53.566366 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/rpc_request_state.py
--rw-r--r--   0        0        0     8688 2023-04-03 14:50:53.566587 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/ticket.py
--rw-r--r--   0        0        0    14528 2023-04-03 14:50:53.566793 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/unit.py
--rw-r--r--   0        0        0    13263 2023-04-03 14:50:53.567022 fabric_cf-1.5.0b2/fabric_cf/actor/core/core/unit_set.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.567201 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/__init__.py
--rw-r--r--   0        0        0    10969 2023-04-03 14:50:53.567422 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/broker_delegation.py
--rw-r--r--   0        0        0     1874 2023-04-03 14:50:53.567633 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/broker_delegation_factory.py
--rw-r--r--   0        0        0    16897 2023-04-03 14:50:53.567918 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/delegation.py
--rw-r--r--   0        0        0     1825 2023-04-03 14:50:53.568190 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/delegation_factory.py
--rw-r--r--   0        0        0     5364 2023-04-03 14:50:53.568399 fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/resource_ticket.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.568570 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/__init__.py
--rw-r--r--   0        0        0    27428 2023-04-03 14:50:53.568871 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/authority_reservation.py
--rw-r--r--   0        0        0     3384 2023-04-03 14:50:53.569249 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
--rw-r--r--   0        0        0    26805 2023-04-03 14:50:53.569537 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/broker_reservation.py
--rw-r--r--   0        0        0     2992 2023-04-03 14:50:53.569880 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/claim_timeout.py
--rw-r--r--   0        0        0     4396 2023-04-03 14:50:53.570217 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/failed_rpc.py
--rw-r--r--   0        0        0     3639 2023-04-03 14:50:53.570449 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/failed_rpc_event.py
--rw-r--r--   0        0        0     2668 2023-04-03 14:50:53.570827 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
--rw-r--r--   0        0        0     2708 2023-04-03 14:50:53.571106 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
--rw-r--r--   0        0        0     2105 2023-04-03 14:50:53.571543 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_query_rpc.py
--rw-r--r--   0        0        0     2703 2023-04-03 14:50:53.571750 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
--rw-r--r--   0        0        0     4158 2023-04-03 14:50:53.571968 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_rpc.py
--rw-r--r--   0        0        0    10726 2023-04-03 14:50:53.572149 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_rpc_event.py
--rw-r--r--   0        0        0    62017 2023-04-03 14:50:53.572423 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.572703 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel_tick.py
--rw-r--r--   0        0        0    55045 2023-04-03 14:50:53.573299 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel_wrapper.py
--rw-r--r--   0        0        0     2363 2023-04-03 14:50:53.573675 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/predecessor_state.py
--rw-r--r--   0        0        0     2860 2023-04-03 14:50:53.573873 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/query_timeout.py
--rw-r--r--   0        0        0     1404 2023-04-03 14:50:53.574038 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/request_types.py
--rw-r--r--   0        0        0    24493 2023-04-03 14:51:26.321598 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation.py
--rw-r--r--   0        0        0    89064 2023-04-03 14:50:53.575058 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_client.py
--rw-r--r--   0        0        0     9994 2023-04-03 14:50:53.575366 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_server.py
--rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.575644 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_states.py
--rw-r--r--   0        0        0    20888 2023-04-03 14:50:53.575901 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/resource_set.py
--rw-r--r--   0        0        0     1614 2023-04-03 14:50:53.576176 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/retry_rpc.py
--rw-r--r--   0        0        0     1899 2023-04-03 14:50:53.576398 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/retry_rpc_event.py
--rw-r--r--   0        0        0     4128 2023-04-03 14:50:53.576854 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_executor.py
--rw-r--r--   0        0        0    31221 2023-04-03 14:50:53.577199 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_manager.py
--rw-r--r--   0        0        0     1772 2023-04-03 14:50:53.577467 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
--rw-r--r--   0        0        0     3579 2023-04-03 14:50:53.577700 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_request.py
--rw-r--r--   0        0        0     1620 2023-04-03 14:50:53.577956 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_request_type.py
--rw-r--r--   0        0        0     1340 2023-04-03 14:50:53.578168 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
--rw-r--r--   0        0        0    12284 2023-04-03 14:50:53.578451 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice.py
--rw-r--r--   0        0        0    12311 2023-04-03 14:50:53.578680 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice_state_machine.py
--rw-r--r--   0        0        0     8319 2023-04-03 14:50:53.578901 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice_table.py
--rw-r--r--   0        0        0     6527 2023-04-03 14:50:53.579044 fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/tick.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.579204 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/__init__.py
--rw-r--r--   0        0        0    35748 2023-04-03 14:50:53.579623 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/actor_management_object.py
--rw-r--r--   0        0        0     8431 2023-04-03 14:50:53.579975 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/authority_management_object.py
--rw-r--r--   0        0        0     6903 2023-04-03 14:50:53.580307 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/broker_management_object.py
--rw-r--r--   0        0        0    27468 2023-04-03 14:50:53.580634 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
--rw-r--r--   0        0        0     9605 2023-04-03 14:50:53.580935 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/container_management_object.py
--rw-r--r--   0        0        0     8973 2023-04-03 14:50:53.581107 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/controller_management_object.py
--rw-r--r--   0        0        0    13007 2023-04-03 14:50:53.581333 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/converter.py
--rw-r--r--   0        0        0     1624 2023-04-03 14:50:53.581543 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/error.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.581729 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/__init__.py
--rw-r--r--   0        0        0    10194 2023-04-03 14:50:53.582040 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_actor.py
--rw-r--r--   0        0        0     3509 2023-04-03 14:50:53.582317 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_authority.py
--rw-r--r--   0        0        0     8066 2023-04-03 14:50:53.582654 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_broker.py
--rw-r--r--   0        0        0     4483 2023-04-03 14:50:53.583057 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_container.py
--rw-r--r--   0        0        0     5300 2023-04-03 14:50:53.583248 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_controller.py
--rw-r--r--   0        0        0     5462 2023-04-03 14:50:53.583439 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
--rw-r--r--   0        0        0     6961 2023-04-03 14:50:53.583636 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     5730 2023-04-03 14:50:53.583847 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.584078 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/__init__.py
--rw-r--r--   0        0        0    24550 2023-04-03 14:50:53.584410 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
--rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.584691 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
--rw-r--r--   0        0        0     5797 2023-04-03 14:50:53.585104 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
--rw-r--r--   0        0        0    15846 2023-04-03 14:50:53.585409 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
--rw-r--r--   0        0        0     4008 2023-04-03 14:50:53.585584 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
--rw-r--r--   0        0        0     8228 2023-04-03 14:50:53.585867 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
--rw-r--r--   0        0        0     2148 2023-04-03 14:50:53.586169 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.586361 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/__init__.py
--rw-r--r--   0        0        0    10935 2023-04-03 14:50:53.586634 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_actor.py
--rw-r--r--   0        0        0     3902 2023-04-03 14:50:53.586852 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_authority.py
--rw-r--r--   0        0        0     8391 2023-04-03 14:50:53.587036 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_broker.py
--rw-r--r--   0        0        0    10119 2023-04-03 14:50:53.587201 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_container.py
--rw-r--r--   0        0        0     9395 2023-04-03 14:50:53.587383 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_controller.py
--rw-r--r--   0        0        0     2855 2023-04-03 14:50:53.587571 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_proxy.py
--rw-r--r--   0        0        0     8655 2023-04-03 14:50:53.587724 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_server_actor.py
--rw-r--r--   0        0        0     7217 2023-04-03 14:50:53.588020 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_object.py
--rw-r--r--   0        0        0     7841 2023-04-03 14:50:53.588258 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_object_manager.py
--rw-r--r--   0        0        0     4972 2023-04-03 14:50:53.588521 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_utils.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.588706 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/__init__.py
--rw-r--r--   0        0        0     1604 2023-04-03 14:50:53.588914 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/client_mng.py
--rw-r--r--   0        0        0     1570 2023-04-03 14:50:53.589110 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/event_mng.py
--rw-r--r--   0        0        0     1802 2023-04-03 14:50:53.589285 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
--rw-r--r--   0        0        0     1741 2023-04-03 14:50:53.589460 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/result_client_mng.py
--rw-r--r--   0        0        0     1554 2023-04-03 14:50:53.589750 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/result_event_mng.py
--rw-r--r--   0        0        0     1904 2023-04-03 14:50:53.590017 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
--rw-r--r--   0        0        0    15777 2023-04-03 14:50:53.590202 fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/server_actor_management_object.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590369 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/__init__.py
--rw-r--r--   0        0        0     7756 2023-04-03 14:50:53.590739 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/base_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590945 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/__init__.py
--rw-r--r--   0        0        0    30995 2023-04-03 14:50:53.591225 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/actor_database.py
--rw-r--r--   0        0        0     2616 2023-04-03 14:50:53.591517 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/client_database.py
--rw-r--r--   0        0        0     3584 2023-04-03 14:50:53.591758 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/server_actor_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.591940 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/__init__.py
--rw-r--r--   0        0        0    12823 2023-04-03 14:50:53.592182 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
--rw-r--r--   0        0        0     2831 2023-04-03 14:50:53.592374 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/config_token.py
--rw-r--r--   0        0        0     2286 2023-04-03 14:50:53.592660 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
--rw-r--r--   0        0        0     7108 2023-04-03 14:50:53.592865 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/handler_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593035 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/__init__.py
--rw-r--r--   0        0        0     3612 2023-04-03 14:50:53.593263 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593460 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/db/__init__.py
--rw-r--r--   0        0        0     4285 2023-04-03 14:50:53.593798 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
--rw-r--r--   0        0        0    14268 2023-04-03 14:50:53.594012 fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.594246 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/__init__.py
--rw-r--r--   0        0        0    28295 2023-04-03 14:50:53.594548 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/authority_calendar_policy.py
--rw-r--r--   0        0        0     8891 2023-04-03 14:50:53.595030 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/broker_calendar_policy.py
--rw-r--r--   0        0        0    63111 2023-04-03 14:50:53.595571 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
--rw-r--r--   0        0        0    19814 2023-04-03 14:50:53.595878 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_calendar_policy.py
--rw-r--r--   0        0        0     9812 2023-04-03 14:50:53.596091 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_simple_policy.py
--rw-r--r--   0        0        0     9524 2023-04-03 14:50:53.596306 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
--rw-r--r--   0        0        0     1814 2023-04-03 14:50:53.596494 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/fifo_queue.py
--rw-r--r--   0        0        0     2981 2023-04-03 14:50:53.596828 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/inventory.py
--rw-r--r--   0        0        0     2785 2023-04-03 14:50:53.597031 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/inventory_for_type.py
--rw-r--r--   0        0        0    14499 2023-04-03 14:50:53.597231 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_node_control.py
--rw-r--r--   0        0        0    28363 2023-04-03 14:50:53.597532 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_node_inventory.py
--rw-r--r--   0        0        0     5435 2023-04-03 14:50:53.597856 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_service_control.py
--rw-r--r--   0        0        0    22745 2023-04-03 14:50:53.598106 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_service_inventory.py
--rw-r--r--   0        0        0     2032 2023-04-03 14:50:53.598641 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/queue_wrapper.py
--rw-r--r--   0        0        0     5157 2023-04-03 14:50:53.598857 fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/resource_control.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599020 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/__init__.py
--rw-r--r--   0        0        0     1821 2023-04-03 14:50:53.599277 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/actor_location.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599432 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/__init__.py
--rw-r--r--   0        0        0     7798 2023-04-03 14:50:53.599583 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
--rw-r--r--   0        0        0     9013 2023-04-03 14:50:53.599758 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
--rw-r--r--   0        0        0     6686 2023-04-03 14:50:53.599942 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     4809 2023-04-03 14:50:53.600099 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
--rw-r--r--   0        0        0     8466 2023-04-03 14:50:53.600393 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.600601 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/__init__.py
--rw-r--r--   0        0        0    11710 2023-04-03 14:50:53.600939 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
--rw-r--r--   0        0        0     6931 2023-04-03 14:50:53.601111 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
--rw-r--r--   0        0        0     8218 2023-04-03 14:50:53.601343 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.601562 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
--rw-r--r--   0        0        0    15551 2023-04-03 14:50:53.601817 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/translate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.601999 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/__init__.py
--rw-r--r--   0        0        0     4525 2023-04-03 14:50:53.602224 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_authority.py
--rw-r--r--   0        0        0     5726 2023-04-03 14:50:53.602562 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_broker.py
--rw-r--r--   0        0        0     6896 2023-04-03 14:50:53.603120 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_proxy.py
--rw-r--r--   0        0        0     2868 2023-04-03 14:50:53.604580 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
--rw-r--r--   0        0        0     6397 2023-04-03 14:50:53.605005 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_return.py
--rw-r--r--   0        0        0     8303 2023-04-03 14:50:53.605283 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/proxy.py
--rw-r--r--   0        0        0     3013 2023-04-03 14:50:53.605545 fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/proxy_factory.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.605762 fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/__init__.py
--rw-r--r--   0        0        0     7672 2023-04-03 14:50:53.605950 fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/actor_registry.py
--rw-r--r--   0        0        0     2177 2023-04-03 14:50:53.606181 fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/callback_registry.py
--rw-r--r--   0        0        0     4926 2023-04-03 14:50:53.606408 fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/peer_registry.py
--rw-r--r--   0        0        0     3912 2023-04-03 14:50:53.606565 fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/proxy_registry.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.606740 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-03 14:50:53.606931 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/actor_clock.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.607146 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     8224 2023-04-03 14:50:53.607463 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/authority_calendar.py
--rw-r--r--   0        0        0     1667 2023-04-03 14:50:53.607755 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/base_calendar.py
--rw-r--r--   0        0        0    11573 2023-04-03 14:50:53.607991 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/broker_calendar.py
--rw-r--r--   0        0        0     9733 2023-04-03 14:50:53.608213 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/client_calendar.py
--rw-r--r--   0        0        0     5239 2023-04-03 14:50:53.608505 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/controller_calendar.py
--rw-r--r--   0        0        0     2550 2023-04-03 14:50:53.608738 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/source_calendar.py
--rw-r--r--   0        0        0    15769 2023-04-03 14:50:53.609015 fabric_cf-1.5.0b2/fabric_cf/actor/core/time/term.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.609215 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/__init__.py
--rw-r--r--   0        0        0     2213 2023-04-03 14:50:53.609476 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/bids.py
--rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.609992 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/client.py
--rw-r--r--   0        0        0     2063 2023-04-03 14:50:53.610294 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/graceful_interrupt_handler.py
--rw-r--r--   0        0        0     2163 2023-04-03 14:50:53.610582 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/id.py
--rw-r--r--   0        0        0     1488 2023-04-03 14:50:53.610758 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/iterable_queue.py
--rw-r--r--   0        0        0     2263 2023-04-03 14:50:53.611043 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/kernel_timer.py
--rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.611261 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/log_helper.py
--rw-r--r--   0        0        0     2238 2023-04-03 14:50:53.611511 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/notice.py
--rw-r--r--   0        0        0     1999 2023-04-03 14:50:53.611700 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reflection_utils.py
--rw-r--r--   0        0        0     8380 2023-04-03 14:50:53.612072 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_holdings.py
--rw-r--r--   0        0        0     8864 2023-04-03 14:50:53.612305 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_list.py
--rw-r--r--   0        0        0     6796 2023-04-03 14:50:53.612487 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_set.py
--rw-r--r--   0        0        0     3144 2023-04-03 14:50:53.612687 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_state.py
--rw-r--r--   0        0        0     2250 2023-04-03 14:50:53.612855 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/resource_type.py
--rw-r--r--   0        0        0     1690 2023-04-03 14:50:53.613024 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/rpc_exception.py
--rw-r--r--   0        0        0     4440 2023-04-03 14:50:53.613195 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/update_data.py
--rw-r--r--   0        0        0     4188 2023-04-03 14:50:53.613384 fabric_cf-1.5.0b2/fabric_cf/actor/core/util/utils.py
--rw-r--r--   0        0        0     7474 2023-04-03 14:50:53.613876 fabric_cf-1.5.0b2/fabric_cf/actor/db/__init__.py
--rw-r--r--   0        0        0    64154 2023-04-03 14:50:53.614421 fabric_cf-1.5.0b2/fabric_cf/actor/db/psql_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.614689 fabric_cf-1.5.0b2/fabric_cf/actor/fim/__init__.py
--rw-r--r--   0        0        0     6241 2023-04-03 14:50:53.614913 fabric_cf-1.5.0b2/fabric_cf/actor/fim/asm_update_thread.py
--rw-r--r--   0        0        0    28206 2023-04-03 14:50:53.616227 fabric_cf-1.5.0b2/fabric_cf/actor/fim/fim_helper.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616623 fabric_cf-1.5.0b2/fabric_cf/actor/fim/plugins/__init__.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616848 fabric_cf-1.5.0b2/fabric_cf/actor/fim/plugins/broker/__init__.py
--rw-r--r--   0        0        0    23622 2023-04-03 14:50:53.617119 fabric_cf-1.5.0b2/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617325 fabric_cf-1.5.0b2/fabric_cf/actor/handlers/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-03 14:50:53.617552 fabric_cf-1.5.0b2/fabric_cf/actor/handlers/handler_base.py
--rw-r--r--   0        0        0     9305 2023-04-03 14:50:53.617730 fabric_cf-1.5.0b2/fabric_cf/actor/handlers/no_op_handler.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617898 fabric_cf-1.5.0b2/fabric_cf/actor/security/__init__.py
--rw-r--r--   0        0        0     4348 2023-04-03 14:50:53.618115 fabric_cf-1.5.0b2/fabric_cf/actor/security/access_checker.py
--rw-r--r--   0        0        0     2955 2023-04-03 14:50:53.618313 fabric_cf-1.5.0b2/fabric_cf/actor/security/auth_token.py
--rw-r--r--   0        0        0     3982 2023-04-03 14:50:53.618495 fabric_cf-1.5.0b2/fabric_cf/actor/security/fabric_token.py
--rw-r--r--   0        0        0     8635 2023-04-03 14:50:53.618697 fabric_cf-1.5.0b2/fabric_cf/actor/security/pdp_auth.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.618864 fabric_cf-1.5.0b2/fabric_cf/actor/test/__init__.py
--rw-r--r--   0        0        0    10543 2023-04-03 14:50:53.619075 fabric_cf-1.5.0b2/fabric_cf/actor/test/base_test_case.py
--rw-r--r--   0        0        0     4679 2023-04-03 14:50:53.619270 fabric_cf-1.5.0b2/fabric_cf/actor/test/client_callback_helper.py
--rw-r--r--   0        0        0     4642 2023-04-03 14:50:53.619566 fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.jenkins.yaml
--rw-r--r--   0        0        0     4305 2023-04-03 14:50:53.619762 fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4695 2023-04-03 14:50:53.619999 fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.test.yaml
--rw-r--r--   0        0        0     5376 2023-04-03 14:50:53.620212 fabric_cf-1.5.0b2/fabric_cf/actor/test/controller_callback_helper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620415 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620599 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/container/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-03 14:50:53.620872 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/container/container_database_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621040 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/core/__init__.py
--rw-r--r--   0        0        0     4091 2023-04-03 14:50:53.621342 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/core/unit_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621493 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/kernel/__init__.py
--rw-r--r--   0        0        0    19990 2023-04-03 14:50:53.623445 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/kernel/kernel_test.py
--rw-r--r--   0        0        0     3378 2023-04-03 14:50:53.623839 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/kernel/tick_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.624033 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/__init__.py
--rw-r--r--   0        0        0     3176 2023-04-03 14:50:53.624219 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/actor_database_test.py
--rw-r--r--   0        0        0     4733 2023-04-03 14:50:53.624405 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
--rw-r--r--   0        0        0     1963 2023-04-03 14:50:53.624564 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
--rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.624725 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/substrate_database_test.py
--rw-r--r--   0        0        0     2280 2023-04-03 14:50:53.625161 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/substrate_test_base.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.625348 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/__init__.py
--rw-r--r--   0        0        0    21677 2023-04-03 14:50:53.625553 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
--rw-r--r--   0        0        0    23671 2023-04-03 14:50:53.625894 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
--rw-r--r--   0        0        0     4513 2023-04-03 14:50:53.626305 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
--rw-r--r--   0        0        0     1561 2023-04-03 14:50:53.626668 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
--rw-r--r--   0        0        0     8437 2023-04-03 14:50:53.626899 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
--rw-r--r--   0        0        0     7716 2023-04-03 14:50:53.627114 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
--rw-r--r--   0        0        0     1586 2023-04-03 14:50:53.627291 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627471 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/__init__.py
--rw-r--r--   0        0        0     3786 2023-04-03 14:50:53.627666 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/actor_clock_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627830 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:50:53.628007 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.628189 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
--rw-r--r--   0        0        0    14887 2023-04-03 14:50:53.628405 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/term_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.628584 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/util/__init__.py
--rw-r--r--   0        0        0     8041 2023-04-03 14:50:53.628792 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/util/reservation_holdings_test.py
--rw-r--r--   0        0        0     5072 2023-04-03 14:50:53.628930 fabric_cf-1.5.0b2/fabric_cf/actor/test/core/util/reservation_list_test.py
--rw-r--r--   0        0        0     3738 2023-04-03 14:50:53.629079 fabric_cf-1.5.0b2/fabric_cf/actor/test/dummy_authority_proxy.py
--rw-r--r--   0        0        0     1953 2023-04-03 14:50:53.629248 fabric_cf-1.5.0b2/fabric_cf/actor/test/dummy_proxy.py
--rw-r--r--   0        0        0     2498 2023-04-03 14:50:53.629420 fabric_cf-1.5.0b2/fabric_cf/actor/test/fim_test_helper.py
--rw-r--r--   0        0        0       92 2023-04-03 14:50:53.629638 fabric_cf-1.5.0b2/fabric_cf/actor/test/schema/key.avsc
--rw-r--r--   0        0        0    26110 2023-04-03 14:50:53.629868 fabric_cf-1.5.0b2/fabric_cf/actor/test/schema/message.avsc
--rw-r--r--   0        0        0     4503 2023-04-03 14:50:53.630115 fabric_cf-1.5.0b2/fabric_cf/actor/test/test_abqm.py
--rw-r--r--   0        0        0     1892 2023-04-03 14:50:53.630509 fabric_cf-1.5.0b2/fabric_cf/actor/test/test_actor.py
--rw-r--r--   0        0        0     1249 2023-04-03 14:50:53.630745 fabric_cf-1.5.0b2/fabric_cf/actor/test/test_exception.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.630912 fabric_cf-1.5.0b2/fabric_cf/aits/__init__.py
--rw-r--r--   0        0        0     4835 2023-04-03 14:50:53.631209 fabric_cf-1.5.0b2/fabric_cf/aits/config/config.broker.yaml
--rw-r--r--   0        0        0     4817 2023-04-03 14:50:53.631403 fabric_cf-1.5.0b2/fabric_cf/aits/config/config.netam.yaml
--rw-r--r--   0        0        0     4423 2023-04-03 14:50:53.631575 fabric_cf-1.5.0b2/fabric_cf/aits/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4797 2023-04-03 14:50:53.631740 fabric_cf-1.5.0b2/fabric_cf/aits/config/config.siteam.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.631942 fabric_cf-1.5.0b2/fabric_cf/aits/elements/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-03 14:50:53.632283 fabric_cf-1.5.0b2/fabric_cf/aits/elements/constants.py
--rw-r--r--   0        0        0     5966 2023-04-03 14:50:53.632469 fabric_cf-1.5.0b2/fabric_cf/aits/elements/reservation.py
--rw-r--r--   0        0        0     3511 2023-04-03 14:50:53.632760 fabric_cf-1.5.0b2/fabric_cf/aits/elements/slice.py
--rw-r--r--   0        0        0    44915 2023-04-03 14:50:53.632998 fabric_cf-1.5.0b2/fabric_cf/aits/integration_test.py
--rw-r--r--   0        0        0     7196 2023-04-03 14:50:53.633214 fabric_cf-1.5.0b2/fabric_cf/aits/kafka_processor.py
--rw-r--r--   0        0        0    11794 2023-04-03 14:50:53.633571 fabric_cf-1.5.0b2/fabric_cf/aits/manage_helper.py
--rw-r--r--   0        0        0     8725 2023-04-03 14:50:53.633815 fabric_cf-1.5.0b2/fabric_cf/aits/orchestrator_helper.py
--rw-r--r--   0        0        0    16256 2023-04-03 14:50:53.634161 fabric_cf-1.5.0b2/fabric_cf/authority/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.634241 fabric_cf-1.5.0b2/fabric_cf/authority/__init__.py
--rw-r--r--   0        0        0     2164 2023-04-03 14:50:53.634418 fabric_cf-1.5.0b2/fabric_cf/authority/__main__.py
--rw-r--r--   0        0        0    32973 2023-04-03 14:50:53.634699 fabric_cf-1.5.0b2/fabric_cf/authority/am-yes.xml
--rw-r--r--   0        0        0     4936 2023-04-03 14:50:53.634941 fabric_cf-1.5.0b2/fabric_cf/authority/config.al2s.am.yaml
--rw-r--r--   0        0        0     5030 2023-04-03 14:50:53.635111 fabric_cf-1.5.0b2/fabric_cf/authority/config.net.am.yaml
--rw-r--r--   0        0        0     5402 2023-04-03 14:50:53.635298 fabric_cf-1.5.0b2/fabric_cf/authority/config.site.am.geni.yaml
--rw-r--r--   0        0        0     4896 2023-04-03 14:50:53.635465 fabric_cf-1.5.0b2/fabric_cf/authority/config.site.am.yaml
--rw-r--r--   0        0        0     3482 2023-04-03 14:50:53.635628 fabric_cf-1.5.0b2/fabric_cf/authority/docker-compose.geni.yml
--rw-r--r--   0        0        0     3391 2023-04-03 14:50:53.635767 fabric_cf-1.5.0b2/fabric_cf/authority/docker-compose.yml
--rw-r--r--   0        0        0     1242 2023-04-03 14:50:53.635974 fabric_cf-1.5.0b2/fabric_cf/authority/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.636162 fabric_cf-1.5.0b2/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1588 2023-04-03 14:50:53.636606 fabric_cf-1.5.0b2/fabric_cf/authority/net_handler_config.yml
--rw-r--r--   0        0        0     1523 2023-04-03 14:50:53.636812 fabric_cf-1.5.0b2/fabric_cf/authority/oess_handler_config.yml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.636998 fabric_cf-1.5.0b2/fabric_cf/authority/pdp.xml
--rwxr-xr-x   0        0        0     2446 2023-04-03 14:50:53.637179 fabric_cf-1.5.0b2/fabric_cf/authority/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.637346 fabric_cf-1.5.0b2/fabric_cf/authority/test/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-03 14:50:53.637572 fabric_cf-1.5.0b2/fabric_cf/authority/test/al2s_am.py
--rw-r--r--   0        0        0     2459 2023-04-03 14:50:53.637740 fabric_cf-1.5.0b2/fabric_cf/authority/test/net_am.py
--rw-r--r--   0        0        0     2456 2023-04-03 14:50:53.637876 fabric_cf-1.5.0b2/fabric_cf/authority/test/site_am.py
--rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.638045 fabric_cf-1.5.0b2/fabric_cf/authority/test/site_am_geni.py
--rw-r--r--   0        0        0     4729 2023-04-03 14:50:53.638234 fabric_cf-1.5.0b2/fabric_cf/authority/test/test-al2sam.yaml
--rw-r--r--   0        0        0     4838 2023-04-03 14:50:53.638384 fabric_cf-1.5.0b2/fabric_cf/authority/test/test-netam.yaml
--rw-r--r--   0        0        0     5071 2023-04-03 14:50:53.638536 fabric_cf-1.5.0b2/fabric_cf/authority/test/test.geni.yaml
--rw-r--r--   0        0        0     4684 2023-04-03 14:50:53.638673 fabric_cf-1.5.0b2/fabric_cf/authority/test/test.yaml
--rw-r--r--   0        0        0     2581 2023-04-03 14:50:53.638845 fabric_cf-1.5.0b2/fabric_cf/authority/vm_handler_config.yml
--rw-r--r--   0        0        0     1448 2023-04-03 14:50:53.639031 fabric_cf-1.5.0b2/fabric_cf/authority/vnic_net_handler_config.yml
--rw-r--r--   0        0        0    14262 2023-04-03 14:50:53.639328 fabric_cf-1.5.0b2/fabric_cf/broker/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.639412 fabric_cf-1.5.0b2/fabric_cf/broker/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.639603 fabric_cf-1.5.0b2/fabric_cf/broker/__main__.py
--rw-r--r--   0        0        0    27944 2023-04-03 14:50:53.639781 fabric_cf-1.5.0b2/fabric_cf/broker/broker-yes.xml
--rw-r--r--   0        0        0     5035 2023-04-03 14:50:53.640005 fabric_cf-1.5.0b2/fabric_cf/broker/config.broker.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.640163 fabric_cf-1.5.0b2/fabric_cf/broker/core/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.640348 fabric_cf-1.5.0b2/fabric_cf/broker/core/broker_kernel.py
--rw-r--r--   0        0        0     3154 2023-04-03 14:50:53.640636 fabric_cf-1.5.0b2/fabric_cf/broker/docker-compose.yml
--rw-r--r--   0        0        0     1246 2023-04-03 14:50:53.640801 fabric_cf-1.5.0b2/fabric_cf/broker/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.640954 fabric_cf-1.5.0b2/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.641105 fabric_cf-1.5.0b2/fabric_cf/broker/pdp.xml
--rwxr-xr-x   0        0        0     2239 2023-04-03 14:50:53.641257 fabric_cf-1.5.0b2/fabric_cf/broker/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.641487 fabric_cf-1.5.0b2/fabric_cf/broker/test/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-03 14:50:53.641689 fabric_cf-1.5.0b2/fabric_cf/broker/test/broker.py
--rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.641862 fabric_cf-1.5.0b2/fabric_cf/broker/test/test.yaml
--rw-r--r--   0        0        0    20151 2023-04-03 14:50:53.642263 fabric_cf-1.5.0b2/fabric_cf/orchestrator/README.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.642384 fabric_cf-1.5.0b2/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0     3380 2023-04-03 14:50:53.642560 fabric_cf-1.5.0b2/fabric_cf/orchestrator/__main__.py
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.642803 fabric_cf-1.5.0b2/fabric_cf/orchestrator/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.642965 fabric_cf-1.5.0b2/fabric_cf/orchestrator/certs/privkey.pem
--rw-r--r--   0        0        0     4624 2023-04-03 14:50:53.643129 fabric_cf-1.5.0b2/fabric_cf/orchestrator/config.orchestrator.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.643278 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/__init__.py
--rw-r--r--   0        0        0     2917 2023-04-03 14:50:53.643501 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/active_status_checker.py
--rw-r--r--   0        0        0     3050 2023-04-03 14:50:53.643707 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/bqm_wrapper.py
--rw-r--r--   0        0        0     1556 2023-04-03 14:50:53.643947 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/exceptions.py
--rw-r--r--   0        0        0     1884 2023-04-03 14:50:53.644155 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/i_status_update_callback.py
--rw-r--r--   0        0        0    38176 2023-04-03 14:50:53.644447 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/orchestrator_handler.py
--rw-r--r--   0        0        0     5389 2023-04-03 14:50:53.644692 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/orchestrator_kernel.py
--rw-r--r--   0        0        0    34864 2023-04-03 14:50:53.645078 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
--rw-r--r--   0        0        0     3581 2023-04-03 14:50:53.645306 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_converter.py
--rw-r--r--   0        0        0     4880 2023-04-03 14:50:53.645464 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_status_update.py
--rw-r--r--   0        0        0     7876 2023-04-03 14:50:53.645708 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_status_update_thread.py
--rw-r--r--   0        0        0     6179 2023-04-03 14:50:53.645975 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/response_builder.py
--rw-r--r--   0        0        0     8805 2023-04-03 14:50:53.646197 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/slice_defer_thread.py
--rw-r--r--   0        0        0     1972 2023-04-03 14:50:53.646372 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/status_checker.py
--rw-r--r--   0        0        0     1581 2023-04-03 14:50:53.646556 fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/watch_entry.py
--rw-r--r--   0        0        0     3556 2023-04-03 14:50:53.646698 fabric_cf-1.5.0b2/fabric_cf/orchestrator/docker-compose.yml
--rw-r--r--   0        0        0     1252 2023-04-03 14:50:53.646876 fabric_cf-1.5.0b2/fabric_cf/orchestrator/env.template
--rw-r--r--   0        0        0    72323 2023-04-03 14:50:53.647218 fabric_cf-1.5.0b2/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
--rw-r--r--   0        0        0     1626 2023-04-03 14:50:53.647500 fabric_cf-1.5.0b2/fabric_cf/orchestrator/nginx/default.conf
--rw-r--r--   0        0        0    44784 2023-04-03 14:50:53.647965 fabric_cf-1.5.0b2/fabric_cf/orchestrator/openapi.json
--rw-r--r--   0        0        0    30829 2023-04-03 14:50:53.648266 fabric_cf-1.5.0b2/fabric_cf/orchestrator/orchestrator-yes.xml
--rw-r--r--   0        0        0     1548 2023-04-03 14:50:53.648514 fabric_cf-1.5.0b2/fabric_cf/orchestrator/pdp.xml
--rwxr-xr-x   0        0        0     2284 2023-04-03 14:50:53.648696 fabric_cf-1.5.0b2/fabric_cf/orchestrator/setup.sh
--rw-r--r--   0        0        0      430 2023-04-03 14:50:53.648991 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/__init__.py
--rw-r--r--   0        0        0      392 2023-04-03 14:50:53.649220 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.649376 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      311 2023-04-03 14:50:53.649537 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
--rw-r--r--   0        0        0     1241 2023-04-03 14:50:53.649770 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
--rw-r--r--   0        0        0     5197 2023-04-03 14:50:53.649985 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
--rw-r--r--   0        0        0      860 2023-04-03 14:50:53.650215 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
--rw-r--r--   0        0        0      305 2023-04-03 14:50:53.650408 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
--rw-r--r--   0        0        0      631 2023-04-03 14:50:53.650559 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/encoder.py
--rw-r--r--   0        0        0     2275 2023-04-03 14:50:53.650868 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1889 2023-04-03 14:50:53.651022 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     1628 2023-04-03 14:50:53.651195 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/resource.py
--rw-r--r--   0        0        0     3564 2023-04-03 14:50:53.651368 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/resources.py
--rw-r--r--   0        0        0     7311 2023-04-03 14:50:53.651598 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slice.py
--rw-r--r--   0        0        0     3616 2023-04-03 14:50:53.651786 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slice_details.py
--rw-r--r--   0        0        0     5251 2023-04-03 14:50:53.651992 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slices.py
--rw-r--r--   0        0        0     8995 2023-04-03 14:50:53.652138 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/sliver.py
--rw-r--r--   0        0        0     5301 2023-04-03 14:50:53.652316 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slivers.py
--rw-r--r--   0        0        0     3896 2023-04-03 14:50:53.652450 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     2464 2023-04-03 14:50:53.652610 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4929 2023-04-03 14:50:53.652747 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     2870 2023-04-03 14:50:53.652914 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
--rw-r--r--   0        0        0     1983 2023-04-03 14:50:53.653092 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
--rw-r--r--   0        0        0     4503 2023-04-03 14:50:53.653265 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     3984 2023-04-03 14:50:53.653436 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
--rw-r--r--   0        0        0     2512 2023-04-03 14:50:53.653613 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     3879 2023-04-03 14:50:53.653846 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
--rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.654001 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     3846 2023-04-03 14:50:53.654159 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
--rw-r--r--   0        0        0     2446 2023-04-03 14:50:53.654361 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     4233 2023-04-03 14:50:53.654697 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     2635 2023-04-03 14:50:53.654868 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3540 2023-04-03 14:50:53.655073 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/version.py
--rw-r--r--   0        0        0     2536 2023-04-03 14:50:53.655253 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/version_data.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.655440 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-03 14:50:53.655618 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
--rw-r--r--   0        0        0     1894 2023-04-03 14:50:53.655790 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/constants.py
--rw-r--r--   0        0        0     5537 2023-04-03 14:50:53.655976 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/cors_response.py
--rw-r--r--   0        0        0     4321 2023-04-03 14:50:53.656175 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
--rw-r--r--   0        0        0    13841 2023-04-03 14:50:53.656443 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
--rw-r--r--   0        0        0     4449 2023-04-03 14:50:53.656622 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
--rw-r--r--   0        0        0     2530 2023-04-03 14:50:53.656817 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/utils.py
--rw-r--r--   0        0        0     2632 2023-04-03 14:50:53.656988 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/version_controller.py
--rw-r--r--   0        0        0    32481 2023-04-03 14:50:53.657385 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      438 2023-04-03 14:50:53.657698 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/__init__.py
--rw-r--r--   0        0        0     2094 2023-04-03 14:50:53.658010 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
--rw-r--r--   0        0        0     4778 2023-04-03 14:50:53.658235 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
--rw-r--r--   0        0        0     1903 2023-04-03 14:50:53.658437 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
--rw-r--r--   0        0        0      855 2023-04-03 14:50:53.658595 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
--rw-r--r--   0        0        0      809 2023-04-03 14:50:53.658764 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/type_util.py
--rw-r--r--   0        0        0     3452 2023-04-03 14:50:53.658932 fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/util.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.659106 fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/__init__.py
--rw-r--r--   0        0        0     3542 2023-04-03 14:50:53.659281 fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/orchestrator.py
--rwxr-xr-x   0        0        0       78 2023-04-03 14:50:53.659409 fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/test.sh
--rw-r--r--   0        0        0     4452 2023-04-03 14:50:53.659580 fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/test.yaml
--rwxr-xr-x   0        0        0     2900 2023-04-03 14:50:53.659782 fabric_cf-1.5.0b2/fabric_cf/orchestrator/update_swagger_stub.sh
--rw-r--r--   0        0        0    18177 2023-04-03 14:50:53.660187 fabric_cf-1.5.0b2/images/am-pod.png
--rw-r--r--   0        0        0    74927 2023-04-03 14:50:53.660890 fabric_cf-1.5.0b2/images/am.png
--rw-r--r--   0        0        0    18471 2023-04-03 14:50:53.661225 fabric_cf-1.5.0b2/images/broker-pod.png
--rw-r--r--   0        0        0    73799 2023-04-03 14:50:53.661878 fabric_cf-1.5.0b2/images/broker.png
--rw-r--r--   0        0        0    90831 2023-04-03 14:50:53.662835 fabric_cf-1.5.0b2/images/cf.png
--rw-r--r--   0        0        0    19611 2023-04-03 14:50:53.663247 fabric_cf-1.5.0b2/images/orchestrator-pod.png
--rw-r--r--   0        0        0    78622 2023-04-03 14:50:53.664084 fabric_cf-1.5.0b2/images/orchestrator.png
--rw-r--r--   0        0        0   145542 2023-04-03 14:50:53.664854 fabric_cf-1.5.0b2/neo4j/AL2S.graphml
--rw-r--r--   0        0        0    96363 2023-04-03 14:50:53.665732 fabric_cf-1.5.0b2/neo4j/LBNL-ad.graphml
--rw-r--r--   0        0        0    68182 2023-04-03 14:50:53.666334 fabric_cf-1.5.0b2/neo4j/Network-ad.graphml
--rw-r--r--   0        0        0    96375 2023-04-03 14:50:53.666804 fabric_cf-1.5.0b2/neo4j/RENCI-ad.graphml
--rw-r--r--   0        0        0    96286 2023-04-03 14:50:53.667143 fabric_cf-1.5.0b2/neo4j/UKY-ad.graphml
--rw-r--r--   0        0        0  1297955 2023-04-03 14:50:53.672629 fabric_cf-1.5.0b2/neo4j/UKY2.graphml
--rw-r--r--   0        0        0    14808 2023-04-03 14:50:53.673167 fabric_cf-1.5.0b2/neo4j/abqm.graphml
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.673435 fabric_cf-1.5.0b2/neo4j/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.673617 fabric_cf-1.5.0b2/neo4j/certs/privkey.pem
--rwxr-xr-x   0        0        0       91 2023-04-03 14:50:53.673785 fabric_cf-1.5.0b2/orchestrator.sh
--rw-r--r--   0        0        0      698 2023-04-03 14:50:53.673962 fabric_cf-1.5.0b2/psql.upgrade
--rw-r--r--   0        0        0      995 2023-04-03 14:58:50.018658 fabric_cf-1.5.0b2/pyproject.toml
--rw-r--r--   0        0        0      194 2023-04-03 14:58:41.397548 fabric_cf-1.5.0b2/requirements.txt
--rwxr-xr-x   0        0        0     2594 2023-04-03 14:50:53.674345 fabric_cf-1.5.0b2/secrets/create-certs.sh
--rw-r--r--   0        0        0       89 2023-04-03 14:50:53.674677 fabric_cf-1.5.0b2/test-requirements.txt
--rw-r--r--   0        0        0     5645 2023-04-03 14:50:53.674946 fabric_cf-1.5.0b2/tools/cleanup.py
--rw-r--r--   0        0        0     8005 2023-04-03 14:50:53.675250 fabric_cf-1.5.0b2/tools/db_cli.py
--rw-r--r--   0        0        0      208 2023-04-03 14:50:53.675450 fabric_cf-1.5.0b2/tools/install.sh
--rw-r--r--   0        0        0      143 2023-04-03 14:50:53.675627 fabric_cf-1.5.0b2/tox.ini
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 fabric_cf-1.5.0b2/PKG-INFO
+-rw-r--r--   0        0        0     2035 2023-05-11 16:37:35.592130 fabric_cf-1.5.0b3/.gitignore
+-rw-r--r--   0        0        0      851 2023-05-11 16:32:26.699200 fabric_cf-1.5.0b3/Dockerfile-auth
+-rw-r--r--   0        0        0      769 2023-05-11 16:32:36.872162 fabric_cf-1.5.0b3/Dockerfile-broker
+-rw-r--r--   0        0        0     1037 2023-05-11 16:32:57.016934 fabric_cf-1.5.0b3/Dockerfile-cf
+-rw-r--r--   0        0        0      787 2023-05-11 16:32:47.114231 fabric_cf-1.5.0b3/Dockerfile-orchestrator
+-rw-r--r--   0        0        0     1071 2023-04-03 14:50:53.535054 fabric_cf-1.5.0b3/LICENSE
+-rw-r--r--   0        0        0     2046 2023-04-03 14:50:53.535620 fabric_cf-1.5.0b3/README.md
+-rwxr-xr-x   0        0        0       74 2023-04-03 14:50:53.535840 fabric_cf-1.5.0b3/authority.sh
+-rwxr-xr-x   0        0        0       79 2023-04-03 14:50:53.535996 fabric_cf-1.5.0b3/broker.sh
+-rw-r--r--   0        0        0      947 2023-04-03 14:50:53.536169 fabric_cf-1.5.0b3/cleanup_old_schema_from_schema_registry.sh
+-rw-r--r--   0        0        0     2861 2023-04-03 19:02:18.268979 fabric_cf-1.5.0b3/docker-compose-kafka.yaml
+-rw-r--r--   0        0        0     1560 2023-04-03 14:50:53.536634 fabric_cf-1.5.0b3/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0    10757 2023-04-03 19:05:05.566974 fabric_cf-1.5.0b3/docker-compose-test.yaml
+-rwxr-xr-x   0        0        0       45 2023-04-03 14:50:53.536998 fabric_cf-1.5.0b3/docker-entrypoint.sh
+-rw-r--r--   0        0        0      350 2023-04-03 14:50:53.537353 fabric_cf-1.5.0b3/env.template
+-rw-r--r--   0        0        0     1135 2023-04-03 17:25:25.716942 fabric_cf-1.5.0b3/env.template.test
+-rw-r--r--   0        0        0    16609 2023-04-03 14:50:53.537818 fabric_cf-1.5.0b3/fabricNo.AnyActorNoPolicy.xml
+-rw-r--r--   0        0        0     6343 2023-04-03 14:50:53.538166 fabric_cf-1.5.0b3/fabric_cf/Design.md
+-rw-r--r--   0        0        0       24 2023-05-11 16:34:38.443594 fabric_cf-1.5.0b3/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538462 fabric_cf-1.5.0b3/fabric_cf/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538776 fabric_cf-1.5.0b3/fabric_cf/actor/boot/__init__.py
+-rw-r--r--   0        0        0    15281 2023-04-03 14:50:53.539116 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration.py
+-rw-r--r--   0        0        0     1268 2023-04-03 14:50:53.539529 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_exception.py
+-rw-r--r--   0        0        0     2509 2023-04-03 14:50:53.539906 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_loader.py
+-rw-r--r--   0        0        0    23003 2023-05-11 15:20:50.246839 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_processor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540419 fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/__init__.py
+-rw-r--r--   0        0        0     4969 2023-04-03 14:50:53.540687 fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540852 fabric_cf-1.5.0b3/fabric_cf/actor/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.541039 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/__init__.py
+-rw-r--r--   0        0        0     4907 2023-04-03 14:50:53.541250 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_container.py
+-rw-r--r--   0        0        0     1530 2023-04-03 14:50:53.541590 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_event.py
+-rw-r--r--   0        0        0     2176 2023-04-03 14:50:53.541925 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_identity.py
+-rw-r--r--   0        0        0     1991 2023-04-03 14:50:53.542388 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_management_object.py
+-rw-r--r--   0        0        0    21765 2023-04-03 14:50:53.542778 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_mixin.py
+-rw-r--r--   0        0        0     1918 2023-04-03 14:50:53.543106 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_proxy.py
+-rw-r--r--   0        0        0     1323 2023-04-03 14:50:53.543429 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_runnable.py
+-rw-r--r--   0        0        0     4497 2023-04-03 14:50:53.543679 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority.py
+-rw-r--r--   0        0        0     8736 2023-04-03 14:50:53.543930 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_policy.py
+-rw-r--r--   0        0        0     3299 2023-04-03 14:50:53.544153 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_proxy.py
+-rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.545583 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_reservation.py
+-rw-r--r--   0        0        0     6071 2023-04-03 14:50:53.545879 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_base_plugin.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.546104 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_mixin.py
+-rw-r--r--   0        0        0     1492 2023-04-03 14:50:53.546359 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
+-rw-r--r--   0        0        0     3690 2023-04-03 14:50:53.546566 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_proxy.py
+-rw-r--r--   0        0        0     4012 2023-04-03 14:50:53.546780 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_reservation.py
+-rw-r--r--   0        0        0     2442 2023-04-03 14:50:53.547038 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_callback_proxy.py
+-rw-r--r--   0        0        0     9216 2023-04-03 14:50:53.547299 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor.py
+-rw-r--r--   0        0        0     6215 2023-04-11 13:18:18.781604 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
+-rw-r--r--   0        0        0     2640 2023-04-03 14:50:53.547942 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
+-rw-r--r--   0        0        0     5802 2023-04-03 14:50:53.548385 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_policy.py
+-rw-r--r--   0        0        0     7724 2023-04-03 14:50:53.548730 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_reservation.py
+-rw-r--r--   0        0        0     1936 2023-04-03 14:50:53.548982 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_component.py
+-rw-r--r--   0        0        0     9833 2023-04-03 14:50:53.549228 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_concrete_set.py
+-rw-r--r--   0        0        0     2729 2023-04-03 14:50:53.549801 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_clock.py
+-rw-r--r--   0        0        0     3976 2023-04-03 14:50:53.550228 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_database.py
+-rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.550497 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller.py
+-rw-r--r--   0        0        0     2423 2023-04-03 14:50:53.550710 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
+-rw-r--r--   0        0        0     2787 2023-04-03 14:50:53.550900 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_policy.py
+-rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.551118 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_reservation.py
+-rw-r--r--   0        0        0    10332 2023-05-11 15:20:50.247543 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_database.py
+-rw-r--r--   0        0        0    11026 2023-04-03 14:50:53.551566 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_delegation.py
+-rw-r--r--   0        0        0     1867 2023-04-03 14:50:53.551767 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_event.py
+-rw-r--r--   0        0        0     1943 2023-04-03 14:50:53.552014 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_management_object.py
+-rw-r--r--   0        0        0     9044 2023-04-03 14:50:53.552250 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_actor.py
+-rw-r--r--   0        0        0     2534 2023-04-03 14:50:53.552486 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_authority.py
+-rw-r--r--   0        0        0     1452 2023-04-03 14:50:53.552674 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
+-rw-r--r--   0        0        0     6191 2023-04-03 14:50:53.552834 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
+-rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.553039 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_container.py
+-rw-r--r--   0        0        0     2317 2023-04-03 14:50:53.553242 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
+-rw-r--r--   0        0        0     5014 2023-04-03 14:50:53.553457 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
+-rw-r--r--   0        0        0    11147 2023-04-03 14:50:53.553629 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_policy.py
+-rw-r--r--   0        0        0     2304 2023-04-03 14:50:53.553847 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.554059 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy_factory.py
+-rw-r--r--   0        0        0     1658 2023-04-03 14:50:53.554593 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_query_response_handler.py
+-rw-r--r--   0        0        0    14096 2023-04-03 14:50:53.554880 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_mixin.py
+-rw-r--r--   0        0        0     9388 2023-04-03 14:50:53.555129 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_resources.py
+-rw-r--r--   0        0        0     5581 2023-04-03 14:50:53.555376 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_status.py
+-rw-r--r--   0        0        0     8963 2023-04-03 14:50:53.555582 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_resource_control.py
+-rw-r--r--   0        0        0     1336 2023-04-03 14:50:53.555785 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_response_handler.py
+-rw-r--r--   0        0        0     2246 2023-04-03 14:50:53.556014 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_rpc_request_state.py
+-rw-r--r--   0        0        0     5634 2023-04-03 14:50:53.556345 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_actor.py
+-rw-r--r--   0        0        0     6415 2023-04-03 14:50:53.556589 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_policy.py
+-rw-r--r--   0        0        0     4846 2023-04-03 14:50:53.556782 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_reservation.py
+-rw-r--r--   0        0        0    13280 2023-04-03 14:50:53.557016 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_slice.py
+-rw-r--r--   0        0        0     3227 2023-04-03 14:50:53.557270 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate.py
+-rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.557477 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate_database.py
+-rw-r--r--   0        0        0     2943 2023-04-03 14:50:53.557727 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_tick.py
+-rw-r--r--   0        0        0     6121 2023-04-03 14:50:53.557931 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_ticker.py
+-rw-r--r--   0        0        0     1590 2023-04-03 14:50:53.558112 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_queue.py
+-rw-r--r--   0        0        0     1387 2023-04-03 14:50:53.558344 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_task.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.558543 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/__init__.py
+-rw-r--r--   0        0        0    12749 2023-04-03 14:50:53.558881 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/constants.py
+-rw-r--r--   0        0        0     3254 2023-04-03 14:50:53.559144 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/event_logger.py
+-rw-r--r--   0        0        0     5517 2023-04-03 14:50:53.559364 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/exceptions.py
+-rw-r--r--   0        0        0     6108 2023-04-03 14:50:53.559599 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/resource_config.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.559841 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/__init__.py
+-rw-r--r--   0        0        0    24564 2023-04-03 14:50:53.560251 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/container.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.560471 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/__init__.py
+-rw-r--r--   0        0        0     8667 2023-05-11 15:20:50.248592 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/container_database.py
+-rw-r--r--   0        0        0    19263 2023-04-03 14:50:53.561010 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/globals.py
+-rw-r--r--   0        0        0     7053 2023-04-03 14:50:53.561272 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/maintenance.py
+-rw-r--r--   0        0        0     5472 2023-04-03 14:50:53.561525 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/message_service.py
+-rw-r--r--   0        0        0     1508 2023-04-03 14:50:53.561724 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/protocol_descriptor.py
+-rw-r--r--   0        0        0    13005 2023-04-03 14:50:53.562081 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/remote_actor_cache.py
+-rw-r--r--   0        0        0     8040 2023-04-03 14:50:53.562299 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/rpc_producer.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.562481 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/__init__.py
+-rw-r--r--   0        0        0    35633 2023-05-11 15:20:50.249090 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor.py
+-rw-r--r--   0        0        0     1975 2023-04-03 14:50:53.563319 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor_identity.py
+-rw-r--r--   0        0        0    14656 2023-04-03 14:50:53.563570 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority.py
+-rw-r--r--   0        0        0     4845 2023-04-03 14:50:53.563854 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority_policy.py
+-rw-r--r--   0        0        0    20313 2023-04-03 14:50:53.564180 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker.py
+-rw-r--r--   0        0        0     5914 2023-04-03 14:50:53.565067 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker_policy.py
+-rw-r--r--   0        0        0    19290 2023-05-11 15:20:50.249428 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/controller.py
+-rw-r--r--   0        0        0     8604 2023-05-11 15:20:50.249865 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/event_processor.py
+-rw-r--r--   0        0        0     5467 2023-04-03 14:50:53.565861 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/inventory_slice_manager.py
+-rw-r--r--   0        0        0     6171 2023-04-03 14:50:53.566145 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/policy.py
+-rw-r--r--   0        0        0     2042 2023-04-03 14:50:53.566366 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/rpc_request_state.py
+-rw-r--r--   0        0        0     8688 2023-04-03 14:50:53.566587 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/ticket.py
+-rw-r--r--   0        0        0    15442 2023-05-11 15:20:50.250153 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit.py
+-rw-r--r--   0        0        0    13263 2023-04-03 14:50:53.567022 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit_set.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.567201 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/__init__.py
+-rw-r--r--   0        0        0    10969 2023-04-03 14:50:53.567422 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation.py
+-rw-r--r--   0        0        0     1874 2023-04-03 14:50:53.567633 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation_factory.py
+-rw-r--r--   0        0        0    16897 2023-04-03 14:50:53.567918 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation.py
+-rw-r--r--   0        0        0     1825 2023-04-03 14:50:53.568190 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation_factory.py
+-rw-r--r--   0        0        0     5364 2023-04-03 14:50:53.568399 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/resource_ticket.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.568570 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/__init__.py
+-rw-r--r--   0        0        0    27428 2023-04-03 14:50:53.568871 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/authority_reservation.py
+-rw-r--r--   0        0        0     3384 2023-04-03 14:50:53.569249 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
+-rw-r--r--   0        0        0    26805 2023-04-03 14:50:53.569537 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_reservation.py
+-rw-r--r--   0        0        0     2992 2023-04-03 14:50:53.569880 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/claim_timeout.py
+-rw-r--r--   0        0        0     4396 2023-04-03 14:50:53.570217 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc.py
+-rw-r--r--   0        0        0     3639 2023-04-03 14:50:53.570449 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc_event.py
+-rw-r--r--   0        0        0     2668 2023-04-03 14:50:53.570827 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
+-rw-r--r--   0        0        0     2708 2023-04-03 14:50:53.571106 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
+-rw-r--r--   0        0        0     2105 2023-04-03 14:50:53.571543 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_query_rpc.py
+-rw-r--r--   0        0        0     2703 2023-04-03 14:50:53.571750 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
+-rw-r--r--   0        0        0     4158 2023-04-03 14:50:53.571968 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc.py
+-rw-r--r--   0        0        0    10748 2023-05-11 15:20:50.250399 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc_event.py
+-rw-r--r--   0        0        0    63706 2023-05-11 15:20:50.282572 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel.py
+-rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.572703 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_tick.py
+-rw-r--r--   0        0        0    55548 2023-05-11 15:20:50.250916 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_wrapper.py
+-rw-r--r--   0        0        0     2363 2023-04-03 14:50:53.573675 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/predecessor_state.py
+-rw-r--r--   0        0        0     2860 2023-04-03 14:50:53.573873 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/query_timeout.py
+-rw-r--r--   0        0        0     1404 2023-04-03 14:50:53.574038 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/request_types.py
+-rw-r--r--   0        0        0    24493 2023-04-03 14:51:26.321598 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation.py
+-rw-r--r--   0        0        0    89315 2023-05-11 15:20:50.251560 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_client.py
+-rw-r--r--   0        0        0     9994 2023-04-03 14:50:53.575366 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_server.py
+-rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.575644 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_states.py
+-rw-r--r--   0        0        0    20888 2023-04-03 14:50:53.575901 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/resource_set.py
+-rw-r--r--   0        0        0     1614 2023-04-03 14:50:53.576176 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc.py
+-rw-r--r--   0        0        0     1899 2023-04-03 14:50:53.576398 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc_event.py
+-rw-r--r--   0        0        0     4128 2023-04-03 14:50:53.576854 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_executor.py
+-rw-r--r--   0        0        0    31229 2023-05-11 15:20:50.251975 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager.py
+-rw-r--r--   0        0        0     1772 2023-04-03 14:50:53.577467 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
+-rw-r--r--   0        0        0     3579 2023-04-03 14:50:53.577700 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request.py
+-rw-r--r--   0        0        0     1620 2023-04-03 14:50:53.577956 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request_type.py
+-rw-r--r--   0        0        0     1340 2023-04-03 14:50:53.578168 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
+-rw-r--r--   0        0        0    12284 2023-04-03 14:50:53.578451 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice.py
+-rw-r--r--   0        0        0    12613 2023-05-11 16:31:49.234715 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_state_machine.py
+-rw-r--r--   0        0        0     8319 2023-04-03 14:50:53.578901 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_table.py
+-rw-r--r--   0        0        0     6527 2023-04-03 14:50:53.579044 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/tick.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.579204 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/__init__.py
+-rw-r--r--   0        0        0    37415 2023-05-11 15:20:50.252308 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/actor_management_object.py
+-rw-r--r--   0        0        0     8431 2023-04-03 14:50:53.579975 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/authority_management_object.py
+-rw-r--r--   0        0        0     6903 2023-04-11 13:18:18.767746 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/broker_management_object.py
+-rw-r--r--   0        0        0    27727 2023-05-11 15:22:36.518505 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
+-rw-r--r--   0        0        0     9605 2023-04-03 14:50:53.580935 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/container_management_object.py
+-rw-r--r--   0        0        0     8973 2023-04-11 13:18:18.771385 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/controller_management_object.py
+-rw-r--r--   0        0        0    13007 2023-04-03 14:50:53.581333 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/converter.py
+-rw-r--r--   0        0        0     1624 2023-04-03 14:50:53.581543 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/error.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.581729 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/__init__.py
+-rw-r--r--   0        0        0    10194 2023-04-03 14:50:53.582040 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_actor.py
+-rw-r--r--   0        0        0     3509 2023-04-03 14:50:53.582317 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_authority.py
+-rw-r--r--   0        0        0     8200 2023-05-11 15:20:50.252529 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     4483 2023-04-03 14:50:53.583057 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_container.py
+-rw-r--r--   0        0        0     5300 2023-04-03 14:50:53.583248 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_controller.py
+-rw-r--r--   0        0        0     5462 2023-04-03 14:50:53.583439 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
+-rw-r--r--   0        0        0     6960 2023-05-11 16:31:49.235814 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     5730 2023-04-03 14:50:53.583847 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.584078 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/__init__.py
+-rw-r--r--   0        0        0    24550 2023-04-03 14:50:53.584410 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
+-rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.584691 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
+-rw-r--r--   0        0        0     5797 2023-04-03 14:50:53.585104 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
+-rw-r--r--   0        0        0    15846 2023-04-03 14:50:53.585409 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
+-rw-r--r--   0        0        0     4008 2023-04-03 14:50:53.585584 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
+-rw-r--r--   0        0        0     8228 2023-04-03 14:50:53.585867 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
+-rw-r--r--   0        0        0     2148 2023-04-03 14:50:53.586169 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.586361 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/__init__.py
+-rw-r--r--   0        0        0    10935 2023-04-03 14:50:53.586634 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_actor.py
+-rw-r--r--   0        0        0     3902 2023-04-03 14:50:53.586852 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_authority.py
+-rw-r--r--   0        0        0     8391 2023-04-03 14:50:53.587036 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_broker.py
+-rw-r--r--   0        0        0    10119 2023-04-03 14:50:53.587201 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_container.py
+-rw-r--r--   0        0        0     9395 2023-04-03 14:50:53.587383 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_controller.py
+-rw-r--r--   0        0        0     2855 2023-04-03 14:50:53.587571 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_proxy.py
+-rw-r--r--   0        0        0     8655 2023-04-03 14:50:53.587724 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_server_actor.py
+-rw-r--r--   0        0        0     7217 2023-04-03 14:50:53.588020 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object.py
+-rw-r--r--   0        0        0     7841 2023-04-03 14:50:53.588258 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object_manager.py
+-rw-r--r--   0        0        0     4972 2023-04-03 14:50:53.588521 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_utils.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.588706 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/__init__.py
+-rw-r--r--   0        0        0     1604 2023-04-03 14:50:53.588914 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/client_mng.py
+-rw-r--r--   0        0        0     1570 2023-04-03 14:50:53.589110 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/event_mng.py
+-rw-r--r--   0        0        0     1802 2023-04-03 14:50:53.589285 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
+-rw-r--r--   0        0        0     1741 2023-04-03 14:50:53.589460 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_client_mng.py
+-rw-r--r--   0        0        0     1554 2023-04-03 14:50:53.589750 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_event_mng.py
+-rw-r--r--   0        0        0     1904 2023-04-03 14:50:53.590017 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
+-rw-r--r--   0        0        0    15777 2023-04-03 14:50:53.590202 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/server_actor_management_object.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590369 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/__init__.py
+-rw-r--r--   0        0        0     7756 2023-04-03 14:50:53.590739 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/base_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590945 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/__init__.py
+-rw-r--r--   0        0        0    31456 2023-05-11 15:20:50.253712 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/actor_database.py
+-rw-r--r--   0        0        0     2624 2023-05-11 15:20:50.254268 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/client_database.py
+-rw-r--r--   0        0        0     3792 2023-05-11 15:20:50.254603 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/server_actor_database.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.591940 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/__init__.py
+-rw-r--r--   0        0        0    12823 2023-04-03 14:50:53.592182 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
+-rw-r--r--   0        0        0     2831 2023-04-03 14:50:53.592374 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/config_token.py
+-rw-r--r--   0        0        0     2286 2023-04-03 14:50:53.592660 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
+-rw-r--r--   0        0        0     7114 2023-05-11 15:20:50.254849 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/handler_processor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593035 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/__init__.py
+-rw-r--r--   0        0        0     3612 2023-04-03 14:50:53.593263 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593460 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/__init__.py
+-rw-r--r--   0        0        0     4365 2023-05-11 15:20:50.255164 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
+-rw-r--r--   0        0        0    14268 2023-04-03 14:50:53.594012 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.594246 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/__init__.py
+-rw-r--r--   0        0        0    28295 2023-04-03 14:50:53.594548 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/authority_calendar_policy.py
+-rw-r--r--   0        0        0     8891 2023-04-03 14:50:53.595030 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_calendar_policy.py
+-rw-r--r--   0        0        0    63111 2023-04-03 14:50:53.595571 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
+-rw-r--r--   0        0        0    19840 2023-05-11 15:20:50.255474 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_calendar_policy.py
+-rw-r--r--   0        0        0     9815 2023-05-11 15:20:50.255764 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_simple_policy.py
+-rw-r--r--   0        0        0     9546 2023-05-11 15:20:50.255972 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
+-rw-r--r--   0        0        0     1814 2023-04-03 14:50:53.596494 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/fifo_queue.py
+-rw-r--r--   0        0        0     2981 2023-04-03 14:50:53.596828 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory.py
+-rw-r--r--   0        0        0     2785 2023-04-03 14:50:53.597031 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory_for_type.py
+-rw-r--r--   0        0        0    14499 2023-04-03 14:50:53.597231 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_control.py
+-rw-r--r--   0        0        0    28363 2023-04-03 14:50:53.597532 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_inventory.py
+-rw-r--r--   0        0        0     5435 2023-04-03 14:50:53.597856 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_control.py
+-rw-r--r--   0        0        0    22745 2023-04-03 14:50:53.598106 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_inventory.py
+-rw-r--r--   0        0        0     2032 2023-04-03 14:50:53.598641 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/queue_wrapper.py
+-rw-r--r--   0        0        0     5157 2023-04-03 14:50:53.598857 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/resource_control.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599020 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1821 2023-04-03 14:50:53.599277 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/actor_location.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599432 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/__init__.py
+-rw-r--r--   0        0        0     7798 2023-04-03 14:50:53.599583 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
+-rw-r--r--   0        0        0     9013 2023-04-03 14:50:53.599758 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
+-rw-r--r--   0        0        0     6686 2023-04-03 14:50:53.599942 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     4809 2023-04-03 14:50:53.600099 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
+-rw-r--r--   0        0        0     8466 2023-04-03 14:50:53.600393 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.600601 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/__init__.py
+-rw-r--r--   0        0        0    11710 2023-04-03 14:50:53.600939 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
+-rw-r--r--   0        0        0     6931 2023-04-03 14:50:53.601111 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
+-rw-r--r--   0        0        0     8218 2023-04-03 14:50:53.601343 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.601562 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
+-rw-r--r--   0        0        0    15551 2023-04-03 14:50:53.601817 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/translate.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.601999 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/__init__.py
+-rw-r--r--   0        0        0     4525 2023-04-03 14:50:53.602224 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_authority.py
+-rw-r--r--   0        0        0     5726 2023-04-03 14:50:53.602562 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_broker.py
+-rw-r--r--   0        0        0     6896 2023-04-03 14:50:53.603120 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy.py
+-rw-r--r--   0        0        0     2868 2023-04-03 14:50:53.604580 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
+-rw-r--r--   0        0        0     6397 2023-04-03 14:50:53.605005 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_return.py
+-rw-r--r--   0        0        0     8303 2023-04-03 14:50:53.605283 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy.py
+-rw-r--r--   0        0        0     3013 2023-04-03 14:50:53.605545 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy_factory.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.605762 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/__init__.py
+-rw-r--r--   0        0        0     7672 2023-04-03 14:50:53.605950 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/actor_registry.py
+-rw-r--r--   0        0        0     2177 2023-04-03 14:50:53.606181 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/callback_registry.py
+-rw-r--r--   0        0        0     4926 2023-04-03 14:50:53.606408 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/peer_registry.py
+-rw-r--r--   0        0        0     3912 2023-04-03 14:50:53.606565 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/proxy_registry.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.606740 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/__init__.py
+-rw-r--r--   0        0        0     7165 2023-04-03 14:50:53.606931 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/actor_clock.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.607146 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     8224 2023-04-03 14:50:53.607463 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/authority_calendar.py
+-rw-r--r--   0        0        0     1667 2023-04-03 14:50:53.607755 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/base_calendar.py
+-rw-r--r--   0        0        0    11573 2023-04-03 14:50:53.607991 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/broker_calendar.py
+-rw-r--r--   0        0        0     9733 2023-04-03 14:50:53.608213 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/client_calendar.py
+-rw-r--r--   0        0        0     5239 2023-04-03 14:50:53.608505 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/controller_calendar.py
+-rw-r--r--   0        0        0     2550 2023-04-03 14:50:53.608738 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/source_calendar.py
+-rw-r--r--   0        0        0    15769 2023-04-03 14:50:53.609015 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/term.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.609215 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/__init__.py
+-rw-r--r--   0        0        0     2213 2023-04-03 14:50:53.609476 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/bids.py
+-rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.609992 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/client.py
+-rw-r--r--   0        0        0     2063 2023-04-03 14:50:53.610294 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/graceful_interrupt_handler.py
+-rw-r--r--   0        0        0     2163 2023-04-03 14:50:53.610582 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/id.py
+-rw-r--r--   0        0        0     1488 2023-04-03 14:50:53.610758 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/iterable_queue.py
+-rw-r--r--   0        0        0     2263 2023-04-03 14:50:53.611043 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/kernel_timer.py
+-rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.611261 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/log_helper.py
+-rw-r--r--   0        0        0     2238 2023-04-03 14:50:53.611511 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/notice.py
+-rw-r--r--   0        0        0     1999 2023-04-03 14:50:53.611700 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reflection_utils.py
+-rw-r--r--   0        0        0     8380 2023-04-03 14:50:53.612072 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_holdings.py
+-rw-r--r--   0        0        0     8864 2023-04-03 14:50:53.612305 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_list.py
+-rw-r--r--   0        0        0     6700 2023-05-11 15:20:50.256475 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_set.py
+-rw-r--r--   0        0        0     3144 2023-04-03 14:50:53.612687 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_state.py
+-rw-r--r--   0        0        0     2250 2023-04-03 14:50:53.612855 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/resource_type.py
+-rw-r--r--   0        0        0     1690 2023-04-03 14:50:53.613024 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/rpc_exception.py
+-rw-r--r--   0        0        0     4440 2023-04-03 14:50:53.613195 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/update_data.py
+-rw-r--r--   0        0        0     4188 2023-04-03 14:50:53.613384 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/utils.py
+-rw-r--r--   0        0        0     7474 2023-04-03 14:50:53.613876 fabric_cf-1.5.0b3/fabric_cf/actor/db/__init__.py
+-rw-r--r--   0        0        0    58450 2023-05-11 15:20:50.257173 fabric_cf-1.5.0b3/fabric_cf/actor/db/psql_database.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.614689 fabric_cf-1.5.0b3/fabric_cf/actor/fim/__init__.py
+-rw-r--r--   0        0        0     6326 2023-05-11 15:20:50.257526 fabric_cf-1.5.0b3/fabric_cf/actor/fim/asm_update_thread.py
+-rw-r--r--   0        0        0    28243 2023-05-11 15:20:50.258048 fabric_cf-1.5.0b3/fabric_cf/actor/fim/fim_helper.py
+-rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616623 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616848 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/__init__.py
+-rw-r--r--   0        0        0    23622 2023-04-03 14:50:53.617119 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617325 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/__init__.py
+-rw-r--r--   0        0        0     2842 2023-04-03 14:50:53.617552 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/handler_base.py
+-rw-r--r--   0        0        0     9305 2023-04-03 14:50:53.617730 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/no_op_handler.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617898 fabric_cf-1.5.0b3/fabric_cf/actor/security/__init__.py
+-rw-r--r--   0        0        0     4348 2023-04-03 14:50:53.618115 fabric_cf-1.5.0b3/fabric_cf/actor/security/access_checker.py
+-rw-r--r--   0        0        0     2955 2023-04-03 14:50:53.618313 fabric_cf-1.5.0b3/fabric_cf/actor/security/auth_token.py
+-rw-r--r--   0        0        0     3983 2023-05-11 15:20:50.258526 fabric_cf-1.5.0b3/fabric_cf/actor/security/fabric_token.py
+-rw-r--r--   0        0        0     8635 2023-04-03 14:50:53.618697 fabric_cf-1.5.0b3/fabric_cf/actor/security/pdp_auth.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.618864 fabric_cf-1.5.0b3/fabric_cf/actor/test/__init__.py
+-rw-r--r--   0        0        0    10932 2023-04-04 13:01:29.470229 fabric_cf-1.5.0b3/fabric_cf/actor/test/base_test_case.py
+-rw-r--r--   0        0        0     4679 2023-04-03 14:50:53.619270 fabric_cf-1.5.0b3/fabric_cf/actor/test/client_callback_helper.py
+-rw-r--r--   0        0        0     4639 2023-04-05 14:49:38.077013 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.jenkins.yaml
+-rw-r--r--   0        0        0     4305 2023-04-04 15:28:06.631503 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4696 2023-04-05 17:47:55.443819 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.test.yaml
+-rw-r--r--   0        0        0     5376 2023-04-03 14:50:53.620212 fabric_cf-1.5.0b3/fabric_cf/actor/test/controller_callback_helper.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620415 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620599 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/__init__.py
+-rw-r--r--   0        0        0     2815 2023-04-04 13:02:25.891866 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/container_database_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621040 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/__init__.py
+-rw-r--r--   0        0        0     4091 2023-04-04 13:02:48.136107 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/unit_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621493 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/__init__.py
+-rw-r--r--   0        0        0    21480 2023-04-04 15:12:06.450576 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/kernel_test.py
+-rw-r--r--   0        0        0     3378 2023-04-04 15:11:51.860496 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/tick_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.624033 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/__init__.py
+-rw-r--r--   0        0        0     3176 2023-04-04 15:15:43.466105 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/actor_database_test.py
+-rw-r--r--   0        0        0     4729 2023-04-04 17:23:55.100076 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
+-rw-r--r--   0        0        0     1963 2023-04-03 14:50:53.624564 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
+-rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.624725 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_database_test.py
+-rw-r--r--   0        0        0     2280 2023-04-04 15:15:47.470348 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_test_base.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.625348 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/__init__.py
+-rw-r--r--   0        0        0    21995 2023-04-04 17:23:55.095211 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
+-rw-r--r--   0        0        0    23678 2023-04-04 17:23:55.075259 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
+-rw-r--r--   0        0        0     4515 2023-04-04 17:23:55.081745 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
+-rw-r--r--   0        0        0     1561 2023-04-03 14:50:53.626668 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
+-rw-r--r--   0        0        0     8437 2023-04-03 14:50:53.626899 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
+-rw-r--r--   0        0        0     7719 2023-04-04 17:23:55.088766 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
+-rw-r--r--   0        0        0     1586 2023-04-03 14:50:53.627291 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627471 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/__init__.py
+-rw-r--r--   0        0        0     3786 2023-04-03 14:50:53.627666 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/actor_clock_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627830 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:50:53.628007 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
+-rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.628189 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
+-rw-r--r--   0        0        0    14887 2023-04-03 14:50:53.628405 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/term_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.628584 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/__init__.py
+-rw-r--r--   0        0        0     8041 2023-04-03 14:50:53.628792 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_holdings_test.py
+-rw-r--r--   0        0        0     5072 2023-04-03 14:50:53.628930 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_list_test.py
+-rw-r--r--   0        0        0     3738 2023-04-03 14:50:53.629079 fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_authority_proxy.py
+-rw-r--r--   0        0        0     1953 2023-04-03 14:50:53.629248 fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_proxy.py
+-rw-r--r--   0        0        0     2498 2023-04-04 16:00:31.265177 fabric_cf-1.5.0b3/fabric_cf/actor/test/fim_test_helper.py
+-rw-r--r--   0        0        0       92 2023-04-03 15:02:26.648185 fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/key.avsc
+-rw-r--r--   0        0        0    27389 2023-04-03 15:02:26.648701 fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/message.avsc
+-rw-r--r--   0        0        0     4532 2023-04-03 15:21:18.938300 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_abqm.py
+-rw-r--r--   0        0        0     1892 2023-04-03 14:50:53.630509 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_actor.py
+-rw-r--r--   0        0        0     1249 2023-04-03 14:50:53.630745 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_exception.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.630912 fabric_cf-1.5.0b3/fabric_cf/aits/__init__.py
+-rw-r--r--   0        0        0     4826 2023-04-05 16:57:12.446895 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.broker.yaml
+-rw-r--r--   0        0        0     4808 2023-04-05 16:57:36.798748 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.netam.yaml
+-rw-r--r--   0        0        0     4414 2023-04-05 16:57:45.775270 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4788 2023-04-05 16:57:55.683500 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.siteam.yaml
+-rw-r--r--   0        0        0    49220 2023-04-07 14:15:47.763078 fabric_cf-1.5.0b3/fabric_cf/aits/integration_test.py
+-rw-r--r--   0        0        0     7393 2023-04-06 18:22:24.720925 fabric_cf-1.5.0b3/fabric_cf/aits/kafka_processor.py
+-rw-r--r--   0        0        0     8633 2023-04-06 18:12:27.261323 fabric_cf-1.5.0b3/fabric_cf/aits/manage_helper.py
+-rw-r--r--   0        0        0     8339 2023-04-06 16:21:40.377393 fabric_cf-1.5.0b3/fabric_cf/aits/orchestrator_helper.py
+-rw-r--r--   0        0        0    16256 2023-04-03 14:50:53.634161 fabric_cf-1.5.0b3/fabric_cf/authority/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.634241 fabric_cf-1.5.0b3/fabric_cf/authority/__init__.py
+-rw-r--r--   0        0        0     2164 2023-04-03 14:50:53.634418 fabric_cf-1.5.0b3/fabric_cf/authority/__main__.py
+-rw-r--r--   0        0        0    32973 2023-04-03 14:50:53.634699 fabric_cf-1.5.0b3/fabric_cf/authority/am-yes.xml
+-rw-r--r--   0        0        0     4936 2023-04-03 14:50:53.634941 fabric_cf-1.5.0b3/fabric_cf/authority/config.al2s.am.yaml
+-rw-r--r--   0        0        0     5030 2023-04-03 14:50:53.635111 fabric_cf-1.5.0b3/fabric_cf/authority/config.net.am.yaml
+-rw-r--r--   0        0        0     5402 2023-04-03 14:50:53.635298 fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.geni.yaml
+-rw-r--r--   0        0        0     4896 2023-04-03 14:50:53.635465 fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.yaml
+-rw-r--r--   0        0        0     3427 2023-05-11 16:23:44.688550 fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.geni.yml
+-rw-r--r--   0        0        0     3336 2023-05-11 16:23:58.379562 fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.yml
+-rw-r--r--   0        0        0     1188 2023-05-11 16:24:05.923091 fabric_cf-1.5.0b3/fabric_cf/authority/env.template
+-rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.636162 fabric_cf-1.5.0b3/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1588 2023-04-03 14:50:53.636606 fabric_cf-1.5.0b3/fabric_cf/authority/net_handler_config.yml
+-rw-r--r--   0        0        0     1523 2023-04-03 14:50:53.636812 fabric_cf-1.5.0b3/fabric_cf/authority/oess_handler_config.yml
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.636998 fabric_cf-1.5.0b3/fabric_cf/authority/pdp.xml
+-rwxr-xr-x   0        0        0     2446 2023-04-03 14:50:53.637179 fabric_cf-1.5.0b3/fabric_cf/authority/setup.sh
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.637346 fabric_cf-1.5.0b3/fabric_cf/authority/test/__init__.py
+-rw-r--r--   0        0        0     2463 2023-04-03 14:50:53.637572 fabric_cf-1.5.0b3/fabric_cf/authority/test/al2s_am.py
+-rw-r--r--   0        0        0     2459 2023-04-03 14:50:53.637740 fabric_cf-1.5.0b3/fabric_cf/authority/test/net_am.py
+-rw-r--r--   0        0        0     2456 2023-04-03 14:50:53.637876 fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am.py
+-rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.638045 fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am_geni.py
+-rw-r--r--   0        0        0     4729 2023-04-03 14:50:53.638234 fabric_cf-1.5.0b3/fabric_cf/authority/test/test-al2sam.yaml
+-rw-r--r--   0        0        0     4839 2023-04-05 17:18:17.956714 fabric_cf-1.5.0b3/fabric_cf/authority/test/test-netam.yaml
+-rw-r--r--   0        0        0     5071 2023-04-03 14:50:53.638536 fabric_cf-1.5.0b3/fabric_cf/authority/test/test.geni.yaml
+-rw-r--r--   0        0        0     4685 2023-04-05 17:18:17.952345 fabric_cf-1.5.0b3/fabric_cf/authority/test/test.yaml
+-rw-r--r--   0        0        0     2779 2023-05-11 15:20:50.260288 fabric_cf-1.5.0b3/fabric_cf/authority/vm_handler_config.yml
+-rw-r--r--   0        0        0     1448 2023-04-03 14:50:53.639031 fabric_cf-1.5.0b3/fabric_cf/authority/vnic_net_handler_config.yml
+-rw-r--r--   0        0        0    14262 2023-04-03 14:50:53.639328 fabric_cf-1.5.0b3/fabric_cf/broker/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.639412 fabric_cf-1.5.0b3/fabric_cf/broker/__init__.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.639603 fabric_cf-1.5.0b3/fabric_cf/broker/__main__.py
+-rw-r--r--   0        0        0    27944 2023-04-03 14:50:53.639781 fabric_cf-1.5.0b3/fabric_cf/broker/broker-yes.xml
+-rw-r--r--   0        0        0     5035 2023-04-03 14:50:53.640005 fabric_cf-1.5.0b3/fabric_cf/broker/config.broker.yaml
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.640163 fabric_cf-1.5.0b3/fabric_cf/broker/core/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.640348 fabric_cf-1.5.0b3/fabric_cf/broker/core/broker_kernel.py
+-rw-r--r--   0        0        0     3135 2023-05-11 16:25:29.197878 fabric_cf-1.5.0b3/fabric_cf/broker/docker-compose.yml
+-rw-r--r--   0        0        0     1192 2023-05-11 16:25:51.672782 fabric_cf-1.5.0b3/fabric_cf/broker/env.template
+-rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.640954 fabric_cf-1.5.0b3/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.641105 fabric_cf-1.5.0b3/fabric_cf/broker/pdp.xml
+-rwxr-xr-x   0        0        0     2239 2023-04-03 14:50:53.641257 fabric_cf-1.5.0b3/fabric_cf/broker/setup.sh
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.641487 fabric_cf-1.5.0b3/fabric_cf/broker/test/__init__.py
+-rw-r--r--   0        0        0     2507 2023-04-03 14:50:53.641689 fabric_cf-1.5.0b3/fabric_cf/broker/test/broker.py
+-rw-r--r--   0        0        0     5042 2023-04-05 17:51:02.224321 fabric_cf-1.5.0b3/fabric_cf/broker/test/test.yaml
+-rw-r--r--   0        0        0    20305 2023-05-11 15:20:50.261921 fabric_cf-1.5.0b3/fabric_cf/orchestrator/README.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.642384 fabric_cf-1.5.0b3/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0     3355 2023-05-11 15:20:50.262402 fabric_cf-1.5.0b3/fabric_cf/orchestrator/__main__.py
+-rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.642803 fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.642965 fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/privkey.pem
+-rw-r--r--   0        0        0     4859 2023-05-11 16:31:49.236795 fabric_cf-1.5.0b3/fabric_cf/orchestrator/config.orchestrator.yaml
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.643278 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/__init__.py
+-rw-r--r--   0        0        0     2917 2023-04-03 14:50:53.643501 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/active_status_checker.py
+-rw-r--r--   0        0        0     3050 2023-04-03 14:50:53.643707 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/bqm_wrapper.py
+-rw-r--r--   0        0        0     1556 2023-04-03 14:50:53.643947 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/exceptions.py
+-rw-r--r--   0        0        0     1884 2023-04-03 14:50:53.644155 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/i_status_update_callback.py
+-rw-r--r--   0        0        0    39097 2023-05-11 15:20:50.264144 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_handler.py
+-rw-r--r--   0        0        0     5389 2023-04-03 14:50:53.644692 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_kernel.py
+-rw-r--r--   0        0        0    34864 2023-04-03 14:50:53.645078 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
+-rw-r--r--   0        0        0     3581 2023-04-03 14:50:53.645306 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_converter.py
+-rw-r--r--   0        0        0     4880 2023-04-03 14:50:53.645464 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update.py
+-rw-r--r--   0        0        0     7876 2023-04-03 14:50:53.645708 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update_thread.py
+-rw-r--r--   0        0        0     6179 2023-04-03 14:50:53.645975 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/response_builder.py
+-rw-r--r--   0        0        0     8722 2023-04-11 15:09:36.158110 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/slice_defer_thread.py
+-rw-r--r--   0        0        0     1972 2023-04-03 14:50:53.646372 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/status_checker.py
+-rw-r--r--   0        0        0     1581 2023-04-03 14:50:53.646556 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/watch_entry.py
+-rw-r--r--   0        0        0     3501 2023-05-11 16:25:29.205244 fabric_cf-1.5.0b3/fabric_cf/orchestrator/docker-compose.yml
+-rw-r--r--   0        0        0     1198 2023-05-11 16:25:39.495582 fabric_cf-1.5.0b3/fabric_cf/orchestrator/env.template
+-rw-r--r--   0        0        0    72323 2023-04-03 14:50:53.647218 fabric_cf-1.5.0b3/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
+-rw-r--r--   0        0        0     1626 2023-04-03 14:50:53.647500 fabric_cf-1.5.0b3/fabric_cf/orchestrator/nginx/default.conf
+-rw-r--r--   0        0        0    46956 2023-05-11 15:20:50.265345 fabric_cf-1.5.0b3/fabric_cf/orchestrator/openapi.json
+-rw-r--r--   0        0        0    30829 2023-04-03 14:50:53.648266 fabric_cf-1.5.0b3/fabric_cf/orchestrator/orchestrator-yes.xml
+-rw-r--r--   0        0        0     1548 2023-04-03 14:50:53.648514 fabric_cf-1.5.0b3/fabric_cf/orchestrator/pdp.xml
+-rwxr-xr-x   0        0        0     2284 2023-04-03 14:50:53.648696 fabric_cf-1.5.0b3/fabric_cf/orchestrator/setup.sh
+-rw-r--r--   0        0        0      430 2023-04-03 14:50:53.648991 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/__init__.py
+-rw-r--r--   0        0        0      392 2023-04-03 14:50:53.649220 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.649376 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-03 14:50:53.649537 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0        0        0     1241 2023-04-03 14:50:53.649770 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
+-rw-r--r--   0        0        0     5510 2023-05-11 15:20:50.265817 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
+-rw-r--r--   0        0        0      860 2023-04-03 14:50:53.650215 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
+-rw-r--r--   0        0        0      305 2023-04-03 14:50:53.650408 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
+-rw-r--r--   0        0        0      631 2023-04-03 14:50:53.650559 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/encoder.py
+-rw-r--r--   0        0        0     2275 2023-04-03 14:50:53.650868 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1889 2023-04-03 14:50:53.651022 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     1628 2023-04-03 14:50:53.651195 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resource.py
+-rw-r--r--   0        0        0     3564 2023-04-03 14:50:53.651368 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resources.py
+-rw-r--r--   0        0        0     7311 2023-04-03 14:50:53.651598 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice.py
+-rw-r--r--   0        0        0     3616 2023-04-03 14:50:53.651786 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice_details.py
+-rw-r--r--   0        0        0     5251 2023-04-03 14:50:53.651992 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slices.py
+-rw-r--r--   0        0        0     8995 2023-04-03 14:50:53.652138 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/sliver.py
+-rw-r--r--   0        0        0     5301 2023-04-03 14:50:53.652316 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slivers.py
+-rw-r--r--   0        0        0     3896 2023-04-03 14:50:53.652450 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     2464 2023-04-03 14:50:53.652610 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4929 2023-04-03 14:50:53.652747 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     2870 2023-04-03 14:50:53.652914 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
+-rw-r--r--   0        0        0     1983 2023-04-03 14:50:53.653092 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
+-rw-r--r--   0        0        0     4503 2023-04-03 14:50:53.653265 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     3984 2023-04-03 14:50:53.653436 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     2512 2023-04-03 14:50:53.653613 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     3879 2023-04-03 14:50:53.653846 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
+-rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.654001 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     3846 2023-04-03 14:50:53.654159 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
+-rw-r--r--   0        0        0     2446 2023-04-03 14:50:53.654361 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     4233 2023-04-03 14:50:53.654697 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     2635 2023-04-03 14:50:53.654868 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3540 2023-04-03 14:50:53.655073 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version.py
+-rw-r--r--   0        0        0     2536 2023-04-03 14:50:53.655253 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version_data.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.655440 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-03 14:50:53.655618 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
+-rw-r--r--   0        0        0     1941 2023-05-11 15:20:50.266214 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/constants.py
+-rw-r--r--   0        0        0     5537 2023-04-03 14:50:53.655976 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/cors_response.py
+-rw-r--r--   0        0        0     4321 2023-04-03 14:50:53.656175 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
+-rw-r--r--   0        0        0    15207 2023-05-11 15:20:50.266552 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
+-rw-r--r--   0        0        0     4449 2023-04-03 14:50:53.656622 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
+-rw-r--r--   0        0        0     2530 2023-04-03 14:50:53.656817 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/utils.py
+-rw-r--r--   0        0        0     2632 2023-04-05 17:52:22.168825 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/version_controller.py
+-rw-r--r--   0        0        0    34085 2023-05-11 15:20:50.266865 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      438 2023-04-03 14:50:53.657698 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0     2094 2023-04-03 14:50:53.658010 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
+-rw-r--r--   0        0        0     5143 2023-05-11 15:20:50.267349 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
+-rw-r--r--   0        0        0     1903 2023-04-03 14:50:53.658437 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
+-rw-r--r--   0        0        0      855 2023-04-03 14:50:53.658595 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
+-rw-r--r--   0        0        0      809 2023-04-03 14:50:53.658764 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/type_util.py
+-rw-r--r--   0        0        0     3452 2023-04-03 14:50:53.658932 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/util.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.659106 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/__init__.py
+-rw-r--r--   0        0        0     3542 2023-04-03 14:50:53.659281 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/orchestrator.py
+-rwxr-xr-x   0        0        0       78 2023-04-03 14:50:53.659409 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.sh
+-rw-r--r--   0        0        0     4453 2023-04-05 17:51:26.470070 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.yaml
+-rwxr-xr-x   0        0        0     2900 2023-04-03 14:50:53.659782 fabric_cf-1.5.0b3/fabric_cf/orchestrator/update_swagger_stub.sh
+-rw-r--r--   0        0        0    18177 2023-04-03 14:50:53.660187 fabric_cf-1.5.0b3/images/am-pod.png
+-rw-r--r--   0        0        0    74927 2023-04-03 14:50:53.660890 fabric_cf-1.5.0b3/images/am.png
+-rw-r--r--   0        0        0    18471 2023-04-03 14:50:53.661225 fabric_cf-1.5.0b3/images/broker-pod.png
+-rw-r--r--   0        0        0    73799 2023-04-03 14:50:53.661878 fabric_cf-1.5.0b3/images/broker.png
+-rw-r--r--   0        0        0    90831 2023-04-03 14:50:53.662835 fabric_cf-1.5.0b3/images/cf.png
+-rw-r--r--   0        0        0    19611 2023-04-03 14:50:53.663247 fabric_cf-1.5.0b3/images/orchestrator-pod.png
+-rw-r--r--   0        0        0    78622 2023-04-03 14:50:53.664084 fabric_cf-1.5.0b3/images/orchestrator.png
+-rw-r--r--   0        0        0   145542 2023-04-03 14:50:53.664854 fabric_cf-1.5.0b3/neo4j/AL2S.graphml
+-rw-r--r--   0        0        0    96363 2023-04-03 14:50:53.665732 fabric_cf-1.5.0b3/neo4j/LBNL-ad.graphml
+-rw-r--r--   0        0        0    68182 2023-04-03 14:50:53.666334 fabric_cf-1.5.0b3/neo4j/Network-ad.graphml
+-rw-r--r--   0        0        0    96375 2023-04-03 14:50:53.666804 fabric_cf-1.5.0b3/neo4j/RENCI-ad.graphml
+-rw-r--r--   0        0        0    96286 2023-04-03 14:50:53.667143 fabric_cf-1.5.0b3/neo4j/UKY-ad.graphml
+-rw-r--r--   0        0        0  1297955 2023-04-03 14:50:53.672629 fabric_cf-1.5.0b3/neo4j/UKY2.graphml
+-rw-r--r--   0        0        0    14808 2023-04-03 14:50:53.673167 fabric_cf-1.5.0b3/neo4j/abqm.graphml
+-rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.673435 fabric_cf-1.5.0b3/neo4j/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.673617 fabric_cf-1.5.0b3/neo4j/certs/privkey.pem
+-rwxr-xr-x   0        0        0       91 2023-04-03 14:50:53.673785 fabric_cf-1.5.0b3/orchestrator.sh
+-rw-r--r--   0        0        0      698 2023-04-03 14:50:53.673962 fabric_cf-1.5.0b3/psql.upgrade
+-rw-r--r--   0        0        0     1252 2023-05-11 15:29:39.647926 fabric_cf-1.5.0b3/pyproject.toml
+-rwxr-xr-x   0        0        0     2421 2023-04-03 18:36:31.758196 fabric_cf-1.5.0b3/secrets/create-certs.sh
+-rw-r--r--   0        0        0    12796 2023-05-11 16:31:49.237238 fabric_cf-1.5.0b3/tools/audit.py
+-rw-r--r--   0        0        0     8005 2023-04-03 14:50:53.675250 fabric_cf-1.5.0b3/tools/db_cli.py
+-rw-r--r--   0        0        0      354 2023-05-11 16:31:49.238481 fabric_cf-1.5.0b3/tools/install.sh
+-rw-r--r--   0        0        0      143 2023-04-03 14:50:53.675627 fabric_cf-1.5.0b3/tox.ini
+-rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 fabric_cf-1.5.0b3/PKG-INFO
```

### Comparing `fabric_cf-1.5.0b2/.gitignore` & `fabric_cf-1.5.0b3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -142,7 +142,11 @@
 neo4j2/
 neo4j3/
 neo4j4/
 pdp/
 pg_data/
 schema/
 ssl/
+fabric_cf/actor/test/*.graphml
+secrets/kafkacat2-ca1-signed.pem
+secrets/kafkacat1-ca1-signed.pem
+secrets/...
```

### Comparing `fabric_cf-1.5.0b2/Dockerfile-auth` & `fabric_cf-1.5.0b3/Dockerfile-auth`

 * *Files 13% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 VOLUME ["/usr/src/app"]
 
 EXPOSE 11000
 
 RUN apt-get update
 RUN apt-get install cron -y
 
-COPY requirements.txt /usr/src/app/
 COPY docker-entrypoint.sh /usr/src/app/
 COPY fabric_cf /usr/src/app/fabric_cf
-COPY tools/cleanup.py /usr/src/app/fabric_cf/
-COPY tools/install.sh /usr/src/app/fabric_cf/
+COPY pyproject.toml /usr/src/app/
+COPY README.md /usr/src/app/
+COPY tools/audit.py /usr/src/app/
+COPY tools/install.sh /usr/src/app/
 
-RUN pip3 install --no-cache-dir -r requirements.txt
+RUN pip3 install .
 RUN mkdir -p "/etc/fabric/message_bus/schema"
 RUN mkdir -p "/etc/fabric/actor/config"
 RUN mkdir -p "/var/log/actor"
 RUN cp /usr/local/lib/python3.9/site-packages/fabric_mb/message_bus/schema/*.avsc /etc/fabric/message_bus/schema
 RUN pip3 install fabric-am-handlers==${HANDLERS_VER}
-RUN sh /usr/src/app/fabric_cf/install.sh
+RUN sh /usr/src/app/install.sh
 
 ENTRYPOINT ["/usr/src/app/docker-entrypoint.sh"]
 CMD ["fabric_cf.authority"]
```

### Comparing `fabric_cf-1.5.0b2/Dockerfile-broker` & `fabric_cf-1.5.0b3/Dockerfile-cf`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 VOLUME ["/usr/src/app"]
 
 EXPOSE 11000
 
 RUN apt-get update
 RUN apt-get install cron -y
 
-COPY requirements.txt /usr/src/app/
-COPY docker-entrypoint.sh /usr/src/app/
 COPY fabric_cf /usr/src/app/fabric_cf
-COPY tools/cleanup.py /usr/src/app/fabric_cf/
-COPY tools/install.sh /usr/src/app/fabric_cf/
+COPY pyproject.toml /usr/src/app/
+COPY README.md /usr/src/app/
+COPY tools/audit.py /usr/src/app/
+COPY tools/install.sh /usr/src/app/
 
-RUN pip3 install --no-cache-dir -r requirements.txt
+RUN pip3 install .
 RUN mkdir -p "/etc/fabric/message_bus/schema"
 RUN mkdir -p "/etc/fabric/actor/config"
 RUN mkdir -p "/var/log/actor"
 RUN cp /usr/local/lib/python3.9/site-packages/fabric_mb/message_bus/schema/*.avsc /etc/fabric/message_bus/schema
-RUN sh /usr/src/app/fabric_cf/install.sh
 
-ENTRYPOINT ["/usr/src/app/docker-entrypoint.sh"]
-CMD ["fabric_cf.broker"]
+RUN echo "0 2 * * * root /usr/local/bin/python3.9 /usr/src/app/audit.py -f /etc/fabric/actor/config/config.yaml -d 30 -c slices -o remove" >> /etc/crontab
+RUN echo "0/15 * * * * root /usr/local/bin/python3.9 /usr/src/app/audit.py -f /etc/fabric/actor/config/config.yaml -d 30 -c slivers -o close" >> /etc/crontab
+RUN service cron reload
+RUN service cron restart
+
+ENTRYPOINT ["sh"]
+CMD ["tail", "-f", "/dev/null"]
```

### Comparing `fabric_cf-1.5.0b2/Dockerfile-orchestrator` & `fabric_cf-1.5.0b3/Dockerfile-orchestrator`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 EXPOSE 11000
 EXPOSE 8700
 
 RUN apt-get update
 RUN apt-get install cron -y
 
-COPY requirements.txt /usr/src/app/
 COPY docker-entrypoint.sh /usr/src/app/
 COPY fabric_cf /usr/src/app/fabric_cf
-COPY tools/cleanup.py /usr/src/app/fabric_cf/
-COPY tools/install.sh /usr/src/app/fabric_cf/
+COPY pyproject.toml /usr/src/app/
+COPY README.md /usr/src/app/
+COPY tools/audit.py /usr/src/app/
+COPY tools/install.sh /usr/src/app/
 
-RUN pip3 install --no-cache-dir -r requirements.txt
+RUN pip3 install .
 RUN mkdir -p "/etc/fabric/message_bus/schema"
 RUN mkdir -p "/etc/fabric/actor/config"
 RUN mkdir -p "/var/log/actor"
 RUN cp /usr/local/lib/python3.9/site-packages/fabric_mb/message_bus/schema/*.avsc /etc/fabric/message_bus/schema
-RUN sh /usr/src/app/fabric_cf/install.sh
+RUN sh /usr/src/app/install.sh
 
 ENTRYPOINT ["/usr/src/app/docker-entrypoint.sh"]
 CMD ["fabric_cf.orchestrator"]
```

### Comparing `fabric_cf-1.5.0b2/LICENSE` & `fabric_cf-1.5.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/README.md` & `fabric_cf-1.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/cleanup_old_schema_from_schema_registry.sh` & `fabric_cf-1.5.0b3/cleanup_old_schema_from_schema_registry.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/docker-compose-kafka.yaml` & `fabric_cf-1.5.0b3/docker-compose-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/docker-compose-no-ssl-kafka.yaml` & `fabric_cf-1.5.0b3/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/docker-compose-test.yaml` & `fabric_cf-1.5.0b3/docker-compose-test.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -18,40 +18,28 @@
   broker1:
     image: confluentinc/cp-kafka:latest
     restart: always
     hostname: broker1
     container_name: broker1
     depends_on:
       - zookeeper
-    volumes:
-      - ${KAFKA_SSL_SECRETS_DIR}:/etc/kafka/secrets
     ports:
       - 9092:9092
       - 19092:19092
     environment:
       KAFKA_BROKER_ID: 1
       KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
-      KAFKA_LISTENER_SECURITY_PROTOCOL_MAP: SSL:SSL,SSL_HOST:SSL
-      KAFKA_ADVERTISED_LISTENERS: SSL://broker1:9092,SSL_HOST://localhost:19092
+      KAFKA_LISTENER_SECURITY_PROTOCOL_MAP: PLAINTEXT:PLAINTEXT,PLAINTEXT_HOST:PLAINTEXT
+      KAFKA_ADVERTISED_LISTENERS: PLAINTEXT://broker1:9092,PLAINTEXT_HOST://localhost:19092
       KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR: 1
       KAFKA_GROUP_INITIAL_REBALANCE_DELAY_MS: 0
       KAFKA_CONFLUENT_LICENSE_TOPIC_REPLICATION_FACTOR: 1
       KAFKA_TRANSACTION_STATE_LOG_MIN_ISR: 1
       KAFKA_TRANSACTION_STATE_LOG_REPLICATION_FACTOR: 1
 
-
-      KAFKA_SSL_KEYSTORE_FILENAME: kafka.broker1.keystore.jks
-      KAFKA_SSL_KEYSTORE_CREDENTIALS: broker1_keystore_creds
-      KAFKA_SSL_KEY_CREDENTIALS: broker1_sslkey_creds
-      KAFKA_SSL_TRUSTSTORE_FILENAME: kafka.broker1.truststore.jks
-      KAFKA_SSL_TRUSTSTORE_CREDENTIALS: broker1_truststore_creds
-      KAFKA_SSL_ENDPOINT_IDENTIFICATION_ALGORITHM: " "
-      KAFKA_SSL_CLIENT_AUTH: requested
-      KAFKA_SECURITY_INTER_BROKER_PROTOCOL: SSL
-
   schemaregistry:
     image: confluentinc/cp-schema-registry:latest
     container_name: schemaregistry
     restart: always
     depends_on:
       - zookeeper
       - broker1
@@ -60,26 +48,14 @@
     ports:
       - 8081:8081
     environment:
       SCHEMA_REGISTRY_KAFKASTORE_BOOTSTRAP_SERVERS: broker1:9092
       SCHEMA_REGISTRY_KAFKASTORE_CONNECTION_URL: zookeeper:2181
       SCHEMA_REGISTRY_HOST_NAME: schemaregistry
       SCHEMA_REGISTRY_LISTENERS: http://0.0.0.0:8081
-      SCHEMA_REGISTRY_KAFKASTORE_SECURITY_PROTOCOL: SSL
-
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_TRUSTSTORE_LOCATION: /etc/kafka/secrets/kafka.schemaregistry.truststore.jks
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_TRUSTSTORE_PASSWORD: fabric
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_KEYSTORE_LOCATION: /etc/kafka/secrets/kafka.schemaregistry.keystore.jks
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_KEYSTORE_PASSWORD: fabric
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_KEY_PASSWORD: fabric
-      SCHEMA_REGISTRY_KAFKASTORE_SSL_ENDPOINT_IDENTIFICATION_ALGORITHM: " "
-
-      SCHEMA_REGISTRY_SSL_KEYSTORE_LOCATION: /etc/kafka/secrets/kafka.schemaregistry.keystore.jks
-      SCHEMA_REGISTRY_SSL_KEYSTORE_PASSWORD: fabric
-      SCHEMA_REGISTRY_SSL_KEY_PASSWORD: fabric
       SCHEMA_REGISTRY_DEBUG: 'true'
   database:
     image: fabrictestbed/postgres:12.3
     container_name: database
     restart: always
     ports:
       - 5432:5432
```

### Comparing `fabric_cf-1.5.0b2/fabricNo.AnyActorNoPolicy.xml` & `fabric_cf-1.5.0b3/fabricNo.AnyActorNoPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/Design.md` & `fabric_cf-1.5.0b3/fabric_cf/Design.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_exception.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_loader.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/boot/configuration_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,14 @@
         # peers between actors of same type aren't allowed unless the actors are both brokers
         if peer_type == actor_type and peer_type != ActorType.Broker:
             raise ConfigurationException(
                 "Invalid peer type: broker can only talk to broker, orchestrator or site authority")
 
         container = ManagementUtils.connect(caller=self.actor.get_identity())
         mgmt_actor = container.get_actor(guid=actor_guid)
-        self.logger.info(f"Management Actor: {mgmt_actor} === {type(mgmt_actor)}")
         if mgmt_actor is None and container.get_last_error() is not None:
             self.logger.error(container.get_last_error())
 
         self.vertex_to_registry_cache(peer=peer)
 
         try:
             client = RemoteActorCacheSingleton.get().establish_peer(mgmt_actor=mgmt_actor, peer_guid=peer_guid,
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_container.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_event.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_identity.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_actor_runnable.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_runnable.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_authority_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_base_plugin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_broker_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_callback_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_actor_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor_management_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         Add reservations
         @param reservations : reservations to be added
         @param caller: caller
         @return reservation ids on success and error code on failure (ResultStringsAvro)
         """
 
     @abstractmethod
-    def extend_reservation(self, *, reservation: id, new_end_time: datetime, sliver: BaseSliver,
+    def extend_reservation(self, *, reservation: ID, new_end_time: datetime, sliver: BaseSliver,
                            caller: AuthToken, dependencies: List[ReservationPredecessorAvro] = None) -> ResultAvro:
         """
         Extend a reservation
         @param reservation : reservation to be extended
         @param new_end_time: new end time
         @param sliver: new sliver
         @param caller: caller
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_callback_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_client_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_component.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_component.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_concrete_set.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_concrete_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_container_clock.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_container_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_controller_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,16 @@
 
         @throws Exception in case of error
         """
 
     @abstractmethod
     def get_reservations(self, *, slice_id: ID = None, graph_node_id: str = None, project_id: str = None,
                          email: str = None, oidc_sub: str = None, rid: ID = None,
-                         states: list[int] = None, site: str = None, rsv_type: str = None) -> List[ABCReservationMixin]:
+                         states: list[int] = None, site: str = None,
+                         rsv_type: list[str] = None) -> List[ABCReservationMixin]:
         """
         Retrieves the reservations.
 
         @return list of reservations
 
         @throws Exception in case of error
         """
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_delegation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_event.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_container.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_proxy_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_query_response_handler.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_query_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_resources.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_reservation_status.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_status.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_resource_control.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_response_handler.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_rpc_request_state.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_server_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_slice.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_substrate.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_substrate_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_tick.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_ticker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_ticker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_timer_queue.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/apis/abc_timer_task.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_task.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/common/constants.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/constants.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/common/event_logger.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/event_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/common/exceptions.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/common/resource_config.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/resource_config.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/container.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/db/container_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/container_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,31 +139,31 @@
                     act_obj = pickle.loads(pickled_actor)
                     result.append(act_obj)
             return result
         except Exception as e:
             self.logger.error(e)
         return result
 
-    def get_actor(self, *, actor_name: str) -> dict:
+    def get_actor(self, *, actor_name: str) -> ABCActorMixin or None:
         """
         Get Actor
-        @param name actor name
+        @param actor_name actor name
         @return actor
         """
         result = None
         try:
             act_dict = self.db.get_actor(name=actor_name)
             if act_dict is not None:
                 pickled_actor = act_dict.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                 return pickle.loads(pickled_actor)
         except Exception as e:
             self.logger.error(e)
         return result
 
-    def get_actor_id(self, *, actor_name: str) -> dict:
+    def get_actor_id(self, *, actor_name: str) -> int or None:
         """
         Get Actor
         @param name actor name
         @return actor
         """
         result = None
         try:
@@ -196,15 +196,15 @@
     def add_container_properties(self, *, properties: dict):
         """
         Add container properties
         @param properties properties
         """
         self.db.add_miscellaneous(name=self.PropertyContainer, properties=properties)
 
-    def get_container_properties(self) -> dict:
+    def get_container_properties(self) -> dict or None:
         """
         Get Container Properties
         @return properties
         """
         result = None
         try:
             result = self.db.get_miscellaneous(name=self.PropertyContainer)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/globals.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/globals.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/maintenance.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/maintenance.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/message_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/message_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/protocol_descriptor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/remote_actor_cache.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/remote_actor_cache.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/container/rpc_producer.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/rpc_producer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,32 +19,32 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+import time
 import traceback
 from typing import List, Dict
 
 from fabric_cf.actor.boot.configuration import ActorConfig
-from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation, DelegationState
+from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
 from fabric_cf.actor.core.apis.abc_timer_task import ABCTimerTask
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin, ActorType
 from fabric_cf.actor.core.apis.abc_actor_event import ABCActorEvent
 from fabric_cf.actor.core.apis.abc_actor_proxy import ABCActorProxy
 from fabric_cf.actor.core.apis.abc_actor_runnable import ABCActorRunnable
 from fabric_cf.actor.core.apis.abc_query_response_handler import ABCQueryResponseHandler
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
 from fabric_cf.actor.core.common.exceptions import ActorException
 from fabric_cf.actor.core.container.message_service import MessageService
 from fabric_cf.actor.core.core.event_processor import TickEvent, EventType, EventProcessor
-from fabric_cf.actor.core.delegation.delegation_factory import DelegationFactory
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
 from fabric_cf.actor.core.kernel.kernel_wrapper import KernelWrapper
 from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.slice import SliceTypes
 from fabric_cf.actor.core.kernel.slice_state_machine import SliceState
 from fabric_cf.actor.core.proxies.proxy import Proxy
@@ -148,27 +148,27 @@
 
     def close_by_rid(self, *, rid: ID):
         self.wrapper.close(rid=rid)
 
     def close(self, *, reservation: ABCReservationMixin):
         if reservation is not None:
             if not self.recovered:
-                self.logger.debug("Adding reservation: {} to closing list".format(reservation.get_reservation_id()))
+                #self.logger.debug("Adding reservation: {} to closing list".format(reservation.get_reservation_id()))
                 self.closing.add(reservation=reservation)
             else:
-                self.logger.debug("Closing reservation: {}".format(reservation.get_reservation_id()))
+                #self.logger.debug("Closing reservation: {}".format(reservation.get_reservation_id()))
                 self.wrapper.close(rid=reservation.get_reservation_id())
 
     def close_slice_reservations(self, *, slice_id: ID):
         self.wrapper.close_slice_reservations(slice_id=slice_id)
 
     def close_reservations(self, *, reservations: ReservationSet):
-        for reservation in reservations.values():
+        for reservation in reservations.reservations.values():
             try:
-                self.logger.debug("Closing reservation: {}".format(reservation.get_reservation_id()))
+                #self.logger.debug("Closing reservation: {}".format(reservation.get_reservation_id()))
                 self.close(reservation=reservation)
             except Exception as e:
                 self.logger.error(traceback.format_exc())
                 self.logger.error("Could not close for #{} {}".format(reservation.get_reservation_id(), e))
 
     def error(self, *, err: str):
         """
@@ -204,23 +204,31 @@
                 current_cycle = cycle
             else:
                 current_cycle = self.current_cycle + 1
 
             while current_cycle <= cycle:
                 self.logger.info("actor_tick: {} start".format(current_cycle))
                 self.current_cycle = current_cycle
+                begin = time.time()
                 self.policy.prepare(cycle=self.current_cycle)
+                self.logger.info(f"POLICY TIME: {time.time() - begin:.0f}")
 
                 if self.first_tick:
                     self.reset()
 
+                begin = time.time()
                 self.tick_handler()
+                self.logger.info(f"ACTOR TICK TIME: {time.time() - begin:.0f}")
+                begin = time.time()
                 self.policy.finish(cycle=self.current_cycle)
+                self.logger.info(f"POLICY FINISH TIME: {time.time() - begin:.0f}")
 
+                begin = time.time()
                 self.wrapper.tick()
+                self.logger.info(f"KERNEL TIME: {time.time() - begin:.0f}")
 
                 self.first_tick = False
                 self.logger.info("actor_tick: {} end".format(current_cycle))
                 current_cycle += 1
         except Exception as e:
             self.logger.debug(traceback.format_exc())
             raise e
@@ -839,14 +847,15 @@
             if isinstance(incoming, TickEvent):
                 self.event_processors[EventType.TickEvent].enqueue(incoming=incoming)
             else:
                 self.event_processors[EventType.InterActorEvent].enqueue(incoming=incoming)
             self.logger.debug("Added event to event queue {}".format(incoming.__class__.__name__))
         except Exception as e:
             self.logger.error(f"Failed to queue event: {incoming.__class__.__name__} e: {e}")
+            self.logger.error(traceback.format_exc())
 
     def queue_event_sync(self, *, incoming: ABCActorEvent):
         """
         Queue an even on Actor Event Queue
         """
         try:
             self.event_processors[EventType.SyncEvent].enqueue(incoming=incoming)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/actor_identity.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/authority_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/broker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/broker_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/controller.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
-import queue
-import threading
+import concurrent.futures
+import time
 import traceback
 from typing import TYPE_CHECKING
 
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_actor_mixin import ActorType
@@ -76,14 +76,16 @@
         self.modifying_lease = ReservationSet()
         # Peer registry.
         self.registry = PeerRegistry()
         # initialization status
         self.initialized = False
         self.type = ActorType.Orchestrator
         self.asm_update_thread = AsmUpdateThread(name=f"{self.get_name()}-asm-thread", logger=self.logger)
+        self.thread_pool = concurrent.futures.ThreadPoolExecutor(max_workers=2,
+                                                                 thread_name_prefix=self.__class__.__name__)
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['recovered']
         del state['wrapper']
         del state['logger']
         del state['clock']
@@ -99,14 +101,15 @@
         del state['redeeming']
         del state['extending_lease']
         del state['modifying_lease']
         del state['registry']
 
         del state['asm_update_thread']
         del state['event_processors']
+        del state['thread_pool']
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.recovered = False
         self.wrapper = None
         self.logger = None
@@ -122,14 +125,16 @@
         self.extending_ticket = ReservationSet()
         self.redeeming = ReservationSet()
         self.extending_lease = ReservationSet()
         self.modifying_lease = ReservationSet()
         self.registry = PeerRegistry()
         self.asm_update_thread = AsmUpdateThread(name=f"{self.get_name()}-asm-thread", logger=self.logger)
         self.event_processors = {}
+        self.thread_pool = concurrent.futures.ThreadPoolExecutor(max_workers=2,
+                                                                 thread_name_prefix=self.__class__.__name__)
 
     def set_logger(self, logger):
         super(Controller, self).set_logger(logger=logger)
         self.asm_update_thread.set_logger(logger=logger)
 
     def start(self):
         self.asm_update_thread.set_logger(logger=self.logger)
@@ -186,19 +191,23 @@
         raise ControllerException("Not implemented")
 
     def close_expiring(self):
         """
         Issues close requests on all reservations scheduled for closing on the
         current cycle
         """
+        begin = time.time()
         rset = self.policy.get_closing(cycle=self.current_cycle)
 
         if rset is not None and rset.size() > 0:
-            self.logger.info("SlottedSM close expiring for cycle {} expiring {}".format(self.current_cycle, rset))
+            #self.logger.debug("SlottedSM close expiring for cycle {} expiring {}".format(self.current_cycle, rset))
             self.close_reservations(reservations=rset)
+        diff = int(time.time() - begin)
+        if diff > 0:
+            self.logger.info(f"Event close_expiring TIME: {diff}")
 
     def demand(self, *, rid: ID):
         if rid is None:
             raise ControllerException("Invalid argument")
 
         reservation = self.get_reservation(rid=rid)
 
@@ -273,29 +282,32 @@
 
             self.initialized = True
 
     def process_redeeming(self):
         """
         Issue redeem requests on all reservations scheduled for redeeming on the current cycle
         """
+        begin = time.time()
         rset = self.policy.get_redeeming(cycle=self.current_cycle)
 
         if rset is not None and rset.size() > 0:
-            self.logger.info("SlottedController redeem for cycle {} redeeming {}".format(self.current_cycle, rset))
-
+            #self.logger.debug("SlottedController redeem for cycle {} redeeming {}".format(self.current_cycle, rset))
             self.redeem_reservations(rset=rset)
+        diff = int(time.time() - begin)
+        if diff > 0:
+            self.logger.info(f"Event redeeming TIME: {diff}")
 
     def redeem(self, *, reservation: ABCControllerReservation):
         if not self.recovered:
             self.redeeming.add(reservation=reservation)
         else:
             self.wrapper.redeem(reservation=reservation)
 
     def redeem_reservations(self, *, rset: ReservationSet):
-        for reservation in rset.values():
+        for reservation in rset.reservations.values():
             try:
                 if isinstance(reservation, ABCControllerReservation):
                     self.redeem(reservation=reservation)
                 else:
                     self.logger.warning("Reservation #{} cannot be redeemed".format(reservation.get_reservation_id()))
             except Exception as e:
                 self.logger.error(traceback.format_exc())
@@ -314,17 +326,24 @@
                     self.ticket_client(reservation=reservation)
                 else:
                     self.logger.warning("Reservation #{} cannot be ticketed".format(reservation.get_reservation_id()))
             except Exception as e:
                 self.logger.error("Could not ticket for #{} e: {}".format(reservation.get_reservation_id(), e))
 
     def tick_handler(self):
-        self.close_expiring()
-        self.process_redeeming()
+        futures = [self.thread_pool.submit(self.close_expiring),
+                   self.thread_pool.submit(self.process_redeeming)]
+        #self.close_expiring()
+        #self.process_redeeming()
         self.bid()
+        # Wait for Close and Redeem processing to finish
+        while True:
+            done, not_done = concurrent.futures.wait(futures, timeout=1)
+            if not_done is None or len(not_done) == 0:
+                break
 
     def update_lease(self, *, reservation: ABCReservationMixin, update_data, caller: AuthToken):
         if not self.is_recovered() or self.is_stopped():
             raise ControllerException("This actor cannot receive calls")
 
         self.wrapper.update_lease(reservation=reservation, update_data=update_data, caller=caller)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/event_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/event_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,17 @@
         for event in events:
             try:
                 begin = time.time()
                 if isinstance(event, ABCTimerTask):
                     event.execute()
                 else:
                     event.process()
-                self.logger.info(f"Event {event.__class__.__name__} TIME: {time.time() - begin:.0f}")
+                diff = int(time.time() - begin)
+                if diff > 0:
+                    self.logger.info(f"Event {event.__class__.__name__} TIME: {diff}")
             except Exception as e:
                 self.logger.error(f"Error while processing event {type(event)}, {e}")
                 self.logger.error(traceback.format_exc())
 
     def __run(self):
         while True:
             with self.condition:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/inventory_slice_manager.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/inventory_slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/rpc_request_state.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/ticket.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/unit.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import threading
 from enum import Enum
 
+from fim.slivers.attached_components import ComponentType
 from fim.slivers.base_sliver import BaseSliver
 from fim.slivers.network_node import NodeSliver
 from fim.slivers.network_service import NetworkServiceSliver
 
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.plugins.handlers.config_token import ConfigToken
 from fabric_cf.actor.core.util.id import ID
@@ -508,10 +509,21 @@
         try:
             self.lock.acquire()
             self.sliver.set_label_allocations(sliver.get_label_allocations())
             if isinstance(self.sliver, NodeSliver) and isinstance(sliver, NodeSliver):
                 self.sliver.management_ip = sliver.management_ip
                 if sliver.attached_components_info is not None:
                     for device in sliver.attached_components_info.devices.values():
-                        self.sliver.attached_components_info.devices[device.get_name()].label_allocations = device.label_allocations
+                        existing_device = self.sliver.attached_components_info.devices[device.get_name()]
+                        existing_device.label_allocations = device.label_allocations
+
+                        # Copy label allocations for Interfaces
+                        if device.get_type() in [ComponentType.SmartNIC, ComponentType.SharedNIC]:
+                            ns_name = list(device.network_service_info.network_services.keys())[0]
+                            ns = device.network_service_info.network_services[ns_name]
+                            existing_ifs = existing_device.network_service_info.network_services[ns_name].interface_info.interfaces
+                            for ifs in ns.interface_info.interfaces.values():
+                                existing_ifs[ifs.get_name()].label_allocations = ifs.label_allocations
+
+                        #self.sliver.attached_components_info.devices[device.get_name()].label_allocations = device.label_allocations
         finally:
             self.lock.release()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/core/unit_set.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/broker_delegation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/broker_delegation_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/delegation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/delegation_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/delegation/resource_ticket.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/resource_ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/authority_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/broker_query_model_publisher.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_query_model_publisher.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/broker_reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/claim_timeout.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/claim_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/failed_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/failed_rpc_event.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_failed_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_query_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_query_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/incoming_rpc_event.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,23 +51,23 @@
 
     def do_process_actor(self, *, actor: ABCActorMixin):
         """
         Process Incoming RPC events common for all actors
         """
         processed = True
         if self.rpc.get_request_type() == RPCRequestType.Query:
-            actor.get_logger().info("processing query from <{}>".format(self.rpc.get_caller().get_name()))
+            actor.get_logger().debug("processing query from <{}>".format(self.rpc.get_caller().get_name()))
             result = actor.query(query=self.rpc.get(), caller=self.rpc.get_caller())
 
             from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
             RPCManagerSingleton.get().query_result(actor=actor, remote_actor=self.rpc.get_callback(),
                                                    request_id=self.rpc.get_message_id(),
                                                    response=result, caller=actor.get_identity())
         elif self.rpc.get_request_type() == RPCRequestType.QueryResult:
-            actor.get_logger().info("processing query response from <{}>".format(self.rpc.get_caller().get_name()))
+            actor.get_logger().debug("processing query response from <{}>".format(self.rpc.get_caller().get_name()))
             result = self.rpc.get()
             if self.rpc.get_response_handler() is not None:
                 handler = self.rpc.get_response_handler()
                 handler.handle(status=self.rpc.get_error(), result=result)
             else:
                 actor.get_logger().warning("No response handler is associated with the queryResponse. "
                                            "Ignoring queryResponse")
@@ -77,68 +77,68 @@
 
     def do_process_client(self, *, client: ABCClientActor):
         """
         Process Incoming RPC events common for client actors
         """
         processed = True
         if self.rpc.get_request_type() == RPCRequestType.UpdateLease:
-            client.get_logger().info("processing update lease from <{}>".format(self.rpc.get_caller().get_name()))
+            client.get_logger().debug("processing update lease from <{}>".format(self.rpc.get_caller().get_name()))
             if self.rpc.get().get_resources().get_resources() is not None:
-                client.get_logger().info("inbound lease is {}".format(
+                client.get_logger().debug("inbound lease is {}".format(
                     self.rpc.get().get_resources().get_resources()))
 
             client.update_lease(reservation=self.rpc.get(), update_data=self.rpc.get_update_data(),
                                 caller=self.rpc.get_caller())
         elif self.rpc.get_request_type() == RPCRequestType.UpdateTicket:
-            client.get_logger().info("processing update ticket from <{}>".format(self.rpc.get_caller().get_name()))
+            client.get_logger().debug("processing update ticket from <{}>".format(self.rpc.get_caller().get_name()))
             client.update_ticket(reservation=self.rpc.get(), update_data=self.rpc.get_update_data(),
                                  caller=self.rpc.get_caller())
-            client.get_logger().info("update ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
+            client.get_logger().debug("update ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
         elif self.rpc.get_request_type() == RPCRequestType.UpdateDelegation:
-            client.get_logger().info("processing update delegation from <{}>".format(self.rpc.get_caller().get_name()))
+            client.get_logger().debug("processing update delegation from <{}>".format(self.rpc.get_caller().get_name()))
             client.update_delegation(delegation=self.rpc.get(), update_data=self.rpc.get_update_data(),
                                      caller=self.rpc.get_caller())
-            client.get_logger().info("update delegation processed from <{}>".format(self.rpc.get_caller().get_name()))
+            client.get_logger().debug("update delegation processed from <{}>".format(self.rpc.get_caller().get_name()))
         else:
             processed = self.do_process_actor(actor=client)
         return processed
 
     def do_process_server(self, *, server: ABCServerActor):
         """
         Process Incoming RPC events common for server actors
         """
         processed = True
         if self.rpc.get_request_type() == RPCRequestType.ClaimDelegation:
-            server.get_logger().info("processing claim delegation from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("processing claim delegation from <{}>".format(self.rpc.get_caller().get_name()))
             server.claim_delegation(delegation=self.rpc.get(), callback=self.rpc.get_callback(),
                                     caller=self.rpc.get_caller())
-            server.get_logger().info("claim processed from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("claim processed from <{}>".format(self.rpc.get_caller().get_name()))
 
         elif self.rpc.get_request_type() == RPCRequestType.ReclaimDelegation:
-            server.get_logger().info("processing reclaim delegation from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("processing reclaim delegation from <{}>".format(self.rpc.get_caller().get_name()))
             server.reclaim_delegation(delegation=self.rpc.get(), callback=self.rpc.get_callback(),
                                       caller=self.rpc.get_caller())
-            server.get_logger().info("reclaim processed from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("reclaim processed from <{}>".format(self.rpc.get_caller().get_name()))
 
         elif self.rpc.get_request_type() == RPCRequestType.Ticket:
-            server.get_logger().info("processing ticket from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("processing ticket from <{}>".format(self.rpc.get_caller().get_name()))
             server.ticket(reservation=self.rpc.get(), callback=self.rpc.get_callback(),
                           caller=self.rpc.get_caller())
-            server.get_logger().info("ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
 
         elif self.rpc.get_request_type() == RPCRequestType.ExtendTicket:
-            server.get_logger().info("processing extend ticket from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("processing extend ticket from <{}>".format(self.rpc.get_caller().get_name()))
             server.extend_ticket(reservation=self.rpc.get(), caller=self.rpc.get_caller(),
                                  callback=self.rpc.get_callback())
-            server.get_logger().info("extend ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("extend ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
 
         elif self.rpc.get_request_type() == RPCRequestType.Relinquish:
-            server.get_logger().info("processing relinquish from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("processing relinquish from <{}>".format(self.rpc.get_caller().get_name()))
             server.relinquish(reservation=self.rpc.get(), caller=self.rpc.get_caller())
-            server.get_logger().info("relinquish processed from <{}>".format(self.rpc.get_caller().get_name()))
+            server.get_logger().debug("relinquish processed from <{}>".format(self.rpc.get_caller().get_name()))
 
         else:
             processed = self.do_process_actor(actor=server)
         return processed
 
     def do_process_broker(self, *, broker: ABCBrokerMixin):
         """
@@ -151,30 +151,30 @@
 
     def do_process_authority(self, *, authority: ABCAuthority):
         """
         Process Incoming RPC events common for AMs
         """
         processed = True
         if self.rpc.get_request_type() == RPCRequestType.Redeem:
-            authority.get_logger().info("processing redeem from <{}>".format(self.rpc.get_caller().get_name()))
+            authority.get_logger().debug("processing redeem from <{}>".format(self.rpc.get_caller().get_name()))
             authority.redeem(reservation=self.rpc.get(), callback=self.rpc.get_callback(),
                              caller=self.rpc.get_caller())
 
         elif self.rpc.get_request_type() == RPCRequestType.ExtendLease:
-            authority.get_logger().info("processing extend lease from <{}>".format(self.rpc.get_caller().get_name()))
+            authority.get_logger().debug("processing extend lease from <{}>".format(self.rpc.get_caller().get_name()))
             authority.extend_lease(reservation=self.rpc.get(), caller=self.rpc.get_caller(),
                                    callback=self.rpc.get_callback())
 
         elif self.rpc.get_request_type() == RPCRequestType.ModifyLease:
-            authority.get_logger().info("processing modify lease from <{}>".format(self.rpc.get_caller().get_name()))
+            authority.get_logger().debug("processing modify lease from <{}>".format(self.rpc.get_caller().get_name()))
             authority.modify_lease(reservation=self.rpc.get(), caller=self.rpc.get_caller(),
                                    callback=self.rpc.get_callback())
 
         elif self.rpc.get_request_type() == RPCRequestType.Close:
-            authority.get_logger().info("processing close from <{}>".format(self.rpc.get_caller().get_name()))
+            authority.get_logger().debug("processing close from <{}>".format(self.rpc.get_caller().get_name()))
             authority.close(reservation=self.rpc.get())
 
         else:
             processed = self.do_process_server(server=authority)
         return processed
 
     def do_process_controller(self, *, controller: ABCController):
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,15 +479,15 @@
 
             identity.name = self.plugin.get_actor().get_name()
             identity.guid = self.plugin.get_actor().get_guid()
             result.set_owner(owner=identity)
             self.register_slice(slice_object=result)
         return result
 
-    def get_reservation(self, *, rid: ID) -> ABCReservationMixin:
+    def get_reservation(self, *, rid: ID) -> ABCReservationMixin or None:
         """
         Returns the specified reservation.
         @param rid reservation id
         @return reservation
         """
         if rid is not None:
             return self.reservations.get(rid=rid)
@@ -594,19 +594,39 @@
     def __probe_pending(self, *, reservation: ABCReservationMixin):
         """
         Probes to check for completion of pending operation.
         @param reservation the reservation being probed
         @throws Exception rare
         """
         try:
+            begin = time.time()
             reservation.lock()
+            now = time.time()
+            diff = int(now - begin)
+            if diff > 0:
+                self.logger.info(f"RES LOCK TIME: {diff} - {reservation.get_reservation_id()}")
+            begin = time.time()
             reservation.prepare_probe()
             reservation.probe_pending()
+            now = time.time()
+            diff = int(now - begin)
+            if diff > 0:
+                self.logger.info(f"RES PROBE TIME: {diff} - {reservation.get_reservation_id()}")
+            begin = time.time()
             self.plugin.get_database().update_reservation(reservation=reservation)
+            now = time.time()
+            diff = int(now - begin)
+            if diff > 0:
+                self.logger.info(f"RES DB UPDATE TIME: {diff} - {reservation.get_reservation_id()}")
+            begin = time.time()
             reservation.service_probe()
+            now = time.time()
+            diff = int(now - begin)
+            if diff > 0:
+                self.logger.info(f"RES SERVICE PROBE TIME: {diff} - {reservation.get_reservation_id()}")
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.error(err=f"An error occurred during probe pending for reservation #{reservation.get_reservation_id()}",
                        e=e)
         finally:
             reservation.unlock()
 
@@ -679,23 +699,39 @@
 
     def redeem(self, *, reservation: ABCClientReservation):
         """
         Redeem a reservation
         @param reservation reservation
         """
         try:
+            begin = time.time()
             reservation.lock()
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"REDEEM LOCK TIME: {diff}")
+            begin = time.time()
             if reservation.can_redeem():
                 reservation.reserve(policy=self.policy)
             else:
                 raise KernelException("The current reservation state prevent it from being redeemed")
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"REDEEM TIME: {diff}")
+            begin = time.time()
 
             self.plugin.get_database().update_reservation(reservation=reservation)
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"REDEEM DB TIME: {diff}")
+            begin = time.time()
             if not reservation.is_failed():
                 reservation.service_reserve()
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"REDEEM SERVICE TIME: {diff}")
         except Exception as e:
             self.logger.error(f"An error occurred during redeem for reservation #{reservation.get_reservation_id()} "
                               f"e: {e}")
             self.logger.error(traceback.format_exc())
         finally:
             reservation.unlock()
 
@@ -1193,26 +1229,28 @@
             finally:
                 self.lock.release()
             self.logger.info(f"KERNEL DEL TICK TIME: {time.time() - begin:.0f}")
 
             begin = time.time()
             for reservation in self.reservations.values():
                 self.__probe_pending(reservation=reservation)
-            self.logger.info(f"KERNEL RES TICK TIME: {time.time() - begin:.0f}")
+            self.logger.info(f"KERNEL RES TICK TIME: {time.time() - begin:.0f} {self.reservations.size()}")
 
             begin = time.time()
             try:
                 self.lock.acquire()
                 for slice_obj in self.slices.get_client_slices():
                     self.__probe_pending_slices(slice_obj=slice_obj)
             finally:
                 self.lock.release()
             self.logger.info(f"KERNEL SLC TICK TIME: {time.time() - begin:.0f}")
 
+            begin = time.time()
             self.__purge()
+            self.logger.info(f"KERNEL PURGE TICK TIME: {time.time() - begin:.0f}")
             self.check_nothing_pending()
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.error(err="exception in Kernel.tick", e=e)
 
     def has_something_pending(self) -> bool:
         """
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel_tick.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/kernel_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+import time
 import traceback
 from datetime import datetime
 from typing import List, Dict
 
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
@@ -644,27 +645,40 @@
         Role: Controller
         @param reservation the reservation being redeemed
         @throws Exception in case of error
         """
         if reservation is None:
             raise KernelException(Constants.INVALID_ARGUMENT)
 
+        '''
         slice_object = reservation.get_slice()
-
         for r in slice_object.get_reservations().values():
             self.logger.debug("redeem() Reservation {} is in state: {}".format(r.get_reservation_id(),
                                                                                ReservationStates(r.get_state()).name))
-
+        '''
+        begin = time.time()
         target = self.kernel.validate(rid=reservation.get_reservation_id())
+        diff = int(time.time() - begin)
+        if diff > 0:
+            self.logger.info(f"REDEEM KERNEL VAL TIME: {diff}")
+        begin = time.time()
 
         if target is None:
             self.logger.error("Redeem on a reservation not registered with the kernel")
 
         target.validate_redeem()
+        diff = int(time.time() - begin)
+        if diff > 0:
+            self.logger.info(f"REDEEM VAL TIME: {diff}")
+        begin = time.time()
         self.kernel.redeem(reservation=target)
+        diff = int(time.time() - begin)
+        if diff > 0:
+            self.logger.info(f"REDEEM TIME: {diff}")
+        begin = time.time()
 
     def redeem_request(self, *, reservation: ABCAuthorityReservation, caller: AuthToken,
                        callback: ABCControllerCallbackProxy, compare_sequence_numbers: bool):
         """
         Processes an incoming request for a new lease.
         Role: Authority
         @param reservation reservation representing the lease request. Must
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/predecessor_state.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/predecessor_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/query_timeout.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/query_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/request_types.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/request_types.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_client.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 import threading
 import time
 import traceback
 from typing import TYPE_CHECKING, List, Tuple
 
 from fim.slivers.attached_components import ComponentType
 from fim.slivers.base_sliver import BaseSliver
-from fim.slivers.capacities_labels import Labels, ReservationInfo
-from fim.slivers.network_node import NodeSliver, NodeType
+from fim.slivers.capacities_labels import Labels
+from fim.slivers.network_node import NodeType
 from fim.slivers.network_service import NetworkServiceSliver
 
 from fabric_cf.actor.core.apis.abc_authority_policy import ABCAuthorityPolicy
 from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ReservationException
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
@@ -197,17 +197,17 @@
         del state['previous_resources']
         del state['bid_pending']
         del state['dirty']
         del state['expired']
         del state['pending_recover']
         del state['state_transition']
         del state['service_pending']
-
         del state['suggested']
         del state['thread_lock']
+        del state['policy']
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.actor = None
         self.logger = None
         self.slice = None
@@ -215,14 +215,15 @@
         self.previous_resources = None
         self.bid_pending = False
         self.dirty = False
         self.expired = False
         self.pending_recover = False
         self.state_transition = False
         self.service_pending = ReservationPendingStates.None_
+        self.policy = None
 
         self.suggested = True
         self.thread_lock = threading.Lock()
 
     def restore(self, *, actor: ABCActorMixin, slice_obj: ABCSlice):
         """
         Must be invoked after creating reservation from unpickling
@@ -915,22 +916,24 @@
             self.leased_resources.prepare_probe()
 
     def prepare_redeem(self):
         assert self.resources is not None
         assert self.resources.sliver is not None
         sliver = self.resources.sliver
 
+        '''
         self.logger.info(f"Redeem prepared for Sliver: {sliver}")
         if isinstance(sliver, NetworkServiceSliver) and sliver.interface_info is not None:
             for ifs in sliver.interface_info.interfaces.values():
                 self.logger.info(f"Interface Sliver: {ifs}")
 
         if isinstance(sliver, NodeSliver) and sliver.attached_components_info is not None:
             for c in sliver.attached_components_info.devices.values():
                 self.logger.info(f"Component: {c}")
+        '''
 
     def probe_join_state(self):
         """
         Called from a probe to monitor asynchronous processing related to the joinstate for controller.
         @raises Exception passed through from prepareJoin or prepareRedeem
         """
         if self.state == ReservationStates.Closed or self.state == ReservationStates.Failed:
@@ -1078,20 +1081,20 @@
             return ret_val
         if self.resources.sliver is not None and isinstance(self.resources.sliver, NetworkServiceSliver) and \
                 self.pending_state == ReservationPendingStates.None_ and self.joinstate == JoinState.NoJoin:
             self.logger.debug("Checking dependency state")
             # Check dependencies
             closed_preds = 0
             for pred_state in self.get_redeem_predecessors():
-                if pred_state.get_reservation().is_closed():
+                if pred_state.get_reservation().is_closed() or pred_state.get_reservation().is_closing():
                     closed_preds += 1
 
             #if closed_preds > len(self.get_redeem_predecessors()):
             if closed_preds:
-                self.logger.debug(f"Found dependencies# {closed_preds} in closed state")
+                self.logger.debug(f"Found dependencies# {closed_preds} in closed/closing state")
                 ret_val = True
         return ret_val
 
     def probe_pending(self):
         # Process join state to complete or restart join-related operations for Controller
         if self.joinstate != JoinState.NoJoin:
             self.probe_join_state()
@@ -1134,24 +1137,26 @@
         if self.leased_resources is None:
             return
 
         # Handling for close completion. Note that this reservation could
         # "stick" once we enter the CloseWait state, if we never hear back from
         # the authority. There is no harm to purging a CloseWait reservation,
         # but we just leave them for now.
-        close_by_deps = self.__are_dependencies_closed()
-        if (self.pending_state == ReservationPendingStates.Closing and self.leased_resources.is_closed()) or \
-                close_by_deps:
-
-            if not close_by_deps:
-                self.logger.debug("LEASED RESOURCES are closed")
-                msg = "local close complete"
-            else:
-                msg = "close by dependencies"
+        #close_by_deps = self.__are_dependencies_closed()
+        #if (self.leased_resources is not None and self.pending_state == ReservationPendingStates.Closing and
+        #    self.leased_resources.is_closed()) or close_by_deps:
+
+        #    if not close_by_deps:
+        #        self.logger.debug("LEASED RESOURCES are closed")
+        #        msg = "local close complete"
+        #    else:
+        #        msg = "close by dependencies"
 
+        if self.pending_state == ReservationPendingStates.Closing:
+            msg = "local close complete"
             self.transition(prefix=msg, state=ReservationStates.CloseWait, pending=ReservationPendingStates.None_)
 
             try:
                 self.sequence_lease_out += 1
                 RPCManagerSingleton.get().close(reservation=self)
             except Exception as e:
                 self.logger.error("authority reports close error: {}".format(e))
@@ -1801,15 +1806,15 @@
                                    error_message=error_message)
             self.logger.debug(f"Update ASM completed for  Reservation# {self.rid} State# {self.get_reservation_state()} "
                               f"Slice Graph# {self.slice.get_graph_id()}")
 
         except Exception as e:
             self.logger.error(f"Failed to update the ASM Graph: {e}")
             self.logger.error(traceback.format_exc())
-        self.logger.info(f"ASM TIME: {time.time() - begin:.0f}")
+        #self.logger.info(f"ASM TIME: {time.time() - begin:.0f}")
 
     def mark_close_by_ticket_review(self, *, update_data: UpdateData):
         if self.last_ticket_update is not None:
             self.last_ticket_update.absorb(other=update_data)
 
 
 class ClientReservationFactory:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_server.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_server.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/reservation_states.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_states.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/resource_set.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/resource_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/retry_rpc.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/retry_rpc_event.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_executor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_executor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_manager.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,30 +305,30 @@
         state.set_type(rtype=RPCRequestType.ClaimDelegation)
 
         rpc = RPCRequest(request=state, actor=actor, proxy=proxy, delegation=delegation,
                          sequence=delegation.get_sequence_out())
         # Schedule a timeout
         rpc.timer = KernelTimer.schedule(queue=actor, task=ClaimTimeout(req=rpc), delay=self.CLAIM_TIMEOUT_SECONDS)
         if proxy.get_logger() is not None:
-            proxy.get_logger().info(f"Timer started: {rpc.timer} for Claim")
+            proxy.get_logger().debug(f"Timer started: {rpc.timer} for Claim")
         self.enqueue(rpc=rpc)
 
     def do_reclaim_delegation(self, *, actor: ABCActorMixin, proxy: ABCBrokerProxy, delegation: ABCDelegation,
                               callback: ABCClientCallbackProxy, caller: AuthToken):
         state = proxy.prepare_reclaim_delegation(delegation=delegation, callback=callback,
                                                  caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.ReclaimDelegation)
 
         rpc = RPCRequest(request=state, actor=actor, proxy=proxy, delegation=delegation,
                          sequence=delegation.get_sequence_out())
         # Schedule a timeout
         rpc.timer = KernelTimer.schedule(queue=actor, task=ReclaimTimeout(req=rpc), delay=self.CLAIM_TIMEOUT_SECONDS)
         if proxy.get_logger() is not None:
-            proxy.get_logger().info(f"Timer started: {rpc.timer} for Reclaim")
+            proxy.get_logger().debug(f"Timer started: {rpc.timer} for Reclaim")
         self.enqueue(rpc=rpc)
 
     def do_ticket(self, *, actor: ABCActorMixin, proxy: ABCBrokerProxy, reservation: ABCClientReservation,
                   callback: ABCClientCallbackProxy, caller: AuthToken):
         state = proxy.prepare_ticket(reservation=reservation, callback=callback, caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.Ticket)
@@ -425,15 +425,15 @@
                  query: dict, handler: ABCQueryResponseHandler, caller: AuthToken):
         state = remote_actor.prepare_query(callback=local_actor, query=query, caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.Query)
         rpc = RPCRequest(request=state, actor=actor, proxy=remote_actor, handler=handler)
         # Timer
         rpc.timer = KernelTimer.schedule(queue=actor, task=QueryTimeout(req=rpc), delay=self.QUERY_TIMEOUT_SECONDS)
-        remote_actor.get_logger().info(f"Timer started: {rpc.timer} for Query")
+        remote_actor.get_logger().debug(f"Timer started: {rpc.timer} for Query")
         self.enqueue(rpc=rpc)
 
     def do_query_result(self, *, actor: ABCActorMixin, remote_actor: ABCCallbackProxy, request_id: str,
                         response: dict, caller: AuthToken):
         state = remote_actor.prepare_query_result(request_id=request_id, response=response, caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.QueryResult)
@@ -450,15 +450,15 @@
             if request is not None:
                 if request.timer:
                     actor.get_logger().debug(f"Canceling the timer: {request.timer}")
                 request.cancel_timer()
                 if request.handler is not None:
                     rpc.set_response_handler(response_handler=request.handler)
 
-        actor.get_logger().info(f"Inbound {rpc.get_request_type()} request from "
+        actor.get_logger().debug(f"Inbound {rpc.get_request_type()} request from "
                                 f"<{rpc.get_caller().get_name()}>:{rpc.get()}")
 
         self.__log_sliver(reservation=rpc.get(), logger=actor.get_logger())
 
         if rpc.get_request_type() == RPCRequestType.QueryResult:
             if request is None:
                 actor.get_logger().warning("No queryRequest to match to inbound queryResponse. Ignoring response")
@@ -481,17 +481,17 @@
                 failed = FailedRPC(e=exception, request_type=rpc.get_failed_request_type(), auth=rpc.caller)
 
             if failed is not None:
                 actor.queue_event(incoming=FailedRPCEvent(actor=actor, failed=failed))
 
         else:
             actor.get_logger().debug("Added to actor queue to be processed")
-            start = time.time()
+            #start = time.time()
             actor.queue_event(incoming=IncomingRPCEvent(actor=actor, rpc=rpc))
-            actor.get_logger().info(f"Kafka Queue event: {time.time() - start:.0f}")
+            #actor.get_logger().info(f"Kafka Queue event: {time.time() - start:.0f}")
 
     def add_pending_request(self, *, guid: ID, request: RPCRequest):
         try:
             self.pending_lock.acquire()
             from fabric_cf.actor.core.container.globals import GlobalsSingleton
             logger = GlobalsSingleton.get().get_logger()
             logger.debug(f"Added request with rid: {guid}")
@@ -526,15 +526,15 @@
             self.num_queued -= 1
             if self.num_queued == 0:
                 self.stats_lock.notify_all()
 
     def enqueue(self, *, rpc: RPCRequest):
         from fabric_cf.actor.core.container.globals import GlobalsSingleton
         logger = GlobalsSingleton.get().get_logger()
-        logger.info(f"Outbound {rpc.get_request_type()} : {rpc.get()}")
+        logger.debug(f"Outbound {rpc.get_request_type()} : {rpc.get()}")
         self.__log_sliver(reservation=rpc.get(), logger=logger)
         if not self.started:
             logger.warning("Ignoring RPC request: container is shutting down")
             return
         if rpc.handler is not None:
             self.add_pending_request(guid=rpc.request.get_message_id(), request=rpc)
 
@@ -565,8 +565,8 @@
             if isinstance(reservation, ABCServerReservation) and reservation.get_requested_resources() is not None:
                 sliver = reservation.get_requested_resources().get_sliver()
             else:
                 if reservation.get_resources() is not None:
                     sliver = reservation.get_resources().get_sliver()
 
             if sliver is not None:
-                logger.info(f"Sliver: {sliver_to_str(sliver=sliver)}")
+                logger.debug(f"Sliver: {sliver_to_str(sliver=sliver)}")
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_manager_singleton.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager_singleton.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_request.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/rpc_request_type.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/sequence_comparison_codes.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/sequence_comparison_codes.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice_state_machine.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_state_machine.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,31 +242,37 @@
                 self.state = SliceState.StableOK
 
         elif operation.command == SliceCommand.Delete:
             if self.state != SliceState.Dead:
                 self.state = SliceState.Closing
 
         elif operation.command == SliceCommand.Reevaluate:
+            has_error = False
             if reservations is None or reservations.size() == 0:
                 return state_changed, self.state
 
             bins = StateBins()
             for r in reservations.values():
                 bins.add(s=r.get_state())
                 if r.get_pending_state() in [ReservationPendingStates.ModifyingLease,
                                              ReservationPendingStates.ExtendingTicket,
                                              ReservationPendingStates.ExtendingLease,
                                              ReservationPendingStates.Redeeming,
                                              ReservationPendingStates.Ticketing,
                                              ReservationPendingStates.Priming]:
                     bins.add(s=r.get_pending_state())
+                if not has_error and r.get_error_message() is not None and len(r.get_error_message()) > 0:
+                    has_error = True
 
             if self.state == SliceState.Nascent or self.state == SliceState.Configuring:
                 if not bins.has_state_other_than(ReservationStates.Active, ReservationStates.Closed):
-                    self.state = SliceState.StableOK
+                    if not has_error:
+                        self.state = SliceState.StableOK
+                    else:
+                        self.state = SliceState.StableError
 
                 if (not bins.has_state_other_than(ReservationStates.Active, ReservationStates.Failed,
                                                   ReservationStates.Closed)) and \
                         bins.has_state(s=ReservationStates.Failed):
                     self.state = SliceState.StableError
 
                 if not bins.has_state_other_than(ReservationStates.Closed, ReservationStates.CloseWait,
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/slice_table.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_table.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/kernel/tick.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/actor_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/actor_management_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,20 +98,44 @@
         actor = ActorRegistrySingleton.get().get_actor(actor_name_or_guid=actor_name)
 
         if actor is None:
             raise ManageException(Constants.OBJECT_NOT_FOUND.format("Managed Object", actor_name))
 
         self.set_actor(actor=actor)
 
+    def make_local_db_object(self, *, actor: ABCActorMixin):
+        # Make a read only instance to return queries to avoid locking with Actor processing
+        from fabric_cf.actor.core.container.globals import GlobalsSingleton
+        config = GlobalsSingleton.get().get_config()
+
+        user = config.get_global_config().get_database()[Constants.PROPERTY_CONF_DB_USER]
+        password = config.get_global_config().get_database()[Constants.PROPERTY_CONF_DB_PASSWORD]
+        db_host = config.get_global_config().get_database()[Constants.PROPERTY_CONF_DB_HOST]
+        db_name = config.get_global_config().get_database()[Constants.PROPERTY_CONF_DB_NAME]
+
+        from fabric_cf.actor.core.apis.abc_actor_mixin import ActorType
+        if actor.get_type() in [ActorType.Orchestrator, ActorType.Authority]:
+            from fabric_cf.actor.core.plugins.substrate.db.substrate_actor_database import SubstrateActorDatabase
+            self.db = SubstrateActorDatabase(user=user, password=password, database=db_name, db_host=db_host,
+                                             logger=self.logger)
+        else:
+            from fabric_cf.actor.core.plugins.db.server_actor_database import ServerActorDatabase
+            self.db = ServerActorDatabase(user=user, password=password, database=db_name, db_host=db_host,
+                                          logger=self.logger)
+        self.db.set_actor_name(name=self.actor.get_name())
+        self.db.initialize()
+        self.db.actor_added(actor=actor)
+
     def set_actor(self, *, actor: ABCActorMixin):
         if self.actor is None:
             self.actor = actor
-            self.db = actor.get_plugin().get_database()
+            #self.db = actor.get_plugin().get_database()
             self.logger = actor.get_logger()
             self.id = actor.get_guid()
+            self.make_local_db_object(actor=actor)
 
     def get_slices(self, *, slice_id: ID, caller: AuthToken, slice_name: str = None, email: str = None,
                    states: List[int] = None, project: str = None, limit: int = None,
                    offset: int = None) -> ResultSliceAvro:
         result = ResultSliceAvro()
         result.status = ResultAvro()
 
@@ -341,36 +365,37 @@
             self.logger.error("get_sites: {}".format(e))
             result.status.set_code(ErrorCodes.ErrorInternalError.value)
             result.status.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
             result.status = ManagementObject.set_exception_details(result=result.status, e=e)
 
         return result
 
-
     def get_reservations(self, *, caller: AuthToken, states: List[int] = None,
                          slice_id: ID = None, rid: ID = None, oidc_claim_sub: str = None,
                          email: str = None, rid_list: List[str] = None, type: str = None,
                          site: str = None, node_id: str = None) -> ResultReservationAvro:
         result = ResultReservationAvro()
         result.status = ResultAvro()
 
         if caller is None:
             result.status.set_code(ErrorCodes.ErrorInvalidArguments.value)
             result.status.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
             return result
 
         try:
-
+            rsv_type = None
+            if type is not None:
+                rsv_type = type.split(",")
             res_list = None
             try:
                 if rid_list is not None:
                     res_list = self.db.get_reservations_by_rids(rid=rid_list)
                 else:
                     res_list = self.db.get_reservations(slice_id=slice_id, rid=rid, email=email,
-                                                        states=states, rsv_type=type, site=site,
+                                                        states=states, rsv_type=rsv_type, site=site,
                                                         graph_node_id=node_id)
             except Exception as e:
                 self.logger.error("getReservations:db access {}".format(e))
                 result.status.set_code(ErrorCodes.ErrorDatabaseError.value)
                 result.status.set_message(ErrorCodes.ErrorDatabaseError.interpret(exception=e))
                 result.status = ManagementObject.set_exception_details(result=result.status, e=e)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/authority_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/authority_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/broker_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/broker_management_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     def demand_reservation_rid(self, *, rid: ID, caller: AuthToken) -> ResultAvro:
         return self.client_helper.demand_reservation_rid(rid=rid, caller=caller)
 
     def demand_reservation(self, *, reservation: ReservationMng, caller: AuthToken) -> ResultAvro:
         return self.client_helper.demand_reservation(reservation=reservation, caller=caller)
 
-    def extend_reservation(self, *, reservation: id, new_end_time: datetime, sliver: BaseSliver,
+    def extend_reservation(self, *, reservation: ID, new_end_time: datetime, sliver: BaseSliver,
                            caller: AuthToken, dependencies: List[ReservationPredecessorAvro] = None) -> ResultAvro:
         return self.client_helper.extend_reservation(reservation=reservation, new_end_time=new_end_time,
                                                      sliver=sliver, caller=caller, dependencies=dependencies)
 
     def claim_delegations(self, *, broker: ID, did: str, caller: AuthToken) -> ResultDelegationAvro:
         return self.client_helper.claim_delegations(broker=broker, did=did, caller=caller)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/client_actor_management_object_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/client_actor_management_object_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,15 @@
             self.logger.error("demand_reservation {}".format(e))
             result.set_code(ErrorCodes.ErrorInternalError.value)
             result.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
             result = ManagementObject.set_exception_details(result=result, e=e)
 
         return result
 
-    def extend_reservation(self, *, reservation: id, new_end_time: datetime, sliver: BaseSliver,
+    def extend_reservation(self, *, reservation: ID, new_end_time: datetime, sliver: BaseSliver,
                            caller: AuthToken, dependencies: List[ReservationPredecessorAvro] = None) -> ResultAvro:
         result = ResultAvro()
 
         if reservation is None or caller is None or (new_end_time is None and sliver is None):
             result.set_code(ErrorCodes.ErrorInvalidArguments.value)
             result.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
             return result
@@ -454,15 +454,20 @@
                         rset.set_sliver(sliver=sliver)
 
                     self.actor.extend(rid=r.get_reservation_id(), resources=rset, term=new_term,
                                       dependencies=redeem_dep_res_list)
 
                     return result
 
-            result = self.client.execute_on_actor_thread_and_wait(runnable=Runner(actor=self.client))
+            # Process Extend for Renew synchronously
+            if new_end_time is not None:
+                result = self.client.execute_on_actor_thread_and_wait(runnable=Runner(actor=self.client))
+            # Process Extend for Modify asynchronously
+            else:
+                self.client.execute_on_actor_thread(runnable=Runner(actor=self.client))
 
         except Exception as e:
             self.logger.error("extend_reservation {}".format(e))
             result.set_code(ErrorCodes.ErrorInternalError.value)
             result.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
             result = ManagementObject.set_exception_details(result=result, e=e)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/container_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/container_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/controller_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/controller_management_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def demand_reservation_rid(self, *, rid: ID, caller: AuthToken) -> ResultAvro:
         return self.client_helper.demand_reservation_rid(rid=rid, caller=caller)
 
     def demand_reservation(self, *, reservation: ReservationMng, caller: AuthToken) -> ResultAvro:
         return self.client_helper.demand_reservation(reservation=reservation, caller=caller)
 
-    def extend_reservation(self, *, reservation: id, new_end_time: datetime, sliver: BaseSliver,
+    def extend_reservation(self, *, reservation: ID, new_end_time: datetime, sliver: BaseSliver,
                            caller: AuthToken, dependencies: List[ReservationPredecessorAvro] = None) -> ResultAvro:
         return self.client_helper.extend_reservation(reservation=reservation, new_end_time=new_end_time, 
                                                      sliver=sliver, caller=caller, dependencies=dependencies)
 
     def modify_reservation(self, *, rid: ID, modified_sliver: BaseSliver, caller: AuthToken) -> ResultAvro:
         return self.client_helper.modify_reservation(rid=rid, modified_sliver=modified_sliver, caller=caller)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/converter.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/error.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_broker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from fim.slivers.base_sliver import BaseSliver
 from fim.user import GraphFormat
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.apis.abc_mgmt_broker_mixin import ABCMgmtBrokerMixin
 from fabric_cf.actor.core.common.exceptions import ManageException
 from fabric_cf.actor.core.manage.kafka.kafka_server_actor import KafkaServerActor
+from fabric_cf.actor.core.time.actor_clock import ActorClock
 from fabric_cf.actor.core.util.id import ID
 
 
 class KafkaBroker(KafkaServerActor, ABCMgmtBrokerMixin):
     def add_reservation(self, *, reservation: TicketReservationAvro) -> ID:
         request = AddReservationAvro()
         request.guid = str(self.management_id)
@@ -132,14 +133,15 @@
                            dependencies: List[ReservationPredecessorAvro] = None) -> bool:
         request = ExtendReservationAvro()
         request.guid = str(self.management_id)
         request.auth = self.auth
         request.message_id = str(ID())
         request.callback_topic = self.callback_topic
         request.rid = str(reservation)
+        request.end_time = ActorClock.to_milliseconds(when=new_end_time)
         request.sliver = sliver
 
         status, response = self.send_request(request)
 
         return status.code == 0
 
     def claim_delegations(self, *, broker: ID, did: ID) -> DelegationAvro:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_container.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,14 @@
                     status.code = ErrorCodes.ErrorTransportTimeout.value
                     status.message = ErrorCodes.ErrorTransportTimeout.interpret()
                 else:
                     self.logger.debug(Constants.MANAGEMENT_INTER_ACTOR_INBOUND_MESSAGE.format(message_wrapper.response))
                     status = message_wrapper.response.status
                     if status.code == 0:
                         rret_val = message_wrapper.response
-
             else:
                 self.logger.debug(Constants.MANAGEMENT_INTER_ACTOR_MESSAGE_FAILED.format(
                     request.get_message_name(), self.kafka_topic))
                 status.code = ErrorCodes.ErrorTransportFailure.value
                 status.message = ErrorCodes.ErrorTransportFailure.interpret()
 
         except Exception as e:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/kafka/services/kafka_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_broker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_container.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/local/local_server_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_object_manager.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/management_utils.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/client_mng.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/event_mng.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/result_client_mng.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/messages/result_event_mng.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/manage/server_actor_management_object.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/server_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/base_plugin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/actor_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/actor_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import pickle
 import threading
+import time
 import traceback
 from datetime import datetime
 from typing import List
 
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin, ActorType
 from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
@@ -111,29 +112,29 @@
             raise DatabaseException(Constants.OBJECT_NOT_FOUND.format("actor", self.actor_name))
 
     def revisit(self, *, actor: ABCActorMixin, properties: dict):
         return
 
     def get_actor_id_from_name(self, *, actor_name: str) -> int or None:
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             actor = self.db.get_actor(name=actor_name)
             self.actor_id = actor['act_id']
             self.actor_type = ActorType(actor['act_type'])
             return self.actor_id
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return None
 
     def get_slice_by_id(self, *, slc_id: int) -> ABCSlice or None:
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             slice_dict = self.db.get_slice_by_id(slc_id=slc_id)
             if slice_dict is not None:
                 pickled_slice = slice_dict.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                 return pickle.loads(pickled_slice)
         except Exception as e:
             self.logger.error(e)
         finally:
@@ -150,15 +151,15 @@
             properties = pickle.dumps(slice_object)
             oidc_claim_sub = None
             email = None
             if slice_object.get_owner() is not None:
                 oidc_claim_sub = slice_object.get_owner().get_oidc_sub_claim()
                 email = slice_object.get_owner().get_email()
 
-            self.lock.acquire()
+            #self.lock.acquire()
             self.db.add_slice(slc_guid=str(slice_object.get_slice_id()),
                               slc_state=slice_object.get_state().value,
                               slc_name=slice_object.get_name(),
                               slc_type=slice_object.get_slice_type().value,
                               slc_resource_type=str(slice_object.get_resource_type()),
                               properties=properties,
                               slc_graph_id=slice_object.get_graph_id(),
@@ -172,15 +173,15 @@
 
     def update_slice(self, *, slice_object: ABCSlice):
         # Update the slice only when there are changes to be reflected in database
         if not slice_object.is_dirty():
             return
         slice_object.clear_dirty()
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(slice_object)
             self.db.update_slice(slc_guid=str(slice_object.get_slice_id()),
                                  slc_name=slice_object.get_name(),
                                  slc_type=slice_object.get_slice_type().value,
                                  slc_state=slice_object.get_state().value,
                                  slc_resource_type=str(slice_object.get_resource_type()),
                                  properties=properties,
@@ -188,27 +189,27 @@
                                  lease_end=slice_object.get_lease_end(), lease_start=slice_object.get_lease_start())
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_slice(self, *, slice_id: ID):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.db.remove_slice(slc_guid=str(slice_id))
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def get_slices(self, *, slice_id: ID = None, slice_name: str = None, project_id: str = None, email: str = None,
                    states: list[int] = None, oidc_sub: str = None, slc_type: List[SliceTypes] = None,
                    limit: int = None, offset: int = None, lease_end: datetime = None) -> List[ABCSlice] or None:
         result = []
         try:
             try:
-                self.lock.acquire()
+                #self.lock.acquire()
                 slice_type = None
                 if slc_type is not None:
                     slice_type = [x.value for x in slc_type]
                 sid = str(slice_id) if slice_id is not None else None
                 slices = self.db.get_slices(slice_id=sid, slice_name=slice_name, project_id=project_id, email=email,
                                             states=states, oidc_sub=oidc_sub, slc_type=slice_type, limit=limit,
                                             offset=offset, lease_end=lease_end)
@@ -226,15 +227,15 @@
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def add_reservation(self, *, reservation: ABCReservationMixin):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Adding reservation {} to slice {}".format(reservation.get_reservation_id(),
                                                                          reservation.get_slice()))
             properties = pickle.dumps(reservation)
             oidc_claim_sub = None
             email = None
             if reservation.get_slice() is not None and reservation.get_slice().get_owner() is not None:
                 oidc_claim_sub = reservation.get_slice().get_owner().get_oidc_sub_claim()
@@ -263,41 +264,48 @@
 
     def update_reservation(self, *, reservation: ABCReservationMixin):
         # Update the reservation only when there are changes to be reflected in database
         if not reservation.is_dirty():
             return
         reservation.clear_dirty()
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Updating reservation {} in slice {}".format(reservation.get_reservation_id(),
                                                                            reservation.get_slice()))
 
             site = None
             rsv_type = None
             if reservation.get_resources() is not None and reservation.get_resources().get_sliver() is not None:
                 site = reservation.get_resources().get_sliver().get_site()
                 rsv_type = reservation.get_resources().get_sliver().get_type().name
-
+            begin = time.time()
             properties = pickle.dumps(reservation)
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"PICKLE TIME: {diff}")
+            begin = time.time()
             self.db.update_reservation(slc_guid=str(reservation.get_slice_id()),
                                        rsv_resid=str(reservation.get_reservation_id()),
                                        rsv_category=reservation.get_category().value,
                                        rsv_state=reservation.get_state().value,
                                        rsv_pending=reservation.get_pending_state().value,
                                        rsv_joining=reservation.get_join_state().value,
                                        properties=properties,
                                        rsv_graph_node_id=reservation.get_graph_node_id(),
-                                       site=site, rsv_type = rsv_type)
+                                       site=site, rsv_type=rsv_type)
+            diff = int(time.time() - begin)
+            if diff > 0:
+                self.logger.info(f"DB TIME: {diff}")
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_reservation(self, *, rid: ID):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Removing reservation {}".format(rid))
             try:
                 self.db.remove_unit(unt_uid=str(rid))
             except Exception as e:
                 self.logger.debug("No associated Unit associated with the reservation")
             self.db.remove_reservation(rsv_resid=str(rid))
         finally:
@@ -341,15 +349,15 @@
             res_obj = self._load_reservation_from_pickled_object(pickled_res=pickled_res, slc_id=slc_id)
             result.append(res_obj)
         return result
 
     def get_client_reservations(self, *, slice_id: ID = None) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             sid = str(slice_id) if slice_id is not None else None
             res_dict_list = self.db.get_reservations(slice_id=sid,
                                                      category=[ReservationCategory.Broker.value,
                                                                ReservationCategory.Authority.value])
             if self.lock.locked():
                 self.lock.release()
             result = self._load_reservations_from_db(res_dict_list=res_dict_list)
@@ -359,15 +367,15 @@
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def get_holdings(self, *, slice_id: ID = None) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             sid = str(slice_id) if slice_id is not None else None
             res_dict_list = self.db.get_reservations(slice_id=sid, category=[ReservationCategory.Client.value])
             if self.lock.locked():
                 self.lock.release()
             result = self._load_reservations_from_db(res_dict_list=res_dict_list)
         except Exception as e:
             self.logger.error(e)
@@ -375,48 +383,49 @@
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def get_broker_reservations(self) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             res_dict_list = self.db.get_reservations(category=[ReservationCategory.Broker.value])
             if self.lock.locked():
                 self.lock.release()
             result = self._load_reservations_from_db(res_dict_list=res_dict_list)
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def get_authority_reservations(self) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             result = []
             res_dict_list = self.db.get_reservations(category=[ReservationCategory.Authority.value])
             if self.lock.locked():
                 self.lock.release()
             result = self._load_reservations_from_db(res_dict_list=res_dict_list)
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def get_reservations(self, *, slice_id: ID = None, graph_node_id: str = None, project_id: str = None,
                          email: str = None, oidc_sub: str = None, rid: ID = None,
-                         states: list[int] = None, site: str = None, rsv_type: int = None) -> List[ABCReservationMixin]:
+                         states: list[int] = None, site: str = None,
+                         rsv_type: list[str] = None) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             sid = str(slice_id) if slice_id is not None else None
             res_id = str(rid) if rid is not None else None
             res_dict_list = self.db.get_reservations(slice_id=sid, graph_node_id=graph_node_id,
                                                      project_id=project_id, email=email, oidc_sub=oidc_sub, rid=res_id,
                                                      states=states, site=site, rsv_type=rsv_type)
             if self.lock.locked():
                self.lock.release()
@@ -427,61 +436,61 @@
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def get_reservations_by_rids(self, *, rid: List[str]) -> List[ABCReservationMixin]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             res_dict_list = self.db.get_reservations_by_rids(rsv_resid_list=rid)
             if self.lock.locked():
                 self.lock.release()
             result = self._load_reservations_from_db(res_dict_list=res_dict_list)
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def add_broker(self, *, broker: ABCBrokerProxy):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Adding broker {}({})".format(broker.get_name(), broker.get_guid()))
             properties = pickle.dumps(broker)
             self.db.add_proxy(act_id=self.actor_id, prx_name=broker.get_name(), properties=properties)
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def update_broker(self, *, broker: ABCBrokerProxy):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Updating broker {}({})".format(broker.get_name(), broker.get_guid()))
             properties = pickle.dumps(broker)
             self.db.update_proxy(act_id=self.actor_id, prx_name=broker.get_name(), properties=properties)
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_broker(self, *, broker: ABCBrokerProxy):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Removing broker {}({})".format(broker.get_name(), broker.get_guid()))
             self.db.remove_proxy(act_id=self.actor_id, prx_name=broker.get_name())
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def set_actor_name(self, *, name: str):
         self.actor_name = name
 
     def get_brokers(self) -> List[ABCBrokerProxy] or None:
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             result = []
             broker_dict_list = self.db.get_proxies(act_id=self.actor_id)
             if broker_dict_list is not None:
                 for b in broker_dict_list:
                     pickled_broker = b.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                     broker_obj = pickle.loads(pickled_broker)
                     result.append(broker_obj)
@@ -494,15 +503,15 @@
                 self.lock.release()
         return None
 
     def add_delegation(self, *, delegation: ABCDelegation):
         self.logger.debug("Adding delegation {} to slice {}".format(delegation.get_delegation_id(),
                                                                     delegation.get_slice_id()))
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(delegation)
             self.db.add_delegation(slice_id=str(delegation.get_slice_id()),
                                    dlg_graph_id=str(delegation.get_delegation_id()),
                                    dlg_state=delegation.get_state().value,
                                    properties=properties)
             self.logger.debug(
                 "Delegation {} added to slice {}".format(delegation.get_delegation_id(),
@@ -513,28 +522,28 @@
 
     def update_delegation(self, *, delegation: ABCDelegation):
         # Update the delegation only when there are changes to be reflected in database
         if not delegation.is_dirty():
             return
         delegation.clear_dirty()
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Updating delegation {} in slice {}".format(delegation.get_delegation_id(),
                                                                           delegation.get_slice_id()))
             properties = pickle.dumps(delegation)
             self.db.update_delegation(dlg_graph_id=str(delegation.get_delegation_id()),
                                       dlg_state=delegation.get_state().value,
                                       properties=properties)
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_delegation(self, *, dlg_graph_id: str):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug("Removing delegation {}".format(dlg_graph_id))
             self.db.remove_delegation(dlg_graph_id=str(dlg_graph_id))
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def _load_delegation_from_pickled_instance(self, pickled_del: bytes, slc_id: int) -> ABCDelegation:
@@ -554,33 +563,34 @@
             dlg_obj = self._load_delegation_from_pickled_instance(pickled_del=pickled_del, slc_id=slc_id)
             result.append(dlg_obj)
 
         return result
 
     def get_delegation(self, *, dlg_graph_id: str) -> ABCDelegation or None:
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             dlg_dict = self.db.get_delegation(dlg_graph_id=str(dlg_graph_id))
             if self.lock.locked():
                 self.lock.release()
             return self._load_delegation_from_db(dlg_dict_list=[dlg_dict])[0]
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return None
 
     def get_delegations(self, *, slice_id: ID = None, states: List[int] = None) -> List[ABCDelegation]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             sid = str(slice_id) if slice_id is not None else None
             dlg_dict_list = self.db.get_delegations(slc_guid=sid, states=states)
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
             result = self._load_delegation_from_db(dlg_dict_list=dlg_dict_list)
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
@@ -616,35 +626,35 @@
         except Exception as e:
             self.logger.error(e)
         return result
 
     def add_site(self, *, site: Site):
         self.logger.debug(f"Adding site {site.get_name()}")
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(site)
             self.db.add_site(site_name=site.get_name(), state=site.get_state().value, properties=properties)
             self.logger.debug(f"Site {site.get_name()} added")
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def update_site(self, *, site: Site):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug(f"Updating site {site.get_name()}")
             properties = pickle.dumps(site)
             self.db.update_site(site_name=site.get_name(), state=site.get_state().value, properties=properties)
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_site(self, *, site_name: str):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.logger.debug(f"Removing site {site_name}")
             self.db.remove_site(site_name=site_name)
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def _load_site_from_db(self, site_list: List[dict]) -> List[Site]:
@@ -657,15 +667,15 @@
             site = pickle.loads(pickled_site)
             result.append(site)
 
         return result
 
     def get_site(self, *, site_name: str) -> Site or None:
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             site_list = self.db.get_site(site_name=site_name)
             if self.lock.locked():
                 self.lock.release()
             if site_list is not None and len(site_list) > 0:
                 return self._load_site_from_db(site_list=site_list)[0]
         except Exception as e:
             self.logger.error(e)
@@ -674,43 +684,44 @@
             if self.lock.locked():
                 self.lock.release()
         return None
 
     def get_sites(self) -> List[Site]:
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             site_list = self.db.get_sites()
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
             result = self._load_site_from_db(site_list=site_list)
         except Exception as e:
             self.logger.error(e)
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def add_config_mapping(self, key: str, config_mapping: ConfigurationMapping):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(config_mapping)
             self.db.add_config_mapping(cfgm_type=key, act_id=self.actor_id, properties=properties)
         except Exception as e:
             self.logger.error(e)
             self.logger.error(traceback.format_exc())
             raise e
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def get_config_mappings(self) -> List[ConfigurationMapping]:
         cfg_map_list = None
         result = []
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             cfg_map_list = self.db.get_config_mappings(act_id=self.actor_id)
         except Exception as e:
             self.logger.error(e)
             self.logger.error(traceback.format_exc())
         finally:
             if self.lock.locked():
                 self.lock.release()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/client_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/client_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         """
         Removes the specified client record
         @param guid client guid
         @throws Exception in case of error
         """
 
     @abstractmethod
-    def get_client(self, *, guid: ID) -> Client:
+    def get_client(self, *, guid: ID) -> Client or None:
         """
         Retrieves the specified client record
         @param guid client guid
         @return vector of properties
         @throws Exception in case of error
         """
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/db/server_actor_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/server_actor_database.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,60 +32,65 @@
 from fabric_cf.actor.core.util.client import Client
 from fabric_cf.actor.core.util.id import ID
 
 
 class ServerActorDatabase(ActorDatabase, ClientDatabase):
     def add_client(self, *, client: Client):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(client)
             self.db.add_client(act_id=self.actor_id, clt_name=client.get_name(), clt_guid=str(client.get_guid()),
                                properties=properties)
         finally:
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
 
     def update_client(self, *, client: Client):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(client)
             self.db.update_client(act_id=self.actor_id, clt_name=client.get_name(), properties=properties)
         finally:
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
 
     def remove_client(self, *, guid: ID):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.db.remove_client_by_guid(act_id=self.actor_id, clt_guid=str(guid))
         finally:
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
 
-    def get_client(self, *, guid: ID) -> Client:
+    def get_client(self, *, guid: ID) -> Client or None:
         result = None
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             client_dict = self.db.get_client_by_guid(clt_guid=str(guid))
             if client_dict is not None:
                 pickled_client = client_dict.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                 return pickle.loads(pickled_client)
         except Exception as e:
             self.logger.error(e)
         finally:
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
         return result
 
     def get_clients(self) -> List[Client]:
         result = None
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             result = []
             client_dict_list = self.db.get_clients()
             if client_dict_list is not None:
                 for c in client_dict_list:
                     pickled_client = c.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                     client_obj = pickle.loads(pickled_client)
                     result.append(client_obj)
             return result
         except Exception as e:
             self.logger.error(e)
         finally:
-            self.lock.release()
+            if self.lock.locked():
+                self.lock.release()
         return result
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/config_token.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/config_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/handlers/handler_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/handler_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,42 +99,42 @@
             self.lock.acquire()
             self.config_mappings[mapping.get_key()] = mapping
             self.plugin.get_database().add_config_mapping(key=mapping.get_key(), config_mapping=mapping)
         finally:
             self.lock.release()
 
     def create(self, unit: ConfigToken):
-        self.logger.info("Executing Create")
+        self.logger.debug("Executing Create")
 
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_CREATE,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
 
         self.plugin.configuration_complete(token=unit, properties=result)
-        self.logger.info("Executing Create completed")
+        self.logger.debug("Executing Create completed")
 
     def delete(self, unit: ConfigToken):
-        self.logger.info("Executing Delete")
+        self.logger.debug("Executing Delete")
 
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_DELETE,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
 
         self.plugin.configuration_complete(token=unit, properties=result)
-        self.logger.info("Executing Delete completed")
+        self.logger.debug("Executing Delete completed")
 
     def modify(self, unit: ConfigToken):
-        self.logger.info("Executing Modify")
+        self.logger.debug("Executing Modify")
 
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_MODIFY,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
 
         self.plugin.configuration_complete(token=unit, properties=result)
-        self.logger.info("Executing Modify completed")
+        self.logger.debug("Executing Modify completed")
 
     def set_logger(self, *, logger):
         self.logger = logger
 
     def set_plugin(self, *, plugin: BasePlugin):
         self.plugin = plugin
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/authority_substrate.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/authority_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,23 @@
 
         return result
 
     def add_unit(self, *, u: Unit):
         try:
             if u.get_resource_type() is None:
                 raise DatabaseException(Constants.INVALID_ARGUMENT)
-            self.lock.acquire()
+            #self.lock.acquire()
             if self.get_unit(uid=u.get_id()) is not None:
                 self.logger.info("unit {} is already present in database".format(u.get_id()))
                 return
 
             slice_id = str(u.get_slice_id())
-            parent = self.get_unit(uid=u.get_parent_id())
+            parent = None
+            if u.get_parent_id() is not None:
+                parent = self.get_unit(uid=u.get_parent_id())
             parent_id = None
             if parent is not None:
                 parent_id = parent['unt_id']
             res_id = str(u.get_reservation_id())
 
             properties = pickle.dumps(u)
             self.db.add_unit(slc_guid=slice_id, rsv_resid=res_id,
@@ -71,15 +73,15 @@
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def get_units(self, *, rid: ID):
         result = None
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             result = []
             unit_dict_list = self.db.get_units(rsv_resid=str(rid))
             if unit_dict_list is not None:
                 for u in unit_dict_list:
                     pickled_unit = u.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                     unit_obj = pickle.loads(pickled_unit)
                     result.append(unit_obj)
@@ -89,21 +91,21 @@
         finally:
             if self.lock.locked():
                 self.lock.release()
         return result
 
     def remove_unit(self, *, uid: ID):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             self.db.remove_unit(unt_uid=str(uid))
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def update_unit(self, *, u: Unit):
         try:
-            self.lock.acquire()
+            #self.lock.acquire()
             properties = pickle.dumps(u)
             self.db.update_unit(unt_uid=str(u.get_id()), properties=properties)
         finally:
             if self.lock.locked():
                 self.lock.release()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/authority_calendar_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/authority_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/broker_calendar_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/broker_simpler_units_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_simpler_units_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_calendar_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_calendar_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
        
         @raises Exception in case of error
         """
         rvset = self.calendar.get_pending()
         if rvset is None:
             return
 
-        for reservation in rvset.values():
+        for reservation in rvset.reservations.values():
             if reservation.is_failed():
                 # This reservation has failed. Remove it from the list. This is
                 # a separate case, because we may fail but not satisfy the
                 # condition of the else statement.
                 self.logger.debug("Removing failed reservation from the pending list: {}".format(reservation))
                 self.calendar.remove_pending(reservation=reservation)
                 self.pending_notify.remove(reservation=reservation)
@@ -211,15 +211,15 @@
 
         @raises Exception in case of error
         """
 
     def get_closing(self, *, cycle: int) -> ReservationSet:
         closing = self.calendar.get_closing(cycle=cycle)
         result = ReservationSet()
-        for reservation in closing.values():
+        for reservation in closing.reservations.values():
             if not reservation.is_failed():
                 self.calendar.add_pending(reservation=reservation)
                 result.add(reservation=reservation)
             else:
                 self.logger.warning("Removing failed reservation from the closing list: {}".format(reservation))
         return result
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_simple_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_simple_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,20 +173,20 @@
         @throws Exception in case of error rare
         """
         result = ReservationSet()
         renewing = self.calendar.get_renewing(cycle=cycle)
         if renewing is None or renewing.size() == 0:
             return result
 
-        self.logger.debug("Renewing = {}".format(renewing.size()))
+        #self.logger.debug("Renewing = {}".format(renewing.size()))
         for reservation in renewing.values():
-            self.logger.debug("Renewing res: {}".format(reservation))
+            #self.logger.debug("Renewing res: {}".format(reservation))
 
             if reservation.is_renewable():
-                self.logger.debug("Found a renewable reservation that needs an extension.")
+                #self.logger.debug("Found a renewable reservation that needs an extension.")
                 if reservation.is_closed() or reservation.is_closing() or reservation.is_failed():
                     self.logger.debug("Found a renewable reservation that is closing/closed/or failed")
                 else:
                     suggested_term = reservation.get_suggested_term()
                     suggested_resources = reservation.get_suggested_resources()
                     current_term = reservation.get_term()
                     approved_resources = reservation.get_resources().abstract_clone()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/controller_ticket_review_policy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_ticket_review_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,42 +80,42 @@
         """
         Check to make sure all reservations are Ticketed (not Failed or Nascent)
         before calling the parent method.
 
         @throws Exception in case of error
         """
         # add all of our pendingRedeem, so they can be checked
-        for reservation in self.pending_redeem.values():
+        for reservation in self.pending_redeem.reservations.values():
             self.calendar.add_pending(reservation=reservation)
 
         # get set of reservations that need to be redeemed
         my_pending = self.calendar.get_pending()
 
         # keep track of status of the slice containing each reservation
         slice_status_map = {}
 
         # nothing to do!
         if my_pending is None:
             return
 
         # check the status of the Slice of each reservation
-        for reservation in my_pending.values():
+        for reservation in my_pending.reservations.values():
             slice_obj = reservation.get_slice()
             slice_id = slice_obj.get_slice_id()
 
             # only want to do this for 'new' tickets
             if reservation.is_failed() or reservation.is_ticketed() or reservation.is_ticketing():
                 # check if we've examined this slice already
                 if slice_id not in slice_status_map:
                     # set the default status
                     slice_status_map[slice_id] = TicketReviewSliceState.Redeemable
                     # examine every reservation contained within the slice,
                     # looking for either a Failed or Nascent reservation
                     # we have to look at everything in a slice once, to determine all/any Sites with failures
-                    for slice_reservation in slice_obj.get_reservations().values():
+                    for slice_reservation in slice_obj.get_reservations_list():
 
                         # If any Reservations that are being redeemed, that means the
                         # slice has already cleared TicketReview.
                         if slice_reservation.is_redeeming():
                             if slice_status_map[slice_id] == TicketReviewSliceState.Nascent:
                                 # There shouldn't be any Nascent reservations, if a reservation is being Redeemed.
                                 self.logger.error(
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/fifo_queue.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/fifo_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/inventory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/inventory_for_type.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory_for_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_node_control.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_node_inventory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_service_control.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/network_service_inventory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/queue_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/policy/resource_control.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/actor_location.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/actor_location.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/kafka_retun.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_retun.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/actor_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/authority_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/broker_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/services/controller_service.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/kafka/translate.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/translate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_authority.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_broker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_proxy_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/local/local_return.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_return.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/proxies/proxy_factory.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/actor_registry.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/actor_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/callback_registry.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/callback_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/peer_registry.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/peer_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/registry/proxy_registry.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/proxy_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/actor_clock.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/actor_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/authority_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/authority_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/base_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/base_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/broker_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/broker_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/client_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/client_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/controller_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/controller_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/calendar/source_calendar.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/source_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/time/term.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/term.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/bids.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/bids.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/client.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/graceful_interrupt_handler.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/graceful_interrupt_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/id.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/id.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/iterable_queue.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/iterable_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/kernel_timer.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/kernel_timer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/log_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/log_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/notice.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/notice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reflection_utils.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_holdings.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_holdings.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_list.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_list.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_set.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-import datetime
 import threading
 
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.common.exceptions import FrameworkException
 from fabric_cf.actor.core.util.id import ID
 
 
@@ -212,13 +211,10 @@
             return result
         finally:
             self.lock.release()
 
     def values(self) -> list:
         try:
             self.lock.acquire()
-            result = []
-            for r in self.reservations.values():
-                result.append(r)
-            return result
+            return list(self.reservations.values())
         finally:
             self.lock.release()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/reservation_state.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/resource_type.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/rpc_exception.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/rpc_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/update_data.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/update_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/core/util/utils.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/db/__init__.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/db/psql_database.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/db/psql_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import logging
 import pickle
+import threading
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from typing import List
 
 from sqlalchemy import create_engine, desc
 from sqlalchemy.orm import scoped_session, sessionmaker
 
@@ -58,14 +59,26 @@
     """
     OBJECT_NOT_FOUND = "{} Not Found {}"
 
     def __init__(self, *, user: str, password: str, database: str, db_host: str, logger):
         # Connecting to PostgreSQL server at localhost using psycopg2 DBAPI
         self.db_engine = create_engine("postgresql+psycopg2://{}:{}@{}/{}".format(user, password, db_host, database))
         self.logger = logger
+        self.session_factory = sessionmaker(bind=self.db_engine)
+        self.sessions = {}
+
+    def get_session(self):
+        thread_id = threading.get_ident()
+        session = None
+        if thread_id in self.sessions:
+            session = self.sessions.get(thread_id)
+        else:
+            session = scoped_session(self.session_factory)
+            self.sessions[thread_id] = session
+        return session
 
     def create_db(self):
         """
         Create the database
         """
         Base.metadata.create_all(self.db_engine)
 
@@ -75,288 +88,287 @@
         """
         self.logger = logger
 
     def reset_db(self):
         """
         Reset the database
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Clients).delete()
-                session.query(ConfigMappings).delete()
-                session.query(Proxies).delete()
-                session.query(Units).delete()
-                session.query(Delegations).delete()
-                session.query(Reservations).delete()
-                session.query(Slices).delete()
-                session.query(ManagerObjects).delete()
-                session.query(Miscellaneous).delete()
-                session.query(Actors).delete()
-
+            session.query(Clients).delete()
+            session.query(ConfigMappings).delete()
+            session.query(Proxies).delete()
+            session.query(Units).delete()
+            session.query(Delegations).delete()
+            session.query(Reservations).delete()
+            session.query(Slices).delete()
+            session.query(ManagerObjects).delete()
+            session.query(Miscellaneous).delete()
+            session.query(Actors).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def add_actor(self, *, name: str, guid: str, act_type: int, properties):
         """
         Add an actor
         @param name name
         @param guid guid
         @param act_type actor type
         @param properties pickle dump for actor instance
         """
+        session = self.get_session()
         try:
             # Save the actor in the database
             actor_obj = Actors(act_name=name, act_guid=guid, act_type=act_type, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(actor_obj)
-
+            session.add(actor_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_actor(self, *, name: str, properties):
         """
         Update an actor
         @param name name
         @param properties pickle dump for actor instance
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                actor = session.query(Actors).filter_by(act_name=name).first()
-                if actor is not None:
-                    actor.properties = properties
-
+            actor = session.query(Actors).filter_by(act_name=name).one_or_none()
+            if actor is not None:
+                actor.properties = properties
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_actor(self, *, name: str):
         """
         Remove an actor
         @param name name
         """
+        session = self.get_session()
         try:
             # Delete the actor in the database
-            with session_scope(self.db_engine) as session:
-                session.query(Actors).filter(Actors.act_name == name).delete()
-
+            session.query(Actors).filter_by(act_name=name).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def get_actors(self) -> list:
         """
         Get all actors
         @return list of actors
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Actors).all():
-                    actor = {'act_guid': row.act_guid, 'act_name': row.act_name, 'act_type': row.act_type,
-                             'properties': row.properties, 'act_id': row.act_id}
-                    result.append(actor.copy())
-                    actor.clear()
+            for row in session.query(Actors).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_actors_by_name_and_type(self, *, actor_name: str, act_type: int) -> list:
         """
         Get actors by name and  actor type
         @param actor_name actor name
         @param act_type actor type
         @return list of actors
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Actors).filter(Actors.act_type == act_type).filter(
-                        Actors.act_name.like(actor_name)).all():
-                    actor = {'act_guid': row.act_guid, 'act_name': row.act_name, 'act_type': row.act_type,
-                             'properties': row.properties, 'act_id': row.act_id}
-                    result.append(actor.copy())
-                    actor.clear()
+            for row in session.query(Actors).filter(Actors.act_type == act_type).filter(
+                    Actors.act_name.like(actor_name)).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_actors_by_name(self, *, act_name: str) -> list:
         """
         Get actors by name
         @param act_name actor name
         @return list of actors
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Actors).filter(Actors.act_name.like(act_name)).all():
-                    actor = {'act_guid': row.act_guid, 'act_name': row.act_name, 'act_type': row.act_type,
-                             'properties': row.properties, 'act_id': row.act_id}
-                    result.append(actor.copy())
-                    actor.clear()
+            for row in session.query(Actors).filter(Actors.act_name.like(act_name)).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_actor(self, *, name: str) -> dict:
         """
         Get actor by name
         @return actor
         """
         result = {}
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                actor = session.query(Actors).filter_by(act_name=name).first()
-                if actor is not None:
-                    result['act_guid'] = actor.act_guid
-                    result['act_name'] = actor.act_name
-                    result['act_type'] = actor.act_type
-                    result['properties'] = actor.properties
-                    result['act_id'] = actor.act_id
-                else:
-                    result = None
-                    self.logger.error("Actor: {} not found!".format(name))
+            actor = session.query(Actors).filter_by(act_name=name).one_or_none()
+            if actor is not None:
+                result['act_guid'] = actor.act_guid
+                result['act_name'] = actor.act_name
+                result['act_type'] = actor.act_type
+                result['properties'] = actor.properties
+                result['act_id'] = actor.act_id
+            else:
+                result = None
+                self.logger.error("Actor: {} not found!".format(name))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_miscellaneous(self, *, name: str, properties: dict):
         """
         Add Miscellaneous entries
         @param name name
         @param properties properties
 
         """
+        session = self.get_session()
         try:
             msc_obj = Miscellaneous(msc_path=name, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(msc_obj)
-
+            session.add(msc_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_miscellaneous(self, *, name: str, properties: dict):
         """
         Add Miscellaneous entries
         @param name name
         @param properties properties
 
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                msc_obj = session.query(Miscellaneous).filter(Miscellaneous.msc_path == name).first()
-                if msc_obj is not None:
-                    msc_obj.properties = properties
+            msc_obj = session.query(Miscellaneous).filter_by(msc_path=name).one_or_none()
+            if msc_obj is not None:
+                msc_obj.properties = properties
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_miscellaneous(self, *, name: str):
         """
         Remove Miscellaneous entries
         @param name name
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Miscellaneous).filter(Miscellaneous.msc_path == name).delete()
+            session.query(Miscellaneous).filter_by(msc_path=name).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def get_miscellaneous(self, *, name: str) -> dict or None:
         """
         Get Miscellaneous entry
         @param name name
         @return entry identified by name
         """
         result = {}
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                msc_obj = session.query(Miscellaneous).filter_by(msc_path=name).first()
-                if msc_obj is not None:
-                    result = msc_obj.properties
-                else:
-                    return None
+            msc_obj = session.query(Miscellaneous).filter_by(msc_path=name).one_or_none()
+            if msc_obj is not None:
+                result = msc_obj.properties
+            else:
+                return None
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_manager_object(self, *, manager_key: str, properties: dict, act_id: int = None):
         """
         Add mananger object
         @param manager_key management object key
         @param properties properties
         @param act_id actor id
         """
+        session = self.get_session()
         try:
             if act_id is not None:
                 mng_obj = ManagerObjects(mo_key=manager_key, mo_act_id=act_id, properties=properties)
             else:
                 mng_obj = ManagerObjects(mo_key=manager_key, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(mng_obj)
-
+            session.add(mng_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_manager_object(self, *, manager_key: str):
         """
         Remove management object
         @param manager_key management object key
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(ManagerObjects).filter(ManagerObjects.mo_key == manager_key).delete()
+            session.query(ManagerObjects).filter_by(mo_key=manager_key).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_manager_object_by_actor(self, *, act_id: int):
         """
         Remove management object by actor id
         @param act_id actor id
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(ManagerObjects).filter(ManagerObjects.mo_act_id == act_id).delete()
+            session.query(ManagerObjects).filter_by(mo_act_id=act_id).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def get_manager_objects(self, *, act_id: int = None) -> list:
         """
         Get Management objects
         @param act_id actor id
         @return list of objects
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                if act_id is None:
-                    for row in session.query(ManagerObjects).all():
-                        mo = {'mo_act_id': row.mo_act_id, 'mo_key': row.mo_key, 'properties': row.properties,
-                              'mo_id': row.mo_id}
-                        result.append(mo.copy())
-                        mo.clear()
-                else:
-                    for row in session.query(ManagerObjects).filter(ManagerObjects.mo_act_id == act_id).all():
-                        mo = {'mo_act_id': row.mo_act_id, 'mo_key': row.mo_key, 'properties': row.properties,
-                              'mo_id': row.mo_id}
-                        result.append(mo.copy())
-                        mo.clear()
+            if act_id is None:
+                rows = session.query(ManagerObjects).all()
+            else:
+                rows = session.query(ManagerObjects).filter_by(mo_act_id=act_id).all()
 
+            for row in rows:
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_manager_objects_by_actor_name(self, *, act_name: str = None) -> list:
         """
@@ -377,42 +389,36 @@
     def get_manager_object(self, *, mo_key: str) -> dict:
         """
         Get Management object by key
         @param mo_key management object key
         @return objects
         """
         result = {}
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                mo_obj = session.query(ManagerObjects).filter_by(mo_key=mo_key).first()
-                if mo_obj is not None:
-                    result['mo_id'] = mo_obj.mo_id
-                    result['mo_key'] = mo_obj.mo_key
-                    if mo_obj.mo_act_id is not None:
-                        result['mo_act_id'] = mo_obj.mo_act_id
-                    result['properties'] = mo_obj.properties
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Manager Object", mo_key))
+            mo_obj = session.query(ManagerObjects).filter_by(mo_key=mo_key).one_or_none()
+            if mo_obj is not None:
+                result = self.generate_dict_from_row(mo_obj)
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Manager Object", mo_key))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_manager_containers(self) -> list:
         """
         Get Management object for the container i.e entry with no actor id
         @return object
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for mo_obj in session.query(ManagerObjects).filter(ManagerObjects.mo_act_id.is_(None)).all():
-                    mo = {'mo_id': mo_obj.mo_id, 'mo_key': mo_obj.mo_key, 'properties': mo_obj.properties}
-                    result.append(mo.copy())
-                    mo.clear()
+            for mo_obj in session.query(ManagerObjects).filter(ManagerObjects.mo_act_id.is_(None)).all():
+                result.append(self.generate_dict_from_row(mo_obj))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_slice(self, *, slc_guid: str, slc_name: str, slc_type: int, slc_state: int, lease_start: datetime = None,
                   lease_end: datetime = None, slc_resource_type: str, properties, slc_graph_id: str = None,
@@ -428,24 +434,27 @@
         @param lease_end Lease End time
         @param properties pickled instance
         @param slc_graph_id slice graph id
         @param oidc_claim_sub User OIDC Sub
         @param email User Email
         @param project_id Project Id
         """
+        session = self.get_session()
         try:
             slc_obj = Slices(slc_guid=slc_guid, slc_name=slc_name, slc_type=slc_type, slc_state=slc_state,
                              oidc_claim_sub=oidc_claim_sub, email=email, slc_resource_type=slc_resource_type,
                              lease_start=lease_start, lease_end=lease_end, properties=properties,
                              project_id=project_id)
             if slc_graph_id is not None:
                 slc_obj.slc_graph_id = slc_graph_id
-            with session_scope(self.db_engine) as session:
-                session.add(slc_obj)
+            
+            session.add(slc_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_slice(self, *, slc_guid: str, slc_name: str, slc_type: int, slc_state: int, slc_resource_type: str,
                      properties, slc_graph_id: str = None, lease_start: datetime = None, lease_end: datetime = None):
         """
         Update a slice
@@ -455,73 +464,60 @@
         @param slc_state slice state
         @param slc_resource_type slice resource type
         @param lease_start Lease Start time
         @param lease_end Lease End time
         @param properties pickled instance
         @param slc_graph_id slice graph id
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                slc_obj = session.query(Slices).filter(Slices.slc_guid == slc_guid).first()
-                if slc_obj is not None:
-                    slc_obj.properties = properties
-                    slc_obj.slc_name = slc_name
-                    slc_obj.slc_type = slc_type
-                    slc_obj.slc_resource_type = slc_resource_type
-                    slc_obj.slc_state = slc_state
-                    slc_obj.lease_start = lease_start
-                    slc_obj.lease_end = lease_end
-                    if slc_graph_id is not None:
-                        slc_obj.slc_graph_id = slc_graph_id
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Slice", slc_guid))
+            slc_obj = session.query(Slices).filter_by(slc_guid=slc_guid).one_or_none()
+            if slc_obj is not None:
+                slc_obj.properties = properties
+                slc_obj.slc_name = slc_name
+                slc_obj.slc_type = slc_type
+                slc_obj.slc_resource_type = slc_resource_type
+                slc_obj.slc_state = slc_state
+                slc_obj.lease_start = lease_start
+                slc_obj.lease_end = lease_end
+                if slc_graph_id is not None:
+                    slc_obj.slc_graph_id = slc_graph_id
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Slice", slc_guid))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_slice(self, *, slc_guid: str):
         """
         Remove Slice
         @param slc_guid slice id
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Slices).filter(Slices.slc_guid == slc_guid).delete()
+            session.query(Slices).filter_by(slc_guid=slc_guid).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_slice_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a slice row read from database
-        """
-        if row is None:
-            return None
-
-        slice_obj = {'slc_id': row.slc_id, 'slc_guid': row.slc_guid, 'slc_name': row.slc_name,
-                     'slc_type': row.slc_type, 'slc_resource_type': row.slc_resource_type, 'slc_state': row.slc_state,
-                     'project_id': row.project_id, 'lease_start': row.lease_start, 'lease_end': row.lease_end,
-                     'properties': row.properties}
-        if row.slc_graph_id is not None:
-            slice_obj['slc_graph_id'] = row.slc_graph_id
-
-        return slice_obj
-
     def get_slice_ids(self) -> list:
         """
         Get slice ids for an actor
         @param act_id actor id
         @return list of slice ids
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Slices).all():
-                    result.append(row.slc_id)
+            for row in session.query(Slices).all():
+                result.append(row.slc_id)
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     @staticmethod
     def create_slices_filter(*, slice_id: str = None, slice_name: str = None, project_id: str = None, email: str = None,
@@ -538,15 +534,15 @@
             filter_dict['email'] = email
         if oidc_sub is not None:
             filter_dict['oidc_claim_sub'] = oidc_sub
         return filter_dict
 
     def get_slices(self, *, slice_id: str = None, slice_name: str = None, project_id: str = None, email: str = None,
                    states: list[int] = None, oidc_sub: str = None, slc_type: list[int] = None, limit: int = None,
-                   offset: int = None, lease_end: datetime = None) -> list:
+                   offset: int = None, lease_end: datetime = None) -> List[dict]:
         """
         Get slices for an actor
         @param slice_id actor id
         @param slice_name slice name
         @param project_id project id
         @param email email
         @param states states
@@ -554,57 +550,56 @@
         @param slc_type slice type
         @param limit limit
         @param offset offset
         @param lease_end lease_end
         @return list of slices
         """
         result = []
+        session = self.get_session()
         try:
             filter_dict = self.create_slices_filter(slice_id=slice_id, slice_name=slice_name, project_id=project_id,
                                                     email=email, oidc_sub=oidc_sub)
-            with session_scope(self.db_engine) as session:
-                rows = session.query(Slices).filter_by(**filter_dict)
 
-                if lease_end is not None:
-                    rows = rows.filter(Slices.lease_end < lease_end)
+            rows = session.query(Slices).filter_by(**filter_dict)
 
-                rows = rows.order_by(desc(Slices.lease_end))
+            if lease_end is not None:
+                rows = rows.filter(Slices.lease_end < lease_end)
 
-                if states is not None:
-                    rows = rows.filter(Slices.slc_state.in_(states))
+            rows = rows.order_by(desc(Slices.lease_end))
 
-                if slc_type is not None:
-                    rows = rows.filter(Slices.slc_type.in_(slc_type))
+            if states is not None:
+                rows = rows.filter(Slices.slc_state.in_(states))
 
-                if offset is not None and limit is not None:
-                    rows = rows.offset(offset).limit(limit)
+            if slc_type is not None:
+                rows = rows.filter(Slices.slc_type.in_(slc_type))
 
-                for row in rows.all():
-                    slice_obj = self.generate_slice_dict_from_row(row)
-                    result.append(slice_obj.copy())
-                    slice_obj.clear()
+            if offset is not None and limit is not None:
+                rows = rows.offset(offset).limit(limit)
+
+            for row in rows.all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_slice_by_id(self, *, slc_id: int) -> dict:
         """
         Get slice by id for an actor
         @param slc_id slice id
         @return slice dictionary
         """
         result = {}
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                slc_obj = session.query(Slices).filter(Slices.slc_id == slc_id).first()
-                if slc_obj is not None:
-                    result = self.generate_slice_dict_from_row(slc_obj)
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Slice", slc_id))
+            slc_obj = session.query(Slices).filter_by(slc_id=slc_id).one_or_none()
+            if slc_obj is not None:
+                result = self.generate_dict_from_row(slc_obj)
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Slice", slc_id))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_reservation(self, *, slc_guid: str, rsv_resid: str, rsv_category: int, rsv_state: int,
                         rsv_pending: int, rsv_joining: int, properties, lease_start: datetime = None,
@@ -624,26 +619,29 @@
         @param rsv_graph_node_id graph id
         @param oidc_claim_sub OIDC Sub claim
         @param email User email
         @param project_id Project id
         @param site site
         @param rsv_type reservation type
         """
+        session = self.get_session()
         try:
             slc_id = self.get_slc_id_by_slice_id(slice_id=slc_guid)
             rsv_obj = Reservations(rsv_slc_id=slc_id, rsv_resid=rsv_resid, rsv_category=rsv_category,
                                    rsv_state=rsv_state, rsv_pending=rsv_pending, rsv_joining=rsv_joining,
                                    lease_start=lease_start, lease_end=lease_end,
                                    properties=properties, oidc_claim_sub=oidc_claim_sub, email=email,
                                    project_id=project_id, site=site, rsv_type=rsv_type)
             if rsv_graph_node_id is not None:
                 rsv_obj.rsv_graph_node_id = rsv_graph_node_id
-            with session_scope(self.db_engine) as session:
-                session.add(rsv_obj)
+            
+            session.add(rsv_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_reservation(self, *, slc_guid: str, rsv_resid: str, rsv_category: int, rsv_state: int,
                            rsv_pending: int, rsv_joining: int, properties, lease_start: datetime = None,
                            lease_end: datetime = None, rsv_graph_node_id: str = None, site: str = None,
                            rsv_type: str = None):
@@ -658,69 +656,55 @@
         @param properties pickled instance
         @param lease_start Lease start time
         @param lease_end Lease end time
         @param rsv_graph_node_id graph id
         @param site site
         @param rsv_type reservation type
         """
+        session = self.get_session()
         try:
-            slc_id = self.get_slc_id_by_slice_id(slice_id=slc_guid)
-            with session_scope(self.db_engine) as session:
-                rsv_obj = session.query(Reservations).filter(Reservations.rsv_slc_id == slc_id).filter(
-                    Reservations.rsv_resid == rsv_resid).first()
-                if rsv_obj is not None:
-                    rsv_obj.rsv_category = rsv_category
-                    rsv_obj.rsv_state = rsv_state
-                    rsv_obj.rsv_pending = rsv_pending
-                    rsv_obj.rsv_joining = rsv_joining
-                    rsv_obj.properties = properties
-                    rsv_obj.lease_end = lease_end
-                    rsv_obj.lease_start = lease_start
-                    if site is not None:
-                        rsv_obj.site = site
-                    if rsv_graph_node_id is not None:
-                        rsv_obj.rsv_graph_node_id = rsv_graph_node_id
-                    if rsv_type is not None:
-                        rsv_obj.rsv_type = rsv_type
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Reservation", rsv_resid))
+            rsv_obj = session.query(Reservations).filter_by(rsv_resid=rsv_resid).one()
+            if rsv_obj is not None:
+                rsv_obj.rsv_category = rsv_category
+                rsv_obj.rsv_state = rsv_state
+                rsv_obj.rsv_pending = rsv_pending
+                rsv_obj.rsv_joining = rsv_joining
+                rsv_obj.properties = properties
+                rsv_obj.lease_end = lease_end
+                rsv_obj.lease_start = lease_start
+                if site is not None:
+                    rsv_obj.site = site
+                if rsv_graph_node_id is not None:
+                    rsv_obj.rsv_graph_node_id = rsv_graph_node_id
+                if rsv_type is not None:
+                    rsv_obj.rsv_type = rsv_type
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Reservation", rsv_resid))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_reservation(self, *, rsv_resid: str):
         """
         Remove a reservation
         @param rsv_resid reservation guid
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Reservations).filter(Reservations.rsv_resid == rsv_resid).delete()
+            session.query(Reservations).filter_by(rsv_resid=rsv_resid).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_reservation_dict_from_row(row) -> dict:
-        """
-        Generate a dictionary representing a reservation row read from database
-        @param row row
-        """
-        if row is None:
-            return None
-        rsv_obj = {'rsv_id': row.rsv_id, 'rsv_slc_id': row.rsv_slc_id, 'rsv_resid': row.rsv_resid,
-                   'rsv_category': row.rsv_category, 'rsv_state': row.rsv_state,
-                   'rsv_pending': row.rsv_pending, 'rsv_joining': row.rsv_joining,
-                   'properties': row.properties, 'rsv_graph_node_id': row.rsv_graph_node_id}
-
-        return rsv_obj
-
     def create_reservation_filter(self, *, slice_id: str = None, graph_node_id: str = None, project_id: str = None,
-                                  email: str = None, oidc_sub: str = None, rid: str = None, site: str = None,
-                                  rsv_type: str = None) -> dict:
+                                  email: str = None, oidc_sub: str = None, rid: str = None, site: str = None) -> dict:
 
         filter_dict = {}
         if slice_id is not None:
             slc_id = self.get_slc_id_by_slice_id(slice_id=slice_id)
             filter_dict['rsv_slc_id'] = slc_id
         if graph_node_id is not None:
             filter_dict['rsv_graph_node_id'] = graph_node_id
@@ -730,21 +714,19 @@
             filter_dict['email'] = email
         if oidc_sub is not None:
             filter_dict['oidc_claim_sub'] = oidc_sub
         if rid is not None:
             filter_dict['rsv_resid'] = rid
         if site is not None:
             filter_dict['site'] = site
-        if rsv_type is not None:
-            filter_dict['rsv_type'] = rsv_type
         return filter_dict
 
     def get_reservations(self, *, slice_id: str = None, graph_node_id: str = None, project_id: str = None,
                          email: str = None, oidc_sub: str = None, rid: str = None, states: list[int] = None,
-                         category: list[int] = None, site: str = None, rsv_type: str = None) -> list:
+                         category: list[int] = None, site: str = None, rsv_type: list[str] = None) -> List[dict]:
         """
         Get Reservations for an actor
         @param slice_id slice id
         @param graph_node_id graph node id
         @param project_id project id
         @param email email
         @param oidc_sub oidc sub
@@ -753,318 +735,289 @@
         @param category reservation category
         @param site site name
         @param rsv_type rsv_type
 
         @return list of reservations
         """
         result = []
+        session = self.get_session()
         try:
             filter_dict = self.create_reservation_filter(slice_id=slice_id, graph_node_id=graph_node_id,
                                                          project_id=project_id, email=email, oidc_sub=oidc_sub,
-                                                         rid=rid, site=site, rsv_type=rsv_type)
-            with session_scope(self.db_engine) as session:
-                rows = session.query(Reservations).filter_by(**filter_dict)
-
-                if states is not None:
-                    rows = rows.filter(Reservations.rsv_state.in_(states))
-
-                if category is not None:
-                    rows = rows.filter(Reservations.rsv_category.in_(category))
-
-                for row in rows.all():
-                    rsv_obj = self.generate_reservation_dict_from_row(row)
-                    result.append(rsv_obj.copy())
-                    rsv_obj.clear()
+                                                         rid=rid, site=site)
+            rows = session.query(Reservations).filter_by(**filter_dict)
+
+            if rsv_type is not None:
+                rows = rows.filter(Reservations.rsv_type.in_(rsv_type))
+
+            if states is not None:
+                rows = rows.filter(Reservations.rsv_state.in_(states))
+
+            if category is not None:
+                rows = rows.filter(Reservations.rsv_category.in_(category))
+
+            for row in rows.all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_reservations_by_rids(self, *, rsv_resid_list: list) -> list:
         """
         Get Reservations for an actor by reservation ids
         @param act_id actor id
         @param rsv_resid_list reservation guid list
         @return list of reservations
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Reservations).filter(Reservations.rsv_resid.in_(rsv_resid_list)).all():
-                    rsv_obj = self.generate_reservation_dict_from_row(row)
-                    result.append(rsv_obj.copy())
-                    rsv_obj.clear()
+            for row in session.query(Reservations).filter(Reservations.rsv_resid.in_(rsv_resid_list)).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_proxy(self, *, act_id: int, prx_name: str, properties):
         """
         Add a proxy
         @param act_id actor id
         @param prx_name proxy name
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
             prx_obj = Proxies(prx_act_id=act_id, prx_name=prx_name, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(prx_obj)
+            session.add(prx_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_proxy(self, *, act_id: int, prx_name: str, properties):
         """
         Update a proxy
         @param act_id actor id
         @param prx_name proxy name
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                prx_obj = session.query(Proxies).filter(Proxies.prx_act_id == act_id).filter(
-                    Proxies.prx_name == prx_name).first()
-                if prx_obj is not None:
-                    prx_obj.properties = properties
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Proxy", prx_name))
+            prx_obj = session.query(Proxies).filter_by(prx_act_id=act_id).filter(
+                Proxies.prx_name == prx_name).one_or_none()
+            if prx_obj is not None:
+                prx_obj.properties = properties
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Proxy", prx_name))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_proxy(self, *, act_id: int, prx_name: str):
         """
         Remove a proxy
         @param act_id actor id
         @param prx_name proxy name
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Proxies).filter(Proxies.prx_act_id == act_id).filter(
-                    Proxies.prx_name == prx_name).delete()
+            session.query(Proxies).filter(Proxies.prx_act_id == act_id).filter(Proxies.prx_name == prx_name).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_proxy_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a proxy row read from database
-        """
-        if row is None:
-            return None
-
-        prx_obj = {'prx_id': row.prx_id, 'prx_act_id': row.prx_act_id, 'prx_name': row.prx_name,
-                   'properties': row.properties}
-
-        return prx_obj
-
     def get_proxies(self, *, act_id: int) -> list:
         """
         Get Proxies
         @param act_id actor id
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Proxies).filter(Proxies.prx_act_id == act_id).all():
-                    prx_obj = self.generate_proxy_dict_from_row(row)
-                    result.append(prx_obj.copy())
-                    prx_obj.clear()
+            for row in session.query(Proxies).filter_by(prx_act_id=act_id).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_config_mapping(self, *, act_id: int, cfgm_type: str, properties):
         """
         Add handlers mapping
         @param act_id actor id
         @param cfgm_type type
         @param properties properties
         """
+        session = self.get_session()
         try:
             cfg_obj = ConfigMappings(cfgm_act_id=act_id, cfgm_type=cfgm_type, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(cfg_obj)
+            session.add(cfg_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_config_mapping(self, *, act_id: int, cfgm_type: str, properties):
         """
         Update handlers mapping
         @param act_id actor id
         @param cfgm_type type
         @param properties properties
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                cfg_obj = session.query(ConfigMappings).filter(ConfigMappings.cfgm_act_id == act_id).filter(
-                    ConfigMappings.cfgm_type == cfgm_type).first()
-                if cfg_obj is not None:
-                    cfg_obj.properties = properties
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Config Mapping", cfgm_type))
+            cfg_obj = session.query(ConfigMappings).filter(ConfigMappings.cfgm_act_id == act_id).filter(
+                ConfigMappings.cfgm_type == cfgm_type).one_or_none()
+            if cfg_obj is not None:
+                cfg_obj.properties = properties
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Config Mapping", cfgm_type))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_config_mapping(self, *, cfgm_type: str):
         """
         Remove handlers mapping
         @param cfgm_type handlers mapping type
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(ConfigMappings).filter(ConfigMappings.cfgm_type == cfgm_type).delete()
+            session.query(ConfigMappings).filter_by(cfgm_type=cfgm_type).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_config_mapping_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a handlers mapping row read from database
-        """
-        if row is None:
-            return None
-
-        cfg_obj = {'cfgm_id': row.cfgm_id, 'cfgm_act_id': row.cfgm_act_id, 'cfgm_type': row.cfgm_type,
-                   'properties': row.properties}
-
-        return cfg_obj
-
     def get_config_mappings(self, *, act_id: int) -> list:
         """
         Get Config Mappings
         @param act_id actor id
         @retur list of mappings
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(ConfigMappings).filter(ConfigMappings.cfgm_act_id == act_id).all():
-                    cfg_obj = self.generate_config_mapping_dict_from_row(row)
-                    result.append(cfg_obj.copy())
-                    cfg_obj.clear()
+            for row in session.query(ConfigMappings).filter_by(cfgm_act_id=act_id).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_client(self, *, act_id: int, clt_name: str, clt_guid: str, properties):
         """
         Add a client
         @param act_id actor id
         @param clt_name client name
         @param clt_guid client guid
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
             clt_obj = Clients(clt_act_id=act_id, clt_name=clt_name, clt_guid=clt_guid, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(clt_obj)
+            session.add(clt_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_client(self, *, act_id: int, clt_name: str, properties):
         """
         Update a client
         @param act_id actor id
         @param clt_name client name
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                clt_obj = session.query(Clients).filter(Clients.clt_act_id == act_id).filter(
-                    Clients.clt_name == clt_name).first()
-                if clt_obj is not None:
-                    clt_obj.properties = properties
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Client", clt_name))
+            clt_obj = session.query(Clients).filter(Clients.clt_act_id == act_id).filter(
+                Clients.clt_name == clt_name).one_or_none()
+            if clt_obj is not None:
+                clt_obj.properties = properties
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Client", clt_name))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_client_by_name(self, *, act_id: int, clt_name: str):
         """
         Remove a client by name
         @param act_id actor id
         @param clt_name client name
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Clients).filter(Clients.clt_act_id == act_id).filter(
-                    Clients.clt_name == clt_name).delete()
+            session.query(Clients).filter(Clients.clt_act_id == act_id).filter(Clients.clt_name == clt_name).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_client_by_guid(self, *, act_id: int, clt_guid: str):
         """
         Remove client by guid
         @param act_id actor id
         @param clt_guid client guid
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Clients).filter(Clients.clt_act_id == act_id).filter(
-                    Clients.clt_guid == clt_guid).delete()
+            session.query(Clients).filter(Clients.clt_act_id == act_id).filter(Clients.clt_guid == clt_guid).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_client_dict_from_row(clt_obj) -> dict or None:
-        """
-        Generate dictionary representing a client row read from database
-        """
-        if clt_obj is None:
-            return None
-
-        result = {'clt_id': clt_obj.clt_id, 'clt_act_id': clt_obj.clt_act_id, 'clt_name': clt_obj.clt_name,
-                  'clt_guid': clt_obj.clt_guid, 'properties': clt_obj.properties}
-
-        return result
-
     def get_client_by_guid(self, *, clt_guid: str) -> dict:
         """
         Get Client by name
         @param act_id actor id
         @param clt_guid client guid
         @return client
         """
         result = None
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                clt_obj = session.query(Clients).filter(Clients.clt_guid == clt_guid).first()
-                if clt_obj is None:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Client", clt_guid))
-                result = self.generate_client_dict_from_row(clt_obj)
+            clt_obj = session.query(Clients).filter_by(clt_guid=clt_guid).one_or_none()
+            if clt_obj is None:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Client", clt_guid))
+            result = self.generate_dict_from_row(clt_obj)
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_clients(self) -> list:
         """
         Get Clients
         @param act_id actor id
         @return client list
         """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Clients).all():
-                    clt_obj = self.generate_client_dict_from_row(row)
-                    result.append(clt_obj.copy())
-                    clt_obj.clear()
+            for row in session.query(Clients).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_unit(self, *, slc_guid: str, rsv_resid: str, unt_uid: str, unt_unt_id: int,
                  unt_state: int, properties):
@@ -1074,332 +1027,311 @@
         @param slc_guid slice guid
         @param rsv_resid reservation id
         @param unt_uid unit id
         @param unt_unt_id parent unit id
         @param unt_state unit state
         @param properties properties
         """
+        session = self.get_session()
         try:
             slc_id = self.get_slc_id_by_slice_id(slice_id=slc_guid)
             rsv_id = self.get_rsv_id_by_reservation_id(reservation_id=rsv_resid)
 
             unt_obj = Units(unt_uid=unt_uid,
                             unt_slc_id=slc_id,
                             unt_rsv_id=rsv_id,
                             unt_state=unt_state, properties=properties)
             if unt_unt_id is not None:
                 unt_obj.unt_unt_id = unt_unt_id
-            with session_scope(self.db_engine) as session:
-                session.add(unt_obj)
+            session.add(unt_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_unit_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a unit row read from database
-        """
-        if row is None:
-            return None
-
-        result = {'unt_id': row.unt_id, 'unt_uid': row.unt_uid, 'unt_unt_id': row.unt_unt_id,
-                  'unt_slc_id': row.unt_slc_id, 'unt_rsv_id': row.unt_rsv_id, 'unt_state': row.unt_state,
-                  'properties': row.properties}
-
-        return result
-
     def get_unit(self, *, unt_uid: str) -> dict or None:
         """
         Get Unit
         @param act_id actor id
         @param unt_uid unit guid
         @return Unit dict
         """
         result = None
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                unt_obj = session.query(Units).filter(Units.unt_uid == unt_uid).first()
-                if unt_obj is None:
-                    self.logger.error("Unit with guid {} not found".format(unt_uid))
-                    return result
-                result = self.generate_unit_dict_from_row(unt_obj)
+            unt_obj = session.query(Units).filter_by(unt_uid=unt_uid).one_or_none()
+            if unt_obj is None:
+                self.logger.debug("Unit with guid {} not found".format(unt_uid))
+                return result
+            result = self.generate_dict_from_row(unt_obj)
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_units(self, *, rsv_resid: str):
         """
         Get Units
         @param act_id actor id
         @param rsv_resid reservation guid
         @return Unit list
         """
         result = []
+        session = self.get_session()
         try:
             rsv_obj = self.get_reservations(rid=rsv_resid)[0]
             if rsv_obj is None:
                 raise DatabaseException(self.OBJECT_NOT_FOUND.format("Reservation", rsv_resid))
 
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Units).filter(Units.unt_rsv_id == rsv_obj['rsv_id']).all():
-                    unt_obj = self.generate_unit_dict_from_row(row)
-                    result.append(unt_obj.copy())
-                    unt_obj.clear()
+            for row in session.query(Units).filter_by(unt_rsv_id=rsv_obj['rsv_id']).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def remove_unit(self, *, unt_uid: str):
         """
         Remove a unit
         @param unt_uid unit id
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Units).filter(Units.unt_uid == unt_uid).delete()
+            session.query(Units).filter_by(unt_uid=unt_uid).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_unit(self, *, unt_uid: str, properties):
         """
         Add Unit
         @param unt_uid unit id
         @param properties properties
         """
         result = None
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                unt_obj = session.query(Units).filter(Units.unt_uid == unt_uid).first()
-                if unt_obj is None:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Unit", unt_uid))
-                unt_obj.properties = properties
+            unt_obj = session.query(Units).filter_by(unt_uid=unt_uid).one_or_none()
+            if unt_obj is None:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Unit", unt_uid))
+            unt_obj.properties = properties
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_delegation(self, *, slice_id: str, dlg_graph_id: str, dlg_state: int, properties, site: str = None):
         """
         Add delegation
         @param slice_id slice id
         @param dlg_graph_id graph id
         @param dlg_state state
         @param properties properties
         @param site site
         """
+        session = self.get_session()
         try:
             slc_id = self.get_slc_id_by_slice_id(slice_id=slice_id)
             dlg_obj = Delegations(dlg_slc_id=slc_id, dlg_graph_id=dlg_graph_id,
                                   dlg_state=dlg_state, properties=properties, site=site)
-            with session_scope(self.db_engine) as session:
-                session.add(dlg_obj)
+            session.add(dlg_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_delegation(self, *, dlg_graph_id: str, dlg_state: int, properties, site: str = None):
         """
         Update delegation
         @param dlg_graph_id graph id
         @param dlg_state state
         @param properties properties
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                dlg_obj = session.query(Delegations).filter(Delegations.dlg_graph_id == dlg_graph_id).first()
-                if dlg_obj is not None:
-                    dlg_obj.dlg_state = dlg_state
-                    dlg_obj.properties = properties
-                    if site is not None:
-                        dlg_obj.site = site
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Delegation", dlg_graph_id))
+            dlg_obj = session.query(Delegations).filter_by(dlg_graph_id=dlg_graph_id).one_or_none()
+            if dlg_obj is not None:
+                dlg_obj.dlg_state = dlg_state
+                dlg_obj.properties = properties
+                if site is not None:
+                    dlg_obj.site = site
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Delegation", dlg_graph_id))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_delegation(self, *, dlg_graph_id: str):
         """
         Remove delegation
         @param dlg_graph_id graph id
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Delegations).filter(Delegations.dlg_graph_id == dlg_graph_id).delete()
+            session.query(Delegations).filter_by(dlg_graph_id=dlg_graph_id).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_delegation_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a delegation row read from database
-        """
-        if row is None:
-            return None
-
-        dlg_obj = {'dlg_id': row.dlg_id, 'dlg_slc_id': row.dlg_slc_id,
-                   'dlg_graph_id':row.dlg_graph_id, 'dlg_state': row.dlg_state, 'properties': row.properties}
-
-        return dlg_obj
-
     def get_slc_id_by_slice_id(self, *, slice_id: str) -> int:
         slices = self.get_slices(slice_id=slice_id)
         if slices is None or len(slices) == 0:
             raise DatabaseException(self.OBJECT_NOT_FOUND.format("Slice", slice_id))
         return slices[0]['slc_id']
 
     def get_rsv_id_by_reservation_id(self, *, reservation_id: str) -> int:
         reservations = self.get_reservations(rid=reservation_id)
         if reservations is None or len(reservations) == 0:
             raise DatabaseException(self.OBJECT_NOT_FOUND.format("Reservation", reservation_id))
         return reservations[0]['rsv_id']
 
-    def get_delegations(self, *, slc_guid: str = None, states: List[int] = None) -> list:
+    def get_delegations(self, *, slc_guid: str = None, states: List[int] = None) -> List[dict]:
         """
         Get delegations
         @param slc_guid slice guid
         @param states delegation state
         @param list of delegations
         """
         result = []
+        session = self.get_session()
         try:
             slc_id = self.get_slc_id_by_slice_id(slice_id=slc_guid)
-            with session_scope(self.db_engine) as session:
-                rows = session.query(Delegations)
-                if slc_guid is not None:
-                    rows = rows.filter(Delegations.dlg_slc_id == slc_id)
-                if states is not None:
-                    rows = rows.filter(Delegations.dlg_state.in_(states))
-                for row in rows.all():
-                    dlg_obj = self.generate_delegation_dict_from_row(row)
-                    result.append(dlg_obj.copy())
-                    dlg_obj.clear()
+            rows = session.query(Delegations)
+            if slc_guid is not None:
+                rows = rows.filter(Delegations.dlg_slc_id == slc_id)
+            if states is not None:
+                rows = rows.filter(Delegations.dlg_state.in_(states))
+            for row in rows.all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_delegation(self, *, dlg_graph_id: str) -> dict:
         """
         Get delegation
         @param dlg_graph_id delegation graph id
         @return delegation
         """
         result = {}
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                dlg_obj = session.query(Delegations).filter(Delegations.dlg_graph_id == dlg_graph_id).first()
-                if dlg_obj is not None:
-                    result = self.generate_delegation_dict_from_row(dlg_obj)
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Delegation", dlg_graph_id))
+            dlg_obj = session.query(Delegations).filter_by(dlg_graph_id=dlg_graph_id).one_or_none()
+            if dlg_obj is not None:
+                result = self.generate_dict_from_row(dlg_obj)
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Delegation", dlg_graph_id))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def add_site(self, *, site_name: str, state: int, properties):
         """
         Add a site
         @param site_name Site Name
         @param state state
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
             site_obj = Sites(name=site_name, state=state, properties=properties)
-            with session_scope(self.db_engine) as session:
-                session.add(site_obj)
+            session.add(site_obj)
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def update_site(self, *, site_name: str, state: int, properties):
         """
         Update a site
         @param site_name Site Name
         @param state state
         @param properties pickled instance
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                site_obj = session.query(Sites).filter(Sites.name == site_name).first()
-                if site_obj is not None:
-                    site_obj.properties = properties
-                    site_obj.state = state
-                else:
-                    raise DatabaseException(self.OBJECT_NOT_FOUND.format("Sites", site_name))
+            site_obj = session.query(Sites).filter_by(name=site_name).one_or_none()
+            if site_obj is not None:
+                site_obj.properties = properties
+                site_obj.state = state
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Sites", site_name))
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def remove_site(self, *, site_name: str):
         """
         Remove a proxy
         @param site_name site_name
         """
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                session.query(Sites).filter(Sites.name == site_name).delete()
+            session.query(Sites).filter_by(name=site_name).delete()
+            session.commit()
         except Exception as e:
+            session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
-    @staticmethod
-    def generate_site_dict_from_row(row) -> dict:
-        """
-        Generate dictionary representing a site row read from database
-        """
-        if row is None:
-            return None
-
-        site_obj = {'name': row.name, 'properties': row.properties}
-
-        return site_obj
-
     def get_sites(self) -> list:
         """
         Get Sites
 =        """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Sites).all():
-                    site_obj = self.generate_site_dict_from_row(row)
-                    result.append(site_obj.copy())
-                    site_obj.clear()
+            for row in session.query(Sites).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
     def get_site(self, *, site_name: str) -> list:
         """
         Get Sites
 =        """
         result = []
+        session = self.get_session()
         try:
-            with session_scope(self.db_engine) as session:
-                for row in session.query(Sites).filter(Sites.name == site_name).all():
-                    site_obj = self.generate_site_dict_from_row(row)
-                    result.append(site_obj.copy())
-                    site_obj.clear()
+            for row in session.query(Sites).filter_by(name=site_name).all():
+                result.append(self.generate_dict_from_row(row=row))
         except Exception as e:
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
         return result
 
+    @staticmethod
+    def generate_dict_from_row(row):
+        d = row.__dict__.copy()
+        for k in row.__dict__:
+            if d[k] is None:
+                d.pop(k)
+        return d
+
 
 def test():
     logger = logging.getLogger('PsqlDatabase')
-    db = PsqlDatabase(user='fabric', password='fabric', database='am', db_host='127.0.0.1:8432', logger=logger)
+    db = PsqlDatabase(user='fabric', password='fabric', database='am', db_host='127.0.0.1:5432', logger=logger)
     db.create_db()
     db.reset_db()
 
     # Actor Operations
     prop = {'abc':'def'}
 
     db.add_actor(name="test-actor1", guid="12345", act_type=1, properties=pickle.dumps(prop))
@@ -1456,15 +1388,15 @@
     db.add_reservation(slc_guid="1234", rsv_resid="rsv_567", rsv_category=1, rsv_state=2,
                        rsv_pending=3, rsv_joining=4, properties=pickle.dumps(prop))
     print("Reservations after add {}".format(db.get_reservations()))
     prop['update'] = 'test'
     db.update_reservation(slc_guid="1234", rsv_resid="rsv_567", rsv_category=1, rsv_state=2,
                           rsv_pending=3, rsv_joining=5, properties=pickle.dumps(prop))
     print("Reservations after update {}".format(db.get_reservations()))
-    print("Reservations after by state {}".format(db.get_reservations(slice_id="1234", state=[2])))
+    print("Reservations after by state {}".format(db.get_reservations(slice_id="1234", states=[2])))
 
     print("Reservations after by rid {}".format(db.get_reservations(rid="rsv_567")))
     print("Reservations after by rid list {}".format(db.get_reservations_by_rids(rsv_resid_list=["rsv_567"])))
 
     db.remove_reservation(rsv_resid="rsv_567")
     print("Reservations after delete {}".format(db.get_reservations()))
 
@@ -1474,18 +1406,18 @@
     prop['prx-update'] = 'fly'
     db.update_proxy(act_id=actor_id, prx_name="prx-123", properties=pickle.dumps(prop))
     print("Proxies after update {}".format(db.get_proxies(act_id=actor_id)))
     db.remove_proxy(act_id=actor_id, prx_name="prx-123")
     print("Proxies after remove {}".format(db.get_proxies(act_id=actor_id)))
 
     # Config Mapping operations
-    db.add_config_mapping(act_id=actor_id, cfgm_type="cfg-1", properties=prop)
+    db.add_config_mapping(act_id=actor_id, cfgm_type="cfg-1", properties=pickle.dumps(prop))
     print("Config Mappings after add {}".format(db.get_config_mappings(act_id=actor_id)))
     prop['cfg-update'] = 'done'
-    db.update_config_mapping(act_id=actor_id, cfgm_type="cfg-1", properties=prop)
+    db.update_config_mapping(act_id=actor_id, cfgm_type="cfg-1", properties=pickle.dumps(prop))
     db.remove_config_mapping(cfgm_type="cfg-1")
     print("Config Mappings after remove {}".format(db.get_config_mappings(act_id=actor_id)))
 
     # Client operations
     db.add_client(act_id=actor_id, clt_name="clt-test", clt_guid="clt-1234", properties=pickle.dumps(prop))
     print("Clients after add {}".format(db.get_clients()))
     print("Clients after by guid {}".format(db.get_client_by_guid(clt_guid="clt-1234")))
@@ -1510,21 +1442,21 @@
     db.remove_reservation(rsv_resid="rsv_567")
     db.reset_db()
     print("Get all actors after reset {}".format(db.get_actors()))
 
 
 def test2():
     logger = logging.getLogger('PsqlDatabase')
-    db = PsqlDatabase(user='fabric', password='fabric', database='broker', db_host='152.54.15.56:5432', logger=logger)
+    db = PsqlDatabase(user='fabric', password='fabric', database='broker', db_host='127.0.0.1:5432', logger=logger)
     from fabric_cf.actor.core.kernel.reservation_states import ReservationStates
     states = [ReservationStates.Active.value,
               ReservationStates.ActiveTicketed.value,
               ReservationStates.Ticketed.value,
               ReservationStates.Nascent.value]
-    res = db.get_reservations(graph_node_id='node+renc-data-sw:ip+192.168.11.3-ns', state=states)
+    res = db.get_reservations(graph_node_id='node+renc-data-sw:ip+192.168.11.3-ns', states=states)
     print(f"All {len(res)}")
     for r in res:
         print(r['rsv_state'])
     print("Get all actors after reset {}".format(db.get_actors()))
 
 def test3():
     logger = logging.getLogger('PsqlDatabase')
@@ -1553,27 +1485,27 @@
                  properties=pickle.dumps(prop), lease_start=datetime.now(timezone.utc), lease_end=datetime.now(timezone.utc),
                  slc_state=SliceState.StableError.value, email="kthare10@email.unc.edu")
 
     db.add_slice(slc_guid="1234", slc_name="test-slice3", slc_type=1, slc_resource_type="def",
                  properties=pickle.dumps(prop), lease_start=datetime.now(timezone.utc), lease_end=datetime.now(timezone.utc),
                  slc_state=SliceState.Configuring.value, email="kthare10@email.unc.edu")
 
-    ss = db.get_slices(state=[SliceState.Dead.value, SliceState.Closing.value],
+    ss = db.get_slices(states=[SliceState.Dead.value, SliceState.Closing.value],
                        email="kthare10@email.unc.edu")
 
     assert len(ss) == 2
 
-    ss = db.get_slices(state=[SliceState.StableOK.value, SliceState.StableError.value],
+    ss = db.get_slices(states=[SliceState.StableOK.value, SliceState.StableError.value],
                        email="kthare10@email.unc.edu")
 
     assert len(ss) == 2
 
-    ss = db.get_slices(state=[SliceState.Configuring.value],
+    ss = db.get_slices(states=[SliceState.Configuring.value],
                        email="kthare10@email.unc.edu")
 
     assert len(ss) == 1
 
 
 if __name__ == '__main__':
     test2()
-    test()
-    test3()
+    #test()
+    #test3()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/fim/asm_update_thread.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/fim/asm_update_thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -144,16 +144,18 @@
         return events
 
     def __process_events(self, *, events: list):
         for event in events:
             try:
                 begin = time.time()
                 event.process()
-                self.logger.info(f"Event {event.__class__.__name__} "
-                                 f"TIME: {time.time() - begin:.0f}")
+                diff = int(time.time() - begin)
+                if diff > 0:
+                    self.logger.info(f"Event {event.__class__.__name__} "
+                                     f"TIME: {time.time() - begin:.0f}")
             except Exception as e:
                 self.logger.error(f"Error while processing event {type(event)}, {e}")
                 self.logger.error(traceback.format_exc())
 
     def __run(self):
         self.logger.info(f"Thread {self.name} started")
         while True:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/fim/fim_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/fim/fim_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import logging
 import random
+import traceback
 from typing import Tuple, List, Union
 
 from fim.graph.abc_property_graph import ABCPropertyGraph, ABCGraphImporter
 from fim.graph.neo4j_property_graph import Neo4jGraphImporter, Neo4jPropertyGraph
 from fim.graph.networkx_property_graph import NetworkXGraphImporter
 from fim.graph.resources.abc_arm import ABCARMPropertyGraph
 from fim.graph.resources.abc_cbm import ABCCBMPropertyGraph
@@ -331,31 +332,30 @@
                 diff = graph_sliver.diff(other_sliver=sliver)
                 if diff is not None:
                     for cname in diff.removed.components:
                         reservation_info = ReservationInfo()
                         reservation_info.reservation_state = ReservationStates.Failed.name
                         node.components[cname].set_properties(reservation_info=reservation_info)
 
+                topo_component_dict = node.components
                 for component in sliver.attached_components_info.devices.values():
-                    cname = component.get_name()
-                    node.components[cname].set_properties(
-                                                          labels=component.labels,
-                                                          label_allocations=component.label_allocations,
-                                                          capacity_allocations=component.capacity_allocations,
-                                                          node_map=component.node_map)
+                    topo_component = topo_component_dict[component.get_name()]
+                    topo_component.set_properties(labels=component.labels,
+                                                  label_allocations=component.label_allocations,
+                                                  capacity_allocations=component.capacity_allocations,
+                                                  node_map=component.node_map)
                     # Update Mac address
                     if component.network_service_info is not None and \
                             component.network_service_info.network_services is not None:
+                        topo_ifs_dict = topo_component.interfaces
                         for ns in component.network_service_info.network_services.values():
                             if ns.interface_info is None or ns.interface_info.interfaces is None:
                                 continue
-
                             for ifs in ns.interface_info.interfaces.values():
-                                topo_component = node.components[cname]
-                                topo_ifs = topo_component.interfaces[ifs.get_name()]
+                                topo_ifs = topo_ifs_dict[ifs.get_name()]
                                 topo_ifs.set_properties(labels=ifs.labels,
                                                         label_allocations=ifs.label_allocations,
                                                         node_map=ifs.node_map)
                                 if ifs.peer_labels is not None:
                                     topo_ifs.set_properties(peer_labels=ifs.peer_labels)
 
                                 if ifs.capacities is not None:
@@ -366,18 +366,19 @@
             node.set_properties(labels=sliver.labels,
                                 label_allocations=sliver.label_allocations,
                                 capacity_allocations=sliver.capacity_allocations,
                                 reservation_info=sliver.reservation_info,
                                 node_map=sliver.node_map,
                                 gateway=sliver.gateway)
             if sliver.interface_info is not None:
+                topo_ifs_dict = node.interfaces
                 for ifs in sliver.interface_info.interfaces.values():
                     if ifs.get_name() not in node.interfaces:
                         continue
-                    topo_ifs = node.interfaces[ifs.get_name()]
+                    topo_ifs = topo_ifs_dict[ifs.get_name()]
                     topo_ifs.set_properties(labels=ifs.labels,
                                             label_allocations=ifs.label_allocations,
                                             node_map=ifs.node_map)
 
                     if ifs.peer_labels is not None:
                         topo_ifs.set_properties(peer_labels=ifs.peer_labels)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/handlers/handler_base.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/handlers/handler_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/handlers/no_op_handler.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/handlers/no_op_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/security/access_checker.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/security/access_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/security/auth_token.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/security/auth_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/security/fabric_token.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/security/fabric_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         @raise Exception in case of error
         """
         try:
             # validate the token
             verify_exp = self.oauth_config.get(Constants.PROPERTY_CONF_O_AUTH_VERIFY_EXP, True)
 
             if self.jwt_validator is not None:
-                self.logger.info("Validating CI Logon token")
+                self.logger.debug("Validating CI Logon token")
                 code, token_or_exception = self.jwt_validator.validate_jwt(token=self.encoded_token,
                                                                            verify_exp=verify_exp)
                 if code is not ValidateCode.VALID:
                     self.logger.error(f"Unable to validate provided token: {code}/{token_or_exception}")
                     raise TokenException(f"Unable to validate provided token: {code}/{token_or_exception}")
             else:
                 raise TokenException("JWT Token validator not initialized, skipping validation")
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/security/pdp_auth.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/security/pdp_auth.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/base_test_case.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/base_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import logging
 
+from fabric_cf.actor.boot.configuration import Configuration
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin, ActorType
 from fabric_cf.actor.core.apis.abc_authority import ABCAuthority
 from fabric_cf.actor.core.apis.abc_authority_policy import ABCAuthorityPolicy
 from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
 from fabric_cf.actor.core.apis.abc_broker_mixin import ABCBrokerMixin
 from fabric_cf.actor.core.apis.abc_broker_policy_mixin import ABCBrokerPolicyMixin
 from fabric_cf.actor.core.apis.abc_container_database import ABCContainerDatabase
@@ -60,23 +61,27 @@
     controller_guid = "test-orchestrator-guid"
     authority_guid = "test-authority-guid"
     broker_guid = "test-broker-guid"
 
     db_user = 'fabric'
     db_pwd = 'fabric'
     db_name = 'test'
-    db_host = '152.54.15.56:5432'
+    db_host = 'localhost:5432'
 
     logger = logging.getLogger('BaseTestCase')
     log_format = '%(asctime)s - %(name)s - {%(filename)s:%(lineno)d} - [%(threadName)s] - %(levelname)s - %(message)s'
     logging.basicConfig(format=log_format, filename="./actor.log")
     logger.setLevel(logging.INFO)
 
     Term.set_cycles = False
 
+    def get_config(self) -> Configuration:
+        from fabric_cf.actor.core.container.globals import GlobalsSingleton
+        return GlobalsSingleton.get().get_config()
+
     def get_container_database(self) -> ABCContainerDatabase:
         from fabric_cf.actor.core.container.globals import GlobalsSingleton
         return GlobalsSingleton.get().get_container().get_database()
 
     def get_actor_clock(self) -> ActorClock:
         from fabric_cf.actor.core.container.globals import GlobalsSingleton
         return GlobalsSingleton.get().get_container().get_actor_clock()
@@ -214,42 +219,42 @@
         actor.set_actor_clock(clock=self.get_actor_clock())
         actor.set_policy(policy=self.get_authority_policy())
         actor.set_plugin(plugin=self.get_plugin(name=name))
         return actor
 
     def get_actor(self, *, name: str = actor_name, guid: ID = actor_guid) -> ABCActorMixin:
         actor = self.get_uninitialized_actor(name=name, guid=guid)
-        actor.initialize(config=None)
+        actor.initialize(config=self.get_config().get_actor_config())
         self.register_new_actor(actor=actor)
         return actor
 
     def get_controller(self, *, name: str = controller_name, guid: ID = controller_guid) -> ABCController:
         actor = self.get_uninitialized_controller(name=name, guid=guid)
-        actor.initialize(config=None)
+        actor.initialize(config=self.get_config().get_actor_config())
         self.register_new_actor(actor=actor)
         return actor
 
     def get_broker(self, *, name: str = broker_name, guid: ID = broker_guid) -> ABCBrokerMixin:
         actor = self.get_uninitialized_broker(name=name, guid=guid)
-        actor.initialize(config=None)
+        actor.initialize(config=self.get_config().get_actor_config())
         self.register_new_actor(actor=actor)
         return actor
 
     def get_authority(self, *, name: str = authority_name, guid: ID = authority_guid) -> ABCAuthority:
         actor = self.get_uninitialized_authority(name=name, guid=guid)
-        actor.initialize(config=None)
+        actor.initialize(config=self.get_config().get_actor_config())
         self.register_new_actor(actor=actor)
         return actor
 
     def register_new_actor(self, *, actor: ABCActorMixin):
         db = self.get_container_database()
         db.remove_actor(actor_name=actor.get_name())
         db.add_actor(actor=actor)
         ActorRegistrySingleton.get().unregister(actor=actor)
         ActorRegistrySingleton.get().register_actor(actor=actor)
-        actor.actor_added(config=None)
+        actor.actor_added(config=self.get_config().get_actor_config())
         actor.start()
 
     def get_registered_new_actor(self) -> ABCActorMixin:
         actor = self.get_actor()
         self.register_new_actor(actor=actor)
         return actor
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/client_callback_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/client_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.jenkins.yaml` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.jenkins.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server: localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: ./schema/key.avsc
   kafka-value-schema: ./schema/message.avsc
   kafka-ssl-ca-location:  ../../../secrets/snakeoil-ca-1.crt
   kafka-ssl-certificate-location:  ../../../secrets/kafkacat1-ca1-signed.pem
   kafka-ssl-key-location:  ../../../secrets/kafkacat1.client.key
   kafka-ssl-key-password:  fabric
-  kafka-security-protocol: SSL
+  kafka-security-protocol: PLAINTEXT
   kafka-group-id: fabric-cf
   kafka-sasl-mechanism:
   kafka-sasl-producer-username:
   kafka-sasl-producer-password:
   kafka-sasl-consumer-username:
   kafka-sasl-consumer-password:
   prometheus.port: 11000
@@ -71,15 +71,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: test
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: site1-am-conainer
 
 time:
   # This section controls settings, which are generally useful
   # when running under emulation. These settings allow you to
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.orchestrator.yaml` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.orchestrator.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: 152.54.15.56:29092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://152.54.15.56:8081
   kafka-key-schema: ./schema/key.avsc
   kafka-value-schema: ./schema/message.avsc
   kafka-ssl-ca-location:  ../../../secrets/snakeoil-ca-1.crt
   kafka-ssl-certificate-location:  ../../../secrets/kafkacat1-ca1-signed.pem
   kafka-ssl-key-location:  ../../../secrets/kafkacat1.client.key
   kafka-ssl-key-password:  fabric
-  kafka-security-protocol: SSL
+  kafka-security-protocol: PLAINTEXT
   kafka-group-id: fabric-cf
   kafka-sasl-mechanism:
   kafka-sasl-producer-username:
   kafka-sasl-producer-password:
   kafka-sasl-consumer-username:
   kafka-sasl-consumer-password:
   prometheus.port: 11000
@@ -71,15 +71,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: test
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: orchestrator-conainer
 
 bqm:
   # in seconds (default set to 300 seconds)
   refresh-interval: 300
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/config/config.test.yaml` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server:  localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: ../../schema/key.avsc
   kafka-value-schema: ../../schema/message.avsc
   kafka-ssl-ca-location:  ../../../../../secrets/snakeoil-ca-1.crt
   kafka-ssl-certificate-location:  ../../../../../secrets/kafkacat1-ca1-signed.pem
   kafka-ssl-key-location:  ../../../../../secrets/kafkacat1.client.key
   kafka-ssl-key-password:  fabric
-  kafka-security-protocol: SSL
+  kafka-security-protocol: PLAINTEXT
   kafka-group-id: fabric-cf
   kafka-sasl-mechanism:
   kafka-sasl-producer-username:
   kafka-sasl-producer-password:
   kafka-sasl-consumer-username:
   kafka-sasl-consumer-password:
   prometheus.port: 11000
@@ -71,15 +71,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: test
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: site1-am-conainer
 
 time:
   # This section controls settings, which are generally useful
   # when running under emulation. These settings allow you to
@@ -112,15 +112,15 @@
 
 actor:
   type: authority
   name: site1-am
   guid: site1-am-guid
   description: Site AM
   kafka-topic: site1-am-topic
-  substrate.file: ../../neo4j/RENCI-ad.graphml
+  substrate.file: ../../../neo4j/RENCI-ad.graphml
   policy:
       module: fabric_cf.actor.core.policy.authority_calendar_policy
       class: AuthorityCalendarPolicy
   resources:
       - resource:
             type: VM
             label: VM AM
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/controller_callback_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/controller_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/container/container_database_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/container_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/core/unit_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/unit_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/kernel/kernel_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/kernel_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     def enforceReservationExistsInDatabase(self, *, db: ABCDatabase, rid: ID):
         res = db.get_reservations(rid=rid)
         self.assertIsNotNone(res)
         self.assertEqual(len(res), 1)
 
     def enforceReservationNotInDatabase(self, *, db: ABCDatabase, rid: ID):
         res = db.get_reservations(rid=rid)
-        self.assertIsNone(res)
         self.assertEqual(len(res), 0)
 
     def enforceSliceExistsInDatabase(self, *, db: ABCDatabase, slice_id: ID):
         slice_obj = db.get_slices(slice_id=slice_id)
         self.assertIsNotNone(slice_obj)
         self.assertEqual(len(slice_obj), 1)
 
@@ -241,76 +240,100 @@
     def test_e_re_register_reservation(self):
         actor = self.prepare_actor()
         kernel = self.get_kernel_wrapper(actor=actor)
         db = actor.get_plugin().get_database()
 
         slice_obj = SliceFactory.create(slice_id=ID(), name="test_slice")
 
+        # Register a reservation without registering the slice; it should fail
         res_list = []
         for i in range(10):
             res = ClientReservationFactory.create(rid=ID())
             res.set_slice(slice_object=slice_obj)
             res_list.append(res)
 
             failed = False
             try:
                 kernel.register_reservation(reservation=res)
             except Exception:
                 failed = True
 
             self.assertTrue(failed)
-
+            # get it back
             self.assertIsNone(kernel.get_reservation(rid=res.get_reservation_id()))
+            # make sure it is not in the database
             self.enforceReservationNotInDatabase(db=db, rid=res.get_reservation_id())
+            # make sure slice is not present
             self.assertIsNone(kernel.get_slice(slice_id=slice_obj.get_slice_id()))
             self.enforceSliceNotInDatabase(db=db, slice_id=slice_obj.get_slice_id())
 
+        # Register Slice
         kernel.register_slice(slice_object=slice_obj)
 
+        # Register the reservations now, it should succeed
         for res in res_list:
-
+            # get it back
             self.assertIsNone(kernel.get_reservation(rid=res.get_reservation_id()))
+            # make sure it is not in the database
             self.enforceReservationNotInDatabase(db=db, rid=res.get_reservation_id())
 
+            # re-register on a new reservation should fail
             failed = False
             try:
                 kernel.re_register_reservation(reservation=res)
             except Exception:
                 failed = True
 
             self.assertTrue(failed)
+            # get it back
             self.assertIsNone(kernel.get_reservation(rid=res.get_reservation_id()))
+            # make sure it is not in the database
             self.enforceReservationNotInDatabase(db=db, rid=res.get_reservation_id())
 
+            # register the reservation
             kernel.register_reservation(reservation=res)
-
+            # get it back
             self.assertIsNotNone(kernel.get_reservation(rid=res.get_reservation_id()))
+            # make sure it is in the database
             self.enforceReservationExistsInDatabase(db=db, rid=res.get_reservation_id())
 
+        # Create another kernel wrapper. This will be "equivalent" to starting with a clean kernel.
         kernel2 = self.get_kernel_wrapper(actor=actor)
-        kernel2.re_register_slice(slice_object=slice_obj)
 
         for res in res_list:
-
+            # make sure the new kernel does not know about this reservation
             self.assertIsNone(kernel2.get_reservation(rid=res.get_reservation_id()))
+            # make sure the reservation is in the database
             self.enforceReservationExistsInDatabase(db=db, rid=res.get_reservation_id())
 
+            # Try to register the reservation with the new kernel. This should fail since there is
+            # already a record in the database.
             failed = False
             try:
-                kernel.re_register_reservation(reservation=res)
+                kernel2.re_register_reservation(reservation=res)
             except Exception:
                 failed = True
 
+            # Check that the previous attempt did not leave the reservation in the kernel data structures and
+            # that it did not affect the database.
             self.assertTrue(failed)
+            # make sure the new kernel does not know about this reservation
             self.assertIsNone(kernel2.get_reservation(rid=res.get_reservation_id()))
+            # make sure the reservation is in the database
             self.enforceReservationExistsInDatabase(db=db, rid=res.get_reservation_id())
 
-            kernel2.register_reservation(reservation=res)
+        # re-register the slice: this will clear any previous state created by the first kernel
+        kernel2.re_register_slice(slice_object=slice_obj)
+        for res in res_list:
+            # re-register the reservation.
+            kernel2.re_register_reservation(reservation=res)
 
+            # Check if registered.
             self.assertIsNotNone(kernel2.get_reservation(rid=res.get_reservation_id()))
+            # Check the database.
             self.enforceReservationExistsInDatabase(db=db, rid=res.get_reservation_id())
 
     def test_f_re_register_slice(self):
         actor = self.prepare_actor()
         kernel = self.get_kernel_wrapper(actor=actor)
         db = actor.get_plugin().get_database()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/kernel/tick_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/tick_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/actor_database_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/actor_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from fabric_cf.actor.core.plugins.handlers.configuration_mapping import ConfigurationMapping
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.resource_type import ResourceType
 
 
 class AnsibleHandlerProcessorTest(unittest.TestCase):
     from fabric_cf.actor.core.container.globals import Globals
-    Globals.config_file = "../../config/config.test.yaml"
+    Globals.config_file = "./config/config.test.yaml"
     Constants.SUPERBLOCK_LOCATION = './state_recovery.lock'
 
     from fabric_cf.actor.core.container.globals import GlobalsSingleton
     GlobalsSingleton.get().start(force_fresh=True)
     while not GlobalsSingleton.get().start_completed:
         time.sleep(0.0001)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/authority_substrate_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/authority_substrate_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/substrate_database_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/plugins/substrate_test_base.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_test_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     logger = logging.getLogger('AuthorityCalendarPolicyTest')
     log_format = '%(asctime)s - %(name)s - {%(filename)s:%(lineno)d} - [%(threadName)s] - %(levelname)s - %(message)s'
     logging.basicConfig(format=log_format, filename="actor.log")
     logger.setLevel(logging.INFO)
 
     from fabric_cf.actor.core.container.globals import Globals
-    Globals.config_file = "./config/config.test.yaml"
+    Globals.config_file = "../../config/config.test.yaml"
     Constants.SUPERBLOCK_LOCATION = './state_recovery.lock'
 
     from fabric_cf.actor.core.container.globals import GlobalsSingleton
     GlobalsSingleton.get().start(force_fresh=True)
     while not GlobalsSingleton.get().start_completed:
         time.sleep(0.0001)
 
@@ -180,15 +180,22 @@
                                                        term=term,
                                                        rtype=rtype)
         ticket = Ticket(resource_ticket=resource_ticket, plugin=actor.get_plugin(), authority=None)
         ticket.delegation_id = source.get_delegation_id()
         return ticket
 
     def get_request_slice(self):
-        return SliceFactory.create(slice_id=ID(), name="test-slice")
+        slice_obj =  SliceFactory.create(slice_id=ID(), name="test-slice")
+        config = {
+            Constants.PROJECT_ID: "10c0094a-abaf-4ef9-a532-2be53e2a896b",
+            Constants.TAGS: "Component.GPU, Component.Storage",
+            Constants.CLAIMS_EMAIL: 'test@email.unc.edu'
+        }
+        slice_obj.set_config_properties(value=config)
+        return slice_obj
 
     def get_request(self, term: Term, ticket: Ticket, sliver: BaseSliver):
         rset = ResourceSet(units=1, rtype=ResourceType(resource_type=sliver.resource_type.name), sliver=sliver)
         rset.set_resources(cset=ticket)
         slice_object = self.get_request_slice()
         return AuthorityReservationFactory.create(resources=rset, term=term, slice_obj=slice_object, rid=ID())
 
@@ -266,27 +273,27 @@
         uset = rset.get_resources()
         self.assertIsNotNone(uset)
         self.assertEqual(self.TicketUnits, uset.get_units())
 
         u = uset.get_set().values().__iter__().__next__()
         self.assertEqual(self.my_unit, u)
 
-    def test_a_create(self):
+    def _test_a_create(self):
         authority = self.get_authority()
         self.assertIsNotNone(authority)
 
-    def test_b_donate(self):
+    def _test_b_donate(self):
         site = self.get_authority()
         policy = site.get_policy()
         self.check_before_donate_delegation(site)
         delegation = self.get_delegation(site)
         policy.donate_delegation(delegation=delegation)
         self.check_after_donate_donate_delegation(site)
 
-    def test_c_redeem(self):
+    def _test_c_redeem(self):
         site = self.get_authority()
         policy = site.get_policy()
         controller = self.get_controller()
         proxy = ControllerCallbackHelper(name=controller.get_name(), guid=controller.get_guid())
         authority_proxy = ControllerCallbackHelper(name=site.get_name(), guid=site.get_guid())
 
         ActorRegistrySingleton.get().register_callback(callback=proxy)
@@ -335,15 +342,15 @@
         for c in range(cycle, self.DonateEndCycle):
             site.external_tick(cycle=c)
             while site.get_current_cycle() != c:
                 time.sleep(0.001)
 
         handler.check_termination()
 
-    def test_d_extend_lease(self):
+    def _test_d_extend_lease(self):
         site = self.get_authority()
         policy = site.get_policy()
         controller = self.get_controller()
         proxy = ControllerCallbackHelper(name=controller.get_name(), guid=controller.get_guid())
         auth_proxy = ControllerCallbackHelper(name=site.get_name(), guid=site.get_guid())
         ActorRegistrySingleton.get().register_callback(callback=proxy)
         ActorRegistrySingleton.get().register_callback(callback=auth_proxy)
@@ -395,15 +402,15 @@
                 print("Extending Lease")
                 site.extend_lease(reservation=extend, caller=proxy.get_identity())
             site.external_tick(cycle=cycle)
             while site.get_current_cycle() != cycle:
                 time.sleep(0.001)
         handler.check_termination()
 
-    def test_e_close(self):
+    def _test_e_close(self):
         site = self.get_authority()
         policy = site.get_policy()
         controller = self.get_controller()
         proxy = ControllerCallbackHelper(name=controller.get_name(), guid=controller.get_guid())
         authority_proxy = ControllerCallbackHelper(name=site.get_name(), guid=site.get_guid())
 
         ActorRegistrySingleton.get().register_callback(callback=proxy)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,22 +195,22 @@
         adm = self.adms[adm_index]
         broker_delegation = BrokerDelegationFactory.create(adm.graph_id, slice_id=slice_obj.get_slice_id(),
                                                            broker=broker)
         broker_delegation.set_graph(graph=adm)
         broker_delegation.set_slice_object(slice_object=slice_obj)
         return broker_delegation
 
-    def test_a_create(self):
+    def _test_a_create(self):
         """
         Tests if the actor and the policy can be instantiated.
         """
         self.get_broker()
         self.assertIsNotNone(self.broker)
 
-    def test_b_allocate_ticket(self):
+    def _test_b_allocate_ticket(self):
         """
         Requests a ticket for all resources. Checks if the ticket is
         allocated for what was asked. Checks the term. Checks whether the
         reservation is closed when it expires.
         """
         self.broker = self.get_broker()
         controller = self.get_controller()
@@ -253,15 +253,15 @@
                 last_called = proxy.get_called()
 
         self.broker.await_no_pending_reservations()
 
         self.assertEqual(1, proxy.get_called())
         self.assertTrue(request.is_closed())
 
-    def test_c_allocate_ticket2(self):
+    def _test_c_allocate_ticket2(self):
         """
         Requests a ticket for all resources. Checks if the ticket is
         allocated for what was asked. Checks the term. Checks whether the
         reservation is closed when it expires. Repeat one more time.
         """
         broker = self.get_broker()
         controller = self.get_controller()
@@ -314,15 +314,15 @@
                 broker.ticket(reservation=request, callback=proxy, caller=proxy.get_identity())
 
         broker.await_no_pending_reservations()
 
         self.assertEqual(2, proxy.get_called())
         self.assertTrue(request.is_closed())
 
-    def test_d_extend_ticket(self):
+    def _test_d_extend_ticket(self):
         """
         Requests a ticket for all resources. Checks if the ticket is
         allocated for what was asked. Checks the term. Checks whether the
         reservation is closed when it expires. Repeat one more time.
         """
         broker = self.get_broker()
         controller = self.get_controller()
@@ -375,15 +375,15 @@
                 print("Extend done")
 
         broker.await_no_pending_reservations()
 
         self.assertEqual(2, proxy.get_called())
         self.assertTrue(reservation.is_closed())
 
-    def test_e_donate(self):
+    def _test_e_donate(self):
         broker = self.get_broker()
         policy = broker.get_policy()
 
         slice_obj = SliceFactory.create(slice_id=ID(), name="inventory_slice")
         slice_obj.set_inventory(value=True)
 
         adm_list_len = len(self.adms)
@@ -393,15 +393,15 @@
         for i in range(0, adm_list_len):
             source = self.get_source_delegation(self.broker, slice_obj, adm_index=i)
             self.broker.register_delegation(delegation=source)
             self.broker.donate_delegation(delegation=source)
 
             self.assertEqual(i + 1, len(policy.delegations))
 
-    def test_f_query(self):
+    def _test_f_query(self):
         broker = self.get_broker()
         policy = broker.get_policy()
 
         request = BrokerPolicy.get_broker_query_model_query(level=1)
         response = policy.query(p=request)
 
         print(response)
@@ -421,15 +421,15 @@
             self.broker.register_delegation(delegation=source)
             self.broker.donate_delegation(delegation=source)
 
             response = policy.query(p=request)
             print(response)
             self.check_query_response(response, i + 1)
 
-    def test_g_advanced_request(self):
+    def _test_g_advanced_request(self):
         broker = self.get_broker()
         controller = self.get_controller()
         policy = broker.get_policy()
         policy.allocation_horizon = 10
 
         clock = broker.get_actor_clock()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,20 +62,20 @@
     def get_controller_instance(self) -> ABCActorMixin:
         return ControllerTestWrapper()
 
     def get_controller_policy(self) -> ABCControllerPolicy:
         policy = ControllerSimplePolicyTestWrapper()
         return policy
 
-    def test_a_create(self):
+    def _test_a_create(self):
         controller = self.get_controller()
         for i in range(1, 101):
             controller.external_tick(cycle=i)
 
-    def test_b_demand(self):
+    def _test_b_demand(self):
         controller = self.get_controller()
         clock = controller.get_actor_clock()
         Term.clock = clock
         resources = ResourceSet(units=1, rtype=ResourceType(resource_type="1"))
         slice_obj = SliceFactory.create(slice_id=ID(), name="myslice")
         controller.register_slice(slice_object=slice_obj)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_test_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     ControllerTicketReviewPolicyTestWrapper
 
 
 class ControllerTicketReviewPolicyTest(ControllerSimplePolicyTest):
     def get_controller_policy(self) -> ABCControllerPolicy:
         return ControllerTicketReviewPolicyTestWrapper()
 
-    def test_c_fail(self):
+    def _test_c_fail(self):
         controller = self.get_controller()
         clock = controller.get_actor_clock()
         Term.clock = clock
 
         resources = ResourceSet(units=1, rtype=ResourceType(resource_type="1"))
         slice_obj = SliceFactory.create(slice_id=ID(), name="fail")
         controller.register_slice(slice_object=slice_obj)
@@ -73,15 +73,15 @@
                 time.sleep(0.001)
 
             if i >= start and (i < (end - 1)):
                 self.assertTrue(r1.is_closed())
                 self.assertTrue(r2.is_closed())
                 self.assertTrue(r2.get_notices().__contains__(Constants.CLOSURE_BY_TICKET_REVIEW_POLICY))
 
-    def test_d_nascent(self):
+    def _test_d_nascent(self):
         controller = self.get_controller()
         clock = controller.get_actor_clock()
         Term.clock = clock
 
         resources = ResourceSet(units=1, rtype=ResourceType(resource_type="1"))
         slice_obj = SliceFactory.create(slice_id=ID(), name="nascent")
         controller.register_slice(slice_object=slice_obj)
@@ -118,15 +118,15 @@
                 self.assertTrue(r1.is_active())
                 self.assertTrue(r2.is_active())
 
             if i > end:
                 self.assertTrue(r1.is_closed())
                 self.assertTrue(r2.is_closed())
 
-    def test_e_fail_and_nascent(self):
+    def _test_e_fail_and_nascent(self):
         controller = self.get_controller()
         clock = controller.get_actor_clock()
         Term.clock = clock
 
         resources = ResourceSet(units=1, rtype=ResourceType(resource_type="1"))
         slice_obj = SliceFactory.create(slice_id=ID(), name="fail_nascent")
         controller.register_slice(slice_object=slice_obj)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/actor_clock_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/actor_clock_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/time/term_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/term_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/util/reservation_holdings_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_holdings_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/core/util/reservation_list_test.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_list_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/dummy_authority_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/dummy_proxy.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/fim_test_helper.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/fim_test_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/schema/message.avsc` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/message.avsc`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9641225038402458%*

 * *Differences: {'0': "{'fields': {insert: [(4, OrderedDict([('name', 'token'), ('type', ['null', 'string']), "*

 * *      "('default', None)]))]}}",*

 * * '15': "{'fields': {insert: [(1, OrderedDict([('name', 'delegation_name'), ('type', ['null', "*

 * *       "'string']), ('default', None)]))]}}",*

 * * '20': "{'fields': {insert: [(7, OrderedDict([('name', 'sites'), ('type', ['null', "*

 * *       "OrderedDict([('type', 'array'), ('items', 'fabric.cf.model.SiteRecord')])]), ('default', "*

 * *       'None)]))]}}',*

 * * '22': "{'fields': {insert: [(11, Or […]*

```diff
@@ -20,14 +20,22 @@
             {
                 "default": null,
                 "name": "email",
                 "type": [
                     "null",
                     "string"
                 ]
+            },
+            {
+                "default": null,
+                "name": "token",
+                "type": [
+                    "null",
+                    "string"
+                ]
             }
         ],
         "name": "AuthRecord",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
     {
@@ -286,14 +294,33 @@
         "name": "BrokerQueryModelRecord",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
     {
         "fields": [
             {
+                "name": "name",
+                "type": "string"
+            },
+            {
+                "default": null,
+                "name": "maint_info",
+                "type": [
+                    "null",
+                    "bytes"
+                ]
+            }
+        ],
+        "name": "SiteRecord",
+        "namespace": "fabric.cf.model",
+        "type": "record"
+    },
+    {
+        "fields": [
+            {
                 "name": "slice_name",
                 "type": "string"
             },
             {
                 "name": "guid",
                 "type": "string"
             },
@@ -383,14 +410,30 @@
             {
                 "default": null,
                 "name": "lease_start",
                 "type": [
                     "null",
                     "int"
                 ]
+            },
+            {
+                "default": null,
+                "name": "project_id",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            {
+                "default": null,
+                "name": "project_name",
+                "type": [
+                    "null",
+                    "string"
+                ]
             }
         ],
         "name": "SliceRecord",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
     {
@@ -792,14 +835,22 @@
         "fields": [
             {
                 "name": "delegation_id",
                 "type": "string"
             },
             {
                 "default": null,
+                "name": "delegation_name",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            {
+                "default": null,
                 "name": "sequence",
                 "type": [
                     "null",
                     "int"
                 ]
             },
             {
@@ -1086,14 +1137,25 @@
                         "items": "fabric.cf.model.UnitRecord",
                         "type": "array"
                     }
                 ]
             },
             {
                 "default": null,
+                "name": "sites",
+                "type": [
+                    "null",
+                    {
+                        "items": "fabric.cf.model.SiteRecord",
+                        "type": "array"
+                    }
+                ]
+            },
+            {
+                "default": null,
                 "name": "proxies",
                 "type": [
                     "null",
                     {
                         "items": "fabric.cf.model.ProxyRecord",
                         "type": "array"
                     }
@@ -1283,14 +1345,25 @@
                 "type": [
                     "null",
                     "string"
                 ]
             },
             {
                 "default": null,
+                "name": "states",
+                "type": [
+                    "null",
+                    {
+                        "items": "int",
+                        "type": "array"
+                    }
+                ]
+            },
+            {
+                "default": null,
                 "name": "reservation_state",
                 "type": [
                     "null",
                     "int"
                 ]
             },
             {
@@ -1336,14 +1409,22 @@
             {
                 "default": null,
                 "name": "graph_format",
                 "type": [
                     "null",
                     "int"
                 ]
+            },
+            {
+                "default": null,
+                "name": "site",
+                "type": [
+                    "null",
+                    "string"
+                ]
             }
         ],
         "name": "RequestById",
         "namespace": "fabric.cf.model",
         "type": "record"
     },
     {
@@ -1533,19 +1614,34 @@
                 "type": "string"
             },
             {
                 "name": "actor_guid",
                 "type": "string"
             },
             {
+                "default": null,
                 "name": "properties",
-                "type": {
-                    "type": "map",
-                    "values": "string"
-                }
+                "type": [
+                    "null",
+                    {
+                        "type": "map",
+                        "values": "string"
+                    }
+                ]
+            },
+            {
+                "default": null,
+                "name": "sites",
+                "type": [
+                    "null",
+                    {
+                        "items": "fabric.cf.model.SiteRecord",
+                        "type": "array"
+                    }
+                ]
             },
             {
                 "default": null,
                 "name": "id_token",
                 "type": [
                     "null",
                     "string"
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/test_abqm.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_abqm.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
             f.write(cbm_string)
 
         self.n4j_imp.delete_all_graphs()
 
     def test_cbm(self):
         self.n4j_imp.delete_all_graphs()
         # these are produced by substrate tests
-        cbm = '../../../neo4j/abqm-l2-cbm.graphml'
+        #cbm = '../../../neo4j/abqm-l2-cbm.graphml'
+        cbm = 'cbm.graphml'
 
         plain_cbm = self.n4j_imp.import_graph_from_file_direct(graph_file=cbm)
         cbm = Neo4jCBMFactory.create(Neo4jPropertyGraph(graph_id=plain_cbm.graph_id,
                                      importer=self.n4j_imp))
         cbm.validate_graph()
 
         print('CBM ID is ' + cbm.graph_id)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/test_actor.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/actor/test/test_exception.py` & `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/config/config.broker.yaml` & `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.broker.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
   #kafka-server: broker1:9092
   #kafka-schema-registry-url: http://schemaregistry:8081
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server: localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: /etc/fabric/message_bus/schema/key.avsc
   kafka-value-schema: /etc/fabric/message_bus/schema/message.avsc
   kafka-ssl-ca-location:  /etc/fabric/message_bus/ssl/cacert.pem
   kafka-ssl-certificate-location:  /etc/fabric/message_bus/ssl/client.pem
   kafka-ssl-key-location:  /etc/fabric/message_bus/ssl/client.key
   kafka-ssl-key-password:  fabric
   kafka-security-protocol: SSL
@@ -73,15 +73,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: broker
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: broker-conainer
 
 time:
   # This section controls settings, which are generally useful
   # when running under emulation. These settings allow you to
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/config/config.netam.yaml` & `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.netam.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
   #kafka-server: broker1:9092
   #kafka-schema-registry-url: http://schemaregistry:8081
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server: localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: /etc/fabric/message_bus/schema/key.avsc
   kafka-value-schema: /etc/fabric/message_bus/schema/message.avsc
   kafka-ssl-ca-location:  /etc/fabric/message_bus/ssl/cacert.pem
   kafka-ssl-certificate-location:  /etc/fabric/message_bus/ssl/client.pem
   kafka-ssl-key-location:  /etc/fabric/message_bus/ssl/client.key
   kafka-ssl-key-password:  fabric
   kafka-security-protocol: SSL
@@ -73,15 +73,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: am
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: net1-am-conainer
 
 time:
   # This section controls settings, which are generally useful
   # when running under emulation. These settings allow you to
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/config/config.orchestrator.yaml` & `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.orchestrator.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
   #kafka-server: broker1:9092
   #kafka-schema-registry-url: http://schemaregistry:8081
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server: localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: /etc/fabric/message_bus/schema/key.avsc
   kafka-value-schema: /etc/fabric/message_bus/schema/message.avsc
   kafka-ssl-ca-location:  /etc/fabric/message_bus/ssl/cacert.pem
   kafka-ssl-certificate-location:  /etc/fabric/message_bus/ssl/client.pem
   kafka-ssl-key-location:  /etc/fabric/message_bus/ssl/client.key
   kafka-ssl-key-password:  fabric
   kafka-security-protocol: SSL
@@ -69,15 +69,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: orchestrator
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 pdp:
   url: http://localhost:8082/services/pdp
   enable: False
 
 neo4j:
   url: bolt://neo4j3:9687
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/config/config.siteam.yaml` & `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.siteam.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
   #kafka-server: broker1:9092
   #kafka-schema-registry-url: http://schemaregistry:8081
-  kafka-server: 152.54.15.56:29092
-  kafka-schema-registry-url: http://152.54.15.56:8081
+  kafka-server: localhost:19092
+  kafka-schema-registry-url: http://localhost:8081
   kafka-key-schema: /etc/fabric/message_bus/schema/key.avsc
   kafka-value-schema: /etc/fabric/message_bus/schema/message.avsc
   kafka-ssl-ca-location:  /etc/fabric/message_bus/ssl/cacert.pem
   kafka-ssl-certificate-location:  /etc/fabric/message_bus/ssl/client.pem
   kafka-ssl-key-location:  /etc/fabric/message_bus/ssl/client.key
   kafka-ssl-key-password:  fabric
   kafka-security-protocol: SSL
@@ -73,15 +73,15 @@
   key-refresh: 00:10:00
   verify-exp: False
 
 database:
   db-user: fabric
   db-password: fabric
   db-name: am
-  db-host: 152.54.15.56:5432
+  db-host: localhost:5432
 
 container:
   container.guid: site1-am-conainer
 
 time:
   # This section controls settings, which are generally useful
   # when running under emulation. These settings allow you to
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/elements/reservation.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_kernel.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,157 +19,144 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-import json
-from typing import List
+import threading
 
-from fim.slivers.capacities_labels import JSONField, Capacities, Labels, CapacityHints
+from fim.user import GraphFormat
 
-from .constants import Constants
+from fabric_cf.actor.core.apis.abc_mgmt_controller_mixin import ABCMgmtControllerMixin
+from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.manage.management_utils import ManagementUtils
+from fabric_cf.actor.core.util.id import ID
+from fabric_cf.orchestrator.core.bqm_wrapper import BqmWrapper
+from fabric_cf.orchestrator.core.exceptions import OrchestratorException
+from fabric_cf.orchestrator.core.reservation_status_update_thread import ReservationStatusUpdateThread
+from fabric_cf.orchestrator.core.slice_defer_thread import SliceDeferThread
 
 
-class Reservation(JSONField):
+class OrchestratorKernel:
     """
-    Class represents the reservations received
+    Class responsible for starting Orchestrator Threads; also holds Management Actor and Broker information
     """
+
     def __init__(self):
-        self.name = None
-        self.site = None
-        self.resource_type = None
-        self.graph_node_id = None
-        self.slice_id = None
-        self.reservation_id = None
-        self.management_ip = None
-        self.capacities = None
-        self.allocated_capacities = None
-        self.capacity_hints = None
-        self.labels = None
-        self.allocated_labels = None
-        self.join_state = None
-        self.pending_state = None
-        self.reservation_state = None
-        self.notices = None
-        self.lease_end = None
-
-    def get_name(self) -> str:
-        return self.name
-
-    def get_site(self) -> str:
-        return self.site
-
-    def get_type(self) -> str:
-        return self.resource_type
-
-    def get_graph_node_id(self) -> str:
-        return self.graph_node_id
-
-    def get_slice_id(self) -> str:
-        return self.slice_id
-
-    def get_management_ip(self) -> str:
-        return self.management_ip
-
-    def get_capacities(self) -> Capacities:
-        return self.capacities
-
-    def get_labels(self) -> Labels:
-        return self.labels
-
-    def get_allocated_capacities(self) -> Capacities:
-        return self.allocated_capacities
-
-    def get_capacity_hints(self) -> CapacityHints:
-        return self.capacity_hints
-
-    def get_allocated_labels(self) -> Labels:
-        return self.labels
-
-    def get_join_state(self) -> str:
-        return self.join_state
-
-    def get_state(self) -> str:
-        return self.reservation_state
-
-    def get_pending_state(self) -> str:
-        return self.pending_state
-
-    def get_notices(self) -> str:
-        return self.notices
-
-    def set_fields(self, **kwargs):
-        """
-        Universal integer setter for all fields.
-        Values should be non-negative integers. Throws a RuntimeError
-        if you try to set a non-existent field.
-        :param kwargs:
-        :return: self to support call chaining
-        """
-        for k, v in kwargs.items():
-            try:
-                # will toss an exception if field is not defined
-                self.__getattribute__(k)
-                if k == Constants.PROP_CAPACITIES or k == Constants.PROP_ALLOCATED_CAPACITIES:
-                    c = Capacities()
-                    v = c.from_json(json_string=v)
-                elif k == Constants.PROP_LABELS or k == Constants.PROP_ALLOCATED_LABELS:
-                    l = Labels()
-                    v = l.from_json(json_string=v)
-                elif k == Constants.PROP_CAPACITY_HINTS:
-                    ch = CapacityHints()
-                    v = ch.from_json(json_string=v)
-                self.__setattr__(k, v)
-            except AttributeError:
-                raise RuntimeError(f"Unable to set field {k} of reservation, no such field available")
-        return self
-
-    def to_json(self) -> str:
-        """
-        Dumps to JSON the __dict__ of the instance. Be careful as the fields in this
-        class should only be those that can be present in JSON output.
-        If there are no values in the object, returns empty string.
-        :return:
-        """
-        d = self.__dict__.copy()
-        for k in self.__dict__:
-            if d[k] is None:
-                d.pop(k)
-            elif k == Constants.PROP_CAPACITIES or k == Constants.PROP_LABELS or \
-                    k == Constants.PROP_ALLOCATED_CAPACITIES or k == Constants.PROP_ALLOCATED_LABELS or \
-                    k == Constants.PROP_CAPACITY_HINTS:
-                d[k] = d[k].to_json()
-        if len(d) == 0:
-            return ''
-        return json.dumps(d, skipkeys=True, sort_keys=True, indent=4)
+        self.defer_thread = None
+        self.sut = None
+        self.broker = None
+        self.logger = None
+        self.controller = None
+        self.lock = threading.Lock()
+        self.bqm_cache = {}
+        
+    def get_saved_bqm(self, *, graph_format: GraphFormat) -> BqmWrapper:
+        """
+        Get Saved BQM from cache
+        """
+        try:
+            self.lock.acquire()
+            saved_bqm = self.bqm_cache.get(graph_format, None)
+            return saved_bqm
+        finally:
+            self.lock.release()
+
+    def save_bqm(self, *, bqm: str, graph_format: GraphFormat):
+        try:
+            self.lock.acquire()
+            saved_bqm = self.bqm_cache.get(graph_format, None)
+            if saved_bqm is None:
+                from fabric_cf.actor.core.container.globals import GlobalsSingleton
+                refresh_interval = GlobalsSingleton.get().get_config().get_global_config().get_bqm_config().get(
+                    Constants.REFRESH_INTERVAL, None)
+                saved_bqm = BqmWrapper()
+                saved_bqm.set_refresh_interval(refresh_interval=int(refresh_interval))
+            saved_bqm.save(bqm=bqm, graph_format=graph_format)
+            self.bqm_cache[graph_format] = saved_bqm
+        finally:
+            self.lock.release()
 
+    def set_broker(self, *, broker: ID):
+        """
+        Set Broker
+        :param broker:
+        :return:
+        """
+        self.broker = broker
 
-class ReservationFactory:
-    """
-    Factory class to instantiate Reservation
-    """
-    @staticmethod
-    def create_reservations(*, reservation_list: List[dict]) -> List[Reservation]:
+    def get_broker(self) -> ID:
+        """
+        Get Broker
+        :return:
+        """
+        return self.broker
+
+    def get_defer_thread(self) -> SliceDeferThread:
+        return self.defer_thread
+
+    def get_sut(self) -> ReservationStatusUpdateThread:
+        """
+        Get SUT thread
+        :return:
+        """
+        return self.sut
+
+    def get_logger(self):
+        """
+        Get logger
+        :return:
+        """
+        if self.logger is None:
+            from fabric_cf.actor.core.container.globals import GlobalsSingleton
+            self.logger = GlobalsSingleton.get().get_logger()
+        return self.logger
+
+    def get_management_actor(self) -> ABCMgmtControllerMixin:
         """
-        Create list of reservations from JSON List
-        :param reservation_list reservation list
-        :return list of reservations
-        """
-        result = []
-        for r_dict in reservation_list:
-            reservation = ReservationFactory.create(reservation_dict=r_dict)
-            result.append(reservation)
-
-        return result
-
-    @staticmethod
-    def create(*, reservation_dict: dict) -> Reservation:
-        """
-        Create reservations from JSON
-        :param reservation_dict reservation jso
-        :return reservation
-        """
-        reservation_json = json.dumps(reservation_dict)
-        res_obj = Reservation().from_json(json_string=reservation_json)
-        return res_obj
+        Get Management actor
+        :return:
+        """
+        if self.controller is None:
+            self.controller = ManagementUtils.get_local_actor()
+        return self.controller
+
+    def stop_threads(self):
+        """
+        Stop threads
+        :return:
+        """
+        if self.defer_thread is not None:
+            self.defer_thread.stop()
+        #if self.sut is not None:
+        #    self.sut.stop()
+
+    def start_threads(self):
+        """
+        Start threads
+        :return:
+        """
+        self.get_logger().debug("Starting SliceDeferThread")
+        self.defer_thread = SliceDeferThread(kernel=self)
+        self.defer_thread.start()
+        #self.get_logger().debug("Starting ReservationStatusUpdateThread")
+        #self.sut = ReservationStatusUpdateThread()
+        #self.sut.start()
+
+
+class OrchestratorKernelSingleton:
+    __instance = None
+
+    def __init__(self):
+        if self.__instance is not None:
+            raise OrchestratorException("Singleton can't be created twice !")
+
+    def get(self):
+        """
+        Actually create an instance
+        """
+        if self.__instance is None:
+            self.__instance = OrchestratorKernel()
+        return self.__instance
+
+    get = classmethod(get)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/aits/kafka_processor.py` & `fabric_cf-1.5.0b3/fabric_cf/aits/kafka_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,23 +66,21 @@
         self.logger = logger
 
     def setup_kafka(self):
         """
         Set up Kafka Producer and Consumer
         """
         producer_conf = {
-                Constants.BOOTSTRAP_SERVERS: "152.54.15.56:29092",
-                #Constants.BOOTSTRAP_SERVERS: "localhost:19092",
-                Constants.SECURITY_PROTOCOL: "SSL",
+                Constants.BOOTSTRAP_SERVERS: "localhost:19092",
+                Constants.SECURITY_PROTOCOL: "PLAINTEXT",
                 Constants.SSL_CA_LOCATION: "../../secrets/snakeoil-ca-1.crt",
                 Constants.SSL_CERTIFICATE_LOCATION: "../../secrets/kafkacat1-ca1-signed.pem",
                 Constants.SSL_KEY_LOCATION: "../../secrets/kafkacat1.client.key",
                 Constants.SSL_KEY_PASSWORD: "fabric",
-                #Constants.SCHEMA_REGISTRY_URL: "http://localhost:8081"
-                Constants.SCHEMA_REGISTRY_URL: "http://152.54.15.56:8081"
+                Constants.SCHEMA_REGISTRY_URL: "http://localhost:8081"
         }
 
         self.key_schema = "../actor/test/schema/key.avsc"
         self.val_schema = "../actor/test/schema/message.avsc"
 
         from fabric_mb.message_bus.producer import AvroProducerApi
         self.producer = AvroProducerApi(producer_conf=producer_conf, key_schema_location=self.key_schema,
@@ -118,14 +116,20 @@
             self.actor_cache[self.broker_name] = mgmt_actor
 
             mgmt_actor = KafkaActor(guid=ID(uid=self.am_guid), kafka_topic=self.am_topic, auth=self.auth,
                                     logger=self.logger, message_processor=self.message_processor, producer=self.producer)
 
             self.actor_cache[self.am_name] = mgmt_actor
 
+            mgmt_actor = KafkaActor(guid=ID(uid=self.net_am_guid), kafka_topic=self.net_am_topic, auth=self.auth,
+                                    logger=self.logger, message_processor=self.message_processor,
+                                    producer=self.producer)
+
+            self.actor_cache[self.net_am_name] = mgmt_actor
+
             mgmt_actor = KafkaActor(guid=ID(uid=self.orchestrator_guid), kafka_topic=self.orchestrator_topic,
                                     auth=self.auth, logger=self.logger, message_processor=self.message_processor,
                                     producer=self.producer)
 
             self.actor_cache[self.orchestrator_name] = mgmt_actor
         finally:
             self.lock.release()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/Readme.md` & `fabric_cf-1.5.0b3/fabric_cf/authority/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/__main__.py` & `fabric_cf-1.5.0b3/fabric_cf/authority/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/am-yes.xml` & `fabric_cf-1.5.0b3/fabric_cf/authority/am-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/config.al2s.am.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/config.al2s.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/config.net.am.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/config.net.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/config.site.am.geni.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/config.site.am.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/docker-compose.geni.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 version: '3.6'
 services:
 
   neo4j:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: site1-am-neo4j
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     network_mode: host
     volumes:
       - ${NEO4J_DATA_PATH_HOST:-$(pwd)/neo4j/data}:${NEO4J_DATA_PATH_DOCKER:-/data}
       - ${NEO4J_IMPORTS_PATH_HOST:-$(pwd)/neo4j/imports}:${NEO4J_IMPORTS_PATH_DOCKER:-/imports}
       - ${NEO4J_LOGS_PATH_HOST:-$(pwd)/neo4j/logs}:${NEO4J_LOGS_PATH_DOCKER:-/logs}
       - ../../../neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ../../../neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_bolt_listen__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_http_advertised__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_http_listen__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_https_advertised__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
-      - NEO4J_dbms_connector_https_listen__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
+      - NEO4J_server_bolt_advertised__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_bolt_listen__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_http_advertised__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_http_listen__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_https_advertised__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_server_https_listen__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_dbms_memory_pagecache_size=${NEO4J_dbms_memory_pagecache_size:-512M}
   database:
     image: fabrictestbed/postgres:12.3
     container_name: site1-am-db
     restart: always
     network_mode: host
     volumes:
       - ./pg_data/data:${PGDATA:-/var/lib/postgresql/data}
@@ -47,28 +48,27 @@
       - ${PDP_NEW_POLICIES_PATH_HOST:-$(pwd)/newpolicies}:/policies
   am:
     init: true
     build:
       network: host
       context: ../../../
       dockerfile: Dockerfile-auth
-    image: authority:1.4.5
+    image: authority:1.5.0
     container_name: site1-am
     restart: always
     depends_on:
       - database
       - neo4j
     network_mode: host
     volumes:
       - ./neo4j:/usr/src/app/neo4j
       - ./config.yaml:/etc/fabric/actor/config/config.yaml
       - ./arm.graphml:/etc/fabric/actor/config/neo4j/arm.graphml
       - ./logs/:/var/log/actor
       - ./vm_handler_config.yml:/etc/fabric/actor/config/vm_handler_config.yml
-      - ./vnic_net_handler_config.yml:/etc/fabric/actor/config/vnic_net_handler_config.yml
       - ../../../../AMHandlers/fabric_am/playbooks:/etc/fabric/actor/playbooks
       - ../../../../AMHandlers/fabric_am/playbooks/inventory:/etc/fabric/actor/playbooks/inventory
       - ~/.ssh:/root/.ssh
       - ../../../secrets/snakeoil-ca-1.crt:/etc/fabric/message_bus/ssl/cacert.pem
       - ../../../secrets/kafkacat1.client.key:/etc/fabric/message_bus/ssl/client.key
       - ../../../secrets/kafkacat1-ca1-signed.pem:/etc/fabric/message_bus/ssl/client.pem
       #- ./state_recovery.lock:/usr/src/app/state_recovery.lock
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/docker-compose.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.geni.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 version: '3.6'
 services:
 
   neo4j:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: site1-am-neo4j
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     network_mode: host
     volumes:
       - ${NEO4J_DATA_PATH_HOST:-$(pwd)/neo4j/data}:${NEO4J_DATA_PATH_DOCKER:-/data}
       - ${NEO4J_IMPORTS_PATH_HOST:-$(pwd)/neo4j/imports}:${NEO4J_IMPORTS_PATH_DOCKER:-/imports}
       - ${NEO4J_LOGS_PATH_HOST:-$(pwd)/neo4j/logs}:${NEO4J_LOGS_PATH_DOCKER:-/logs}
       - ../../../neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ../../../neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_bolt_listen__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_http_advertised__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_http_listen__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_https_advertised__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
-      - NEO4J_dbms_connector_https_listen__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
+      - NEO4J_server_bolt_advertised__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_bolt_listen__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_http_advertised__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_http_listen__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_https_advertised__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_server_https_listen__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_dbms_memory_pagecache_size=${NEO4J_dbms_memory_pagecache_size:-512M}
   database:
     image: fabrictestbed/postgres:12.3
     container_name: site1-am-db
     restart: always
     network_mode: host
     volumes:
       - ./pg_data/data:${PGDATA:-/var/lib/postgresql/data}
@@ -47,27 +48,28 @@
       - ${PDP_NEW_POLICIES_PATH_HOST:-$(pwd)/newpolicies}:/policies
   am:
     init: true
     build:
       network: host
       context: ../../../
       dockerfile: Dockerfile-auth
-    image: authority:1.4.5
+    image: authority:1.5.0
     container_name: site1-am
     restart: always
     depends_on:
       - database
       - neo4j
     network_mode: host
     volumes:
       - ./neo4j:/usr/src/app/neo4j
       - ./config.yaml:/etc/fabric/actor/config/config.yaml
       - ./arm.graphml:/etc/fabric/actor/config/neo4j/arm.graphml
       - ./logs/:/var/log/actor
       - ./vm_handler_config.yml:/etc/fabric/actor/config/vm_handler_config.yml
+      - ./vnic_net_handler_config.yml:/etc/fabric/actor/config/vnic_net_handler_config.yml
       - ../../../../AMHandlers/fabric_am/playbooks:/etc/fabric/actor/playbooks
       - ../../../../AMHandlers/fabric_am/playbooks/inventory:/etc/fabric/actor/playbooks/inventory
       - ~/.ssh:/root/.ssh
       - ../../../secrets/snakeoil-ca-1.crt:/etc/fabric/message_bus/ssl/cacert.pem
       - ../../../secrets/kafkacat1.client.key:/etc/fabric/message_bus/ssl/client.key
       - ../../../secrets/kafkacat1-ca1-signed.pem:/etc/fabric/message_bus/ssl/client.pem
       #- ./state_recovery.lock:/usr/src/app/state_recovery.lock
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/env.template` & `fabric_cf-1.5.0b3/fabric_cf/broker/env.template`

 * *Files 18% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 NEO4J_IMPORTS_PATH_DOCKER=/imports
 NEO4J_IMPORTS_PATH_HOST=./neo4j/imports
 NEO4J_LOGS_PATH_DOCKER=/logs
 NEO4J_LOGS_PATH_HOST=./neo4j/logs
 NEO4J_PASS=password
 NEO4J_UID=1000
 NEO4J_USER=neo4j
-NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:7687
-NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:7687
-NEO4J_dbms_connector_http_advertised__address=0.0.0.0:7474
-NEO4J_dbms_connector_http_listen__address=0.0.0.0:7474
-NEO4J_dbms_connector_https_advertised__address=0.0.0.0:7473
-NEO4J_dbms_connector_https_listen__address=0.0.0.0:7473
+NEO4J_server_bolt_advertised__address=:8687
+NEO4J_server_bolt_listen__address=:8687
+NEO4J_server_http_advertised__address=:8474
+NEO4J_server_http_listen__address=:8474
+NEO4J_server_https_advertised__address=:8473
+NEO4J_server_https_listen__address=:8473
+NEO4J_dbms_memory_pagecache_size=8G
 
 # postgres configuration
 POSTGRES_HOST=database
 POSTGRES_PORT=5432
 POSTGRES_USER=fabric
 POSTGRES_PASSWORD=fabric
 PGDATA=/var/lib/postgresql/data/pgdata
-POSTGRES_DB=am
+POSTGRES_DB=broker
 
 PDP_NEW_CONF_PATH_HOST=./pdp/conf
 PDP_NEW_POLICIES_PATH_HOST=./pdp/policies
 PDP_GID=1000
 PDP_UID=1000
 
 CF_GID=1000
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.0b3/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/net_handler_config.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/oess_handler_config.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/oess_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/pdp.xml` & `fabric_cf-1.5.0b3/fabric_cf/authority/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/setup.sh` & `fabric_cf-1.5.0b3/fabric_cf/authority/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/al2s_am.py` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/al2s_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/net_am.py` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/net_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/site_am.py` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/site_am_geni.py` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am_geni.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/test-al2sam.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/test-al2sam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/test-netam.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/test-netam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: localhost:9092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://0.0.0.0:8081
   kafka-key-schema: ../../../schema/key.avsc
   kafka-value-schema: ../../../schema/message.avsc
   kafka-ssl-ca-location:
   kafka-ssl-certificate-location:
   kafka-ssl-key-location:
   kafka-ssl-key-password:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/test.geni.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/test.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/test/test.yaml` & `fabric_cf-1.5.0b3/fabric_cf/authority/test/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: localhost:9092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://0.0.0.0:8081
   kafka-key-schema: ../../../schema/key.avsc
   kafka-value-schema: ../../../schema/message.avsc
   kafka-ssl-ca-location:
   kafka-ssl-certificate-location:
   kafka-ssl-key-location:
   kafka-ssl-key-password:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/vm_handler_config.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/vm_handler_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,26 @@
     default_centos8_stream: centos
     default_centos9_stream: centos
     default_centos_7: centos
     default_centos_8: centos
     default_debian_10: debian
     default_debian_11: debian
     default_fedora_35: fedora
+    default_fedora_36: fedora
+    default_fedora_37: fedora
     default_rocky_8: rocky
+    default_rocky_9: rocky
     default_ubuntu_18: ubuntu
     default_ubuntu_20: ubuntu
     default_ubuntu_21: ubuntu
     default_ubuntu_22: ubuntu
+    docker_rocky_8: rocky
+    docker_rocky_9: rocky
+    docker_ubuntu_20: ubuntu
+    docker_ubuntu_22: ubuntu
 playbooks:
   location: /etc/fabric/actor/playbooks
   inventory_location: /etc/fabric/actor/playbooks/inventory
   admin_ssh_key: /root/.ssh/id_rsa_nova
   VM: head_vm_provisioning.yml
   GPU: worker_pci_provisioning.yml
   SmartNIC: worker_pci_provisioning.yml
@@ -58,8 +65,8 @@
   config:
     post_boot: head_vm_post_boot_config.yml
     SmartNIC: nmcli_config_nw_interface.yml
     SharedNIC: nmcli_config_nw_interface.yml
     Storage: storage_config.yml
   cleanup:
     NVME: nvme_cleanup.yml
-    ALL: head_vm_provisioning.yml
+    ALL: head_vm_provisioning.yml
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/authority/vnic_net_handler_config.yml` & `fabric_cf-1.5.0b3/fabric_cf/authority/vnic_net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/Readme.md` & `fabric_cf-1.5.0b3/fabric_cf/broker/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/__main__.py` & `fabric_cf-1.5.0b3/fabric_cf/broker/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/broker-yes.xml` & `fabric_cf-1.5.0b3/fabric_cf/broker/broker-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/config.broker.yaml` & `fabric_cf-1.5.0b3/fabric_cf/broker/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/core/broker_kernel.py` & `fabric_cf-1.5.0b3/fabric_cf/broker/core/broker_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/docker-compose.yml` & `fabric_cf-1.5.0b3/fabric_cf/broker/docker-compose.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 version: '3.6'
 services:
 
   neo4j:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: broker-neo4j
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     networks:
       - frontend
       - backend
     volumes:
       - ${NEO4J_DATA_PATH_HOST:-$(pwd)/neo4j/data}:${NEO4J_DATA_PATH_DOCKER:-/data}
       - ${NEO4J_IMPORTS_PATH_HOST:-$(pwd)/neo4j/imports}:${NEO4J_IMPORTS_PATH_DOCKER:-/imports}
       - ${NEO4J_LOGS_PATH_HOST:-$(pwd)/neo4j/logs}:${NEO4J_LOGS_PATH_DOCKER:-/logs}
       - ../../../neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ../../../neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_bolt_listen__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_http_advertised__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_http_listen__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_https_advertised__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
-      - NEO4J_dbms_connector_https_listen__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
+      - NEO4J_server_bolt_advertised__address=${NEO4J_server_bolt_advertised__address:-server:7687}
+      - NEO4J_server_bolt_listen__address=${NEO4J_server_bolt_advertised__address:-server:7687}
+      - NEO4J_server_http_advertised__address=${NEO4J_server_http_advertised__address:-server:7474}
+      - NEO4J_server_http_listen__address=${NEO4J_server_http_advertised__address:-server:7474}
+      - NEO4J_server_https_advertised__address=${NEO4J_server_https_advertised__address:-server:7473}
+      - NEO4J_server_https_listen__address=${NEO4J_server_https_advertised__address:-server:7473}
+      - NEO4J_dbms_memory_pagecache_size=${NEO4J_dbms_memory_pagecache_size:-512M}
   database:
     image: fabrictestbed/postgres:12.3
     container_name: broker-db
     restart: always
     networks:
       - backend
     volumes:
@@ -49,15 +50,15 @@
     volumes:
       - ${PDP_NEW_CONF_PATH_HOST:-$(pwd)/newconf}:/conf
       - ${PDP_NEW_POLICIES_PATH_HOST:-$(pwd)/newpolicies}:/policies
   broker:
     build:
       context: ../../../
       dockerfile: Dockerfile-broker
-    image: broker:1.4.5
+    image: broker:1.5.0
     container_name: broker
     restart: always
     networks:
       - frontend
       - backend
     depends_on:
       - database
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/env.template` & `fabric_cf-1.5.0b3/fabric_cf/authority/env.template`

 * *Files 22% similar despite different names*

```diff
@@ -17,28 +17,29 @@
 NEO4J_IMPORTS_PATH_DOCKER=/imports
 NEO4J_IMPORTS_PATH_HOST=./neo4j/imports
 NEO4J_LOGS_PATH_DOCKER=/logs
 NEO4J_LOGS_PATH_HOST=./neo4j/logs
 NEO4J_PASS=password
 NEO4J_UID=1000
 NEO4J_USER=neo4j
-NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:8687
-NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:8687
-NEO4J_dbms_connector_http_advertised__address=0.0.0.0:8474
-NEO4J_dbms_connector_http_listen__address=0.0.0.0:8474
-NEO4J_dbms_connector_https_advertised__address=0.0.0.0:8473
-NEO4J_dbms_connector_https_listen__address=0.0.0.0:8473
+NEO4J_server_bolt_advertised__address=:7687
+NEO4J_server_bolt_listen__address=:7687
+NEO4J_server_http_advertised__address=:7474
+NEO4J_server_http_listen__address=:7474
+NEO4J_server_https_advertised__address=:7473
+NEO4J_server_https_listen__address=:7473
+NEO4J_dbms_memory_pagecache_size=2G
 
 # postgres configuration
 POSTGRES_HOST=database
 POSTGRES_PORT=5432
 POSTGRES_USER=fabric
 POSTGRES_PASSWORD=fabric
 PGDATA=/var/lib/postgresql/data/pgdata
-POSTGRES_DB=broker
+POSTGRES_DB=am
 
 PDP_NEW_CONF_PATH_HOST=./pdp/conf
 PDP_NEW_POLICIES_PATH_HOST=./pdp/policies
 PDP_GID=1000
 PDP_UID=1000
 
 CF_GID=1000
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.0b3/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/pdp.xml` & `fabric_cf-1.5.0b3/fabric_cf/broker/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/setup.sh` & `fabric_cf-1.5.0b3/fabric_cf/broker/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/test/broker.py` & `fabric_cf-1.5.0b3/fabric_cf/broker/test/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/broker/test/test.yaml` & `fabric_cf-1.5.0b3/fabric_cf/broker/test/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: localhost:9092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://0.0.0.0:8081
   kafka-key-schema: ../../../schema/key.avsc
   kafka-value-schema: ../../../schema/message.avsc
   kafka-ssl-ca-location:
   kafka-ssl-certificate-location:
   kafka-ssl-key-location:
   kafka-ssl-key-password:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/README.md` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 Resource | Action | Input | Output
 :--------|:----:|:---:|:---:
 `/` | GET: Retrieve a listing of user slices |  | Slice Format
 `/{slice_id}` | GET: Retrieve Slice properties | `slice_id` Slice ID | Slice Format
 `/create` | POST: Request to create slice as described in the request. Request would be a graph ML describing the requested resources. Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources. | `sliceName` Slice Name, `sshKey` SSH Key, `leaseEndTime` Lease End Time, `GraphML Representing the Slice` body | Slice Format
 `/renew/{slice_id}` | POST: Request to extend slice be renewed with their expiration extended. If possible, the orchestrator should extend the slivers to the requested expiration time, or to a sooner time if policy limits apply. | `slice_id` Slice ID, `newLeaseEndTime` New Lease End Time for the Slice | Slice Format
 `/delete/{slice_id}` | DELETE: Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary, de-provisioned and un-allocated at the respective sites. | `slice_id` Slice ID | Slice Format
+`/delete` | DELETE: Request to delete all slices of a user within a project. Email and Project Id information is available in the token. | | Slice Format
 
 Example: Slice format
 ```json
 {
   "data": [
     {
       "model": "string",
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/__main__.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import signal
 import time
 import traceback
 
 import connexion
 import prometheus_client
 import waitress
-from flask import jsonify
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.util.graceful_interrupt_handler import GracefulInterruptHandler
 from fabric_cf.orchestrator.core.exceptions import OrchestratorException
 from fabric_cf.orchestrator.swagger_server import encoder
 
 
@@ -69,14 +68,15 @@
             # start swagger
             app = connexion.App(__name__, specification_dir='swagger_server/swagger/')
             app.json = encoder.JSONEncoder
             app.add_api('swagger.yaml', arguments={'title': 'Fabric Orchestrator API'}, pythonic_params=True)
 
             # Start up the server to expose the metrics.
             waitress.serve(app, port=int(rest_port_str), threads=8)
+
             while True:
                 time.sleep(0.0001)
                 if h.interrupted:
                     GlobalsSingleton.get().stop()
                     OrchestratorKernelSingleton.get().stop_threads()
     except Exception:
         traceback.print_exc()
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/certs/fullchain.pem` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/certs/privkey.pem` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/config.orchestrator.yaml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/config.orchestrator.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -117,14 +117,25 @@
   # The number of the first tick
   time.firstTick: 0
 
   # This property controls if time advances automatically (false) or
   # manually (true)
   time.manual: false
 
+audit:
+  name: audit
+  guid: audit-guid
+  description: audit
+  kafka-topic: audit
+  kafka-sasl-mechanism:
+  kafka-sasl-producer-username:
+  kafka-sasl-producer-password:
+  kafka-sasl-consumer-username:
+  kafka-sasl-consumer-password:
+
 actor:
   type: orchestrator
   name: orchestrator
   guid: orchestrator-guid
   description: orchestrator
   kafka-topic: orchestrator-topic
   policy:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/active_status_checker.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/active_status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/bqm_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/bqm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/exceptions.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/i_status_update_callback.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/i_status_update_callback.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/orchestrator_handler.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,48 +482,63 @@
             self.logger.error(traceback.format_exc())
             self.logger.error(f"Exception occurred processing modify_slice e: {e}")
             raise e
         finally:
             if topology is not None and topology.graph_model is not None:
                 topology.graph_model.delete_graph()
 
-    def delete_slice(self, *, token: str, slice_id: str = None):
+    def delete_slices(self, *, token: str, slice_id: str = None):
         """
-        Delete User Slice
+        Delete a user slice identified by slice_id if specified otherwise all user slices within a project
         :param token Fabric Identity Token
         :param slice_id Slice Id
         :raises Raises an exception in case of failure
         """
         try:
+            failed_to_delete_slice_ids = []
             controller = self.controller_state.get_management_actor()
             self.logger.debug(f"delete_slice invoked for Controller: {controller}")
 
             slice_guid = ID(uid=slice_id) if slice_id is not None else None
             fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.delete)
+            project, tags, project_name = fabric_token.get_first_project()
 
-            slice_list = controller.get_slices(slice_id=slice_guid, email=fabric_token.get_email())
+            self.logger.debug(f"Get Slices: {project} {fabric_token.get_email()} ")
+            states = None
+            if slice_guid is None:
+                states = [SliceState.StableError.value,
+                          SliceState.StableOK.value,
+                          SliceState.ModifyOK.value,
+                          SliceState.ModifyError.value]
+            slice_list = controller.get_slices(slice_id=slice_guid, email=fabric_token.get_email(),
+                                               project=project, states=states)
 
             if slice_list is None or len(slice_list) == 0:
-                raise OrchestratorException(f"Slice# {slice_id} not found",
-                                            http_error_code=NOT_FOUND)
-
-            slice_object = next(iter(slice_list))
-
-            slice_state = SliceState(slice_object.get_state())
-            if SliceState.is_dead_or_closing(state=slice_state):
-                raise OrchestratorException(f"Slice# {slice_id} already closed",
-                                            http_error_code=BAD_REQUEST)
-
-            if not SliceState.is_stable(state=slice_state) and not SliceState.is_modified(state=slice_state):
-                self.logger.info(f"Unable to delete Slice# {slice_guid} that is not yet stable, try again later")
-                raise OrchestratorException(f"Unable to delete Slice# {slice_guid} that is not yet stable, "
-                                            f"try again later")
+                if slice_id is not None:
+                    msg = f"Slice# {slice_id} not found"
+                    raise OrchestratorException(msg, http_error_code=NOT_FOUND)
 
             self.__authorize_request(id_token=token, action_id=ActionId.delete)
-            controller.close_reservations(slice_id=slice_guid)
+
+            for slice_object in slice_list:
+                slice_state = SliceState(slice_object.get_state())
+                if SliceState.is_dead_or_closing(state=slice_state):
+                    self.logger.debug(f"Slice# {slice_object.get_slice_id()} already closed")
+                    continue
+
+                if not SliceState.is_stable(state=slice_state) and not SliceState.is_modified(state=slice_state):
+                    self.logger.info(f"Unable to delete Slice# {slice_object.get_slice_id()} that is not yet stable, "
+                                     f"try again later")
+                    failed_to_delete_slice_ids.append(slice_object.get_slice_id())
+                    continue
+
+                controller.close_reservations(slice_id=ID(uid=slice_object.get_slice_id()))
+            if len(failed_to_delete_slice_ids) > 0:
+                raise OrchestratorException(f"Unable to delete Slices {failed_to_delete_slice_ids} that are not yet "
+                                            f"stable, try again later")
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.logger.error(f"Exception occurred processing delete_slice e: {e}")
             raise e
 
     def modify_accept(self, *, token: str, slice_id: str) -> dict:
         """
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_converter.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_status_update.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/reservation_status_update_thread.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/response_builder.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/response_builder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/slice_defer_thread.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/slice_defer_thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import traceback
 
 from fabric_cf.actor.core.kernel.reservation_states import ReservationStates
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.iterable_queue import IterableQueue
 from fabric_cf.orchestrator.core.exceptions import OrchestratorException
 from fabric_cf.orchestrator.core.orchestrator_slice_wrapper import OrchestratorSliceWrapper
-from fabric_cf.orchestrator.core.reservation_status_update import ReservationStatusUpdate
 
 
 class SliceDeferThread:
     """
     This runs as a standalone thread started by Orchestrator and deals with issuing demand for the slivers for
     the newly created slices. The purpose of this thread is to help orchestrator respond back to the create
     without waiting for the slivers to be demanded
@@ -181,15 +180,15 @@
                 self.logger.debug(f"Issuing close for reservation: {r}")
                 self.mgmt_actor.close_reservation(rid=ID(uid=r))
 
             for rid, modified_res in controller_slice.computed_modify_reservations.items():
                 self.logger.debug(f"Issuing extend for modified reservation: {rid}")
                 if not self.mgmt_actor.extend_reservation(reservation=ID(uid=rid), sliver=modified_res.sliver,
                                                           new_end_time=None, dependencies=modified_res.dependencies):
-                    self.logger.error(f"Could not demand resources: {self.mgmt_actor.get_last_error()}")
+                    self.logger.error(f"Could not extend rid: {rid} error: {self.mgmt_actor.get_last_error()}")
                     continue
                 self.logger.debug(f"Issued extend for reservation #{rid} successfully")
 
             for r in controller_slice.computed_modify_properties_reservations:
                 self.logger.debug(f"Issuing modify for reservation: {r}")
                 self.mgmt_actor.modify_reservation(rid=ID(uid=str(r.get_reservation_id())),
                                                    modified_sliver=r.sliver)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/status_checker.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/core/watch_entry.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/watch_entry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/docker-compose.yml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/docker-compose.yml`

 * *Files 16% similar despite different names*

```diff
@@ -12,35 +12,36 @@
       - 0.0.0.0:443:443
     volumes:
       - ./nginx/default.conf:/etc/nginx/conf.d/default.conf
       - ./certs/fullchain.pem:/etc/ssl/public.pem
       - ./certs/privkey.pem:/etc/ssl/private.pem
     restart: always
   neo4j:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: orchestrator-neo4j
     restart: always
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     networks:
       - frontend
       - backend
     volumes:
       - ${NEO4J_DATA_PATH_HOST:-$(pwd)/neo4j/data}:${NEO4J_DATA_PATH_DOCKER:-/data}
       - ${NEO4J_IMPORTS_PATH_HOST:-$(pwd)/neo4j/imports}:${NEO4J_IMPORTS_PATH_DOCKER:-/imports}
       - ${NEO4J_LOGS_PATH_HOST:-$(pwd)/neo4j/logs}:${NEO4J_LOGS_PATH_DOCKER:-/logs}
       - ../../../neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ../../../neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_bolt_listen__address=${NEO4J_dbms_connector_bolt_advertised__address:-0.0.0.0:7687}
-      - NEO4J_dbms_connector_http_advertised__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_http_listen__address=${NEO4J_dbms_connector_http_advertised__address:-0.0.0.0:7474}
-      - NEO4J_dbms_connector_https_advertised__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
-      - NEO4J_dbms_connector_https_listen__address=${NEO4J_dbms_connector_https_advertised__address:-0.0.0.0:7473}
+      - NEO4J_server_bolt_advertised__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_bolt_listen__address=${NEO4J_server_bolt_advertised__address:-:7687}
+      - NEO4J_server_http_advertised__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_http_listen__address=${NEO4J_server_http_advertised__address:-:7474}
+      - NEO4J_server_https_advertised__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_server_https_listen__address=${NEO4J_server_https_advertised__address:-:7473}
+      - NEO4J_dbms_memory_pagecache_size=${NEO4J_dbms_memory_pagecache_size:-512M}
   database:
     image: fabrictestbed/postgres:12.3
     container_name: orchestrator-db
     restart: always
     networks:
       - backend
     volumes:
@@ -63,15 +64,15 @@
     volumes:
       - ${PDP_NEW_CONF_PATH_HOST:-$(pwd)/newconf}:/conf
       - ${PDP_NEW_POLICIES_PATH_HOST:-$(pwd)/newpolicies}:/policies
   orchestrator:
     build:
       context: ../../../
       dockerfile: Dockerfile-orchestrator
-    image: orchestrator:1.4.5
+    image: orchestrator:1.5.0
     container_name: orchestrator
     restart: always
     depends_on:
       - database
       - neo4j
     networks:
       - frontend
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/nginx/default.conf` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/nginx/default.conf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/openapi.json` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935881423883656%*

 * *Differences: {"'paths'": "{'/slices': {'get': {'parameters': {2: {'schema': {'maximum': 200}}}}}, "*

 * *            "'/slices/create': {'post': {'parameters': {0: {'schema': {'minLength': 3}}}}}, "*

 * *            "'/slices/delete': OrderedDict([('delete', OrderedDict([('tags', ['slices']), "*

 * *            "('summary', 'Delete all slices for a User within a project.'), ('description', "*

 * *            "'Delete all slices for a User within a project. User identity email and project id is "*

 * *            "available in the bearer token.\ […]*

```diff
@@ -733,15 +733,15 @@
                         "explode": true,
                         "in": "query",
                         "name": "limit",
                         "required": false,
                         "schema": {
                             "default": 5,
                             "format": "int32",
-                            "maximum": 20,
+                            "maximum": 200,
                             "minimum": 1,
                             "type": "integer"
                         },
                         "style": "form"
                     },
                     {
                         "description": "number of items to skip before starting to collect the result set",
@@ -838,14 +838,15 @@
                     {
                         "description": "Slice Name",
                         "explode": true,
                         "in": "query",
                         "name": "name",
                         "required": true,
                         "schema": {
+                            "minLength": 3,
                             "type": "string"
                         },
                         "style": "form"
                     },
                     {
                         "description": "User SSH Key",
                         "explode": true,
@@ -941,14 +942,90 @@
                 ],
                 "summary": "Create slice",
                 "tags": [
                     "slices"
                 ]
             }
         },
+        "/slices/delete": {
+            "delete": {
+                "description": "Delete all slices for a User within a project. User identity email and project id is available in the bearer token.\n",
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_200_ok_no_content"
+                                }
+                            }
+                        },
+                        "description": "OK"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_400_bad_request"
+                                }
+                            }
+                        },
+                        "description": "Bad Request"
+                    },
+                    "401": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_401_unauthorized"
+                                }
+                            }
+                        },
+                        "description": "Unauthorized"
+                    },
+                    "403": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_403_forbidden"
+                                }
+                            }
+                        },
+                        "description": "Forbidden"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_404_not_found"
+                                }
+                            }
+                        },
+                        "description": "Not Found"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_500_internal_server_error"
+                                }
+                            }
+                        },
+                        "description": "Internal Server Error"
+                    }
+                },
+                "security": [
+                    {
+                        "bearerAuth": []
+                    }
+                ],
+                "summary": "Delete all slices for a User within a project.",
+                "tags": [
+                    "slices"
+                ]
+            }
+        },
         "/slices/delete/{slice_id}": {
             "delete": {
                 "description": "Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary, de-provisioned and un-allocated at the respective sites.\n",
                 "parameters": [
                     {
                         "description": "Slice identified by universally unique identifier",
                         "explode": false,
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/orchestrator-yes.xml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/orchestrator-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/pdp.xml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/setup.sh` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,25 @@
     :type lease_end_time: str
 
     :rtype: Slivers
     """
     return rc.slices_create_post(body, name, ssh_key, lease_end_time)
 
 
+def slices_delete_delete():  # noqa: E501
+    """Delete all slices for a User within a project.
+
+    Delete all slices for a User within a project. User identity email and project id is available in the bearer token.  # noqa: E501
+
+
+    :rtype: Status200OkNoContent
+    """
+    return rc.slices_delete_delete()
+
+
 def slices_delete_slice_id_delete(slice_id):  # noqa: E501
     """Delete slice.
 
     Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary,
     de-provisioned and un-allocated at the respective sites.  # noqa: E501
 
     :param slice_id: Slice identified by universally unique identifier
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/encoder.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/__init__.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/base_model_.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/resource.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/resources.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slice.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slice_details.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slices.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/sliver.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/slivers.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/version.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/models/version_data.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/constants.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 
 RESOURCES_PATH = '/resources'
 PORTAL_RESOURCES_PATH = '/portalresources'
 
 SLICES_CREATE_PATH = '/slices/create'
 SLICES_MODIFY_PATH = '/slices/modify/{slice_id}'
 SLICES_MODIFY_ACCEPT_PATH = '/slices/modify/{slice_id}/accept'
-SLICES_DELETE_PATH = '/slices/delete/{slice_id}'
+SLICES_DELETE_PATH = '/slices/delete'
+SLICES_DELETE_SLICE_ID_PATH = '/slices/delete/{slice_id}'
 SLICES_GET_PATH = '/slices'
 SLICES_GET_SLICE_ID_PATH = '/slices/{slice_id}'
 SLICES_RENEW_PATH = '/slices/renew/{slice_id}'
 SLICE_STATUS_SLICE_ID_PATH = '/slices/status/{slice_id}'
 
 
 SLIVERS_GET_PATH = '/slivers'
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/cors_response.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/cors_response.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/resources_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/slices_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slices_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from fabric_cf.orchestrator.swagger_server.models.slice_details import SliceDetails  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent  # noqa: E501
 from fabric_cf.orchestrator.swagger_server import received_counter, success_counter, failure_counter
 from fabric_cf.orchestrator.swagger_server.response.constants import POST_METHOD, SLICES_CREATE_PATH, DELETE_METHOD, \
     SLICES_DELETE_PATH, GET_METHOD, SLICES_GET_PATH, SLICES_RENEW_PATH, SLICES_GET_SLICE_ID_PATH, SLICES_MODIFY_PATH, \
-    SLICES_MODIFY_ACCEPT_PATH
+    SLICES_MODIFY_ACCEPT_PATH, SLICES_DELETE_SLICE_ID_PATH
 from fabric_cf.orchestrator.swagger_server.response.utils import get_token, cors_error_response, cors_success_response
 
 
 def slices_create_post(body, name, ssh_key, lease_end_time) -> Slivers:  # noqa: E501
     """Create slice
 
     Request to create slice as described in the request. Request would be a graph ML describing the requested resources.
@@ -83,49 +83,84 @@
         return cors_error_response(error=e)
     except Exception as e:
         logger.exception(e)
         failure_counter.labels(POST_METHOD, SLICES_CREATE_PATH).inc()
         return cors_error_response(error=e)
 
 
+def slices_delete_delete():  # noqa: E501
+    """Delete all slices for a User within a project.
+
+    Delete all slices for a User within a project. User identity email and project id is available in the bearer token.  # noqa: E501
+
+
+    :rtype: Status200OkNoContent
+    """
+    handler = OrchestratorHandler()
+    logger = handler.get_logger()
+    received_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+    try:
+        token = get_token()
+        handler.delete_slices(token=token)
+        success_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+
+        slice_info = Status200OkNoContentData()
+        slice_info.details = f"Slices for user have been successfully deleted"
+        response = Status200OkNoContent()
+        response.data = [slice_info]
+        response.size = len(response.data)
+        response.status = 200
+        response.type = 'no_content'
+        return cors_success_response(response_body=response)
+
+    except OrchestratorException as e:
+        logger.exception(e)
+        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+        return cors_error_response(error=e)
+    except Exception as e:
+        logger.exception(e)
+        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+        return cors_error_response(error=e)
+
+
 def slices_delete_slice_id_delete(slice_id) -> Status200OkNoContent:  # noqa: E501
     """Delete slice.
 
     Request to delete slice. On success, resources associated with slice or sliver are stopped if necessary,
     de-provisioned and un-allocated at the respective sites.  # noqa: E501
 
     :param slice_id: Slice identified by universally unique identifier
     :type slice_id: str
 
     :rtype: Status200OkNoContent
     """
     handler = OrchestratorHandler()
     logger = handler.get_logger()
-    received_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+    received_counter.labels(DELETE_METHOD, SLICES_DELETE_SLICE_ID_PATH).inc()
     try:
         token = get_token()
-        handler.delete_slice(token=token, slice_id=slice_id)
-        success_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+        handler.delete_slices(token=token, slice_id=slice_id)
+        success_counter.labels(DELETE_METHOD, SLICES_DELETE_SLICE_ID_PATH).inc()
 
         slice_info = Status200OkNoContentData()
         slice_info.details = f"Slice '{slice_id}' has been successfully deleted"
         response = Status200OkNoContent()
         response.data = [slice_info]
         response.size = len(response.data)
         response.status = 200
         response.type = 'no_content'
         return cors_success_response(response_body=response)
 
     except OrchestratorException as e:
         logger.exception(e)
-        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_SLICE_ID_PATH).inc()
         return cors_error_response(error=e)
     except Exception as e:
         logger.exception(e)
-        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_PATH).inc()
+        failure_counter.labels(DELETE_METHOD, SLICES_DELETE_SLICE_ID_PATH).inc()
         return cors_error_response(error=e)
 
 
 def slices_get(name=None, states=None, limit=None, offset=None) -> Slices:  # noqa: E501
     """Retrieve a listing of user slices
 
     Retrieve a listing of user slices # noqa: E501
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/utils.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/response/version_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/version_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from fabric_cf.orchestrator.swagger_server.models import VersionData
 from fabric_cf.orchestrator.swagger_server.models.version import Version  # noqa: E501
 from fabric_cf.orchestrator.swagger_server import received_counter, success_counter, failure_counter, __API_REFERENCE__
 from fabric_cf.orchestrator.swagger_server.response.constants import VERSIONS_PATH, GET_METHOD
 
-from fabric_cf import __VERSION__
+from fabric_cf import __version__
 from fabric_cf.orchestrator.swagger_server.response.cors_response import cors_500, cors_200
 
 
 def version_get() -> Version:  # noqa: E501
     """version
 
     Version # noqa: E501
@@ -42,15 +42,15 @@
     """
     received_counter.labels(GET_METHOD, VERSIONS_PATH).inc()
     from fabric_cf.actor.core.container.globals import GlobalsSingleton
     logger = GlobalsSingleton.get().get_logger()
     try:
         version = VersionData()
         version.reference = __API_REFERENCE__
-        version.version = __VERSION__
+        version.version = __version__
         response = Version()
         response.data = [version]
         response.size = len(response.data)
         response.status = 200
         response.type = 'version'
         success_counter.labels(GET_METHOD, VERSIONS_PATH).inc()
         return cors_200(response_body=response)
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -365,16 +365,16 @@
       - name: name
         in: query
         description: Slice Name
         required: true
         style: form
         explode: true
         schema:
-          type: string
           minLength: 3
+          type: string
       - name: ssh_key
         in: query
         description: User SSH Key
         required: true
         style: form
         explode: true
         schema:
@@ -641,14 +641,62 @@
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/status_200_ok_no_content'
+        "400":
+          description: Bad Request
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_400_bad_request'
+        "401":
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_401_unauthorized'
+        "403":
+          description: Forbidden
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_403_forbidden'
+        "404":
+          description: Not Found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_404_not_found'
+        "500":
+          description: Internal Server Error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_500_internal_server_error'
+      security:
+      - bearerAuth: []
+      x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slices_controller
+  /slices/delete:
+    delete:
+      tags:
+      - slices
+      summary: Delete all slices for a User within a project.
+      description: |
+        Delete all slices for a User within a project. User identity email and project id is available in the bearer token.
+      operationId: slices_delete_delete
+      responses:
+        "200":
+          description: OK
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_200_ok_no_content'
         "400":
           description: Bad Request
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/status_400_bad_request'
         "401":
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,25 @@
             method='POST',
             data=json.dumps(body),
             content_type='text/plain',
             query_string=query_string)
         self.assert200(response,
                        'Response body is : ' + response.data.decode('utf-8'))
 
+    def test_slices_delete_delete(self):
+        """Test case for slices_delete_delete
+
+        Delete all slices for a User within a project.
+        """
+        response = self.client.open(
+            '//slices/delete',
+            method='DELETE')
+        self.assert200(response,
+                       'Response body is : ' + response.data.decode('utf-8'))
+
     def test_slices_delete_slice_id_delete(self):
         """Test case for slices_delete_slice_id_delete
 
         Delete slice.
         """
         response = self.client.open(
             '//slices/delete/{slice_id}'.format(slice_id='slice_id_example'),
@@ -52,15 +63,15 @@
     def test_slices_get(self):
         """Test case for slices_get
 
         Retrieve a listing of user slices
         """
         query_string = [('name', 'name_example'),
                         ('states', 'states_example'),
-                        ('limit', 20),
+                        ('limit', 200),
                         ('offset', 1)]
         response = self.client.open(
             '//slices',
             method='GET',
             query_string=query_string)
         self.assert200(response,
                        'Response body is : ' + response.data.decode('utf-8'))
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/type_util.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/type_util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/swagger_server/util.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/orchestrator.py` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/orchestrator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/test/test.yaml` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: localhost:9092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://0.0.0.0:8081
   kafka-key-schema: ../../../schema/key.avsc
   kafka-value-schema: ../../../schema/message.avsc
   kafka-ssl-ca-location:
   kafka-ssl-certificate-location:
   kafka-ssl-key-location:
   kafka-ssl-key-password:
```

### Comparing `fabric_cf-1.5.0b2/fabric_cf/orchestrator/update_swagger_stub.sh` & `fabric_cf-1.5.0b3/fabric_cf/orchestrator/update_swagger_stub.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/am-pod.png` & `fabric_cf-1.5.0b3/images/am-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/am.png` & `fabric_cf-1.5.0b3/images/am.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/broker-pod.png` & `fabric_cf-1.5.0b3/images/broker-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/broker.png` & `fabric_cf-1.5.0b3/images/broker.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/cf.png` & `fabric_cf-1.5.0b3/images/cf.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/orchestrator-pod.png` & `fabric_cf-1.5.0b3/images/orchestrator-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/images/orchestrator.png` & `fabric_cf-1.5.0b3/images/orchestrator.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/AL2S.graphml` & `fabric_cf-1.5.0b3/neo4j/AL2S.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/LBNL-ad.graphml` & `fabric_cf-1.5.0b3/neo4j/LBNL-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/Network-ad.graphml` & `fabric_cf-1.5.0b3/neo4j/Network-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/RENCI-ad.graphml` & `fabric_cf-1.5.0b3/neo4j/RENCI-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/UKY-ad.graphml` & `fabric_cf-1.5.0b3/neo4j/UKY-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/UKY2.graphml` & `fabric_cf-1.5.0b3/neo4j/UKY2.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/abqm.graphml` & `fabric_cf-1.5.0b3/neo4j/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/certs/fullchain.pem` & `fabric_cf-1.5.0b3/neo4j/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/neo4j/certs/privkey.pem` & `fabric_cf-1.5.0b3/neo4j/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/psql.upgrade` & `fabric_cf-1.5.0b3/psql.upgrade`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/pyproject.toml` & `fabric_cf-1.5.0b3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,36 @@
 description = "Fabric Control Framework"
 dynamic = ["version"]
 
 keywords = ["Swagger", "Fabric Control Framework"]
 
 requires-python = '>=3.9'
 dependencies = [
-    "requests>=2.28.1",
-    "cryptography==3.3.2",
+    "requests >= 2.28.1",
+    "cryptography==40.0.2",
     "psycopg2-binary",
     "sqlalchemy",
     "waitress",
     "prometheus_client",
     "connexion",
     "swagger-ui-bundle",
-    "fabric_fss_utils==1.4.0",
     "PyYAML",
-    "fabric-message-bus==1.4.0",
-    "fabric-fim==1.4.6"]
+    "fabric_fss_utils==1.5.0rc1",
+    "fabric-message-bus==1.5.0b1",
+    "fabric-fim==1.5.0b4"]
+
+[project.optional-dependencies]
+test = ["pytest",
+        "flask_testing",
+        "coverage>=4.0.3",
+        "nose>=1.3.7",
+        "pluggy>=0.3.1",
+        "py>=1.4.31",
+        "randomize>=0.13"
+        ]
 
 [project.urls]
 Home = "https://fabric-testbed.net/"
 Sources = "https://github.com/fabric-testbed/ControlFramework"
+
+[tool.flit.module]
+name = "fabric_cf"
```

### Comparing `fabric_cf-1.5.0b2/secrets/create-certs.sh` & `fabric_cf-1.5.0b3/secrets/create-certs.sh`

 * *Files 13% similar despite different names*

```diff
@@ -2,44 +2,43 @@
 
 set -o nounset \
     -o errexit \
     -o verbose \
     -o xtrace
 
 # Generate CA key
-openssl req -new -x509 -keyout snakeoil-ca-1.key -out snakeoil-ca-1.crt -days 365 -subj '/CN=ca1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric
+openssl req -new -x509 -keyout snakeoil-ca-1.key -out snakeoil-ca-1.crt -days 365 -subj '/CN=ca1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric 
 cp snakeoil-ca-1.crt snakeoil-ca-1-copy.crt
-# openssl req -new -x509 -keyout snakeoil-ca-2.key -out snakeoil-ca-2.crt -days 365 -subj '/CN=ca2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric
 
 # kafkacat1
 openssl genrsa -des3 -passout "pass:fabric" -out kafkacat1.client.key 2048
-openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat1.client.key -new -out kafkacat1.client.req -subj '/CN=kafkacat1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US'
-openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat1.client.req -out kafkacat1-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"
+openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat1.client.key -new -out kafkacat1.client.req -subj '/CN=kafkacat1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' 
+openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat1.client.req -out kafkacat1-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"  -sha256
 
 openssl genrsa -des3 -passout "pass:fabric" -out kafkacat2.client.key 2048
-openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat2.client.key -new -out kafkacat2.client.req -subj '/CN=kafkacat2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US'
-openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat2.client.req -out kafkacat2-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"
+openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat2.client.key -new -out kafkacat2.client.req -subj '/CN=kafkacat2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' 
+openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat2.client.req -out kafkacat2-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric" -sha256
 
 
-for i in broker1 schemaregistry producer consumer
+for i in broker1 schemaregistry producer consumer zookeeper
 do
 	echo $i
 	# Create keystores
 	keytool -genkey -noprompt \
 				 -alias $i \
-				 -dname "CN=$i.test.fabric.io, OU=TEST, O=FABRIC, L=ChapelHill, S=NC, C=US" \
+				 -dname "CN=$i, OU=TEST, O=FABRIC, L=ChapelHill, S=NC, C=US" \
 				 -keystore kafka.$i.keystore.jks \
 				 -keyalg RSA \
 				 -storepass fabric \
 				 -keypass fabric
 
 	# Create CSR, sign the key and import back into keystore
 	keytool -keystore kafka.$i.keystore.jks -alias $i -certreq -file $i.csr -storepass fabric -keypass fabric
 
-	openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in $i.csr -out $i-ca1-signed.crt -days 9999 -CAcreateserial -passin pass:fabric
+	openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in $i.csr -out $i-ca1-signed.crt -days 9999 -CAcreateserial -passin pass:fabric -sha256
 
 	keytool -keystore kafka.$i.keystore.jks -alias CARoot -import -file snakeoil-ca-1.crt -storepass fabric -keypass fabric -noprompt
 
 	keytool -keystore kafka.$i.keystore.jks -alias $i -import -file $i-ca1-signed.crt -storepass fabric -keypass fabric
 
 	# Create truststore and import the CA cert.
 	keytool -keystore kafka.$i.truststore.jks -alias CARoot -import -file snakeoil-ca-1.crt -storepass fabric -keypass fabric -noprompt
```

### Comparing `fabric_cf-1.5.0b2/tools/db_cli.py` & `fabric_cf-1.5.0b3/tools/db_cli.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b2/PKG-INFO` & `fabric_cf-1.5.0b3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: fabric_cf
-Version: 1.5.0b2
+Version: 1.5.0b3
 Summary: Fabric Control Framework
 Keywords: Swagger,Fabric Control Framework
 Author-email: Komal Thareja <kthare10@renci.org>, Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: requests>=2.28.1
-Requires-Dist: cryptography==3.3.2
+Requires-Dist: requests >= 2.28.1
+Requires-Dist: cryptography==40.0.2
 Requires-Dist: psycopg2-binary
 Requires-Dist: sqlalchemy
 Requires-Dist: waitress
 Requires-Dist: prometheus_client
 Requires-Dist: connexion
 Requires-Dist: swagger-ui-bundle
-Requires-Dist: fabric_fss_utils==1.4.0
 Requires-Dist: PyYAML
-Requires-Dist: fabric-message-bus==1.4.0
-Requires-Dist: fabric-fim==1.4.6
+Requires-Dist: fabric_fss_utils==1.5.0rc1
+Requires-Dist: fabric-message-bus==1.5.0b1
+Requires-Dist: fabric-fim==1.5.0b4
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: flask_testing ; extra == "test"
+Requires-Dist: coverage>=4.0.3 ; extra == "test"
+Requires-Dist: nose>=1.3.7 ; extra == "test"
+Requires-Dist: pluggy>=0.3.1 ; extra == "test"
+Requires-Dist: py>=1.4.31 ; extra == "test"
+Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/ControlFramework
+Provides-Extra: test
 
 [![PyPI](https://img.shields.io/pypi/v/fabric-cf?style=plastic)](https://pypi.org/project/fabric-cf/)
 
 # Control Framework
 This repository contains Fabric Control Framework and Actor implementations.
 
 ## Overview
```

