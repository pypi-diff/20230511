# Comparing `tmp/osmosispy-0.0.8.tar.gz` & `tmp/osmosispy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmosispy-0.0.8.tar", max compression
+gzip compressed data, was "osmosispy-0.0.9.tar", max compression
```

## Comparing `osmosispy-0.0.8.tar` & `osmosispy-0.0.9.tar`

### file list

```diff
@@ -1,581 +1,695 @@
--rw-r--r--   0        0        0       84 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/__init__.py
--rw-r--r--   0        0        0     5420 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2.py
--rw-r--r--   0        0        0    22313 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2_grpc.pyi
--rw-r--r--   0        0        0     4844 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.py
--rw-r--r--   0        0        0     4011 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0     1747 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1530 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     5747 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     6040 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     7846 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2590 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2353 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     2038 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     1427 2023-04-19 16:01:14.899568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.py
--rw-r--r--   0        0        0     2064 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.pyi
--rw-r--r--   0        0        0     2553 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2392 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2438 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3025 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2650 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1032 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3423 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     4624 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6246 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2801 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1955 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     1198 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     4846 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.py
--rw-r--r--   0        0        0     7170 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.pyi
--rw-r--r--   0        0        0     4181 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4505 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    12543 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    17113 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    18871 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6342 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3554 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     2940 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4358 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1763 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     7219 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py
--rw-r--r--   0        0        0    12069 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.pyi
--rw-r--r--   0        0        0     1544 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py
--rw-r--r--   0        0        0     1508 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.pyi
--rw-r--r--   0        0        0     1514 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py
--rw-r--r--   0        0        0     3338 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.pyi
--rw-r--r--   0        0        0     3015 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
--rw-r--r--   0        0        0     2955 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
--rw-r--r--   0        0        0     5144 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     1988 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi
--rw-r--r--   0        0        0    10392 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
--rw-r--r--   0        0        0    22435 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
--rw-r--r--   0        0        0    13573 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
--rw-r--r--   0        0        0     5145 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi
--rw-r--r--   0        0        0     3486 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
--rw-r--r--   0        0        0     7010 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.pyi
--rw-r--r--   0        0        0     2141 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
--rw-r--r--   0        0        0     2638 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.pyi
--rw-r--r--   0        0        0     1299 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py
--rw-r--r--   0        0        0     1502 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.pyi
--rw-r--r--   0        0        0     8339 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    13487 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12460 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4039 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2694 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0        0        0     2603 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.pyi
--rw-r--r--   0        0        0     2548 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.py
--rw-r--r--   0        0        0     2229 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0     2152 2023-04-19 16:01:14.903568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2378 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1671 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1167 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2353 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1524 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2685 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1004 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1842 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.py
--rw-r--r--   0        0        0     1640 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     2055 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.py
--rw-r--r--   0        0        0     1326 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     1730 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
--rw-r--r--   0        0        0     2012 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.pyi
--rw-r--r--   0        0        0     1475 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py
--rw-r--r--   0        0        0     1469 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     1813 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py
--rw-r--r--   0        0        0     1473 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0    12364 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py
--rw-r--r--   0        0        0    12322 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.pyi
--rw-r--r--   0        0        0    13234 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0    13772 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    13656 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15710 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    18352 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     6277 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     5830 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     4886 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     8774 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3369 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2200 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py
--rw-r--r--   0        0        0     1484 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.pyi
--rw-r--r--   0        0        0     1317 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1130 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3524 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3911 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4459 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1516 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2295 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1840 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2754 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1122 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     5368 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
--rw-r--r--   0        0        0     6820 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.pyi
--rw-r--r--   0        0        0     1616 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1163 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       98 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3288 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4370 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4483 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1586 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2563 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     3104 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     4601 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1823 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1579 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1061 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3478 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     3259 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    18149 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0    18042 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.pyi
--rw-r--r--   0        0        0    10683 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    15440 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    14598 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4657 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     6490 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     5972 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     7675 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2610 2023-04-19 16:01:14.907568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1805 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1380 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3917 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     2540 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.pyi
--rw-r--r--   0        0        0     4280 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     3413 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6210 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2105 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2129 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     2077 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     2376 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1872 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2674 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1051 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3519 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4758 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     4615 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5044 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6284 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2133 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     5094 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py
--rw-r--r--   0        0        0     4277 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.pyi
--rw-r--r--   0        0        0     1962 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     1102 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     2717 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1204 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2766 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.py
--rw-r--r--   0        0        0     5136 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.pyi
--rw-r--r--   0        0        0     3931 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     4548 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    19205 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    28351 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    26968 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     9115 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0    25592 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.py
--rw-r--r--   0        0        0    27852 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.pyi
--rw-r--r--   0        0        0    11071 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     9946 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     9842 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3547 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     3092 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
--rw-r--r--   0        0        0     8944 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.pyi
--rw-r--r--   0        0        0     5681 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.py
--rw-r--r--   0        0        0    11470 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi
--rw-r--r--   0        0        0     7765 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
--rw-r--r--   0        0        0     2466 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0     4482 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    16227 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     4985 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     5947 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     8732 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     3705 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3641 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
--rw-r--r--   0        0        0     5232 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.pyi
--rw-r--r--   0        0        0     5503 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6363 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     6525 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2441 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     9468 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py
--rw-r--r--   0        0        0     9600 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.pyi
--rw-r--r--   0        0        0     1671 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2.py
--rw-r--r--   0        0        0      838 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2_grpc.pyi
--rw-r--r--   0        0        0    14512 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2.py
--rw-r--r--   0        0        0    15688 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.py
--rw-r--r--   0        0        0     1446 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.pyi
--rw-r--r--   0        0        0     1585 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2.py
--rw-r--r--   0        0        0     1053 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      633 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2125 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2.py
--rw-r--r--   0        0        0    15126 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      627 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1507 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2.py
--rw-r--r--   0        0        0     3484 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.py
--rw-r--r--   0        0        0      628 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.pyi
--rw-r--r--   0        0        0     1588 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2.py
--rw-r--r--   0        0        0     6355 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.py
--rw-r--r--   0        0        0     1651 2023-04-19 16:01:14.911568 osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.pyi
--rw-r--r--   0        0        0     2678 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.py
--rw-r--r--   0        0        0     2821 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2_grpc.pyi
--rw-r--r--   0        0        0     3393 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2458 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     4225 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2070 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     3091 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0      933 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3153 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2.py
--rw-r--r--   0        0        0     5252 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     3224 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2.py
--rw-r--r--   0        0        0     2219 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2.pyi
--rw-r--r--   0        0        0     4328 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.py
--rw-r--r--   0        0        0     1479 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     7539 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.py
--rw-r--r--   0        0        0     9072 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2_grpc.py
--rw-r--r--   0        0        0      338 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2_grpc.pyi
--rw-r--r--   0        0        0     3310 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.py
--rw-r--r--   0        0        0     2385 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.pyi
--rw-r--r--   0        0        0     2998 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.py
--rw-r--r--   0        0        0      851 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     5008 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.py
--rw-r--r--   0        0        0     4070 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2_grpc.pyi
--rw-r--r--   0        0        0     5706 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.py
--rw-r--r--   0        0        0     4291 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.pyi
--rw-r--r--   0        0        0     5112 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1421 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2607 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2274 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    25030 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.py
--rw-r--r--   0        0        0    21172 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    28299 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     8224 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0    20488 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0    15606 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0    15268 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3758 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     3661 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.py
--rw-r--r--   0        0        0     1815 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.pyi
--rw-r--r--   0        0        0     2725 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.py
--rw-r--r--   0        0        0     1021 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     1892 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1128 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1526 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.py
--rw-r--r--   0        0        0      839 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     2533 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     1418 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     2762 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1098 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     3618 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2.py
--rw-r--r--   0        0        0     4654 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2_grpc.pyi
--rw-r--r--   0        0        0     2488 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2.py
--rw-r--r--   0        0        0     2391 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1502 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2.py
--rw-r--r--   0        0        0      971 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2_grpc.pyi
--rw-r--r--   0        0        0    11737 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2.py
--rw-r--r--   0        0        0    14874 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2.pyi
--rw-r--r--   0        0        0    16892 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.py
--rw-r--r--   0        0        0     5850 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     4208 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2.py
--rw-r--r--   0        0        0     4461 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2.pyi
--rw-r--r--   0        0        0     4260 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.py
--rw-r--r--   0        0        0     1094 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     1853 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2.py
--rw-r--r--   0        0        0     1569 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     5004 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2.py
--rw-r--r--   0        0        0     7713 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2_grpc.pyi
--rw-r--r--   0        0        0     1506 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2.py
--rw-r--r--   0        0        0     1033 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2_grpc.pyi
--rw-r--r--   0        0        0    26438 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2.py
--rw-r--r--   0        0        0    21534 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2.pyi
--rw-r--r--   0        0        0    31704 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.py
--rw-r--r--   0        0        0    10228 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     6583 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2.py
--rw-r--r--   0        0        0     7223 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2.pyi
--rw-r--r--   0        0        0     9131 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2719 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2142 2023-04-19 16:01:14.915568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1701 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     7174 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.py
--rw-r--r--   0        0        0     6751 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2_grpc.pyi
--rw-r--r--   0        0        0     3342 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     2474 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     4491 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     1591 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     2885 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2238 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2807 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0     3705 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2_grpc.pyi
--rw-r--r--   0        0        0     4964 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.py
--rw-r--r--   0        0        0     4479 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2_grpc.pyi
--rw-r--r--   0        0        0    10336 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     8210 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0    12358 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     4052 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     1967 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.py
--rw-r--r--   0        0        0     1973 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2_grpc.pyi
--rw-r--r--   0        0        0     2951 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.py
--rw-r--r--   0        0        0     3343 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     1742 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2.py
--rw-r--r--   0        0        0     1148 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2_grpc.pyi
--rw-r--r--   0        0        0    23389 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2.py
--rw-r--r--   0        0        0    23392 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2.pyi
--rw-r--r--   0        0        0    29546 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.py
--rw-r--r--   0        0        0    10416 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     4584 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.py
--rw-r--r--   0        0        0     7676 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2_grpc.pyi
--rw-r--r--   0        0        0     5831 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2.py
--rw-r--r--   0        0        0     6556 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2.pyi
--rw-r--r--   0        0        0    10061 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.py
--rw-r--r--   0        0        0     3517 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     3000 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0     3601 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2_grpc.pyi
--rw-r--r--   0        0        0     1845 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.py
--rw-r--r--   0        0        0     1055 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2_grpc.pyi
--rw-r--r--   0        0        0     3037 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2609 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2136 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.py
--rw-r--r--   0        0        0     1124 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2_grpc.pyi
--rw-r--r--   0        0        0     5572 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4415 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     6778 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2658 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     6212 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.py
--rw-r--r--   0        0        0     6710 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.pyi
--rw-r--r--   0        0        0     9732 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.py
--rw-r--r--   0        0        0     2539 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.pyi
--rw-r--r--   0        0        0     2711 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     2498 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0    10057 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     7944 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     9820 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2456 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0     4519 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.py
--rw-r--r--   0        0        0     4069 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2_grpc.pyi
--rw-r--r--   0        0        0     1786 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.py
--rw-r--r--   0        0        0     1124 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2_grpc.pyi
--rw-r--r--   0        0        0     1663 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.py
--rw-r--r--   0        0        0     1258 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2_grpc.pyi
--rw-r--r--   0        0        0     2455 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.py
--rw-r--r--   0        0        0     1683 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2_grpc.pyi
--rw-r--r--   0        0        0     6233 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.py
--rw-r--r--   0        0        0     4174 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.pyi
--rw-r--r--   0        0        0     8242 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.py
--rw-r--r--   0        0        0     2885 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.pyi
--rw-r--r--   0        0        0    21205 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2.py
--rw-r--r--   0        0        0    48273 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2.pyi
--rw-r--r--   0        0        0    25991 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.py
--rw-r--r--   0        0        0     6123 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     1471 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2.py
--rw-r--r--   0        0        0     1266 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2_grpc.pyi
--rw-r--r--   0        0        0     2208 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2.py
--rw-r--r--   0        0        0     3976 2023-04-19 16:01:14.919568 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2_grpc.pyi
--rw-r--r--   0        0        0     1222 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2.py
--rw-r--r--   0        0        0     1024 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     3488 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2.py
--rw-r--r--   0        0        0     3801 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2173 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2.py
--rw-r--r--   0        0        0     1682 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2_grpc.pyi
--rw-r--r--   0        0        0     3521 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2.py
--rw-r--r--   0        0        0     5667 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2_grpc.pyi
--rw-r--r--   0        0        0     3858 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2.py
--rw-r--r--   0        0        0     6507 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2_grpc.pyi
--rw-r--r--   0        0        0    10988 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2.py
--rw-r--r--   0        0        0    18122 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2231 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2.py
--rw-r--r--   0        0        0     3281 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2_grpc.pyi
--rw-r--r--   0        0        0     1550 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2.py
--rw-r--r--   0        0        0     1743 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2_grpc.pyi
--rw-r--r--   0        0        0      937 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/__init__.py
--rw-r--r--   0        0        0      171 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/exceptions.py
--rw-r--r--   0        0        0    10498 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/grpc_client.py
--rw-r--r--   0        0        0      494 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/pytypes/__init__.py
--rw-r--r--   0        0        0     2669 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/pytypes/common.py
--rw-r--r--   0        0        0     3890 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/pytypes/event.py
--rw-r--r--   0        0        0     2411 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/pytypes/network.py
--rw-r--r--   0        0        0     4308 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/pytypes/tx_resp.py
--rw-r--r--   0        0        0     6185 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/sdk.py
--rw-r--r--   0        0        0      183 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/__init__.py
--rw-r--r--   0        0        0     3247 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/binance.py
--rw-r--r--   0        0        0     2077 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/client.py
--rw-r--r--   0        0        0      948 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/osmosis.py
--rw-r--r--   0        0        0      126 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/trade_data.py
--rw-r--r--   0        0        0      119 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/trading_client/types.py
--rw-r--r--   0        0        0    12879 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/tx.py
--rw-r--r--   0        0        0     9485 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/utils.py
--rw-r--r--   0        0        0    11658 2023-04-19 16:01:14.923569 osmosispy-0.0.8/osmosispy/wallet.py
--rw-r--r--   0        0        0      924 2023-04-19 16:01:14.923569 osmosispy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 osmosispy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/confio/__init__.py
+-rw-r--r--   0        0        0     5420 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2.py
+-rw-r--r--   0        0        0    22610 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2_grpc.pyi
+-rw-r--r--   0        0        0       24 2023-05-11 15:07:28.491743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/__init__.py
+-rw-r--r--   0        0        0     4844 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.py
+-rw-r--r--   0        0        0     4086 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1747 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1555 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5747 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6240 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     7846 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2590 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       30 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2353 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     2088 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1427 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.py
+-rw-r--r--   0        0        0     2114 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2553 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2442 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2438 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3075 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2650 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1032 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3423 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     4774 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6246 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2801 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       29 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1955 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     1223 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4846 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.py
+-rw-r--r--   0        0        0     7345 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4181 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4580 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12543 2023-05-11 15:07:28.495743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    17613 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    18871 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6342 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3554 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3040 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4358 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1763 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       29 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/__init__.py
+-rw-r--r--   0        0        0     7219 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py
+-rw-r--r--   0        0        0    12319 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1544 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py
+-rw-r--r--   0        0        0     1558 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py
+-rw-r--r--   0        0        0     3388 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2_grpc.pyi
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3015 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py
+-rw-r--r--   0        0        0     3055 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi
+-rw-r--r--   0        0        0     5144 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     1988 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi
+-rw-r--r--   0        0        0       49 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/__init__.py
+-rw-r--r--   0        0        0    10392 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py
+-rw-r--r--   0        0        0    23085 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi
+-rw-r--r--   0        0        0    13573 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py
+-rw-r--r--   0        0        0     5145 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi
+-rw-r--r--   0        0        0       39 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3486 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py
+-rw-r--r--   0        0        0     7210 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2141 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py
+-rw-r--r--   0        0        0     2713 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1299 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py
+-rw-r--r--   0        0        0     1527 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2_grpc.pyi
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/__init__.py
+-rw-r--r--   0        0        0     8339 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    13862 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12460 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4039 2023-05-11 15:07:28.499743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       37 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2757 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0        0        0     2703 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2548 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.py
+-rw-r--r--   0        0        0     2304 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2152 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0       31 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1192 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2353 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1574 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2685 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1004 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       31 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/__init__.py
+-rw-r--r--   0        0        0     1842 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.py
+-rw-r--r--   0        0        0     1690 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/__init__.py
+-rw-r--r--   0        0        0     2055 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.py
+-rw-r--r--   0        0        0     1351 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0       48 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py
+-rw-r--r--   0        0        0     2062 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2_grpc.pyi
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py
+-rw-r--r--   0        0        0     1519 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/__init__.py
+-rw-r--r--   0        0        0     1813 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py
+-rw-r--r--   0        0        0     1523 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0       37 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/__init__.py
+-rw-r--r--   0        0        0    12364 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py
+-rw-r--r--   0        0        0    12622 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13234 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0    13972 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.503743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13656 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    16160 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    18352 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     6277 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5830 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     5086 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     8774 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3369 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2200 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py
+-rw-r--r--   0        0        0     1509 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1317 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1155 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3524 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4011 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4459 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1516 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2295 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1890 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2754 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1122 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/__init__.py
+-rw-r--r--   0        0        0     5368 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py
+-rw-r--r--   0        0        0     6920 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1616 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1188 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3288 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4470 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4483 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1586 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2563 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     3204 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     4601 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1823 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1579 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1086 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0       28 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     3284 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18149 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0    18264 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10683 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    15840 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    14598 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4657 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6490 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6172 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     7675 2023-05-11 15:07:28.507743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2610 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       29 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1805 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1405 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3917 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     2590 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4280 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     3563 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6210 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2105 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       31 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2129 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     2127 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2376 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1922 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2674 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1051 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3519 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4858 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4615 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     5194 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6284 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2133 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5094 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py
+-rw-r--r--   0        0        0     4327 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1962 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     1152 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     2717 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1204 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2766 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.py
+-rw-r--r--   0        0        0     5176 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3931 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     4598 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    19205 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    29051 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    26968 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     9115 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0    25592 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.py
+-rw-r--r--   0        0        0    28338 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11071 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    10196 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     9842 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3547 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       27 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3092 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py
+-rw-r--r--   0        0        0     9075 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.511743 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/__init__.py
+-rw-r--r--   0        0        0     5681 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.py
+-rw-r--r--   0        0        0    11642 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi
+-rw-r--r--   0        0        0     7765 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2466 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4482 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    16485 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/__init__.py
+-rw-r--r--   0        0        0     4985 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     6147 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     8732 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     3705 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3641 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py
+-rw-r--r--   0        0        0     5332 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/__init__.py
+-rw-r--r--   0        0        0     5503 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6513 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     6525 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2441 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9468 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py
+-rw-r--r--   0        0        0     9775 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2_grpc.pyi
+-rw-r--r--   0        0        0       30 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2.py
+-rw-r--r--   0        0        0      838 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2_grpc.pyi
+-rw-r--r--   0        0        0       27 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/gogoproto/__init__.py
+-rw-r--r--   0        0        0    14512 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0        0        0    15688 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.py
+-rw-r--r--   0        0        0     1446 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.pyi
+-rw-r--r--   0        0        0       29 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/__init__.py
+-rw-r--r--   0        0        0     1585 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1053 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      633 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2125 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2.py
+-rw-r--r--   0        0        0    15201 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      627 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1507 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2.py
+-rw-r--r--   0        0        0     3509 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.py
+-rw-r--r--   0        0        0      628 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.pyi
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/__init__.py
+-rw-r--r--   0        0        0     1588 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2.py
+-rw-r--r--   0        0        0     6380 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.py
+-rw-r--r--   0        0        0     1651 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.pyi
+-rw-r--r--   0        0        0       26 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime-detector/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime-detector/v1beta1/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2678 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.py
+-rw-r--r--   0        0        0     2807 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3393 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2508 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4225 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2120 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     3091 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0      933 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       50 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/__init__.py
+-rw-r--r--   0        0        0     3153 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2.py
+-rw-r--r--   0        0        0     5302 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3224 2023-05-11 15:07:28.515744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2.py
+-rw-r--r--   0        0        0     2319 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2.pyi
+-rw-r--r--   0        0        0     4328 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1479 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       30 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool-models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool-models/balancer/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool-models/balancer/tx/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool-models/stableswap/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/__init__.py
+-rw-r--r--   0        0        0     7539 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.py
+-rw-r--r--   0        0        0     9172 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2_grpc.py
+-rw-r--r--   0        0        0      338 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2_grpc.pyi
+-rw-r--r--   0        0        0       54 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/__init__.py
+-rw-r--r--   0        0        0     3310 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.py
+-rw-r--r--   0        0        0     2435 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.pyi
+-rw-r--r--   0        0        0     2998 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.py
+-rw-r--r--   0        0        0      851 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       53 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/__init__.py
+-rw-r--r--   0        0        0     5008 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.py
+-rw-r--r--   0        0        0     4120 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5706 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.py
+-rw-r--r--   0        0        0     4391 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.pyi
+-rw-r--r--   0        0        0     5112 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1421 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2607 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2324 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    25030 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0    21922 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    28299 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     8224 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0    20488 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0    16056 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0    16940 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3758 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/__init__.py
+-rw-r--r--   0        0        0     3661 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.py
+-rw-r--r--   0        0        0     1865 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.pyi
+-rw-r--r--   0        0        0     2725 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1021 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc-rate-limit/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc-rate-limit/v1beta1/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1892 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1153 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1526 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0      864 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2533 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     1468 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     2762 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1098 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       36 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/__init__.py
+-rw-r--r--   0        0        0     3618 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2.py
+-rw-r--r--   0        0        0     4704 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2488 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2.py
+-rw-r--r--   0        0        0     2416 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1502 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2.py
+-rw-r--r--   0        0        0      996 2023-05-11 15:07:28.519744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11737 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2.py
+-rw-r--r--   0        0        0    15324 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2.pyi
+-rw-r--r--   0        0        0    16892 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.py
+-rw-r--r--   0        0        0     5850 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4208 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2.py
+-rw-r--r--   0        0        0     4561 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2.pyi
+-rw-r--r--   0        0        0     4260 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     1094 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/__init__.py
+-rw-r--r--   0        0        0     1853 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2.py
+-rw-r--r--   0        0        0     1594 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5004 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2.py
+-rw-r--r--   0        0        0     7774 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1506 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2.py
+-rw-r--r--   0        0        0     1058 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0    26438 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2.py
+-rw-r--r--   0        0        0    22384 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2.pyi
+-rw-r--r--   0        0        0    31704 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10228 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6583 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2.py
+-rw-r--r--   0        0        0     7473 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2.pyi
+-rw-r--r--   0        0        0     9131 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2719 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       30 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2142 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1726 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7174 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.py
+-rw-r--r--   0        0        0     6851 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3342 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     2574 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     4491 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     1591 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool-incentives/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool-incentives/v1beta1/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2885 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2263 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2807 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0     3755 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4964 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.py
+-rw-r--r--   0        0        0     4629 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10336 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     8564 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0    12358 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     4052 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1967 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.py
+-rw-r--r--   0        0        0     2048 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2_grpc.pyi
+-rw-r--r--   0        0        0       36 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/__init__.py
+-rw-r--r--   0        0        0     2951 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.py
+-rw-r--r--   0        0        0     3368 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.523744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1742 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2.py
+-rw-r--r--   0        0        0     1173 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0    23389 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2.py
+-rw-r--r--   0        0        0    24192 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2.pyi
+-rw-r--r--   0        0        0    29546 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.py
+-rw-r--r--   0        0        0    10416 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4584 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.py
+-rw-r--r--   0        0        0     7812 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5831 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2.py
+-rw-r--r--   0        0        0     6806 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2.pyi
+-rw-r--r--   0        0        0    10061 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     3517 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       44 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/__init__.py
+-rw-r--r--   0        0        0     3000 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0     3676 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/__init__.py
+-rw-r--r--   0        0        0       46 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1845 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.py
+-rw-r--r--   0        0        0     1080 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3037 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2659 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2136 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.py
+-rw-r--r--   0        0        0     1149 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5572 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4565 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     6778 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2658 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6212 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.py
+-rw-r--r--   0        0        0     6960 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.pyi
+-rw-r--r--   0        0        0     9732 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.py
+-rw-r--r--   0        0        0     2539 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.pyi
+-rw-r--r--   0        0        0       30 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/__init__.py
+-rw-r--r--   0        0        0     2711 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     2548 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10057 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     8194 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     9820 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2456 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4519 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.py
+-rw-r--r--   0        0        0     4094 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/__init__.py
+-rw-r--r--   0        0        0     1786 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.py
+-rw-r--r--   0        0        0     1149 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1663 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.py
+-rw-r--r--   0        0        0     1283 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2455 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.py
+-rw-r--r--   0        0        0     1708 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6233 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.py
+-rw-r--r--   0        0        0     4374 2023-05-11 15:07:28.527744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.pyi
+-rw-r--r--   0        0        0     8242 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.py
+-rw-r--r--   0        0        0     2885 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.pyi
+-rw-r--r--   0        0        0       28 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/__init__.py
+-rw-r--r--   0        0        0    21205 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2.py
+-rw-r--r--   0        0        0    49345 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2.pyi
+-rw-r--r--   0        0        0    25991 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.py
+-rw-r--r--   0        0        0     6123 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0       35 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2.py
+-rw-r--r--   0        0        0     1291 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2208 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2.py
+-rw-r--r--   0        0        0     4101 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2_grpc.pyi
+-rw-r--r--   0        0        0       33 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2.py
+-rw-r--r--   0        0        0     1049 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0       32 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2.py
+-rw-r--r--   0        0        0     3901 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0       34 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/__init__.py
+-rw-r--r--   0        0        0     2173 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2.py
+-rw-r--r--   0        0        0     1707 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3521 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2.py
+-rw-r--r--   0        0        0     5767 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3858 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2.py
+-rw-r--r--   0        0        0     6657 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10988 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2.py
+-rw-r--r--   0        0        0    18419 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2231 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2.py
+-rw-r--r--   0        0        0     3356 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2_grpc.pyi
+-rw-r--r--   0        0        0       36 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/__init__.py
+-rw-r--r--   0        0        0     1550 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2.py
+-rw-r--r--   0        0        0     1793 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0      937 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/exceptions.py
+-rw-r--r--   0        0        0    10498 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/grpc_client.py
+-rw-r--r--   0        0        0      494 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/pytypes/__init__.py
+-rw-r--r--   0        0        0     2669 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/pytypes/common.py
+-rw-r--r--   0        0        0     3890 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/pytypes/event.py
+-rw-r--r--   0        0        0     2411 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/pytypes/network.py
+-rw-r--r--   0        0        0     4308 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/pytypes/tx_resp.py
+-rw-r--r--   0        0        0     6185 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/sdk.py
+-rw-r--r--   0        0        0      183 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/__init__.py
+-rw-r--r--   0        0        0     3247 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/binance.py
+-rw-r--r--   0        0        0     2077 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/client.py
+-rw-r--r--   0        0        0      948 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/osmosis.py
+-rw-r--r--   0        0        0      126 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/trade_data.py
+-rw-r--r--   0        0        0      119 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/trading_client/types.py
+-rw-r--r--   0        0        0    12879 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/tx.py
+-rw-r--r--   0        0        0     9485 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/utils.py
+-rw-r--r--   0        0        0    11658 2023-05-11 15:07:28.531744 osmosispy-0.0.9/osmosispy/wallet.py
+-rw-r--r--   0        0        0      925 2023-05-11 15:07:28.535744 osmosispy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 osmosispy-0.0.9/PKG-INFO
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/confio/proofs_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/confio/proofs_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _HashOp:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _HashOpEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_HashOp.ValueType], builtins.type):  # noqa: F821
+class _HashOpEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_HashOp.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     NO_HASH: _HashOp.ValueType  # 0
     """NO_HASH is the default if no data passed. Note this is an illegal argument some places."""
     SHA256: _HashOp.ValueType  # 1
     SHA512: _HashOp.ValueType  # 2
     KECCAK: _HashOp.ValueType  # 3
     RIPEMD160: _HashOp.ValueType  # 4
@@ -45,15 +45,15 @@
 """ripemd160(sha256(x))"""
 global___HashOp = HashOp
 
 class _LengthOp:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _LengthOpEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_LengthOp.ValueType], builtins.type):  # noqa: F821
+class _LengthOpEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_LengthOp.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     NO_PREFIX: _LengthOp.ValueType  # 0
     """NO_PREFIX don't include any length info"""
     VAR_PROTO: _LengthOp.ValueType  # 1
     """VAR_PROTO uses protobuf (and go-amino) varint encoding of the length"""
     VAR_RLP: _LengthOp.ValueType  # 2
     """VAR_RLP uses rlp int encoding of the length"""
@@ -94,14 +94,15 @@
 """FIXED64_LITTLE uses little-endian encoding of the length as a 64 bit integer"""
 REQUIRE_32_BYTES: LengthOp.ValueType  # 7
 """REQUIRE_32_BYTES is like NONE, but will fail if the input is not exactly 32 bytes (sha256 output)"""
 REQUIRE_64_BYTES: LengthOp.ValueType  # 8
 """REQUIRE_64_BYTES is like NONE, but will fail if the input is not exactly 64 bytes (sha512 output)"""
 global___LengthOp = LengthOp
 
+@typing_extensions.final
 class ExistenceProof(google.protobuf.message.Message):
     """*
     ExistenceProof takes a key and a value and a set of steps to perform on it.
     The result of peforming all these steps will provide a "root hash", which can
     be compared to the value in a header.
 
     Since it is computationally infeasible to produce a hash collission for any of the used
@@ -142,14 +143,15 @@
         path: collections.abc.Iterable[global___InnerOp] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["leaf", b"leaf"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "leaf", b"leaf", "path", b"path", "value", b"value"]) -> None: ...
 
 global___ExistenceProof = ExistenceProof
 
+@typing_extensions.final
 class NonExistenceProof(google.protobuf.message.Message):
     """
     NonExistenceProof takes a proof of two neighbors, one left of the desired key,
     one right of the desired key. If both proofs are valid AND they are neighbors,
     then there is no valid proof for the given key.
     """
 
@@ -172,14 +174,15 @@
         right: global___ExistenceProof | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["left", b"left", "right", b"right"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "left", b"left", "right", b"right"]) -> None: ...
 
 global___NonExistenceProof = NonExistenceProof
 
+@typing_extensions.final
 class CommitmentProof(google.protobuf.message.Message):
     """
     CommitmentProof is either an ExistenceProof or a NonExistenceProof, or a Batch of such messages
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -205,14 +208,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["batch", b"batch", "compressed", b"compressed", "exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["batch", b"batch", "compressed", b"compressed", "exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["proof", b"proof"]) -> typing_extensions.Literal["exist", "nonexist", "batch", "compressed"] | None: ...
 
 global___CommitmentProof = CommitmentProof
 
+@typing_extensions.final
 class LeafOp(google.protobuf.message.Message):
     """*
     LeafOp represents the raw key-value data we wish to prove, and
     must be flexible to represent the internal transformation from
     the original key-value pairs into the basis hash, for many existing
     merkle trees.
 
@@ -251,14 +255,15 @@
         length: global___LengthOp.ValueType = ...,
         prefix: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["hash", b"hash", "length", b"length", "prefix", b"prefix", "prehash_key", b"prehash_key", "prehash_value", b"prehash_value"]) -> None: ...
 
 global___LeafOp = LeafOp
 
+@typing_extensions.final
 class InnerOp(google.protobuf.message.Message):
     """*
     InnerOp represents a merkle-proof step that is not a leaf.
     It represents concatenating two children and hashing them to provide the next result.
 
     The result of the previous step is passed in, so the signature of this op is:
     innerOp(child) -> output
@@ -289,14 +294,15 @@
         prefix: builtins.bytes = ...,
         suffix: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["hash", b"hash", "prefix", b"prefix", "suffix", b"suffix"]) -> None: ...
 
 global___InnerOp = InnerOp
 
+@typing_extensions.final
 class ProofSpec(google.protobuf.message.Message):
     """*
     ProofSpec defines what the expected parameters are for a given proof type.
     This can be stored in the client and used to validate any incoming proofs.
 
     verify(ProofSpec, Proof) -> Proof | Error
 
@@ -333,14 +339,15 @@
         min_depth: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["inner_spec", b"inner_spec", "leaf_spec", b"leaf_spec"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["inner_spec", b"inner_spec", "leaf_spec", b"leaf_spec", "max_depth", b"max_depth", "min_depth", b"min_depth"]) -> None: ...
 
 global___ProofSpec = ProofSpec
 
+@typing_extensions.final
 class InnerSpec(google.protobuf.message.Message):
     """
     InnerSpec contains all store-specific structure info to determine if two proofs from a
     given store are neighbors.
 
     This enables:
 
@@ -380,14 +387,15 @@
         empty_child: builtins.bytes = ...,
         hash: global___HashOp.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["child_order", b"child_order", "child_size", b"child_size", "empty_child", b"empty_child", "hash", b"hash", "max_prefix_length", b"max_prefix_length", "min_prefix_length", b"min_prefix_length"]) -> None: ...
 
 global___InnerSpec = InnerSpec
 
+@typing_extensions.final
 class BatchProof(google.protobuf.message.Message):
     """
     BatchProof is a group of multiple proof types than can be compressed
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -399,14 +407,15 @@
         *,
         entries: collections.abc.Iterable[global___BatchEntry] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["entries", b"entries"]) -> None: ...
 
 global___BatchProof = BatchProof
 
+@typing_extensions.final
 class BatchEntry(google.protobuf.message.Message):
     """Use BatchEntry not CommitmentProof, to avoid recursion"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXIST_FIELD_NUMBER: builtins.int
     NONEXIST_FIELD_NUMBER: builtins.int
@@ -422,14 +431,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["proof", b"proof"]) -> typing_extensions.Literal["exist", "nonexist"] | None: ...
 
 global___BatchEntry = BatchEntry
 
+@typing_extensions.final
 class CompressedBatchProof(google.protobuf.message.Message):
     """***** all items here are compressed forms ******"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENTRIES_FIELD_NUMBER: builtins.int
     LOOKUP_INNERS_FIELD_NUMBER: builtins.int
@@ -443,14 +453,15 @@
         entries: collections.abc.Iterable[global___CompressedBatchEntry] | None = ...,
         lookup_inners: collections.abc.Iterable[global___InnerOp] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["entries", b"entries", "lookup_inners", b"lookup_inners"]) -> None: ...
 
 global___CompressedBatchProof = CompressedBatchProof
 
+@typing_extensions.final
 class CompressedBatchEntry(google.protobuf.message.Message):
     """Use BatchEntry not CommitmentProof, to avoid recursion"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXIST_FIELD_NUMBER: builtins.int
     NONEXIST_FIELD_NUMBER: builtins.int
@@ -466,14 +477,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["exist", b"exist", "nonexist", b"nonexist", "proof", b"proof"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["proof", b"proof"]) -> typing_extensions.Literal["exist", "nonexist"] | None: ...
 
 global___CompressedBatchEntry = CompressedBatchEntry
 
+@typing_extensions.final
 class CompressedExistenceProof(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     LEAF_FIELD_NUMBER: builtins.int
     PATH_FIELD_NUMBER: builtins.int
@@ -493,14 +505,15 @@
         path: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["leaf", b"leaf"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "leaf", b"leaf", "path", b"path", "value", b"value"]) -> None: ...
 
 global___CompressedExistenceProof = CompressedExistenceProof
 
+@typing_extensions.final
 class CompressedNonExistenceProof(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     LEFT_FIELD_NUMBER: builtins.int
     RIGHT_FIELD_NUMBER: builtins.int
     key: builtins.bytes
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/auth_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class BaseAccount(google.protobuf.message.Message):
     """BaseAccount defines a base account type. It contains all the necessary fields
     for basic account functionality. Any custom account type should extend this
     type for additional functionality (e.g. vesting).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -43,14 +44,15 @@
         sequence: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pub_key", b"pub_key"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["account_number", b"account_number", "address", b"address", "pub_key", b"pub_key", "sequence", b"sequence"]) -> None: ...
 
 global___BaseAccount = BaseAccount
 
+@typing_extensions.final
 class ModuleAccount(google.protobuf.message.Message):
     """ModuleAccount defines an account for modules that holds coins on a pool."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_ACCOUNT_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -68,14 +70,15 @@
         permissions: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_account", b"base_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_account", b"base_account", "name", b"name", "permissions", b"permissions"]) -> None: ...
 
 global___ModuleAccount = ModuleAccount
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the parameters for the auth module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_MEMO_CHARACTERS_FIELD_NUMBER: builtins.int
     TX_SIG_LIMIT_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/genesis_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the auth module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     ACCOUNTS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryAccountsRequest(google.protobuf.message.Message):
     """QueryAccountsRequest is the request type for the Query/Accounts RPC method.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -37,14 +38,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryAccountsRequest = QueryAccountsRequest
 
+@typing_extensions.final
 class QueryAccountsResponse(google.protobuf.message.Message):
     """QueryAccountsResponse is the response type for the Query/Accounts RPC method.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -64,14 +66,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["accounts", b"accounts", "pagination", b"pagination"]) -> None: ...
 
 global___QueryAccountsResponse = QueryAccountsResponse
 
+@typing_extensions.final
 class QueryAccountRequest(google.protobuf.message.Message):
     """QueryAccountRequest is the request type for the Query/Account RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     address: builtins.str
@@ -81,14 +84,15 @@
         *,
         address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address"]) -> None: ...
 
 global___QueryAccountRequest = QueryAccountRequest
 
+@typing_extensions.final
 class QueryAccountResponse(google.protobuf.message.Message):
     """QueryAccountResponse is the response type for the Query/Account RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCOUNT_FIELD_NUMBER: builtins.int
     @property
@@ -100,25 +104,27 @@
         account: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["account", b"account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["account", b"account"]) -> None: ...
 
 global___QueryAccountResponse = QueryAccountResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -130,25 +136,27 @@
         params: cosmos.auth.v1beta1.auth_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryModuleAccountsRequest(google.protobuf.message.Message):
     """QueryModuleAccountsRequest is the request type for the Query/ModuleAccounts RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryModuleAccountsRequest = QueryModuleAccountsRequest
 
+@typing_extensions.final
 class QueryModuleAccountsResponse(google.protobuf.message.Message):
     """QueryModuleAccountsResponse is the response type for the Query/ModuleAccounts RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCOUNTS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/auth/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/authz_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenericAuthorization(google.protobuf.message.Message):
     """GenericAuthorization gives the grantee unrestricted permissions to execute
     the provided method on behalf of the granter's account.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -31,14 +32,15 @@
         *,
         msg: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["msg", b"msg"]) -> None: ...
 
 global___GenericAuthorization = GenericAuthorization
 
+@typing_extensions.final
 class Grant(google.protobuf.message.Message):
     """Grant gives permissions to execute
     the provide method with expiration time.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/event_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class EventGrant(google.protobuf.message.Message):
     """EventGrant is emitted on Msg/Grant"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MSG_TYPE_URL_FIELD_NUMBER: builtins.int
     GRANTER_FIELD_NUMBER: builtins.int
@@ -35,14 +36,15 @@
         granter: builtins.str = ...,
         grantee: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "granter", b"granter", "msg_type_url", b"msg_type_url"]) -> None: ...
 
 global___EventGrant = EventGrant
 
+@typing_extensions.final
 class EventRevoke(google.protobuf.message.Message):
     """EventRevoke is emitted on Msg/Revoke"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MSG_TYPE_URL_FIELD_NUMBER: builtins.int
     GRANTER_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/genesis_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the authz module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUTHORIZATION_FIELD_NUMBER: builtins.int
     @property
@@ -31,14 +32,15 @@
         *,
         authorization: collections.abc.Iterable[global___GrantAuthorization] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["authorization", b"authorization"]) -> None: ...
 
 global___GenesisState = GenesisState
 
+@typing_extensions.final
 class GrantAuthorization(google.protobuf.message.Message):
     """GrantAuthorization defines the GenesisState/GrantAuthorization type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTER_FIELD_NUMBER: builtins.int
     GRANTEE_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryGrantsRequest(google.protobuf.message.Message):
     """QueryGrantsRequest is the request type for the Query/Grants RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTER_FIELD_NUMBER: builtins.int
     GRANTEE_FIELD_NUMBER: builtins.int
@@ -43,14 +44,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "granter", b"granter", "msg_type_url", b"msg_type_url", "pagination", b"pagination"]) -> None: ...
 
 global___QueryGrantsRequest = QueryGrantsRequest
 
+@typing_extensions.final
 class QueryGrantsResponse(google.protobuf.message.Message):
     """QueryGrantsResponse is the response type for the Query/Authorizations RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgGrant(google.protobuf.message.Message):
     """MsgGrant is a request type for Grant method. It declares authorization to the grantee
     on behalf of the granter with the provided expiration time.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -40,14 +41,15 @@
         grant: cosmos.authz.v1beta1.authz_pb2.Grant | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["grant", b"grant"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["grant", b"grant", "grantee", b"grantee", "granter", b"granter"]) -> None: ...
 
 global___MsgGrant = MsgGrant
 
+@typing_extensions.final
 class MsgExecResponse(google.protobuf.message.Message):
     """MsgExecResponse defines the Msg/MsgExecResponse response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULTS_FIELD_NUMBER: builtins.int
     @property
@@ -57,14 +59,15 @@
         *,
         results: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["results", b"results"]) -> None: ...
 
 global___MsgExecResponse = MsgExecResponse
 
+@typing_extensions.final
 class MsgExec(google.protobuf.message.Message):
     """MsgExec attempts to execute the provided messages using
     authorizations granted to the grantee. Each message should have only
     one signer corresponding to the granter of the authorization.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -84,25 +87,27 @@
         grantee: builtins.str = ...,
         msgs: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "msgs", b"msgs"]) -> None: ...
 
 global___MsgExec = MsgExec
 
+@typing_extensions.final
 class MsgGrantResponse(google.protobuf.message.Message):
     """MsgGrantResponse defines the Msg/MsgGrant response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgGrantResponse = MsgGrantResponse
 
+@typing_extensions.final
 class MsgRevoke(google.protobuf.message.Message):
     """MsgRevoke revokes any authorization with the provided sdk.Msg type on the
     granter's account with that has been granted to the grantee.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -119,14 +124,15 @@
         grantee: builtins.str = ...,
         msg_type_url: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "granter", b"granter", "msg_type_url", b"msg_type_url"]) -> None: ...
 
 global___MsgRevoke = MsgRevoke
 
+@typing_extensions.final
 class MsgRevokeResponse(google.protobuf.message.Message):
     """MsgRevokeResponse defines the Msg/MsgRevokeResponse response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/authz/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/authz_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class SendAuthorization(google.protobuf.message.Message):
     """SendAuthorization allows the grantee to spend up to spend_limit coins from
     the granter's account.
 
     Since: cosmos-sdk 0.43
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/bank_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the parameters for the bank module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SEND_ENABLED_FIELD_NUMBER: builtins.int
     DEFAULT_SEND_ENABLED_FIELD_NUMBER: builtins.int
@@ -33,14 +34,15 @@
         send_enabled: collections.abc.Iterable[global___SendEnabled] | None = ...,
         default_send_enabled: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["default_send_enabled", b"default_send_enabled", "send_enabled", b"send_enabled"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class SendEnabled(google.protobuf.message.Message):
     """SendEnabled maps coin denom to a send_enabled status (whether a denom is
     sendable).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -54,14 +56,15 @@
         denom: builtins.str = ...,
         enabled: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "enabled", b"enabled"]) -> None: ...
 
 global___SendEnabled = SendEnabled
 
+@typing_extensions.final
 class Input(google.protobuf.message.Message):
     """Input models transaction input."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     COINS_FIELD_NUMBER: builtins.int
@@ -74,14 +77,15 @@
         address: builtins.str = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "coins", b"coins"]) -> None: ...
 
 global___Input = Input
 
+@typing_extensions.final
 class Output(google.protobuf.message.Message):
     """Output models transaction outputs."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     COINS_FIELD_NUMBER: builtins.int
@@ -94,14 +98,15 @@
         address: builtins.str = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "coins", b"coins"]) -> None: ...
 
 global___Output = Output
 
+@typing_extensions.final
 class Supply(google.protobuf.message.Message):
     """Supply represents a struct that passively keeps track of the total supply
     amounts in the network.
     This message is deprecated now that supply is indexed by denom.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -114,14 +119,15 @@
         *,
         total: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["total", b"total"]) -> None: ...
 
 global___Supply = Supply
 
+@typing_extensions.final
 class DenomUnit(google.protobuf.message.Message):
     """DenomUnit represents a struct that describes a given
     denomination unit of the basic token.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -147,14 +153,15 @@
         exponent: builtins.int = ...,
         aliases: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aliases", b"aliases", "denom", b"denom", "exponent", b"exponent"]) -> None: ...
 
 global___DenomUnit = DenomUnit
 
+@typing_extensions.final
 class Metadata(google.protobuf.message.Message):
     """Metadata represents a struct that describes
     a basic token.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/genesis_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the bank module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     BALANCES_FIELD_NUMBER: builtins.int
@@ -55,14 +56,15 @@
         supply_offsets: collections.abc.Iterable[global___GenesisSupplyOffset] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balances", b"balances", "denom_metadata", b"denom_metadata", "params", b"params", "supply", b"supply", "supply_offsets", b"supply_offsets"]) -> None: ...
 
 global___GenesisState = GenesisState
 
+@typing_extensions.final
 class Balance(google.protobuf.message.Message):
     """Balance defines an account address and balance pair used in the bank module's
     genesis state.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -79,14 +81,15 @@
         address: builtins.str = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "coins", b"coins"]) -> None: ...
 
 global___Balance = Balance
 
+@typing_extensions.final
 class GenesisSupplyOffset(google.protobuf.message.Message):
     """GenesisSupplyOffset encodes the supply offsets, just for genesis.
     The offsets are serialized directly by denom in state.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryBalanceRequest(google.protobuf.message.Message):
     """QueryBalanceRequest is the request type for the Query/Balance RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
@@ -36,14 +37,15 @@
         address: builtins.str = ...,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "denom", b"denom"]) -> None: ...
 
 global___QueryBalanceRequest = QueryBalanceRequest
 
+@typing_extensions.final
 class QueryBalanceResponse(google.protobuf.message.Message):
     """QueryBalanceResponse is the response type for the Query/Balance RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BALANCE_FIELD_NUMBER: builtins.int
     @property
@@ -55,14 +57,15 @@
         balance: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["balance", b"balance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balance", b"balance"]) -> None: ...
 
 global___QueryBalanceResponse = QueryBalanceResponse
 
+@typing_extensions.final
 class QueryAllBalancesRequest(google.protobuf.message.Message):
     """QueryBalanceRequest is the request type for the Query/AllBalances RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -78,14 +81,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "pagination", b"pagination"]) -> None: ...
 
 global___QueryAllBalancesRequest = QueryAllBalancesRequest
 
+@typing_extensions.final
 class QueryAllBalancesResponse(google.protobuf.message.Message):
     """QueryAllBalancesResponse is the response type for the Query/AllBalances RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -104,14 +108,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balances", b"balances", "pagination", b"pagination"]) -> None: ...
 
 global___QueryAllBalancesResponse = QueryAllBalancesResponse
 
+@typing_extensions.final
 class QueryTotalSupplyRequest(google.protobuf.message.Message):
     """QueryTotalSupplyRequest is the request type for the Query/TotalSupply RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -128,14 +133,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryTotalSupplyRequest = QueryTotalSupplyRequest
 
+@typing_extensions.final
 class QueryTotalSupplyResponse(google.protobuf.message.Message):
     """QueryTotalSupplyResponse is the response type for the Query/TotalSupply RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -157,14 +163,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "supply", b"supply"]) -> None: ...
 
 global___QueryTotalSupplyResponse = QueryTotalSupplyResponse
 
+@typing_extensions.final
 class QuerySupplyOfRequest(google.protobuf.message.Message):
     """QuerySupplyOfRequest is the request type for the Query/SupplyOf RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
@@ -174,14 +181,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QuerySupplyOfRequest = QuerySupplyOfRequest
 
+@typing_extensions.final
 class QuerySupplyOfResponse(google.protobuf.message.Message):
     """QuerySupplyOfResponse is the response type for the Query/SupplyOf RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AMOUNT_FIELD_NUMBER: builtins.int
     @property
@@ -193,14 +201,15 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> None: ...
 
 global___QuerySupplyOfResponse = QuerySupplyOfResponse
 
+@typing_extensions.final
 class QueryTotalSupplyWithoutOffsetRequest(google.protobuf.message.Message):
     """QueryTotalSupplyWithoutOffsetRequest is the request type for the Query/TotalSupplyWithoutOffset RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -217,14 +226,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryTotalSupplyWithoutOffsetRequest = QueryTotalSupplyWithoutOffsetRequest
 
+@typing_extensions.final
 class QueryTotalSupplyWithoutOffsetResponse(google.protobuf.message.Message):
     """QueryTotalSupplyWithoutOffsetResponse is the response type for the Query/TotalSupplyWithoutOffset RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -246,14 +256,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "supply", b"supply"]) -> None: ...
 
 global___QueryTotalSupplyWithoutOffsetResponse = QueryTotalSupplyWithoutOffsetResponse
 
+@typing_extensions.final
 class QuerySupplyOfWithoutOffsetRequest(google.protobuf.message.Message):
     """QuerySupplyOfWithoutOffsetRequest is the request type for the Query/SupplyOfWithoutOffset RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
@@ -263,14 +274,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QuerySupplyOfWithoutOffsetRequest = QuerySupplyOfWithoutOffsetRequest
 
+@typing_extensions.final
 class QuerySupplyOfWithoutOffsetResponse(google.protobuf.message.Message):
     """QuerySupplyOfWithoutOffsetResponse is the response type for the Query/SupplyOfWithoutOffset RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AMOUNT_FIELD_NUMBER: builtins.int
     @property
@@ -282,25 +294,27 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> None: ...
 
 global___QuerySupplyOfWithoutOffsetResponse = QuerySupplyOfWithoutOffsetResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest defines the request type for querying x/bank parameters."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse defines the response type for querying x/bank parameters."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -311,14 +325,15 @@
         params: cosmos.bank.v1beta1.bank_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryDenomsMetadataRequest(google.protobuf.message.Message):
     """QueryDenomsMetadataRequest is the request type for the Query/DenomsMetadata RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
@@ -330,14 +345,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryDenomsMetadataRequest = QueryDenomsMetadataRequest
 
+@typing_extensions.final
 class QueryDenomsMetadataResponse(google.protobuf.message.Message):
     """QueryDenomsMetadataResponse is the response type for the Query/DenomsMetadata RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -356,14 +372,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadatas", b"metadatas", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDenomsMetadataResponse = QueryDenomsMetadataResponse
 
+@typing_extensions.final
 class QueryDenomMetadataRequest(google.protobuf.message.Message):
     """QueryDenomMetadataRequest is the request type for the Query/DenomMetadata RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
@@ -373,14 +390,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryDenomMetadataRequest = QueryDenomMetadataRequest
 
+@typing_extensions.final
 class QueryDenomMetadataResponse(google.protobuf.message.Message):
     """QueryDenomMetadataResponse is the response type for the Query/DenomMetadata RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -394,14 +412,15 @@
         metadata: cosmos.bank.v1beta1.bank_pb2.Metadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> None: ...
 
 global___QueryDenomMetadataResponse = QueryDenomMetadataResponse
 
+@typing_extensions.final
 class QueryBaseDenomRequest(google.protobuf.message.Message):
     """QueryBaseDenomRequest defines the request type for the BaseDenom gRPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
@@ -410,14 +429,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryBaseDenomRequest = QueryBaseDenomRequest
 
+@typing_extensions.final
 class QueryBaseDenomResponse(google.protobuf.message.Message):
     """QueryBaseDenomResponse defines the response type for the BaseDenom gRPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_DENOM_FIELD_NUMBER: builtins.int
     base_denom: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgSend(google.protobuf.message.Message):
     """MsgSend represents a message to send coins from one account to another."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FROM_ADDRESS_FIELD_NUMBER: builtins.int
     TO_ADDRESS_FIELD_NUMBER: builtins.int
@@ -37,25 +38,27 @@
         to_address: builtins.str = ...,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "from_address", b"from_address", "to_address", b"to_address"]) -> None: ...
 
 global___MsgSend = MsgSend
 
+@typing_extensions.final
 class MsgSendResponse(google.protobuf.message.Message):
     """MsgSendResponse defines the Msg/Send response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgSendResponse = MsgSendResponse
 
+@typing_extensions.final
 class MsgMultiSend(google.protobuf.message.Message):
     """MsgMultiSend represents an arbitrary multi-in, multi-out send message."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INPUTS_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
@@ -69,14 +72,15 @@
         inputs: collections.abc.Iterable[cosmos.bank.v1beta1.bank_pb2.Input] | None = ...,
         outputs: collections.abc.Iterable[cosmos.bank.v1beta1.bank_pb2.Output] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["inputs", b"inputs", "outputs", b"outputs"]) -> None: ...
 
 global___MsgMultiSend = MsgMultiSend
 
+@typing_extensions.final
 class MsgMultiSendResponse(google.protobuf.message.Message):
     """MsgMultiSendResponse defines the Msg/MultiSend response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/bank/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/abci/v1beta1/abci_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class TxResponse(google.protobuf.message.Message):
     """TxResponse defines a structure containing relevant tx data and metadata. The
     tags are stringified and the log is JSON decoded.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -96,14 +97,15 @@
         events: collections.abc.Iterable[tendermint.abci.types_pb2.Event] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["tx", b"tx"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "codespace", b"codespace", "data", b"data", "events", b"events", "gas_used", b"gas_used", "gas_wanted", b"gas_wanted", "height", b"height", "info", b"info", "logs", b"logs", "raw_log", b"raw_log", "timestamp", b"timestamp", "tx", b"tx", "txhash", b"txhash"]) -> None: ...
 
 global___TxResponse = TxResponse
 
+@typing_extensions.final
 class ABCIMessageLog(google.protobuf.message.Message):
     """ABCIMessageLog defines a structure containing an indexed tx ABCI message log."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MSG_INDEX_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
@@ -122,14 +124,15 @@
         log: builtins.str = ...,
         events: collections.abc.Iterable[global___StringEvent] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["events", b"events", "log", b"log", "msg_index", b"msg_index"]) -> None: ...
 
 global___ABCIMessageLog = ABCIMessageLog
 
+@typing_extensions.final
 class StringEvent(google.protobuf.message.Message):
     """StringEvent defines en Event object wrapper where all the attributes
     contain key/value pairs that are strings instead of raw bytes.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -144,14 +147,15 @@
         type: builtins.str = ...,
         attributes: collections.abc.Iterable[global___Attribute] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["attributes", b"attributes", "type", b"type"]) -> None: ...
 
 global___StringEvent = StringEvent
 
+@typing_extensions.final
 class Attribute(google.protobuf.message.Message):
     """Attribute defines an attribute wrapper where the key and value are
     strings instead of raw bytes.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -165,14 +169,15 @@
         key: builtins.str = ...,
         value: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
 global___Attribute = Attribute
 
+@typing_extensions.final
 class GasInfo(google.protobuf.message.Message):
     """GasInfo defines tx execution gas context."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GAS_WANTED_FIELD_NUMBER: builtins.int
     GAS_USED_FIELD_NUMBER: builtins.int
@@ -186,14 +191,15 @@
         gas_wanted: builtins.int = ...,
         gas_used: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["gas_used", b"gas_used", "gas_wanted", b"gas_wanted"]) -> None: ...
 
 global___GasInfo = GasInfo
 
+@typing_extensions.final
 class Result(google.protobuf.message.Message):
     """Result is the union of ResponseFormat and ResponseCheckTx."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
@@ -216,14 +222,15 @@
         log: builtins.str = ...,
         events: collections.abc.Iterable[tendermint.abci.types_pb2.Event] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "events", b"events", "log", b"log"]) -> None: ...
 
 global___Result = Result
 
+@typing_extensions.final
 class SimulationResponse(google.protobuf.message.Message):
     """SimulationResponse defines the response generated when a transaction is
     successfully simulated.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -240,14 +247,15 @@
         result: global___Result | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["gas_info", b"gas_info", "result", b"result"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["gas_info", b"gas_info", "result", b"result"]) -> None: ...
 
 global___SimulationResponse = SimulationResponse
 
+@typing_extensions.final
 class MsgData(google.protobuf.message.Message):
     """MsgData defines the data returned in a Result object during message
     execution.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -261,14 +269,15 @@
         msg_type: builtins.str = ...,
         data: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "msg_type", b"msg_type"]) -> None: ...
 
 global___MsgData = MsgData
 
+@typing_extensions.final
 class TxMsgData(google.protobuf.message.Message):
     """TxMsgData defines a list of MsgData. A transaction will have a MsgData object
     for each message.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -280,14 +289,15 @@
         *,
         data: collections.abc.Iterable[global___MsgData] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data"]) -> None: ...
 
 global___TxMsgData = TxMsgData
 
+@typing_extensions.final
 class SearchTxsResult(google.protobuf.message.Message):
     """SearchTxsResult defines a structure for querying txs pageable"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_COUNT_FIELD_NUMBER: builtins.int
     COUNT_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/kv/v1beta1/kv_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Pairs(google.protobuf.message.Message):
     """Pairs defines a repeated slice of Pair objects."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAIRS_FIELD_NUMBER: builtins.int
     @property
@@ -29,14 +30,15 @@
         *,
         pairs: collections.abc.Iterable[global___Pair] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pairs", b"pairs"]) -> None: ...
 
 global___Pairs = Pairs
 
+@typing_extensions.final
 class Pair(google.protobuf.message.Message):
     """Pair defines a key/value bytes tuple."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/query/v1beta1/pagination_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PageRequest(google.protobuf.message.Message):
     """PageRequest is to be embedded in gRPC request messages for efficient
     pagination. Ex:
 
      message SomeRequest {
              Foo some_parameter = 1;
              PageRequest pagination = 2;
@@ -65,14 +66,15 @@
         count_total: builtins.bool = ...,
         reverse: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["count_total", b"count_total", "key", b"key", "limit", b"limit", "offset", b"offset", "reverse", b"reverse"]) -> None: ...
 
 global___PageRequest = PageRequest
 
+@typing_extensions.final
 class PageResponse(google.protobuf.message.Message):
     """PageResponse is to be embedded in gRPC response messages where the
     corresponding request message has used PageRequest.
 
      message SomeResponse {
              repeated Bar results = 1;
              PageResponse page = 2;
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ListAllInterfacesRequest(google.protobuf.message.Message):
     """ListAllInterfacesRequest is the request type of the ListAllInterfaces RPC."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ListAllInterfacesRequest = ListAllInterfacesRequest
 
+@typing_extensions.final
 class ListAllInterfacesResponse(google.protobuf.message.Message):
     """ListAllInterfacesResponse is the response type of the ListAllInterfaces RPC."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACE_NAMES_FIELD_NUMBER: builtins.int
     @property
@@ -41,14 +43,15 @@
         *,
         interface_names: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["interface_names", b"interface_names"]) -> None: ...
 
 global___ListAllInterfacesResponse = ListAllInterfacesResponse
 
+@typing_extensions.final
 class ListImplementationsRequest(google.protobuf.message.Message):
     """ListImplementationsRequest is the request type of the ListImplementations
     RPC.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -60,14 +63,15 @@
         *,
         interface_name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["interface_name", b"interface_name"]) -> None: ...
 
 global___ListImplementationsRequest = ListImplementationsRequest
 
+@typing_extensions.final
 class ListImplementationsResponse(google.protobuf.message.Message):
     """ListImplementationsResponse is the response type of the ListImplementations
     RPC.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v1beta1/reflection_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class AppDescriptor(google.protobuf.message.Message):
     """AppDescriptor describes a cosmos-sdk based application"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUTHN_FIELD_NUMBER: builtins.int
     CHAIN_FIELD_NUMBER: builtins.int
@@ -58,14 +59,15 @@
         tx: global___TxDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["authn", b"authn", "chain", b"chain", "codec", b"codec", "configuration", b"configuration", "query_services", b"query_services", "tx", b"tx"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["authn", b"authn", "chain", b"chain", "codec", b"codec", "configuration", b"configuration", "query_services", b"query_services", "tx", b"tx"]) -> None: ...
 
 global___AppDescriptor = AppDescriptor
 
+@typing_extensions.final
 class TxDescriptor(google.protobuf.message.Message):
     """TxDescriptor describes the accepted transaction type"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FULLNAME_FIELD_NUMBER: builtins.int
     MSGS_FIELD_NUMBER: builtins.int
@@ -83,14 +85,15 @@
         fullname: builtins.str = ...,
         msgs: collections.abc.Iterable[global___MsgDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fullname", b"fullname", "msgs", b"msgs"]) -> None: ...
 
 global___TxDescriptor = TxDescriptor
 
+@typing_extensions.final
 class AuthnDescriptor(google.protobuf.message.Message):
     """AuthnDescriptor provides information on how to sign transactions without relying
     on the online RPCs GetTxMetadata and CombineUnsignedTxAndSignatures
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -103,14 +106,15 @@
         *,
         sign_modes: collections.abc.Iterable[global___SigningModeDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["sign_modes", b"sign_modes"]) -> None: ...
 
 global___AuthnDescriptor = AuthnDescriptor
 
+@typing_extensions.final
 class SigningModeDescriptor(google.protobuf.message.Message):
     """SigningModeDescriptor provides information on a signing flow of the application
     NOTE(fdymylja): here we could go as far as providing an entire flow on how
     to sign a message given a SigningModeDescriptor, but it's better to think about
     this another time
     """
 
@@ -134,14 +138,15 @@
         number: builtins.int = ...,
         authn_info_provider_method_fullname: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["authn_info_provider_method_fullname", b"authn_info_provider_method_fullname", "name", b"name", "number", b"number"]) -> None: ...
 
 global___SigningModeDescriptor = SigningModeDescriptor
 
+@typing_extensions.final
 class ChainDescriptor(google.protobuf.message.Message):
     """ChainDescriptor describes chain information of the application"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     id: builtins.str
@@ -151,14 +156,15 @@
         *,
         id: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
 
 global___ChainDescriptor = ChainDescriptor
 
+@typing_extensions.final
 class CodecDescriptor(google.protobuf.message.Message):
     """CodecDescriptor describes the registered interfaces and provides metadata information on the types"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INTERFACES_FIELD_NUMBER: builtins.int
     @property
@@ -169,14 +175,15 @@
         *,
         interfaces: collections.abc.Iterable[global___InterfaceDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["interfaces", b"interfaces"]) -> None: ...
 
 global___CodecDescriptor = CodecDescriptor
 
+@typing_extensions.final
 class InterfaceDescriptor(google.protobuf.message.Message):
     """InterfaceDescriptor describes the implementation of an interface"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FULLNAME_FIELD_NUMBER: builtins.int
     INTERFACE_ACCEPTING_MESSAGES_FIELD_NUMBER: builtins.int
@@ -198,14 +205,15 @@
         interface_accepting_messages: collections.abc.Iterable[global___InterfaceAcceptingMessageDescriptor] | None = ...,
         interface_implementers: collections.abc.Iterable[global___InterfaceImplementerDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fullname", b"fullname", "interface_accepting_messages", b"interface_accepting_messages", "interface_implementers", b"interface_implementers"]) -> None: ...
 
 global___InterfaceDescriptor = InterfaceDescriptor
 
+@typing_extensions.final
 class InterfaceImplementerDescriptor(google.protobuf.message.Message):
     """InterfaceImplementerDescriptor describes an interface implementer"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FULLNAME_FIELD_NUMBER: builtins.int
     TYPE_URL_FIELD_NUMBER: builtins.int
@@ -223,14 +231,15 @@
         fullname: builtins.str = ...,
         type_url: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fullname", b"fullname", "type_url", b"type_url"]) -> None: ...
 
 global___InterfaceImplementerDescriptor = InterfaceImplementerDescriptor
 
+@typing_extensions.final
 class InterfaceAcceptingMessageDescriptor(google.protobuf.message.Message):
     """InterfaceAcceptingMessageDescriptor describes a protobuf message which contains
     an interface represented as a google.protobuf.Any
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -250,14 +259,15 @@
         fullname: builtins.str = ...,
         field_descriptor_names: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["field_descriptor_names", b"field_descriptor_names", "fullname", b"fullname"]) -> None: ...
 
 global___InterfaceAcceptingMessageDescriptor = InterfaceAcceptingMessageDescriptor
 
+@typing_extensions.final
 class ConfigurationDescriptor(google.protobuf.message.Message):
     """ConfigurationDescriptor contains metadata information on the sdk.Config"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BECH32_ACCOUNT_ADDRESS_PREFIX_FIELD_NUMBER: builtins.int
     bech32_account_address_prefix: builtins.str
@@ -267,14 +277,15 @@
         *,
         bech32_account_address_prefix: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["bech32_account_address_prefix", b"bech32_account_address_prefix"]) -> None: ...
 
 global___ConfigurationDescriptor = ConfigurationDescriptor
 
+@typing_extensions.final
 class MsgDescriptor(google.protobuf.message.Message):
     """MsgDescriptor describes a cosmos-sdk message that can be delivered with a transaction"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MSG_TYPE_URL_FIELD_NUMBER: builtins.int
     msg_type_url: builtins.str
@@ -284,25 +295,27 @@
         *,
         msg_type_url: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["msg_type_url", b"msg_type_url"]) -> None: ...
 
 global___MsgDescriptor = MsgDescriptor
 
+@typing_extensions.final
 class GetAuthnDescriptorRequest(google.protobuf.message.Message):
     """GetAuthnDescriptorRequest is the request used for the GetAuthnDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetAuthnDescriptorRequest = GetAuthnDescriptorRequest
 
+@typing_extensions.final
 class GetAuthnDescriptorResponse(google.protobuf.message.Message):
     """GetAuthnDescriptorResponse is the response returned by the GetAuthnDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUTHN_FIELD_NUMBER: builtins.int
     @property
@@ -314,25 +327,27 @@
         authn: global___AuthnDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["authn", b"authn"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["authn", b"authn"]) -> None: ...
 
 global___GetAuthnDescriptorResponse = GetAuthnDescriptorResponse
 
+@typing_extensions.final
 class GetChainDescriptorRequest(google.protobuf.message.Message):
     """GetChainDescriptorRequest is the request used for the GetChainDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetChainDescriptorRequest = GetChainDescriptorRequest
 
+@typing_extensions.final
 class GetChainDescriptorResponse(google.protobuf.message.Message):
     """GetChainDescriptorResponse is the response returned by the GetChainDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHAIN_FIELD_NUMBER: builtins.int
     @property
@@ -344,25 +359,27 @@
         chain: global___ChainDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["chain", b"chain"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["chain", b"chain"]) -> None: ...
 
 global___GetChainDescriptorResponse = GetChainDescriptorResponse
 
+@typing_extensions.final
 class GetCodecDescriptorRequest(google.protobuf.message.Message):
     """GetCodecDescriptorRequest is the request used for the GetCodecDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetCodecDescriptorRequest = GetCodecDescriptorRequest
 
+@typing_extensions.final
 class GetCodecDescriptorResponse(google.protobuf.message.Message):
     """GetCodecDescriptorResponse is the response returned by the GetCodecDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODEC_FIELD_NUMBER: builtins.int
     @property
@@ -374,25 +391,27 @@
         codec: global___CodecDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["codec", b"codec"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["codec", b"codec"]) -> None: ...
 
 global___GetCodecDescriptorResponse = GetCodecDescriptorResponse
 
+@typing_extensions.final
 class GetConfigurationDescriptorRequest(google.protobuf.message.Message):
     """GetConfigurationDescriptorRequest is the request used for the GetConfigurationDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetConfigurationDescriptorRequest = GetConfigurationDescriptorRequest
 
+@typing_extensions.final
 class GetConfigurationDescriptorResponse(google.protobuf.message.Message):
     """GetConfigurationDescriptorResponse is the response returned by the GetConfigurationDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIG_FIELD_NUMBER: builtins.int
     @property
@@ -404,25 +423,27 @@
         config: global___ConfigurationDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["config", b"config"]) -> None: ...
 
 global___GetConfigurationDescriptorResponse = GetConfigurationDescriptorResponse
 
+@typing_extensions.final
 class GetQueryServicesDescriptorRequest(google.protobuf.message.Message):
     """GetQueryServicesDescriptorRequest is the request used for the GetQueryServicesDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetQueryServicesDescriptorRequest = GetQueryServicesDescriptorRequest
 
+@typing_extensions.final
 class GetQueryServicesDescriptorResponse(google.protobuf.message.Message):
     """GetQueryServicesDescriptorResponse is the response returned by the GetQueryServicesDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     QUERIES_FIELD_NUMBER: builtins.int
     @property
@@ -434,25 +455,27 @@
         queries: global___QueryServicesDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["queries", b"queries"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["queries", b"queries"]) -> None: ...
 
 global___GetQueryServicesDescriptorResponse = GetQueryServicesDescriptorResponse
 
+@typing_extensions.final
 class GetTxDescriptorRequest(google.protobuf.message.Message):
     """GetTxDescriptorRequest is the request used for the GetTxDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetTxDescriptorRequest = GetTxDescriptorRequest
 
+@typing_extensions.final
 class GetTxDescriptorResponse(google.protobuf.message.Message):
     """GetTxDescriptorResponse is the response returned by the GetTxDescriptor RPC"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TX_FIELD_NUMBER: builtins.int
     @property
@@ -466,14 +489,15 @@
         tx: global___TxDescriptor | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["tx", b"tx"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["tx", b"tx"]) -> None: ...
 
 global___GetTxDescriptorResponse = GetTxDescriptorResponse
 
+@typing_extensions.final
 class QueryServicesDescriptor(google.protobuf.message.Message):
     """QueryServicesDescriptor contains the list of cosmos-sdk queriable services"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     QUERY_SERVICES_FIELD_NUMBER: builtins.int
     @property
@@ -484,14 +508,15 @@
         *,
         query_services: collections.abc.Iterable[global___QueryServiceDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["query_services", b"query_services"]) -> None: ...
 
 global___QueryServicesDescriptor = QueryServicesDescriptor
 
+@typing_extensions.final
 class QueryServiceDescriptor(google.protobuf.message.Message):
     """QueryServiceDescriptor describes a cosmos-sdk queryable service"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FULLNAME_FIELD_NUMBER: builtins.int
     IS_MODULE_FIELD_NUMBER: builtins.int
@@ -510,14 +535,15 @@
         is_module: builtins.bool = ...,
         methods: collections.abc.Iterable[global___QueryMethodDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fullname", b"fullname", "is_module", b"is_module", "methods", b"methods"]) -> None: ...
 
 global___QueryServiceDescriptor = QueryServiceDescriptor
 
+@typing_extensions.final
 class QueryMethodDescriptor(google.protobuf.message.Message):
     """QueryMethodDescriptor describes a queryable method of a query service
     no other info is provided beside method name and tendermint queryable path
     because it would be redundant with the grpc reflection service
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/reflection/v2alpha1/reflection_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/snapshots/v1beta1/snapshot_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Snapshot(google.protobuf.message.Message):
     """Snapshot contains Tendermint state sync snapshot info."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     FORMAT_FIELD_NUMBER: builtins.int
@@ -42,14 +43,15 @@
         metadata: global___Metadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["chunks", b"chunks", "format", b"format", "hash", b"hash", "height", b"height", "metadata", b"metadata"]) -> None: ...
 
 global___Snapshot = Snapshot
 
+@typing_extensions.final
 class Metadata(google.protobuf.message.Message):
     """Metadata contains SDK-specific snapshot metadata."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHUNK_HASHES_FIELD_NUMBER: builtins.int
     @property
@@ -60,14 +62,15 @@
         *,
         chunk_hashes: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["chunk_hashes", b"chunk_hashes"]) -> None: ...
 
 global___Metadata = Metadata
 
+@typing_extensions.final
 class SnapshotItem(google.protobuf.message.Message):
     """SnapshotItem is an item contained in a rootmulti.Store snapshot."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STORE_FIELD_NUMBER: builtins.int
     IAVL_FIELD_NUMBER: builtins.int
@@ -95,14 +98,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["app_version", b"app_version", "extension", b"extension", "extension_payload", b"extension_payload", "iavl", b"iavl", "item", b"item", "store", b"store"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_version", b"app_version", "extension", b"extension", "extension_payload", b"extension_payload", "iavl", b"iavl", "item", b"item", "store", b"store"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["item", b"item"]) -> typing_extensions.Literal["store", "iavl", "extension", "extension_payload", "app_version"] | None: ...
 
 global___SnapshotItem = SnapshotItem
 
+@typing_extensions.final
 class SnapshotStoreItem(google.protobuf.message.Message):
     """SnapshotStoreItem contains metadata about a snapshotted store."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     name: builtins.str
@@ -111,14 +115,15 @@
         *,
         name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
 
 global___SnapshotStoreItem = SnapshotStoreItem
 
+@typing_extensions.final
 class SnapshotIAVLItem(google.protobuf.message.Message):
     """SnapshotIAVLItem is an exported IAVL node."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
@@ -138,14 +143,15 @@
         version: builtins.int = ...,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "key", b"key", "value", b"value", "version", b"version"]) -> None: ...
 
 global___SnapshotIAVLItem = SnapshotIAVLItem
 
+@typing_extensions.final
 class SnapshotExtensionMeta(google.protobuf.message.Message):
     """SnapshotExtensionMeta contains metadata about an external snapshotter."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     FORMAT_FIELD_NUMBER: builtins.int
@@ -157,14 +163,15 @@
         name: builtins.str = ...,
         format: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["format", b"format", "name", b"name"]) -> None: ...
 
 global___SnapshotExtensionMeta = SnapshotExtensionMeta
 
+@typing_extensions.final
 class SnapshotExtensionPayload(google.protobuf.message.Message):
     """SnapshotExtensionPayload contains payloads of an external snapshotter."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAYLOAD_FIELD_NUMBER: builtins.int
     payload: builtins.bytes
@@ -173,14 +180,15 @@
         *,
         payload: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["payload", b"payload"]) -> None: ...
 
 global___SnapshotExtensionPayload = SnapshotExtensionPayload
 
+@typing_extensions.final
 class SnapshotAppVersion(google.protobuf.message.Message):
     """SnapshotAppVersion contains the app version."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VERSION_FIELD_NUMBER: builtins.int
     version: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/commit_info_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class CommitInfo(google.protobuf.message.Message):
     """CommitInfo defines commit information used by the multi-store when committing
     a version/height.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -34,14 +35,15 @@
         version: builtins.int = ...,
         store_infos: collections.abc.Iterable[global___StoreInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["store_infos", b"store_infos", "version", b"version"]) -> None: ...
 
 global___CommitInfo = CommitInfo
 
+@typing_extensions.final
 class StoreInfo(google.protobuf.message.Message):
     """StoreInfo defines store-specific commit information. It contains a reference
     between a store name and the commit ID.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -57,14 +59,15 @@
         commit_id: global___CommitID | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commit_id", b"commit_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commit_id", b"commit_id", "name", b"name"]) -> None: ...
 
 global___StoreInfo = StoreInfo
 
+@typing_extensions.final
 class CommitID(google.protobuf.message.Message):
     """CommitID defines the committment information when a specific store is
     committed.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/store/v1beta1/listening_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class StoreKVPair(google.protobuf.message.Message):
     """StoreKVPair is a KVStore KVPair used for listening to state changes (Sets and Deletes)
     It optionally includes the StoreKey for the originating KVStore and a Boolean flag to distinguish between Sets and
     Deletes
 
     Since: cosmos-sdk 0.43
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GetValidatorSetByHeightRequest(google.protobuf.message.Message):
     """GetValidatorSetByHeightRequest is the request type for the Query/GetValidatorSetByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -39,14 +40,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "pagination", b"pagination"]) -> None: ...
 
 global___GetValidatorSetByHeightRequest = GetValidatorSetByHeightRequest
 
+@typing_extensions.final
 class GetValidatorSetByHeightResponse(google.protobuf.message.Message):
     """GetValidatorSetByHeightResponse is the response type for the Query/GetValidatorSetByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
     VALIDATORS_FIELD_NUMBER: builtins.int
@@ -65,14 +67,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_height", b"block_height", "pagination", b"pagination", "validators", b"validators"]) -> None: ...
 
 global___GetValidatorSetByHeightResponse = GetValidatorSetByHeightResponse
 
+@typing_extensions.final
 class GetLatestValidatorSetRequest(google.protobuf.message.Message):
     """GetLatestValidatorSetRequest is the request type for the Query/GetValidatorSetByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
@@ -84,14 +87,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___GetLatestValidatorSetRequest = GetLatestValidatorSetRequest
 
+@typing_extensions.final
 class GetLatestValidatorSetResponse(google.protobuf.message.Message):
     """GetLatestValidatorSetResponse is the response type for the Query/GetValidatorSetByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
     VALIDATORS_FIELD_NUMBER: builtins.int
@@ -110,14 +114,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_height", b"block_height", "pagination", b"pagination", "validators", b"validators"]) -> None: ...
 
 global___GetLatestValidatorSetResponse = GetLatestValidatorSetResponse
 
+@typing_extensions.final
 class Validator(google.protobuf.message.Message):
     """Validator is the type for the validator-set."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     PUB_KEY_FIELD_NUMBER: builtins.int
@@ -137,14 +142,15 @@
         proposer_priority: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pub_key", b"pub_key"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "proposer_priority", b"proposer_priority", "pub_key", b"pub_key", "voting_power", b"voting_power"]) -> None: ...
 
 global___Validator = Validator
 
+@typing_extensions.final
 class GetBlockByHeightRequest(google.protobuf.message.Message):
     """GetBlockByHeightRequest is the request type for the Query/GetBlockByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     height: builtins.int
@@ -153,14 +159,15 @@
         *,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height"]) -> None: ...
 
 global___GetBlockByHeightRequest = GetBlockByHeightRequest
 
+@typing_extensions.final
 class GetBlockByHeightResponse(google.protobuf.message.Message):
     """GetBlockByHeightResponse is the response type for the Query/GetBlockByHeight RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_ID_FIELD_NUMBER: builtins.int
     BLOCK_FIELD_NUMBER: builtins.int
@@ -175,25 +182,27 @@
         block: tendermint.types.block_pb2.Block | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block", b"block", "block_id", b"block_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block", b"block", "block_id", b"block_id"]) -> None: ...
 
 global___GetBlockByHeightResponse = GetBlockByHeightResponse
 
+@typing_extensions.final
 class GetLatestBlockRequest(google.protobuf.message.Message):
     """GetLatestBlockRequest is the request type for the Query/GetLatestBlock RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetLatestBlockRequest = GetLatestBlockRequest
 
+@typing_extensions.final
 class GetLatestBlockResponse(google.protobuf.message.Message):
     """GetLatestBlockResponse is the response type for the Query/GetLatestBlock RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_ID_FIELD_NUMBER: builtins.int
     BLOCK_FIELD_NUMBER: builtins.int
@@ -208,25 +217,27 @@
         block: tendermint.types.block_pb2.Block | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block", b"block", "block_id", b"block_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block", b"block", "block_id", b"block_id"]) -> None: ...
 
 global___GetLatestBlockResponse = GetLatestBlockResponse
 
+@typing_extensions.final
 class GetSyncingRequest(google.protobuf.message.Message):
     """GetSyncingRequest is the request type for the Query/GetSyncing RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetSyncingRequest = GetSyncingRequest
 
+@typing_extensions.final
 class GetSyncingResponse(google.protobuf.message.Message):
     """GetSyncingResponse is the response type for the Query/GetSyncing RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SYNCING_FIELD_NUMBER: builtins.int
     syncing: builtins.bool
@@ -235,25 +246,27 @@
         *,
         syncing: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["syncing", b"syncing"]) -> None: ...
 
 global___GetSyncingResponse = GetSyncingResponse
 
+@typing_extensions.final
 class GetNodeInfoRequest(google.protobuf.message.Message):
     """GetNodeInfoRequest is the request type for the Query/GetNodeInfo RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GetNodeInfoRequest = GetNodeInfoRequest
 
+@typing_extensions.final
 class GetNodeInfoResponse(google.protobuf.message.Message):
     """GetNodeInfoResponse is the request type for the Query/GetNodeInfo RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEFAULT_NODE_INFO_FIELD_NUMBER: builtins.int
     APPLICATION_VERSION_FIELD_NUMBER: builtins.int
@@ -268,14 +281,15 @@
         application_version: global___VersionInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["application_version", b"application_version", "default_node_info", b"default_node_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["application_version", b"application_version", "default_node_info", b"default_node_info"]) -> None: ...
 
 global___GetNodeInfoResponse = GetNodeInfoResponse
 
+@typing_extensions.final
 class VersionInfo(google.protobuf.message.Message):
     """VersionInfo is the type for the GetNodeInfoResponse message."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     APP_NAME_FIELD_NUMBER: builtins.int
@@ -307,14 +321,15 @@
         build_deps: collections.abc.Iterable[global___Module] | None = ...,
         cosmos_sdk_version: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_name", b"app_name", "build_deps", b"build_deps", "build_tags", b"build_tags", "cosmos_sdk_version", b"cosmos_sdk_version", "git_commit", b"git_commit", "go_version", b"go_version", "name", b"name", "version", b"version"]) -> None: ...
 
 global___VersionInfo = VersionInfo
 
+@typing_extensions.final
 class Module(google.protobuf.message.Message):
     """Module is the type for VersionInfo"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PATH_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/tendermint/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: cosmos/base/v1beta1/coin.proto
 """Generated protocol buffer code."""
+from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gogoproto import gogo_pb2 as gogoproto_dot_gogo__pb2
-
-
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x63osmos/base/v1beta1/coin.proto\x12\x13\x63osmos.base.v1beta1\x1a\x14gogoproto/gogo.proto\"8\n\x04\x43oin\x12\r\n\x05\x64\x65nom\x18\x01 \x01(\t\x12\x1b\n\x06\x61mount\x18\x02 \x01(\tB\x0b\xda\xde\x1f\x03Int\xc8\xde\x1f\x00:\x04\xe8\xa0\x1f\x01\";\n\x07\x44\x65\x63\x43oin\x12\r\n\x05\x64\x65nom\x18\x01 \x01(\t\x12\x1b\n\x06\x61mount\x18\x02 \x01(\tB\x0b\xda\xde\x1f\x03\x44\x65\x63\xc8\xde\x1f\x00:\x04\xe8\xa0\x1f\x01\"$\n\x08IntProto\x12\x18\n\x03int\x18\x01 \x01(\tB\x0b\xda\xde\x1f\x03Int\xc8\xde\x1f\x00\"$\n\x08\x44\x65\x63Proto\x12\x18\n\x03\x64\x65\x63\x18\x01 \x01(\tB\x0b\xda\xde\x1f\x03\x44\x65\x63\xc8\xde\x1f\x00\x42,Z\"github.com/cosmos/cosmos-sdk/types\xd8\xe1\x1e\x00\x80\xe2\x1e\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'cosmos.base.v1beta1.coin_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(
+    DESCRIPTOR, 'cosmos.base.v1beta1.coin_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\"github.com/cosmos/cosmos-sdk/types\330\341\036\000\200\342\036\000'
-  _COIN.fields_by_name['amount']._options = None
-  _COIN.fields_by_name['amount']._serialized_options = b'\332\336\037\003Int\310\336\037\000'
-  _COIN._options = None
-  _COIN._serialized_options = b'\350\240\037\001'
-  _DECCOIN.fields_by_name['amount']._options = None
-  _DECCOIN.fields_by_name['amount']._serialized_options = b'\332\336\037\003Dec\310\336\037\000'
-  _DECCOIN._options = None
-  _DECCOIN._serialized_options = b'\350\240\037\001'
-  _INTPROTO.fields_by_name['int']._options = None
-  _INTPROTO.fields_by_name['int']._serialized_options = b'\332\336\037\003Int\310\336\037\000'
-  _DECPROTO.fields_by_name['dec']._options = None
-  _DECPROTO.fields_by_name['dec']._serialized_options = b'\332\336\037\003Dec\310\336\037\000'
-  _COIN._serialized_start=77
-  _COIN._serialized_end=133
-  _DECCOIN._serialized_start=135
-  _DECCOIN._serialized_end=194
-  _INTPROTO._serialized_start=196
-  _INTPROTO._serialized_end=232
-  _DECPROTO._serialized_start=234
-  _DECPROTO._serialized_end=270
+    DESCRIPTOR._options = None
+    DESCRIPTOR._serialized_options = b'Z\"github.com/cosmos/cosmos-sdk/types\330\341\036\000\200\342\036\000'
+    _COIN.fields_by_name['amount']._options = None
+    _COIN.fields_by_name['amount']._serialized_options = b'\332\336\037\003Int\310\336\037\000'
+    _COIN._options = None
+    _COIN._serialized_options = b'\350\240\037\001'
+    _DECCOIN.fields_by_name['amount']._options = None
+    _DECCOIN.fields_by_name['amount']._serialized_options = b'\332\336\037\003Dec\310\336\037\000'
+    _DECCOIN._options = None
+    _DECCOIN._serialized_options = b'\350\240\037\001'
+    _INTPROTO.fields_by_name['int']._options = None
+    _INTPROTO.fields_by_name['int']._serialized_options = b'\332\336\037\003Int\310\336\037\000'
+    _DECPROTO.fields_by_name['dec']._options = None
+    _DECPROTO.fields_by_name['dec']._serialized_options = b'\332\336\037\003Dec\310\336\037\000'
+    _COIN._serialized_start = 77
+    _COIN._serialized_end = 133
+    _DECCOIN._serialized_start = 135
+    _DECCOIN._serialized_end = 194
+    _INTPROTO._serialized_start = 196
+    _INTPROTO._serialized_end = 232
+    _DECPROTO._serialized_start = 234
+    _DECPROTO._serialized_end = 270
 # @@protoc_insertion_point(module_scope)
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Coin(google.protobuf.message.Message):
     """Coin defines a token with a denomination and an amount.
 
     NOTE: The amount field is an Int which implements the custom method
     signatures required by gogoproto.
     """
 
@@ -33,14 +34,15 @@
         denom: builtins.str = ...,
         amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "denom", b"denom"]) -> None: ...
 
 global___Coin = Coin
 
+@typing_extensions.final
 class DecCoin(google.protobuf.message.Message):
     """DecCoin defines a token with a denomination and a decimal amount.
 
     NOTE: The amount field is an Dec which implements the custom method
     signatures required by gogoproto.
     """
 
@@ -56,14 +58,15 @@
         denom: builtins.str = ...,
         amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "denom", b"denom"]) -> None: ...
 
 global___DecCoin = DecCoin
 
+@typing_extensions.final
 class IntProto(google.protobuf.message.Message):
     """IntProto defines a Protobuf wrapper around an Int object."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INT_FIELD_NUMBER: builtins.int
     int: builtins.str
@@ -72,14 +75,15 @@
         *,
         int: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["int", b"int"]) -> None: ...
 
 global___IntProto = IntProto
 
+@typing_extensions.final
 class DecProto(google.protobuf.message.Message):
     """DecProto defines a Protobuf wrapper around a Dec object."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEC_FIELD_NUMBER: builtins.int
     dec: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/capability_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Capability(google.protobuf.message.Message):
     """Capability defines an implementation of an object capability. The index
     provided to a Capability must be globally unique.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -30,14 +31,15 @@
         *,
         index: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["index", b"index"]) -> None: ...
 
 global___Capability = Capability
 
+@typing_extensions.final
 class Owner(google.protobuf.message.Message):
     """Owner defines a single capability owner. An owner is defined by the name of
     capability and the module name.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -51,14 +53,15 @@
         module: builtins.str = ...,
         name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["module", b"module", "name", b"name"]) -> None: ...
 
 global___Owner = Owner
 
+@typing_extensions.final
 class CapabilityOwners(google.protobuf.message.Message):
     """CapabilityOwners defines a set of owners of a single Capability. The set of
     owners must be unique.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/capability/v1beta1/genesis_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisOwners(google.protobuf.message.Message):
     """GenesisOwners defines the capability owners with their corresponding index."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     INDEX_OWNERS_FIELD_NUMBER: builtins.int
@@ -36,14 +37,15 @@
         index_owners: cosmos.capability.v1beta1.capability_pb2.CapabilityOwners | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["index_owners", b"index_owners"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["index", b"index", "index_owners", b"index_owners"]) -> None: ...
 
 global___GenesisOwners = GenesisOwners
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the capability module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     OWNERS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/genesis_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the crisis module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONSTANT_FEE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgVerifyInvariant(google.protobuf.message.Message):
     """MsgVerifyInvariant represents a message to verify a particular invariance."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     INVARIANT_MODULE_NAME_FIELD_NUMBER: builtins.int
@@ -32,14 +33,15 @@
         invariant_module_name: builtins.str = ...,
         invariant_route: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["invariant_module_name", b"invariant_module_name", "invariant_route", b"invariant_route", "sender", b"sender"]) -> None: ...
 
 global___MsgVerifyInvariant = MsgVerifyInvariant
 
+@typing_extensions.final
 class MsgVerifyInvariantResponse(google.protobuf.message.Message):
     """MsgVerifyInvariantResponse defines the Msg/VerifyInvariant response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crisis/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/ed25519/keys_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PubKey(google.protobuf.message.Message):
     """PubKey is an ed25519 public key for handling Tendermint keys in SDK.
     It's needed for Any serialization and SDK compatibility.
     It must not be used in a non Tendermint key context because it doesn't implement
     ADR-28. Nevertheless, you will like to use ed25519 in app user level
     then you must create a new proto message and follow ADR-28 for Address construction.
     """
@@ -31,14 +32,15 @@
         *,
         key: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key"]) -> None: ...
 
 global___PubKey = PubKey
 
+@typing_extensions.final
 class PrivKey(google.protobuf.message.Message):
     """Deprecated: PrivKey defines a ed25519 private key.
     NOTE: ed25519 keys must not be used in SDK apps except in a tendermint validator context.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/keys_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class LegacyAminoPubKey(google.protobuf.message.Message):
     """LegacyAminoPubKey specifies a public key type
     which nests multiple public keys and a threshold,
     it uses legacy amino address rules.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/multisig/v1beta1/multisig_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MultiSignature(google.protobuf.message.Message):
     """MultiSignature wraps the signatures from a multisig.LegacyAminoPubKey.
     See cosmos.tx.v1betata1.ModeInfo.Multi for how to specify which signers
     signed and with which modes.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -32,14 +33,15 @@
         *,
         signatures: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["signatures", b"signatures"]) -> None: ...
 
 global___MultiSignature = MultiSignature
 
+@typing_extensions.final
 class CompactBitArray(google.protobuf.message.Message):
     """CompactBitArray is an implementation of a space efficient bit array.
     This is used to ensure that the encoded data takes up a minimal amount of
     space after proto encoding.
     This is not thread safe, and is not intended for concurrent usage.
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256k1/keys_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PubKey(google.protobuf.message.Message):
     """PubKey defines a secp256k1 public key
     Key is the compressed form of the pubkey. The first byte depends is a 0x02 byte
     if the y-coordinate is the lexicographically largest of the two associated with
     the x-coordinate. Otherwise the first byte is a 0x03.
     This prefix is followed with the x-coordinate.
     """
@@ -31,14 +32,15 @@
         *,
         key: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key"]) -> None: ...
 
 global___PubKey = PubKey
 
+@typing_extensions.final
 class PrivKey(google.protobuf.message.Message):
     """PrivKey defines a secp256k1 private key."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     key: builtins.bytes
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/crypto/secp256r1/keys_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PubKey(google.protobuf.message.Message):
     """PubKey defines a secp256r1 ECDSA public key."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     key: builtins.bytes
@@ -29,14 +30,15 @@
         *,
         key: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key"]) -> None: ...
 
 global___PubKey = PubKey
 
+@typing_extensions.final
 class PrivKey(google.protobuf.message.Message):
     """PrivKey defines a secp256r1 ECDSA private key."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SECRET_FIELD_NUMBER: builtins.int
     secret: builtins.bytes
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/distribution_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the set of params for the distribution module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMMUNITY_TAX_FIELD_NUMBER: builtins.int
     BASE_PROPOSER_REWARD_FIELD_NUMBER: builtins.int
@@ -38,14 +39,15 @@
         bonus_proposer_reward: builtins.str = ...,
         withdraw_addr_enabled: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_proposer_reward", b"base_proposer_reward", "bonus_proposer_reward", b"bonus_proposer_reward", "community_tax", b"community_tax", "withdraw_addr_enabled", b"withdraw_addr_enabled"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class ValidatorHistoricalRewards(google.protobuf.message.Message):
     """ValidatorHistoricalRewards represents historical rewards for a validator.
     Height is implicit within the store key.
     Cumulative reward ratio is the sum from the zeroeth period
     until this period of rewards / tokens, per the spec.
     The reference count indicates the number of objects
     which might need to reference this historical entry at any point.
@@ -70,14 +72,15 @@
         cumulative_reward_ratio: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
         reference_count: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["cumulative_reward_ratio", b"cumulative_reward_ratio", "reference_count", b"reference_count"]) -> None: ...
 
 global___ValidatorHistoricalRewards = ValidatorHistoricalRewards
 
+@typing_extensions.final
 class ValidatorCurrentRewards(google.protobuf.message.Message):
     """ValidatorCurrentRewards represents current rewards and current
     period for a validator kept as a running counter and incremented
     each block as long as the validator's tokens remain constant.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -93,14 +96,15 @@
         rewards: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
         period: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["period", b"period", "rewards", b"rewards"]) -> None: ...
 
 global___ValidatorCurrentRewards = ValidatorCurrentRewards
 
+@typing_extensions.final
 class ValidatorAccumulatedCommission(google.protobuf.message.Message):
     """ValidatorAccumulatedCommission represents accumulated commission
     for a validator kept as a running counter, can be withdrawn at any time.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -112,14 +116,15 @@
         *,
         commission: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission", b"commission"]) -> None: ...
 
 global___ValidatorAccumulatedCommission = ValidatorAccumulatedCommission
 
+@typing_extensions.final
 class ValidatorOutstandingRewards(google.protobuf.message.Message):
     """ValidatorOutstandingRewards represents outstanding (un-withdrawn) rewards
     for a validator inexpensive to track, allows simple sanity checks.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -131,14 +136,15 @@
         *,
         rewards: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> None: ...
 
 global___ValidatorOutstandingRewards = ValidatorOutstandingRewards
 
+@typing_extensions.final
 class ValidatorSlashEvent(google.protobuf.message.Message):
     """ValidatorSlashEvent represents a validator slash event.
     Height is implicit within the store key.
     This is needed to calculate appropriate amount of staking tokens
     for delegations which are withdrawn after a slash has occurred.
     """
 
@@ -154,14 +160,15 @@
         validator_period: builtins.int = ...,
         fraction: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fraction", b"fraction", "validator_period", b"validator_period"]) -> None: ...
 
 global___ValidatorSlashEvent = ValidatorSlashEvent
 
+@typing_extensions.final
 class ValidatorSlashEvents(google.protobuf.message.Message):
     """ValidatorSlashEvents is a collection of ValidatorSlashEvent messages."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_SLASH_EVENTS_FIELD_NUMBER: builtins.int
     @property
@@ -171,14 +178,15 @@
         *,
         validator_slash_events: collections.abc.Iterable[global___ValidatorSlashEvent] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_slash_events", b"validator_slash_events"]) -> None: ...
 
 global___ValidatorSlashEvents = ValidatorSlashEvents
 
+@typing_extensions.final
 class FeePool(google.protobuf.message.Message):
     """FeePool is the global fee pool for distribution."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMMUNITY_POOL_FIELD_NUMBER: builtins.int
     @property
@@ -188,14 +196,15 @@
         *,
         community_pool: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["community_pool", b"community_pool"]) -> None: ...
 
 global___FeePool = FeePool
 
+@typing_extensions.final
 class CommunityPoolSpendProposal(google.protobuf.message.Message):
     """CommunityPoolSpendProposal details a proposal for use of community funds,
     together with how many coins are proposed to be spent, and to which
     recipient account.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -217,14 +226,15 @@
         recipient: builtins.str = ...,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "description", b"description", "recipient", b"recipient", "title", b"title"]) -> None: ...
 
 global___CommunityPoolSpendProposal = CommunityPoolSpendProposal
 
+@typing_extensions.final
 class DelegatorStartingInfo(google.protobuf.message.Message):
     """DelegatorStartingInfo represents the starting info for a delegator reward
     period. It tracks the previous validator period, the delegation's amount of
     staking token, and the creation height (to check later on if any slashes have
     occurred). NOTE: Even though validators are slashed to whole staking tokens,
     the delegators within the validator may be left with less than a full token,
     thus sdk.Dec is used.
@@ -245,14 +255,15 @@
         stake: builtins.str = ...,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "previous_period", b"previous_period", "stake", b"stake"]) -> None: ...
 
 global___DelegatorStartingInfo = DelegatorStartingInfo
 
+@typing_extensions.final
 class DelegationDelegatorReward(google.protobuf.message.Message):
     """DelegationDelegatorReward represents the properties
     of a delegator's delegation reward.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -267,14 +278,15 @@
         validator_address: builtins.str = ...,
         reward: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["reward", b"reward", "validator_address", b"validator_address"]) -> None: ...
 
 global___DelegationDelegatorReward = DelegationDelegatorReward
 
+@typing_extensions.final
 class CommunityPoolSpendProposalWithDeposit(google.protobuf.message.Message):
     """CommunityPoolSpendProposalWithDeposit defines a CommunityPoolSpendProposal
     with a deposit
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/genesis_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class DelegatorWithdrawInfo(google.protobuf.message.Message):
     """DelegatorWithdrawInfo is the address for where distributions rewards are
     withdrawn to by default this struct is only used at genesis to feed in
     default withdraw addresses.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -38,14 +39,15 @@
         delegator_address: builtins.str = ...,
         withdraw_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "withdraw_address", b"withdraw_address"]) -> None: ...
 
 global___DelegatorWithdrawInfo = DelegatorWithdrawInfo
 
+@typing_extensions.final
 class ValidatorOutstandingRewardsRecord(google.protobuf.message.Message):
     """ValidatorOutstandingRewardsRecord is used for import/export via genesis json."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     OUTSTANDING_REWARDS_FIELD_NUMBER: builtins.int
@@ -60,14 +62,15 @@
         validator_address: builtins.str = ...,
         outstanding_rewards: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["outstanding_rewards", b"outstanding_rewards", "validator_address", b"validator_address"]) -> None: ...
 
 global___ValidatorOutstandingRewardsRecord = ValidatorOutstandingRewardsRecord
 
+@typing_extensions.final
 class ValidatorAccumulatedCommissionRecord(google.protobuf.message.Message):
     """ValidatorAccumulatedCommissionRecord is used for import / export via genesis
     json.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -85,14 +88,15 @@
         accumulated: cosmos.distribution.v1beta1.distribution_pb2.ValidatorAccumulatedCommission | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["accumulated", b"accumulated"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["accumulated", b"accumulated", "validator_address", b"validator_address"]) -> None: ...
 
 global___ValidatorAccumulatedCommissionRecord = ValidatorAccumulatedCommissionRecord
 
+@typing_extensions.final
 class ValidatorHistoricalRewardsRecord(google.protobuf.message.Message):
     """ValidatorHistoricalRewardsRecord is used for import / export via genesis
     json.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -114,14 +118,15 @@
         rewards: cosmos.distribution.v1beta1.distribution_pb2.ValidatorHistoricalRewards | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["period", b"period", "rewards", b"rewards", "validator_address", b"validator_address"]) -> None: ...
 
 global___ValidatorHistoricalRewardsRecord = ValidatorHistoricalRewardsRecord
 
+@typing_extensions.final
 class ValidatorCurrentRewardsRecord(google.protobuf.message.Message):
     """ValidatorCurrentRewardsRecord is used for import / export via genesis json."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     REWARDS_FIELD_NUMBER: builtins.int
@@ -137,14 +142,15 @@
         rewards: cosmos.distribution.v1beta1.distribution_pb2.ValidatorCurrentRewards | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["rewards", b"rewards", "validator_address", b"validator_address"]) -> None: ...
 
 global___ValidatorCurrentRewardsRecord = ValidatorCurrentRewardsRecord
 
+@typing_extensions.final
 class DelegatorStartingInfoRecord(google.protobuf.message.Message):
     """DelegatorStartingInfoRecord used for import / export via genesis json."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDRESS_FIELD_NUMBER: builtins.int
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
@@ -164,14 +170,15 @@
         starting_info: cosmos.distribution.v1beta1.distribution_pb2.DelegatorStartingInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["starting_info", b"starting_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "starting_info", b"starting_info", "validator_address", b"validator_address"]) -> None: ...
 
 global___DelegatorStartingInfoRecord = DelegatorStartingInfoRecord
 
+@typing_extensions.final
 class ValidatorSlashEventRecord(google.protobuf.message.Message):
     """ValidatorSlashEventRecord is used for import / export via genesis json."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
@@ -195,14 +202,15 @@
         validator_slash_event: cosmos.distribution.v1beta1.distribution_pb2.ValidatorSlashEvent | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["validator_slash_event", b"validator_slash_event"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "period", b"period", "validator_address", b"validator_address", "validator_slash_event", b"validator_slash_event"]) -> None: ...
 
 global___ValidatorSlashEventRecord = ValidatorSlashEventRecord
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the distribution module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     FEE_POOL_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -45,14 +47,15 @@
         params: cosmos.distribution.v1beta1.distribution_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryValidatorOutstandingRewardsRequest(google.protobuf.message.Message):
     """QueryValidatorOutstandingRewardsRequest is the request type for the
     Query/ValidatorOutstandingRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -64,14 +67,15 @@
         *,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_address", b"validator_address"]) -> None: ...
 
 global___QueryValidatorOutstandingRewardsRequest = QueryValidatorOutstandingRewardsRequest
 
+@typing_extensions.final
 class QueryValidatorOutstandingRewardsResponse(google.protobuf.message.Message):
     """QueryValidatorOutstandingRewardsResponse is the response type for the
     Query/ValidatorOutstandingRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -84,14 +88,15 @@
         rewards: cosmos.distribution.v1beta1.distribution_pb2.ValidatorOutstandingRewards | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> None: ...
 
 global___QueryValidatorOutstandingRewardsResponse = QueryValidatorOutstandingRewardsResponse
 
+@typing_extensions.final
 class QueryValidatorCommissionRequest(google.protobuf.message.Message):
     """QueryValidatorCommissionRequest is the request type for the
     Query/ValidatorCommission RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -103,14 +108,15 @@
         *,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_address", b"validator_address"]) -> None: ...
 
 global___QueryValidatorCommissionRequest = QueryValidatorCommissionRequest
 
+@typing_extensions.final
 class QueryValidatorCommissionResponse(google.protobuf.message.Message):
     """QueryValidatorCommissionResponse is the response type for the
     Query/ValidatorCommission RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -124,14 +130,15 @@
         commission: cosmos.distribution.v1beta1.distribution_pb2.ValidatorAccumulatedCommission | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commission", b"commission"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission", b"commission"]) -> None: ...
 
 global___QueryValidatorCommissionResponse = QueryValidatorCommissionResponse
 
+@typing_extensions.final
 class QueryValidatorSlashesRequest(google.protobuf.message.Message):
     """QueryValidatorSlashesRequest is the request type for the
     Query/ValidatorSlashes RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -157,14 +164,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["ending_height", b"ending_height", "pagination", b"pagination", "starting_height", b"starting_height", "validator_address", b"validator_address"]) -> None: ...
 
 global___QueryValidatorSlashesRequest = QueryValidatorSlashesRequest
 
+@typing_extensions.final
 class QueryValidatorSlashesResponse(google.protobuf.message.Message):
     """QueryValidatorSlashesResponse is the response type for the
     Query/ValidatorSlashes RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -183,14 +191,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "slashes", b"slashes"]) -> None: ...
 
 global___QueryValidatorSlashesResponse = QueryValidatorSlashesResponse
 
+@typing_extensions.final
 class QueryDelegationRewardsRequest(google.protobuf.message.Message):
     """QueryDelegationRewardsRequest is the request type for the
     Query/DelegationRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -206,14 +215,15 @@
         delegator_address: builtins.str = ...,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "validator_address", b"validator_address"]) -> None: ...
 
 global___QueryDelegationRewardsRequest = QueryDelegationRewardsRequest
 
+@typing_extensions.final
 class QueryDelegationRewardsResponse(google.protobuf.message.Message):
     """QueryDelegationRewardsResponse is the response type for the
     Query/DelegationRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -226,14 +236,15 @@
         *,
         rewards: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["rewards", b"rewards"]) -> None: ...
 
 global___QueryDelegationRewardsResponse = QueryDelegationRewardsResponse
 
+@typing_extensions.final
 class QueryDelegationTotalRewardsRequest(google.protobuf.message.Message):
     """QueryDelegationTotalRewardsRequest is the request type for the
     Query/DelegationTotalRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -245,14 +256,15 @@
         *,
         delegator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address"]) -> None: ...
 
 global___QueryDelegationTotalRewardsRequest = QueryDelegationTotalRewardsRequest
 
+@typing_extensions.final
 class QueryDelegationTotalRewardsResponse(google.protobuf.message.Message):
     """QueryDelegationTotalRewardsResponse is the response type for the
     Query/DelegationTotalRewards RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -270,14 +282,15 @@
         rewards: collections.abc.Iterable[cosmos.distribution.v1beta1.distribution_pb2.DelegationDelegatorReward] | None = ...,
         total: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.DecCoin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["rewards", b"rewards", "total", b"total"]) -> None: ...
 
 global___QueryDelegationTotalRewardsResponse = QueryDelegationTotalRewardsResponse
 
+@typing_extensions.final
 class QueryDelegatorValidatorsRequest(google.protobuf.message.Message):
     """QueryDelegatorValidatorsRequest is the request type for the
     Query/DelegatorValidators RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -289,14 +302,15 @@
         *,
         delegator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address"]) -> None: ...
 
 global___QueryDelegatorValidatorsRequest = QueryDelegatorValidatorsRequest
 
+@typing_extensions.final
 class QueryDelegatorValidatorsResponse(google.protobuf.message.Message):
     """QueryDelegatorValidatorsResponse is the response type for the
     Query/DelegatorValidators RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -309,14 +323,15 @@
         *,
         validators: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validators", b"validators"]) -> None: ...
 
 global___QueryDelegatorValidatorsResponse = QueryDelegatorValidatorsResponse
 
+@typing_extensions.final
 class QueryDelegatorWithdrawAddressRequest(google.protobuf.message.Message):
     """QueryDelegatorWithdrawAddressRequest is the request type for the
     Query/DelegatorWithdrawAddress RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -328,14 +343,15 @@
         *,
         delegator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address"]) -> None: ...
 
 global___QueryDelegatorWithdrawAddressRequest = QueryDelegatorWithdrawAddressRequest
 
+@typing_extensions.final
 class QueryDelegatorWithdrawAddressResponse(google.protobuf.message.Message):
     """QueryDelegatorWithdrawAddressResponse is the response type for the
     Query/DelegatorWithdrawAddress RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -347,27 +363,29 @@
         *,
         withdraw_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["withdraw_address", b"withdraw_address"]) -> None: ...
 
 global___QueryDelegatorWithdrawAddressResponse = QueryDelegatorWithdrawAddressResponse
 
+@typing_extensions.final
 class QueryCommunityPoolRequest(google.protobuf.message.Message):
     """QueryCommunityPoolRequest is the request type for the Query/CommunityPool RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryCommunityPoolRequest = QueryCommunityPoolRequest
 
+@typing_extensions.final
 class QueryCommunityPoolResponse(google.protobuf.message.Message):
     """QueryCommunityPoolResponse is the response type for the Query/CommunityPool
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgSetWithdrawAddress(google.protobuf.message.Message):
     """MsgSetWithdrawAddress sets the withdraw address for
     a delegator (or validator self-delegation).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -34,25 +35,27 @@
         delegator_address: builtins.str = ...,
         withdraw_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "withdraw_address", b"withdraw_address"]) -> None: ...
 
 global___MsgSetWithdrawAddress = MsgSetWithdrawAddress
 
+@typing_extensions.final
 class MsgSetWithdrawAddressResponse(google.protobuf.message.Message):
     """MsgSetWithdrawAddressResponse defines the Msg/SetWithdrawAddress response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgSetWithdrawAddressResponse = MsgSetWithdrawAddressResponse
 
+@typing_extensions.final
 class MsgWithdrawDelegatorReward(google.protobuf.message.Message):
     """MsgWithdrawDelegatorReward represents delegation withdrawal to a delegator
     from a single validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -66,25 +69,27 @@
         delegator_address: builtins.str = ...,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "validator_address", b"validator_address"]) -> None: ...
 
 global___MsgWithdrawDelegatorReward = MsgWithdrawDelegatorReward
 
+@typing_extensions.final
 class MsgWithdrawDelegatorRewardResponse(google.protobuf.message.Message):
     """MsgWithdrawDelegatorRewardResponse defines the Msg/WithdrawDelegatorReward response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgWithdrawDelegatorRewardResponse = MsgWithdrawDelegatorRewardResponse
 
+@typing_extensions.final
 class MsgWithdrawValidatorCommission(google.protobuf.message.Message):
     """MsgWithdrawValidatorCommission withdraws the full commission to the validator
     address.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -95,25 +100,27 @@
         *,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_address", b"validator_address"]) -> None: ...
 
 global___MsgWithdrawValidatorCommission = MsgWithdrawValidatorCommission
 
+@typing_extensions.final
 class MsgWithdrawValidatorCommissionResponse(google.protobuf.message.Message):
     """MsgWithdrawValidatorCommissionResponse defines the Msg/WithdrawValidatorCommission response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgWithdrawValidatorCommissionResponse = MsgWithdrawValidatorCommissionResponse
 
+@typing_extensions.final
 class MsgFundCommunityPool(google.protobuf.message.Message):
     """MsgFundCommunityPool allows an account to directly
     fund the community pool.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -128,14 +135,15 @@
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
         depositor: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "depositor", b"depositor"]) -> None: ...
 
 global___MsgFundCommunityPool = MsgFundCommunityPool
 
+@typing_extensions.final
 class MsgFundCommunityPoolResponse(google.protobuf.message.Message):
     """MsgFundCommunityPoolResponse defines the Msg/FundCommunityPool response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/distribution/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/evidence_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Equivocation(google.protobuf.message.Message):
     """Equivocation implements the Evidence interface and defines evidence of double
     signing misbehavior.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/genesis_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the evidence module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVIDENCE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryEvidenceRequest(google.protobuf.message.Message):
     """QueryEvidenceRequest is the request type for the Query/Evidence RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVIDENCE_HASH_FIELD_NUMBER: builtins.int
     evidence_hash: builtins.bytes
@@ -31,14 +32,15 @@
         *,
         evidence_hash: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["evidence_hash", b"evidence_hash"]) -> None: ...
 
 global___QueryEvidenceRequest = QueryEvidenceRequest
 
+@typing_extensions.final
 class QueryEvidenceResponse(google.protobuf.message.Message):
     """QueryEvidenceResponse is the response type for the Query/Evidence RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVIDENCE_FIELD_NUMBER: builtins.int
     @property
@@ -50,14 +52,15 @@
         evidence: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["evidence", b"evidence"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["evidence", b"evidence"]) -> None: ...
 
 global___QueryEvidenceResponse = QueryEvidenceResponse
 
+@typing_extensions.final
 class QueryAllEvidenceRequest(google.protobuf.message.Message):
     """QueryEvidenceRequest is the request type for the Query/AllEvidence RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -71,14 +74,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryAllEvidenceRequest = QueryAllEvidenceRequest
 
+@typing_extensions.final
 class QueryAllEvidenceResponse(google.protobuf.message.Message):
     """QueryAllEvidenceResponse is the response type for the Query/AllEvidence RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgSubmitEvidence(google.protobuf.message.Message):
     """MsgSubmitEvidence represents a message that supports submitting arbitrary
     Evidence of misbehavior such as equivocation or counterfactual signing.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -34,14 +35,15 @@
         evidence: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["evidence", b"evidence"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["evidence", b"evidence", "submitter", b"submitter"]) -> None: ...
 
 global___MsgSubmitEvidence = MsgSubmitEvidence
 
+@typing_extensions.final
 class MsgSubmitEvidenceResponse(google.protobuf.message.Message):
     """MsgSubmitEvidenceResponse defines the Msg/SubmitEvidence response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HASH_FIELD_NUMBER: builtins.int
     hash: builtins.bytes
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/evidence/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/feegrant_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class BasicAllowance(google.protobuf.message.Message):
     """BasicAllowance implements Allowance with a one-time grant of tokens
     that optionally expires. The grantee can use up to SpendLimit to cover fees.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -45,14 +46,15 @@
         expiration: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["expiration", b"expiration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["expiration", b"expiration", "spend_limit", b"spend_limit"]) -> None: ...
 
 global___BasicAllowance = BasicAllowance
 
+@typing_extensions.final
 class PeriodicAllowance(google.protobuf.message.Message):
     """PeriodicAllowance extends Allowance to allow for both a maximum cap,
     as well as a limit per time period.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -93,14 +95,15 @@
         period_reset: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["basic", b"basic", "period", b"period", "period_reset", b"period_reset"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["basic", b"basic", "period", b"period", "period_can_spend", b"period_can_spend", "period_reset", b"period_reset", "period_spend_limit", b"period_spend_limit"]) -> None: ...
 
 global___PeriodicAllowance = PeriodicAllowance
 
+@typing_extensions.final
 class AllowedMsgAllowance(google.protobuf.message.Message):
     """AllowedMsgAllowance creates allowance only for specified message types."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOWANCE_FIELD_NUMBER: builtins.int
     ALLOWED_MESSAGES_FIELD_NUMBER: builtins.int
@@ -117,14 +120,15 @@
         allowed_messages: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["allowance", b"allowance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["allowance", b"allowance", "allowed_messages", b"allowed_messages"]) -> None: ...
 
 global___AllowedMsgAllowance = AllowedMsgAllowance
 
+@typing_extensions.final
 class Grant(google.protobuf.message.Message):
     """Grant is stored in the KVStore to record a grant with full context"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTER_FIELD_NUMBER: builtins.int
     GRANTEE_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/genesis_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState contains a set of fee allowances, persisted from the store"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOWANCES_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryAllowanceRequest(google.protobuf.message.Message):
     """QueryAllowanceRequest is the request type for the Query/Allowance RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTER_FIELD_NUMBER: builtins.int
     GRANTEE_FIELD_NUMBER: builtins.int
@@ -35,14 +36,15 @@
         granter: builtins.str = ...,
         grantee: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "granter", b"granter"]) -> None: ...
 
 global___QueryAllowanceRequest = QueryAllowanceRequest
 
+@typing_extensions.final
 class QueryAllowanceResponse(google.protobuf.message.Message):
     """QueryAllowanceResponse is the response type for the Query/Allowance RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOWANCE_FIELD_NUMBER: builtins.int
     @property
@@ -54,14 +56,15 @@
         allowance: cosmos.feegrant.v1beta1.feegrant_pb2.Grant | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["allowance", b"allowance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["allowance", b"allowance"]) -> None: ...
 
 global___QueryAllowanceResponse = QueryAllowanceResponse
 
+@typing_extensions.final
 class QueryAllowancesRequest(google.protobuf.message.Message):
     """QueryAllowancesRequest is the request type for the Query/Allowances RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTEE_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -76,14 +79,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "pagination", b"pagination"]) -> None: ...
 
 global___QueryAllowancesRequest = QueryAllowancesRequest
 
+@typing_extensions.final
 class QueryAllowancesResponse(google.protobuf.message.Message):
     """QueryAllowancesResponse is the response type for the Query/Allowances RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOWANCES_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgGrantAllowance(google.protobuf.message.Message):
     """MsgGrantAllowance adds permission for Grantee to spend up to Allowance
     of fees from the account of Granter.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -40,25 +41,27 @@
         allowance: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["allowance", b"allowance"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["allowance", b"allowance", "grantee", b"grantee", "granter", b"granter"]) -> None: ...
 
 global___MsgGrantAllowance = MsgGrantAllowance
 
+@typing_extensions.final
 class MsgGrantAllowanceResponse(google.protobuf.message.Message):
     """MsgGrantAllowanceResponse defines the Msg/GrantAllowanceResponse response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgGrantAllowanceResponse = MsgGrantAllowanceResponse
 
+@typing_extensions.final
 class MsgRevokeAllowance(google.protobuf.message.Message):
     """MsgRevokeAllowance removes any existing Allowance from Granter to Grantee."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRANTER_FIELD_NUMBER: builtins.int
     GRANTEE_FIELD_NUMBER: builtins.int
@@ -72,14 +75,15 @@
         granter: builtins.str = ...,
         grantee: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["grantee", b"grantee", "granter", b"granter"]) -> None: ...
 
 global___MsgRevokeAllowance = MsgRevokeAllowance
 
+@typing_extensions.final
 class MsgRevokeAllowanceResponse(google.protobuf.message.Message):
     """MsgRevokeAllowanceResponse defines the Msg/RevokeAllowanceResponse response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/feegrant/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/genutil/v1beta1/genesis_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the raw genesis transaction in JSON."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GEN_TXS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/genesis_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the gov module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STARTING_PROPOSAL_ID_FIELD_NUMBER: builtins.int
     DEPOSITS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/gov_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _VoteOption:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _VoteOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_VoteOption.ValueType], builtins.type):  # noqa: F821
+class _VoteOptionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_VoteOption.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     VOTE_OPTION_UNSPECIFIED: _VoteOption.ValueType  # 0
     """VOTE_OPTION_UNSPECIFIED defines a no-op vote option."""
     VOTE_OPTION_YES: _VoteOption.ValueType  # 1
     """VOTE_OPTION_YES defines a yes vote option."""
     VOTE_OPTION_ABSTAIN: _VoteOption.ValueType  # 2
     """VOTE_OPTION_ABSTAIN defines an abstain vote option."""
@@ -54,15 +54,15 @@
 """VOTE_OPTION_NO_WITH_VETO defines a no with veto vote option."""
 global___VoteOption = VoteOption
 
 class _ProposalStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ProposalStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ProposalStatus.ValueType], builtins.type):  # noqa: F821
+class _ProposalStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ProposalStatus.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     PROPOSAL_STATUS_UNSPECIFIED: _ProposalStatus.ValueType  # 0
     """PROPOSAL_STATUS_UNSPECIFIED defines the default propopsal status."""
     PROPOSAL_STATUS_DEPOSIT_PERIOD: _ProposalStatus.ValueType  # 1
     """PROPOSAL_STATUS_DEPOSIT_PERIOD defines a proposal status during the deposit
     period.
     """
@@ -106,14 +106,15 @@
 """
 PROPOSAL_STATUS_FAILED: ProposalStatus.ValueType  # 5
 """PROPOSAL_STATUS_FAILED defines a proposal status of a proposal that has
 failed.
 """
 global___ProposalStatus = ProposalStatus
 
+@typing_extensions.final
 class WeightedVoteOption(google.protobuf.message.Message):
     """WeightedVoteOption defines a unit of vote for vote split.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -128,14 +129,15 @@
         option: global___VoteOption.ValueType = ...,
         weight: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["option", b"option", "weight", b"weight"]) -> None: ...
 
 global___WeightedVoteOption = WeightedVoteOption
 
+@typing_extensions.final
 class TextProposal(google.protobuf.message.Message):
     """TextProposal defines a standard text proposal whose changes need to be
     manually updated in case of approval.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -149,14 +151,15 @@
         title: builtins.str = ...,
         description: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "title", b"title"]) -> None: ...
 
 global___TextProposal = TextProposal
 
+@typing_extensions.final
 class Deposit(google.protobuf.message.Message):
     """Deposit defines an amount deposited by an account address to an active
     proposal.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -174,14 +177,15 @@
         depositor: builtins.str = ...,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "depositor", b"depositor", "proposal_id", b"proposal_id"]) -> None: ...
 
 global___Deposit = Deposit
 
+@typing_extensions.final
 class Proposal(google.protobuf.message.Message):
     """Proposal defines the core field members of a governance proposal."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     CONTENT_FIELD_NUMBER: builtins.int
@@ -225,14 +229,15 @@
         is_expedited: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["content", b"content", "deposit_end_time", b"deposit_end_time", "final_tally_result", b"final_tally_result", "submit_time", b"submit_time", "voting_end_time", b"voting_end_time", "voting_start_time", b"voting_start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["content", b"content", "deposit_end_time", b"deposit_end_time", "final_tally_result", b"final_tally_result", "is_expedited", b"is_expedited", "proposal_id", b"proposal_id", "status", b"status", "submit_time", b"submit_time", "total_deposit", b"total_deposit", "voting_end_time", b"voting_end_time", "voting_start_time", b"voting_start_time"]) -> None: ...
 
 global___Proposal = Proposal
 
+@typing_extensions.final
 class TallyResult(google.protobuf.message.Message):
     """TallyResult defines a standard tally for a governance proposal."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     YES_FIELD_NUMBER: builtins.int
     ABSTAIN_FIELD_NUMBER: builtins.int
@@ -250,14 +255,15 @@
         no: builtins.str = ...,
         no_with_veto: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["abstain", b"abstain", "no", b"no", "no_with_veto", b"no_with_veto", "yes", b"yes"]) -> None: ...
 
 global___TallyResult = TallyResult
 
+@typing_extensions.final
 class Vote(google.protobuf.message.Message):
     """Vote defines a vote on a governance proposal.
     A Vote consists of a proposal ID, the voter, and the vote option.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -283,14 +289,15 @@
         option: global___VoteOption.ValueType = ...,
         options: collections.abc.Iterable[global___WeightedVoteOption] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["option", b"option", "options", b"options", "proposal_id", b"proposal_id", "voter", b"voter"]) -> None: ...
 
 global___Vote = Vote
 
+@typing_extensions.final
 class DepositParams(google.protobuf.message.Message):
     """DepositParams defines the params for deposits on governance proposals."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MIN_DEPOSIT_FIELD_NUMBER: builtins.int
     MAX_DEPOSIT_PERIOD_FIELD_NUMBER: builtins.int
@@ -318,14 +325,15 @@
         min_initial_deposit_ratio: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["max_deposit_period", b"max_deposit_period"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["max_deposit_period", b"max_deposit_period", "min_deposit", b"min_deposit", "min_expedited_deposit", b"min_expedited_deposit", "min_initial_deposit_ratio", b"min_initial_deposit_ratio"]) -> None: ...
 
 global___DepositParams = DepositParams
 
+@typing_extensions.final
 class VotingParams(google.protobuf.message.Message):
     """VotingParams defines the params for voting on governance proposals."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOTING_PERIOD_FIELD_NUMBER: builtins.int
     PROPOSAL_VOTING_PERIODS_FIELD_NUMBER: builtins.int
@@ -347,14 +355,15 @@
         expedited_voting_period: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["expedited_voting_period", b"expedited_voting_period", "voting_period", b"voting_period"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["expedited_voting_period", b"expedited_voting_period", "proposal_voting_periods", b"proposal_voting_periods", "voting_period", b"voting_period"]) -> None: ...
 
 global___VotingParams = VotingParams
 
+@typing_extensions.final
 class TallyParams(google.protobuf.message.Message):
     """TallyParams defines the params for tallying votes on governance proposals."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     QUORUM_FIELD_NUMBER: builtins.int
     THRESHOLD_FIELD_NUMBER: builtins.int
@@ -380,14 +389,15 @@
         veto_threshold: builtins.bytes = ...,
         expedited_threshold: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["expedited_threshold", b"expedited_threshold", "quorum", b"quorum", "threshold", b"threshold", "veto_threshold", b"veto_threshold"]) -> None: ...
 
 global___TallyParams = TallyParams
 
+@typing_extensions.final
 class ProposalVotingPeriod(google.protobuf.message.Message):
     """ProposalVotingPeriod defines custom voting periods for a unique governance
     proposal type.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryProposalRequest(google.protobuf.message.Message):
     """QueryProposalRequest is the request type for the Query/Proposal RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     proposal_id: builtins.int
@@ -31,14 +32,15 @@
         *,
         proposal_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposal_id", b"proposal_id"]) -> None: ...
 
 global___QueryProposalRequest = QueryProposalRequest
 
+@typing_extensions.final
 class QueryProposalResponse(google.protobuf.message.Message):
     """QueryProposalResponse is the response type for the Query/Proposal RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_FIELD_NUMBER: builtins.int
     @property
@@ -49,14 +51,15 @@
         proposal: cosmos.gov.v1beta1.gov_pb2.Proposal | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["proposal", b"proposal"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposal", b"proposal"]) -> None: ...
 
 global___QueryProposalResponse = QueryProposalResponse
 
+@typing_extensions.final
 class QueryProposalsRequest(google.protobuf.message.Message):
     """QueryProposalsRequest is the request type for the Query/Proposals RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_STATUS_FIELD_NUMBER: builtins.int
     VOTER_FIELD_NUMBER: builtins.int
@@ -80,14 +83,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["depositor", b"depositor", "pagination", b"pagination", "proposal_status", b"proposal_status", "voter", b"voter"]) -> None: ...
 
 global___QueryProposalsRequest = QueryProposalsRequest
 
+@typing_extensions.final
 class QueryProposalsResponse(google.protobuf.message.Message):
     """QueryProposalsResponse is the response type for the Query/Proposals RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -105,14 +109,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "proposals", b"proposals"]) -> None: ...
 
 global___QueryProposalsResponse = QueryProposalsResponse
 
+@typing_extensions.final
 class QueryVoteRequest(google.protobuf.message.Message):
     """QueryVoteRequest is the request type for the Query/Vote RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     VOTER_FIELD_NUMBER: builtins.int
@@ -126,14 +131,15 @@
         proposal_id: builtins.int = ...,
         voter: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposal_id", b"proposal_id", "voter", b"voter"]) -> None: ...
 
 global___QueryVoteRequest = QueryVoteRequest
 
+@typing_extensions.final
 class QueryVoteResponse(google.protobuf.message.Message):
     """QueryVoteResponse is the response type for the Query/Vote RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOTE_FIELD_NUMBER: builtins.int
     @property
@@ -145,14 +151,15 @@
         vote: cosmos.gov.v1beta1.gov_pb2.Vote | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["vote", b"vote"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["vote", b"vote"]) -> None: ...
 
 global___QueryVoteResponse = QueryVoteResponse
 
+@typing_extensions.final
 class QueryVotesRequest(google.protobuf.message.Message):
     """QueryVotesRequest is the request type for the Query/Votes RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -168,14 +175,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "proposal_id", b"proposal_id"]) -> None: ...
 
 global___QueryVotesRequest = QueryVotesRequest
 
+@typing_extensions.final
 class QueryVotesResponse(google.protobuf.message.Message):
     """QueryVotesResponse is the response type for the Query/Votes RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOTES_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -192,14 +200,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "votes", b"votes"]) -> None: ...
 
 global___QueryVotesResponse = QueryVotesResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_TYPE_FIELD_NUMBER: builtins.int
     params_type: builtins.str
@@ -211,14 +220,15 @@
         *,
         params_type: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["params_type", b"params_type"]) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOTING_PARAMS_FIELD_NUMBER: builtins.int
     DEPOSIT_PARAMS_FIELD_NUMBER: builtins.int
@@ -240,14 +250,15 @@
         tally_params: cosmos.gov.v1beta1.gov_pb2.TallyParams | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["deposit_params", b"deposit_params", "tally_params", b"tally_params", "voting_params", b"voting_params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["deposit_params", b"deposit_params", "tally_params", b"tally_params", "voting_params", b"voting_params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryDepositRequest(google.protobuf.message.Message):
     """QueryDepositRequest is the request type for the Query/Deposit RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     DEPOSITOR_FIELD_NUMBER: builtins.int
@@ -261,14 +272,15 @@
         proposal_id: builtins.int = ...,
         depositor: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["depositor", b"depositor", "proposal_id", b"proposal_id"]) -> None: ...
 
 global___QueryDepositRequest = QueryDepositRequest
 
+@typing_extensions.final
 class QueryDepositResponse(google.protobuf.message.Message):
     """QueryDepositResponse is the response type for the Query/Deposit RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEPOSIT_FIELD_NUMBER: builtins.int
     @property
@@ -280,14 +292,15 @@
         deposit: cosmos.gov.v1beta1.gov_pb2.Deposit | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["deposit", b"deposit"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["deposit", b"deposit"]) -> None: ...
 
 global___QueryDepositResponse = QueryDepositResponse
 
+@typing_extensions.final
 class QueryDepositsRequest(google.protobuf.message.Message):
     """QueryDepositsRequest is the request type for the Query/Deposits RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -303,14 +316,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "proposal_id", b"proposal_id"]) -> None: ...
 
 global___QueryDepositsRequest = QueryDepositsRequest
 
+@typing_extensions.final
 class QueryDepositsResponse(google.protobuf.message.Message):
     """QueryDepositsResponse is the response type for the Query/Deposits RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEPOSITS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -326,14 +340,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["deposits", b"deposits", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDepositsResponse = QueryDepositsResponse
 
+@typing_extensions.final
 class QueryTallyResultRequest(google.protobuf.message.Message):
     """QueryTallyResultRequest is the request type for the Query/Tally RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     proposal_id: builtins.int
@@ -343,14 +358,15 @@
         *,
         proposal_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposal_id", b"proposal_id"]) -> None: ...
 
 global___QueryTallyResultRequest = QueryTallyResultRequest
 
+@typing_extensions.final
 class QueryTallyResultResponse(google.protobuf.message.Message):
     """QueryTallyResultResponse is the response type for the Query/Tally RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TALLY_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgSubmitProposal(google.protobuf.message.Message):
     """MsgSubmitProposal defines an sdk.Msg type that supports submitting arbitrary
     proposal Content.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -45,14 +46,15 @@
         is_expedited: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["content", b"content"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["content", b"content", "initial_deposit", b"initial_deposit", "is_expedited", b"is_expedited", "proposer", b"proposer"]) -> None: ...
 
 global___MsgSubmitProposal = MsgSubmitProposal
 
+@typing_extensions.final
 class MsgSubmitProposalResponse(google.protobuf.message.Message):
     """MsgSubmitProposalResponse defines the Msg/SubmitProposal response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     proposal_id: builtins.int
@@ -61,14 +63,15 @@
         *,
         proposal_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposal_id", b"proposal_id"]) -> None: ...
 
 global___MsgSubmitProposalResponse = MsgSubmitProposalResponse
 
+@typing_extensions.final
 class MsgVote(google.protobuf.message.Message):
     """MsgVote defines a message to cast a vote."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     VOTER_FIELD_NUMBER: builtins.int
@@ -83,25 +86,27 @@
         voter: builtins.str = ...,
         option: cosmos.gov.v1beta1.gov_pb2.VoteOption.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["option", b"option", "proposal_id", b"proposal_id", "voter", b"voter"]) -> None: ...
 
 global___MsgVote = MsgVote
 
+@typing_extensions.final
 class MsgVoteResponse(google.protobuf.message.Message):
     """MsgVoteResponse defines the Msg/Vote response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgVoteResponse = MsgVoteResponse
 
+@typing_extensions.final
 class MsgVoteWeighted(google.protobuf.message.Message):
     """MsgVoteWeighted defines a message to cast a vote.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -120,28 +125,30 @@
         voter: builtins.str = ...,
         options: collections.abc.Iterable[cosmos.gov.v1beta1.gov_pb2.WeightedVoteOption] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["options", b"options", "proposal_id", b"proposal_id", "voter", b"voter"]) -> None: ...
 
 global___MsgVoteWeighted = MsgVoteWeighted
 
+@typing_extensions.final
 class MsgVoteWeightedResponse(google.protobuf.message.Message):
     """MsgVoteWeightedResponse defines the Msg/VoteWeighted response type.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgVoteWeightedResponse = MsgVoteWeightedResponse
 
+@typing_extensions.final
 class MsgDeposit(google.protobuf.message.Message):
     """MsgDeposit defines a message to submit a deposit to an existing proposal."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROPOSAL_ID_FIELD_NUMBER: builtins.int
     DEPOSITOR_FIELD_NUMBER: builtins.int
@@ -157,14 +164,15 @@
         depositor: builtins.str = ...,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "depositor", b"depositor", "proposal_id", b"proposal_id"]) -> None: ...
 
 global___MsgDeposit = MsgDeposit
 
+@typing_extensions.final
 class MsgDepositResponse(google.protobuf.message.Message):
     """MsgDepositResponse defines the Msg/Deposit response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/gov/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/genesis_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the mint module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINTER_FIELD_NUMBER: builtins.int
     PARAMS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/mint_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Minter(google.protobuf.message.Message):
     """Minter represents the minting state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INFLATION_FIELD_NUMBER: builtins.int
     ANNUAL_PROVISIONS_FIELD_NUMBER: builtins.int
@@ -31,14 +32,15 @@
         inflation: builtins.str = ...,
         annual_provisions: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["annual_provisions", b"annual_provisions", "inflation", b"inflation"]) -> None: ...
 
 global___Minter = Minter
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the mint module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINT_DENOM_FIELD_NUMBER: builtins.int
     INFLATION_RATE_CHANGE_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -41,25 +43,27 @@
         params: cosmos.mint.v1beta1.mint_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryInflationRequest(google.protobuf.message.Message):
     """QueryInflationRequest is the request type for the Query/Inflation RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryInflationRequest = QueryInflationRequest
 
+@typing_extensions.final
 class QueryInflationResponse(google.protobuf.message.Message):
     """QueryInflationResponse is the response type for the Query/Inflation RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -71,27 +75,29 @@
         *,
         inflation: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["inflation", b"inflation"]) -> None: ...
 
 global___QueryInflationResponse = QueryInflationResponse
 
+@typing_extensions.final
 class QueryAnnualProvisionsRequest(google.protobuf.message.Message):
     """QueryAnnualProvisionsRequest is the request type for the
     Query/AnnualProvisions RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryAnnualProvisionsRequest = QueryAnnualProvisionsRequest
 
+@typing_extensions.final
 class QueryAnnualProvisionsResponse(google.protobuf.message.Message):
     """QueryAnnualProvisionsResponse is the response type for the
     Query/AnnualProvisions RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/mint/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/params_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ParameterChangeProposal(google.protobuf.message.Message):
     """ParameterChangeProposal defines a proposal to change one or more parameters."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TITLE_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
@@ -35,14 +36,15 @@
         description: builtins.str = ...,
         changes: collections.abc.Iterable[global___ParamChange] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["changes", b"changes", "description", b"description", "title", b"title"]) -> None: ...
 
 global___ParameterChangeProposal = ParameterChangeProposal
 
+@typing_extensions.final
 class ParamChange(google.protobuf.message.Message):
     """ParamChange defines an individual parameter change, for use in
     ParameterChangeProposal.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBSPACE_FIELD_NUMBER: builtins.int
     KEY_FIELD_NUMBER: builtins.int
@@ -32,14 +33,15 @@
         subspace: builtins.str = ...,
         key: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "subspace", b"subspace"]) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAM_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/params/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/genesis_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the slashing module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     SIGNING_INFOS_FIELD_NUMBER: builtins.int
@@ -46,14 +47,15 @@
         missed_blocks: collections.abc.Iterable[global___ValidatorMissedBlocks] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["missed_blocks", b"missed_blocks", "params", b"params", "signing_infos", b"signing_infos"]) -> None: ...
 
 global___GenesisState = GenesisState
 
+@typing_extensions.final
 class SigningInfo(google.protobuf.message.Message):
     """SigningInfo stores validator signing info of corresponding address."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     VALIDATOR_SIGNING_INFO_FIELD_NUMBER: builtins.int
@@ -69,14 +71,15 @@
         validator_signing_info: cosmos.slashing.v1beta1.slashing_pb2.ValidatorSigningInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["validator_signing_info", b"validator_signing_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "validator_signing_info", b"validator_signing_info"]) -> None: ...
 
 global___SigningInfo = SigningInfo
 
+@typing_extensions.final
 class ValidatorMissedBlocks(google.protobuf.message.Message):
     """ValidatorMissedBlocks contains array of missed blocks of corresponding
     address.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -93,14 +96,15 @@
         address: builtins.str = ...,
         missed_blocks: collections.abc.Iterable[global___MissedBlock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "missed_blocks", b"missed_blocks"]) -> None: ...
 
 global___ValidatorMissedBlocks = ValidatorMissedBlocks
 
+@typing_extensions.final
 class MissedBlock(google.protobuf.message.Message):
     """MissedBlock contains height and missed status as boolean."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     MISSED_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -43,14 +45,15 @@
         params: cosmos.slashing.v1beta1.slashing_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QuerySigningInfoRequest(google.protobuf.message.Message):
     """QuerySigningInfoRequest is the request type for the Query/SigningInfo RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -62,14 +65,15 @@
         *,
         cons_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["cons_address", b"cons_address"]) -> None: ...
 
 global___QuerySigningInfoRequest = QuerySigningInfoRequest
 
+@typing_extensions.final
 class QuerySigningInfoResponse(google.protobuf.message.Message):
     """QuerySigningInfoResponse is the response type for the Query/SigningInfo RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -83,14 +87,15 @@
         val_signing_info: cosmos.slashing.v1beta1.slashing_pb2.ValidatorSigningInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["val_signing_info", b"val_signing_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["val_signing_info", b"val_signing_info"]) -> None: ...
 
 global___QuerySigningInfoResponse = QuerySigningInfoResponse
 
+@typing_extensions.final
 class QuerySigningInfosRequest(google.protobuf.message.Message):
     """QuerySigningInfosRequest is the request type for the Query/SigningInfos RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -103,14 +108,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QuerySigningInfosRequest = QuerySigningInfosRequest
 
+@typing_extensions.final
 class QuerySigningInfosResponse(google.protobuf.message.Message):
     """QuerySigningInfosResponse is the response type for the Query/SigningInfos RPC
     method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/slashing_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ValidatorSigningInfo(google.protobuf.message.Message):
     """ValidatorSigningInfo defines a validator's signing info for monitoring their
     liveness activity.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -59,14 +60,15 @@
         missed_blocks_counter: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["jailed_until", b"jailed_until"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "index_offset", b"index_offset", "jailed_until", b"jailed_until", "missed_blocks_counter", b"missed_blocks_counter", "start_height", b"start_height", "tombstoned", b"tombstoned"]) -> None: ...
 
 global___ValidatorSigningInfo = ValidatorSigningInfo
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params represents the parameters used for by the slashing module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SIGNED_BLOCKS_WINDOW_FIELD_NUMBER: builtins.int
     MIN_SIGNED_PER_WINDOW_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgUnjail(google.protobuf.message.Message):
     """MsgUnjail defines the Msg/Unjail request type"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
@@ -26,14 +27,15 @@
         *,
         validator_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_addr", b"validator_addr"]) -> None: ...
 
 global___MsgUnjail = MsgUnjail
 
+@typing_extensions.final
 class MsgUnjailResponse(google.protobuf.message.Message):
     """MsgUnjailResponse defines the Msg/Unjail response type"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/slashing/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/authz_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _AuthorizationType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _AuthorizationTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_AuthorizationType.ValueType], builtins.type):  # noqa: F821
+class _AuthorizationTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_AuthorizationType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     AUTHORIZATION_TYPE_UNSPECIFIED: _AuthorizationType.ValueType  # 0
     """AUTHORIZATION_TYPE_UNSPECIFIED specifies an unknown authorization type"""
     AUTHORIZATION_TYPE_DELEGATE: _AuthorizationType.ValueType  # 1
     """AUTHORIZATION_TYPE_DELEGATE defines an authorization type for Msg/Delegate"""
     AUTHORIZATION_TYPE_UNDELEGATE: _AuthorizationType.ValueType  # 2
     """AUTHORIZATION_TYPE_UNDELEGATE defines an authorization type for Msg/Undelegate"""
@@ -46,22 +46,24 @@
 """AUTHORIZATION_TYPE_DELEGATE defines an authorization type for Msg/Delegate"""
 AUTHORIZATION_TYPE_UNDELEGATE: AuthorizationType.ValueType  # 2
 """AUTHORIZATION_TYPE_UNDELEGATE defines an authorization type for Msg/Undelegate"""
 AUTHORIZATION_TYPE_REDELEGATE: AuthorizationType.ValueType  # 3
 """AUTHORIZATION_TYPE_REDELEGATE defines an authorization type for Msg/BeginRedelegate"""
 global___AuthorizationType = AuthorizationType
 
+@typing_extensions.final
 class StakeAuthorization(google.protobuf.message.Message):
     """StakeAuthorization defines authorization for delegate/undelegate/redelegate.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Validators(google.protobuf.message.Message):
         """Validators defines list of validator addresses."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ADDRESS_FIELD_NUMBER: builtins.int
         @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/genesis_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the staking module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     LAST_TOTAL_POWER_FIELD_NUMBER: builtins.int
@@ -68,14 +69,15 @@
         exported: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegations", b"delegations", "exported", b"exported", "last_total_power", b"last_total_power", "last_validator_powers", b"last_validator_powers", "params", b"params", "redelegations", b"redelegations", "unbonding_delegations", b"unbonding_delegations", "validators", b"validators"]) -> None: ...
 
 global___GenesisState = GenesisState
 
+@typing_extensions.final
 class LastValidatorPower(google.protobuf.message.Message):
     """LastValidatorPower required for validator set update logic."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     POWER_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryValidatorsRequest(google.protobuf.message.Message):
     """QueryValidatorsRequest is request type for Query/Validators RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -37,14 +38,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "status", b"status"]) -> None: ...
 
 global___QueryValidatorsRequest = QueryValidatorsRequest
 
+@typing_extensions.final
 class QueryValidatorsResponse(google.protobuf.message.Message):
     """QueryValidatorsResponse is response type for the Query/Validators RPC method"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATORS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
@@ -61,14 +63,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "validators", b"validators"]) -> None: ...
 
 global___QueryValidatorsResponse = QueryValidatorsResponse
 
+@typing_extensions.final
 class QueryValidatorRequest(google.protobuf.message.Message):
     """QueryValidatorRequest is response type for the Query/Validator RPC method"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
     validator_addr: builtins.str
@@ -78,14 +81,15 @@
         *,
         validator_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryValidatorRequest = QueryValidatorRequest
 
+@typing_extensions.final
 class QueryValidatorResponse(google.protobuf.message.Message):
     """QueryValidatorResponse is response type for the Query/Validator RPC method"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_FIELD_NUMBER: builtins.int
     @property
@@ -97,14 +101,15 @@
         validator: cosmos.staking.v1beta1.staking_pb2.Validator | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["validator", b"validator"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator", b"validator"]) -> None: ...
 
 global___QueryValidatorResponse = QueryValidatorResponse
 
+@typing_extensions.final
 class QueryValidatorDelegationsRequest(google.protobuf.message.Message):
     """QueryValidatorDelegationsRequest is request type for the
     Query/ValidatorDelegations RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -122,14 +127,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryValidatorDelegationsRequest = QueryValidatorDelegationsRequest
 
+@typing_extensions.final
 class QueryValidatorDelegationsResponse(google.protobuf.message.Message):
     """QueryValidatorDelegationsResponse is response type for the
     Query/ValidatorDelegations RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -147,14 +153,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegation_responses", b"delegation_responses", "pagination", b"pagination"]) -> None: ...
 
 global___QueryValidatorDelegationsResponse = QueryValidatorDelegationsResponse
 
+@typing_extensions.final
 class QueryValidatorUnbondingDelegationsRequest(google.protobuf.message.Message):
     """QueryValidatorUnbondingDelegationsRequest is required type for the
     Query/ValidatorUnbondingDelegations RPC method
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -172,14 +179,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryValidatorUnbondingDelegationsRequest = QueryValidatorUnbondingDelegationsRequest
 
+@typing_extensions.final
 class QueryValidatorUnbondingDelegationsResponse(google.protobuf.message.Message):
     """QueryValidatorUnbondingDelegationsResponse is response type for the
     Query/ValidatorUnbondingDelegations RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -197,14 +205,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "unbonding_responses", b"unbonding_responses"]) -> None: ...
 
 global___QueryValidatorUnbondingDelegationsResponse = QueryValidatorUnbondingDelegationsResponse
 
+@typing_extensions.final
 class QueryDelegationRequest(google.protobuf.message.Message):
     """QueryDelegationRequest is request type for the Query/Delegation RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDR_FIELD_NUMBER: builtins.int
     VALIDATOR_ADDR_FIELD_NUMBER: builtins.int
@@ -218,14 +227,15 @@
         delegator_addr: builtins.str = ...,
         validator_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryDelegationRequest = QueryDelegationRequest
 
+@typing_extensions.final
 class QueryDelegationResponse(google.protobuf.message.Message):
     """QueryDelegationResponse is response type for the Query/Delegation RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATION_RESPONSE_FIELD_NUMBER: builtins.int
     @property
@@ -237,14 +247,15 @@
         delegation_response: cosmos.staking.v1beta1.staking_pb2.DelegationResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["delegation_response", b"delegation_response"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegation_response", b"delegation_response"]) -> None: ...
 
 global___QueryDelegationResponse = QueryDelegationResponse
 
+@typing_extensions.final
 class QueryUnbondingDelegationRequest(google.protobuf.message.Message):
     """QueryUnbondingDelegationRequest is request type for the
     Query/UnbondingDelegation RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -260,14 +271,15 @@
         delegator_addr: builtins.str = ...,
         validator_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryUnbondingDelegationRequest = QueryUnbondingDelegationRequest
 
+@typing_extensions.final
 class QueryUnbondingDelegationResponse(google.protobuf.message.Message):
     """QueryDelegationResponse is response type for the Query/UnbondingDelegation
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -281,14 +293,15 @@
         unbond: cosmos.staking.v1beta1.staking_pb2.UnbondingDelegation | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["unbond", b"unbond"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["unbond", b"unbond"]) -> None: ...
 
 global___QueryUnbondingDelegationResponse = QueryUnbondingDelegationResponse
 
+@typing_extensions.final
 class QueryDelegatorDelegationsRequest(google.protobuf.message.Message):
     """QueryDelegatorDelegationsRequest is request type for the
     Query/DelegatorDelegations RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -306,14 +319,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDelegatorDelegationsRequest = QueryDelegatorDelegationsRequest
 
+@typing_extensions.final
 class QueryDelegatorDelegationsResponse(google.protobuf.message.Message):
     """QueryDelegatorDelegationsResponse is response type for the
     Query/DelegatorDelegations RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -332,14 +346,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegation_responses", b"delegation_responses", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDelegatorDelegationsResponse = QueryDelegatorDelegationsResponse
 
+@typing_extensions.final
 class QueryDelegatorUnbondingDelegationsRequest(google.protobuf.message.Message):
     """QueryDelegatorUnbondingDelegationsRequest is request type for the
     Query/DelegatorUnbondingDelegations RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -357,14 +372,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDelegatorUnbondingDelegationsRequest = QueryDelegatorUnbondingDelegationsRequest
 
+@typing_extensions.final
 class QueryDelegatorUnbondingDelegationsResponse(google.protobuf.message.Message):
     """QueryUnbondingDelegatorDelegationsResponse is response type for the
     Query/UnbondingDelegatorDelegations RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -382,14 +398,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "unbonding_responses", b"unbonding_responses"]) -> None: ...
 
 global___QueryDelegatorUnbondingDelegationsResponse = QueryDelegatorUnbondingDelegationsResponse
 
+@typing_extensions.final
 class QueryRedelegationsRequest(google.protobuf.message.Message):
     """QueryRedelegationsRequest is request type for the Query/Redelegations RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -415,14 +432,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "dst_validator_addr", b"dst_validator_addr", "pagination", b"pagination", "src_validator_addr", b"src_validator_addr"]) -> None: ...
 
 global___QueryRedelegationsRequest = QueryRedelegationsRequest
 
+@typing_extensions.final
 class QueryRedelegationsResponse(google.protobuf.message.Message):
     """QueryRedelegationsResponse is response type for the Query/Redelegations RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -440,14 +458,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "redelegation_responses", b"redelegation_responses"]) -> None: ...
 
 global___QueryRedelegationsResponse = QueryRedelegationsResponse
 
+@typing_extensions.final
 class QueryDelegatorValidatorsRequest(google.protobuf.message.Message):
     """QueryDelegatorValidatorsRequest is request type for the
     Query/DelegatorValidators RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -465,14 +484,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "pagination", b"pagination"]) -> None: ...
 
 global___QueryDelegatorValidatorsRequest = QueryDelegatorValidatorsRequest
 
+@typing_extensions.final
 class QueryDelegatorValidatorsResponse(google.protobuf.message.Message):
     """QueryDelegatorValidatorsResponse is response type for the
     Query/DelegatorValidators RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -491,14 +511,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "validators", b"validators"]) -> None: ...
 
 global___QueryDelegatorValidatorsResponse = QueryDelegatorValidatorsResponse
 
+@typing_extensions.final
 class QueryDelegatorValidatorRequest(google.protobuf.message.Message):
     """QueryDelegatorValidatorRequest is request type for the
     Query/DelegatorValidator RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -514,14 +535,15 @@
         delegator_addr: builtins.str = ...,
         validator_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_addr", b"delegator_addr", "validator_addr", b"validator_addr"]) -> None: ...
 
 global___QueryDelegatorValidatorRequest = QueryDelegatorValidatorRequest
 
+@typing_extensions.final
 class QueryDelegatorValidatorResponse(google.protobuf.message.Message):
     """QueryDelegatorValidatorResponse response type for the
     Query/DelegatorValidator RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -535,14 +557,15 @@
         validator: cosmos.staking.v1beta1.staking_pb2.Validator | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["validator", b"validator"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["validator", b"validator"]) -> None: ...
 
 global___QueryDelegatorValidatorResponse = QueryDelegatorValidatorResponse
 
+@typing_extensions.final
 class QueryHistoricalInfoRequest(google.protobuf.message.Message):
     """QueryHistoricalInfoRequest is request type for the Query/HistoricalInfo RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -554,14 +577,15 @@
         *,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height"]) -> None: ...
 
 global___QueryHistoricalInfoRequest = QueryHistoricalInfoRequest
 
+@typing_extensions.final
 class QueryHistoricalInfoResponse(google.protobuf.message.Message):
     """QueryHistoricalInfoResponse is response type for the Query/HistoricalInfo RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -575,25 +599,27 @@
         hist: cosmos.staking.v1beta1.staking_pb2.HistoricalInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["hist", b"hist"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["hist", b"hist"]) -> None: ...
 
 global___QueryHistoricalInfoResponse = QueryHistoricalInfoResponse
 
+@typing_extensions.final
 class QueryPoolRequest(google.protobuf.message.Message):
     """QueryPoolRequest is request type for the Query/Pool RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryPoolRequest = QueryPoolRequest
 
+@typing_extensions.final
 class QueryPoolResponse(google.protobuf.message.Message):
     """QueryPoolResponse is response type for the Query/Pool RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_FIELD_NUMBER: builtins.int
     @property
@@ -605,25 +631,27 @@
         pool: cosmos.staking.v1beta1.staking_pb2.Pool | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pool", b"pool"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool", b"pool"]) -> None: ...
 
 global___QueryPoolResponse = QueryPoolResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/staking_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _BondStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _BondStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BondStatus.ValueType], builtins.type):  # noqa: F821
+class _BondStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BondStatus.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     BOND_STATUS_UNSPECIFIED: _BondStatus.ValueType  # 0
     """UNSPECIFIED defines an invalid validator status."""
     BOND_STATUS_UNBONDED: _BondStatus.ValueType  # 1
     """UNBONDED defines a validator that is not bonded."""
     BOND_STATUS_UNBONDING: _BondStatus.ValueType  # 2
     """UNBONDING defines a validator that is unbonding."""
@@ -47,14 +47,15 @@
 """UNBONDED defines a validator that is not bonded."""
 BOND_STATUS_UNBONDING: BondStatus.ValueType  # 2
 """UNBONDING defines a validator that is unbonding."""
 BOND_STATUS_BONDED: BondStatus.ValueType  # 3
 """BONDED defines a validator that is bonded."""
 global___BondStatus = BondStatus
 
+@typing_extensions.final
 class HistoricalInfo(google.protobuf.message.Message):
     """HistoricalInfo contains header and validator information for a given block.
     It is stored as part of staking module's state, which persists the `n` most
     recent HistoricalInfo
     (`n` is set by the staking module's `historical_entries` parameter).
     """
 
@@ -73,14 +74,15 @@
         valset: collections.abc.Iterable[global___Validator] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["header", b"header"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["header", b"header", "valset", b"valset"]) -> None: ...
 
 global___HistoricalInfo = HistoricalInfo
 
+@typing_extensions.final
 class CommissionRates(google.protobuf.message.Message):
     """CommissionRates defines the initial commission rates to be used for creating
     a validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -100,14 +102,15 @@
         max_rate: builtins.str = ...,
         max_change_rate: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["max_change_rate", b"max_change_rate", "max_rate", b"max_rate", "rate", b"rate"]) -> None: ...
 
 global___CommissionRates = CommissionRates
 
+@typing_extensions.final
 class Commission(google.protobuf.message.Message):
     """Commission defines commission parameters for a given validator."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMMISSION_RATES_FIELD_NUMBER: builtins.int
     UPDATE_TIME_FIELD_NUMBER: builtins.int
@@ -124,14 +127,15 @@
         update_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commission_rates", b"commission_rates", "update_time", b"update_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission_rates", b"commission_rates", "update_time", b"update_time"]) -> None: ...
 
 global___Commission = Commission
 
+@typing_extensions.final
 class Description(google.protobuf.message.Message):
     """Description defines a validator description."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MONIKER_FIELD_NUMBER: builtins.int
     IDENTITY_FIELD_NUMBER: builtins.int
@@ -157,14 +161,15 @@
         security_contact: builtins.str = ...,
         details: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["details", b"details", "identity", b"identity", "moniker", b"moniker", "security_contact", b"security_contact", "website", b"website"]) -> None: ...
 
 global___Description = Description
 
+@typing_extensions.final
 class Validator(google.protobuf.message.Message):
     """Validator defines a validator, together with the total amount of the
     Validator's bond shares and their exchange rate to coins. Slashing results in
     a decrease in the exchange rate, allowing correct calculation of future
     undelegations without iterating over delegators. When coins are delegated to
     this validator, the validator is credited with a delegation whose number of
     bond shares is based on the amount of coins delegated divided by the current
@@ -227,14 +232,15 @@
         min_self_delegation: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commission", b"commission", "consensus_pubkey", b"consensus_pubkey", "description", b"description", "unbonding_time", b"unbonding_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission", b"commission", "consensus_pubkey", b"consensus_pubkey", "delegator_shares", b"delegator_shares", "description", b"description", "jailed", b"jailed", "min_self_delegation", b"min_self_delegation", "operator_address", b"operator_address", "status", b"status", "tokens", b"tokens", "unbonding_height", b"unbonding_height", "unbonding_time", b"unbonding_time"]) -> None: ...
 
 global___Validator = Validator
 
+@typing_extensions.final
 class ValAddresses(google.protobuf.message.Message):
     """ValAddresses defines a repeated set of validator addresses."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESSES_FIELD_NUMBER: builtins.int
     @property
@@ -244,14 +250,15 @@
         *,
         addresses: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["addresses", b"addresses"]) -> None: ...
 
 global___ValAddresses = ValAddresses
 
+@typing_extensions.final
 class DVPair(google.protobuf.message.Message):
     """DVPair is struct that just has a delegator-validator pair with no other data.
     It is intended to be used as a marshalable pointer. For example, a DVPair can
     be used to construct the key to getting an UnbondingDelegation from state.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -266,14 +273,15 @@
         delegator_address: builtins.str = ...,
         validator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "validator_address", b"validator_address"]) -> None: ...
 
 global___DVPair = DVPair
 
+@typing_extensions.final
 class DVPairs(google.protobuf.message.Message):
     """DVPairs defines an array of DVPair objects."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAIRS_FIELD_NUMBER: builtins.int
     @property
@@ -283,14 +291,15 @@
         *,
         pairs: collections.abc.Iterable[global___DVPair] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pairs", b"pairs"]) -> None: ...
 
 global___DVPairs = DVPairs
 
+@typing_extensions.final
 class DVVTriplet(google.protobuf.message.Message):
     """DVVTriplet is struct that just has a delegator-validator-validator triplet
     with no other data. It is intended to be used as a marshalable pointer. For
     example, a DVVTriplet can be used to construct the key to getting a
     Redelegation from state.
     """
 
@@ -309,14 +318,15 @@
         validator_src_address: builtins.str = ...,
         validator_dst_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "validator_dst_address", b"validator_dst_address", "validator_src_address", b"validator_src_address"]) -> None: ...
 
 global___DVVTriplet = DVVTriplet
 
+@typing_extensions.final
 class DVVTriplets(google.protobuf.message.Message):
     """DVVTriplets defines an array of DVVTriplet objects."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRIPLETS_FIELD_NUMBER: builtins.int
     @property
@@ -326,14 +336,15 @@
         *,
         triplets: collections.abc.Iterable[global___DVVTriplet] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["triplets", b"triplets"]) -> None: ...
 
 global___DVVTriplets = DVVTriplets
 
+@typing_extensions.final
 class Delegation(google.protobuf.message.Message):
     """Delegation represents the bond with tokens held by an account. It is
     owned by one delegator, and is associated with the voting power of one
     validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -354,14 +365,15 @@
         validator_address: builtins.str = ...,
         shares: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "shares", b"shares", "validator_address", b"validator_address"]) -> None: ...
 
 global___Delegation = Delegation
 
+@typing_extensions.final
 class UnbondingDelegation(google.protobuf.message.Message):
     """UnbondingDelegation stores all of a single delegator's unbonding bonds
     for a single validator in an time-ordered list.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -384,14 +396,15 @@
         validator_address: builtins.str = ...,
         entries: collections.abc.Iterable[global___UnbondingDelegationEntry] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "entries", b"entries", "validator_address", b"validator_address"]) -> None: ...
 
 global___UnbondingDelegation = UnbondingDelegation
 
+@typing_extensions.final
 class UnbondingDelegationEntry(google.protobuf.message.Message):
     """UnbondingDelegationEntry defines an unbonding object with relevant metadata."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CREATION_HEIGHT_FIELD_NUMBER: builtins.int
     COMPLETION_TIME_FIELD_NUMBER: builtins.int
@@ -415,14 +428,15 @@
         balance: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["completion_time", b"completion_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balance", b"balance", "completion_time", b"completion_time", "creation_height", b"creation_height", "initial_balance", b"initial_balance"]) -> None: ...
 
 global___UnbondingDelegationEntry = UnbondingDelegationEntry
 
+@typing_extensions.final
 class RedelegationEntry(google.protobuf.message.Message):
     """RedelegationEntry defines a redelegation object with relevant metadata."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CREATION_HEIGHT_FIELD_NUMBER: builtins.int
     COMPLETION_TIME_FIELD_NUMBER: builtins.int
@@ -446,14 +460,15 @@
         shares_dst: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["completion_time", b"completion_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["completion_time", b"completion_time", "creation_height", b"creation_height", "initial_balance", b"initial_balance", "shares_dst", b"shares_dst"]) -> None: ...
 
 global___RedelegationEntry = RedelegationEntry
 
+@typing_extensions.final
 class Redelegation(google.protobuf.message.Message):
     """Redelegation contains the list of a particular delegator's redelegating bonds
     from a particular source validator to a particular destination validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -480,14 +495,15 @@
         validator_dst_address: builtins.str = ...,
         entries: collections.abc.Iterable[global___RedelegationEntry] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "entries", b"entries", "validator_dst_address", b"validator_dst_address", "validator_src_address", b"validator_src_address"]) -> None: ...
 
 global___Redelegation = Redelegation
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the parameters for the staking module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     UNBONDING_TIME_FIELD_NUMBER: builtins.int
     MAX_VALIDATORS_FIELD_NUMBER: builtins.int
@@ -523,14 +539,15 @@
         min_self_delegation: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["unbonding_time", b"unbonding_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["bond_denom", b"bond_denom", "historical_entries", b"historical_entries", "max_entries", b"max_entries", "max_validators", b"max_validators", "min_commission_rate", b"min_commission_rate", "min_self_delegation", b"min_self_delegation", "unbonding_time", b"unbonding_time"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class DelegationResponse(google.protobuf.message.Message):
     """DelegationResponse is equivalent to Delegation except that it contains a
     balance in addition to shares which is more suitable for client responses.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -547,14 +564,15 @@
         balance: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["balance", b"balance", "delegation", b"delegation"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balance", b"balance", "delegation", b"delegation"]) -> None: ...
 
 global___DelegationResponse = DelegationResponse
 
+@typing_extensions.final
 class RedelegationEntryResponse(google.protobuf.message.Message):
     """RedelegationEntryResponse is equivalent to a RedelegationEntry except that it
     contains a balance in addition to shares which is more suitable for client
     responses.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -571,14 +589,15 @@
         balance: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["redelegation_entry", b"redelegation_entry"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["balance", b"balance", "redelegation_entry", b"redelegation_entry"]) -> None: ...
 
 global___RedelegationEntryResponse = RedelegationEntryResponse
 
+@typing_extensions.final
 class RedelegationResponse(google.protobuf.message.Message):
     """RedelegationResponse is equivalent to a Redelegation except that its entries
     contain a balance in addition to shares which is more suitable for client
     responses.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -596,14 +615,15 @@
         entries: collections.abc.Iterable[global___RedelegationEntryResponse] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["redelegation", b"redelegation"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["entries", b"entries", "redelegation", b"redelegation"]) -> None: ...
 
 global___RedelegationResponse = RedelegationResponse
 
+@typing_extensions.final
 class Pool(google.protobuf.message.Message):
     """Pool is used for tracking bonded and not-bonded token supply of the bond
     denomination.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateValidator(google.protobuf.message.Message):
     """MsgCreateValidator defines a SDK message for creating a new validator."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     COMMISSION_FIELD_NUMBER: builtins.int
@@ -53,25 +54,27 @@
         value: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commission", b"commission", "description", b"description", "pubkey", b"pubkey", "value", b"value"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission", b"commission", "delegator_address", b"delegator_address", "description", b"description", "min_self_delegation", b"min_self_delegation", "pubkey", b"pubkey", "validator_address", b"validator_address", "value", b"value"]) -> None: ...
 
 global___MsgCreateValidator = MsgCreateValidator
 
+@typing_extensions.final
 class MsgCreateValidatorResponse(google.protobuf.message.Message):
     """MsgCreateValidatorResponse defines the Msg/CreateValidator response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgCreateValidatorResponse = MsgCreateValidatorResponse
 
+@typing_extensions.final
 class MsgEditValidator(google.protobuf.message.Message):
     """MsgEditValidator defines a SDK message for editing an existing validator."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
@@ -96,25 +99,27 @@
         min_self_delegation: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["description", b"description"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commission_rate", b"commission_rate", "description", b"description", "min_self_delegation", b"min_self_delegation", "validator_address", b"validator_address"]) -> None: ...
 
 global___MsgEditValidator = MsgEditValidator
 
+@typing_extensions.final
 class MsgEditValidatorResponse(google.protobuf.message.Message):
     """MsgEditValidatorResponse defines the Msg/EditValidator response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgEditValidatorResponse = MsgEditValidatorResponse
 
+@typing_extensions.final
 class MsgDelegate(google.protobuf.message.Message):
     """MsgDelegate defines a SDK message for performing a delegation of coins
     from a delegator to a validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -133,25 +138,27 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "delegator_address", b"delegator_address", "validator_address", b"validator_address"]) -> None: ...
 
 global___MsgDelegate = MsgDelegate
 
+@typing_extensions.final
 class MsgDelegateResponse(google.protobuf.message.Message):
     """MsgDelegateResponse defines the Msg/Delegate response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgDelegateResponse = MsgDelegateResponse
 
+@typing_extensions.final
 class MsgBeginRedelegate(google.protobuf.message.Message):
     """MsgBeginRedelegate defines a SDK message for performing a redelegation
     of coins from a delegator and source validator to a destination validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -173,14 +180,15 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "delegator_address", b"delegator_address", "validator_dst_address", b"validator_dst_address", "validator_src_address", b"validator_src_address"]) -> None: ...
 
 global___MsgBeginRedelegate = MsgBeginRedelegate
 
+@typing_extensions.final
 class MsgBeginRedelegateResponse(google.protobuf.message.Message):
     """MsgBeginRedelegateResponse defines the Msg/BeginRedelegate response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMPLETION_TIME_FIELD_NUMBER: builtins.int
     @property
@@ -191,14 +199,15 @@
         completion_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["completion_time", b"completion_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["completion_time", b"completion_time"]) -> None: ...
 
 global___MsgBeginRedelegateResponse = MsgBeginRedelegateResponse
 
+@typing_extensions.final
 class MsgUndelegate(google.protobuf.message.Message):
     """MsgUndelegate defines a SDK message for performing an undelegation from a
     delegate and a validator.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -217,14 +226,15 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "delegator_address", b"delegator_address", "validator_address", b"validator_address"]) -> None: ...
 
 global___MsgUndelegate = MsgUndelegate
 
+@typing_extensions.final
 class MsgUndelegateResponse(google.protobuf.message.Message):
     """MsgUndelegateResponse defines the Msg/Undelegate response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMPLETION_TIME_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/staking/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/signing/v1beta1/signing_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _SignMode:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _SignModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignMode.ValueType], builtins.type):  # noqa: F821
+class _SignModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignMode.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SIGN_MODE_UNSPECIFIED: _SignMode.ValueType  # 0
     """SIGN_MODE_UNSPECIFIED specifies an unknown signing mode and will be
     rejected
     """
     SIGN_MODE_DIRECT: _SignMode.ValueType  # 1
     """SIGN_MODE_DIRECT specifies a signing mode which uses SignDoc and is
@@ -86,14 +86,15 @@
 `SignModeHandler` for EIP-191. The SDK may decide to fully support
 EIP-191 in the future.
 
 Since: cosmos-sdk 0.45.2
 """
 global___SignMode = SignMode
 
+@typing_extensions.final
 class SignatureDescriptors(google.protobuf.message.Message):
     """SignatureDescriptors wraps multiple SignatureDescriptor's."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SIGNATURES_FIELD_NUMBER: builtins.int
     @property
@@ -104,28 +105,31 @@
         *,
         signatures: collections.abc.Iterable[global___SignatureDescriptor] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["signatures", b"signatures"]) -> None: ...
 
 global___SignatureDescriptors = SignatureDescriptors
 
+@typing_extensions.final
 class SignatureDescriptor(google.protobuf.message.Message):
     """SignatureDescriptor is a convenience type which represents the full data for
     a signature including the public key of the signer, signing modes and the
     signature itself. It is primarily used for coordinating signatures between
     clients.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Data(google.protobuf.message.Message):
         """Data represents signature data"""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        @typing_extensions.final
         class Single(google.protobuf.message.Message):
             """Single is the signature data for a single signer"""
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             MODE_FIELD_NUMBER: builtins.int
             SIGNATURE_FIELD_NUMBER: builtins.int
@@ -137,14 +141,15 @@
                 self,
                 *,
                 mode: global___SignMode.ValueType = ...,
                 signature: builtins.bytes = ...,
             ) -> None: ...
             def ClearField(self, field_name: typing_extensions.Literal["mode", b"mode", "signature", b"signature"]) -> None: ...
 
+        @typing_extensions.final
         class Multi(google.protobuf.message.Message):
             """Multi is the signature data for a multisig public key"""
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             BITARRAY_FIELD_NUMBER: builtins.int
             SIGNATURES_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _OrderBy:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _OrderByEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_OrderBy.ValueType], builtins.type):  # noqa: F821
+class _OrderByEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_OrderBy.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     ORDER_BY_UNSPECIFIED: _OrderBy.ValueType  # 0
     """ORDER_BY_UNSPECIFIED specifies an unknown sorting order. OrderBy defaults to ASC in this case."""
     ORDER_BY_ASC: _OrderBy.ValueType  # 1
     """ORDER_BY_ASC defines ascending order"""
     ORDER_BY_DESC: _OrderBy.ValueType  # 2
     """ORDER_BY_DESC defines descending order"""
@@ -45,15 +45,15 @@
 """ORDER_BY_DESC defines descending order"""
 global___OrderBy = OrderBy
 
 class _BroadcastMode:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _BroadcastModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BroadcastMode.ValueType], builtins.type):  # noqa: F821
+class _BroadcastModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BroadcastMode.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     BROADCAST_MODE_UNSPECIFIED: _BroadcastMode.ValueType  # 0
     """zero-value for mode ordering"""
     BROADCAST_MODE_BLOCK: _BroadcastMode.ValueType  # 1
     """BROADCAST_MODE_BLOCK defines a tx broadcasting mode where the client waits for
     the tx to be committed in a block.
     """
@@ -81,14 +81,15 @@
 """
 BROADCAST_MODE_ASYNC: BroadcastMode.ValueType  # 3
 """BROADCAST_MODE_ASYNC defines a tx broadcasting mode where the client returns
 immediately.
 """
 global___BroadcastMode = BroadcastMode
 
+@typing_extensions.final
 class GetTxsEventRequest(google.protobuf.message.Message):
     """GetTxsEventRequest is the request type for the Service.TxsByEvents
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -110,14 +111,15 @@
         order_by: global___OrderBy.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["events", b"events", "order_by", b"order_by", "pagination", b"pagination"]) -> None: ...
 
 global___GetTxsEventRequest = GetTxsEventRequest
 
+@typing_extensions.final
 class GetTxsEventResponse(google.protobuf.message.Message):
     """GetTxsEventResponse is the response type for the Service.TxsByEvents
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -141,14 +143,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "tx_responses", b"tx_responses", "txs", b"txs"]) -> None: ...
 
 global___GetTxsEventResponse = GetTxsEventResponse
 
+@typing_extensions.final
 class BroadcastTxRequest(google.protobuf.message.Message):
     """BroadcastTxRequest is the request type for the Service.BroadcastTxRequest
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -163,14 +166,15 @@
         tx_bytes: builtins.bytes = ...,
         mode: global___BroadcastMode.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["mode", b"mode", "tx_bytes", b"tx_bytes"]) -> None: ...
 
 global___BroadcastTxRequest = BroadcastTxRequest
 
+@typing_extensions.final
 class BroadcastTxResponse(google.protobuf.message.Message):
     """BroadcastTxResponse is the response type for the
     Service.BroadcastTx method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -184,14 +188,15 @@
         tx_response: cosmos.base.abci.v1beta1.abci_pb2.TxResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["tx_response", b"tx_response"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["tx_response", b"tx_response"]) -> None: ...
 
 global___BroadcastTxResponse = BroadcastTxResponse
 
+@typing_extensions.final
 class SimulateRequest(google.protobuf.message.Message):
     """SimulateRequest is the request type for the Service.Simulate
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -214,14 +219,15 @@
         tx_bytes: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["tx", b"tx"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["tx", b"tx", "tx_bytes", b"tx_bytes"]) -> None: ...
 
 global___SimulateRequest = SimulateRequest
 
+@typing_extensions.final
 class SimulateResponse(google.protobuf.message.Message):
     """SimulateResponse is the response type for the
     Service.SimulateRPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -240,14 +246,15 @@
         result: cosmos.base.abci.v1beta1.abci_pb2.Result | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["gas_info", b"gas_info", "result", b"result"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["gas_info", b"gas_info", "result", b"result"]) -> None: ...
 
 global___SimulateResponse = SimulateResponse
 
+@typing_extensions.final
 class GetTxRequest(google.protobuf.message.Message):
     """GetTxRequest is the request type for the Service.GetTx
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -259,14 +266,15 @@
         *,
         hash: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["hash", b"hash"]) -> None: ...
 
 global___GetTxRequest = GetTxRequest
 
+@typing_extensions.final
 class GetTxResponse(google.protobuf.message.Message):
     """GetTxResponse is the response type for the Service.GetTx method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TX_FIELD_NUMBER: builtins.int
     TX_RESPONSE_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/tx/v1beta1/tx_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Tx(google.protobuf.message.Message):
     """Tx is the standard type used for broadcasting transactions."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BODY_FIELD_NUMBER: builtins.int
     AUTH_INFO_FIELD_NUMBER: builtins.int
@@ -50,14 +51,15 @@
         signatures: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["auth_info", b"auth_info", "body", b"body"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["auth_info", b"auth_info", "body", b"body", "signatures", b"signatures"]) -> None: ...
 
 global___Tx = Tx
 
+@typing_extensions.final
 class TxRaw(google.protobuf.message.Message):
     """TxRaw is a variant of Tx that pins the signer's exact binary representation
     of body and auth_info. This is used for signing, broadcasting and
     verification. The binary `serialize(tx: TxRaw)` is stored in Tendermint and
     the hash `sha256(serialize(tx: TxRaw))` becomes the "txhash", commonly used
     as the transaction ID.
     """
@@ -88,14 +90,15 @@
         auth_info_bytes: builtins.bytes = ...,
         signatures: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["auth_info_bytes", b"auth_info_bytes", "body_bytes", b"body_bytes", "signatures", b"signatures"]) -> None: ...
 
 global___TxRaw = TxRaw
 
+@typing_extensions.final
 class SignDoc(google.protobuf.message.Message):
     """SignDoc is the type used for generating sign bytes for SIGN_MODE_DIRECT."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BODY_BYTES_FIELD_NUMBER: builtins.int
     AUTH_INFO_BYTES_FIELD_NUMBER: builtins.int
@@ -124,14 +127,15 @@
         chain_id: builtins.str = ...,
         account_number: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["account_number", b"account_number", "auth_info_bytes", b"auth_info_bytes", "body_bytes", b"body_bytes", "chain_id", b"chain_id"]) -> None: ...
 
 global___SignDoc = SignDoc
 
+@typing_extensions.final
 class TxBody(google.protobuf.message.Message):
     """TxBody is the body of a transaction that all signers sign over."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MESSAGES_FIELD_NUMBER: builtins.int
     MEMO_FIELD_NUMBER: builtins.int
@@ -178,14 +182,15 @@
         extension_options: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
         non_critical_extension_options: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["extension_options", b"extension_options", "memo", b"memo", "messages", b"messages", "non_critical_extension_options", b"non_critical_extension_options", "timeout_height", b"timeout_height"]) -> None: ...
 
 global___TxBody = TxBody
 
+@typing_extensions.final
 class AuthInfo(google.protobuf.message.Message):
     """AuthInfo describes the fee and signer modes that are used to sign a
     transaction.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -212,14 +217,15 @@
         fee: global___Fee | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["fee", b"fee"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["fee", b"fee", "signer_infos", b"signer_infos"]) -> None: ...
 
 global___AuthInfo = AuthInfo
 
+@typing_extensions.final
 class SignerInfo(google.protobuf.message.Message):
     """SignerInfo describes the public key and signing mode of a single top-level
     signer.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -250,19 +256,21 @@
         sequence: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["mode_info", b"mode_info", "public_key", b"public_key"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["mode_info", b"mode_info", "public_key", b"public_key", "sequence", b"sequence"]) -> None: ...
 
 global___SignerInfo = SignerInfo
 
+@typing_extensions.final
 class ModeInfo(google.protobuf.message.Message):
     """ModeInfo describes the signing mode of a single or nested multisig signer."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class Single(google.protobuf.message.Message):
         """Single is the mode info for a single signer. It is structured as a message
         to allow for additional fields such as locale for SIGN_MODE_TEXTUAL in the
         future
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -273,14 +281,15 @@
         def __init__(
             self,
             *,
             mode: cosmos.tx.signing.v1beta1.signing_pb2.SignMode.ValueType = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["mode", b"mode"]) -> None: ...
 
+    @typing_extensions.final
     class Multi(google.protobuf.message.Message):
         """Multi is the mode info for a multisig public key"""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         BITARRAY_FIELD_NUMBER: builtins.int
         MODE_INFOS_FIELD_NUMBER: builtins.int
@@ -317,14 +326,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["multi", b"multi", "single", b"single", "sum", b"sum"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["multi", b"multi", "single", b"single", "sum", b"sum"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["sum", b"sum"]) -> typing_extensions.Literal["single", "multi"] | None: ...
 
 global___ModeInfo = ModeInfo
 
+@typing_extensions.final
 class Fee(google.protobuf.message.Message):
     """Fee includes the amount of coins paid in fees and the maximum
     gas to be used by the transaction. The ratio yields an effective "gasprice",
     which must be above some miminum to be accepted into the mempool.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryCurrentPlanRequest(google.protobuf.message.Message):
     """QueryCurrentPlanRequest is the request type for the Query/CurrentPlan RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryCurrentPlanRequest = QueryCurrentPlanRequest
 
+@typing_extensions.final
 class QueryCurrentPlanResponse(google.protobuf.message.Message):
     """QueryCurrentPlanResponse is the response type for the Query/CurrentPlan RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -47,14 +49,15 @@
         plan: cosmos.upgrade.v1beta1.upgrade_pb2.Plan | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["plan", b"plan"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["plan", b"plan"]) -> None: ...
 
 global___QueryCurrentPlanResponse = QueryCurrentPlanResponse
 
+@typing_extensions.final
 class QueryAppliedPlanRequest(google.protobuf.message.Message):
     """QueryCurrentPlanRequest is the request type for the Query/AppliedPlan RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -66,14 +69,15 @@
         *,
         name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
 
 global___QueryAppliedPlanRequest = QueryAppliedPlanRequest
 
+@typing_extensions.final
 class QueryAppliedPlanResponse(google.protobuf.message.Message):
     """QueryAppliedPlanResponse is the response type for the Query/AppliedPlan RPC
     method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -85,14 +89,15 @@
         *,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height"]) -> None: ...
 
 global___QueryAppliedPlanResponse = QueryAppliedPlanResponse
 
+@typing_extensions.final
 class QueryUpgradedConsensusStateRequest(google.protobuf.message.Message):
     """QueryUpgradedConsensusStateRequest is the request type for the Query/UpgradedConsensusState
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -106,14 +111,15 @@
         *,
         last_height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["last_height", b"last_height"]) -> None: ...
 
 global___QueryUpgradedConsensusStateRequest = QueryUpgradedConsensusStateRequest
 
+@typing_extensions.final
 class QueryUpgradedConsensusStateResponse(google.protobuf.message.Message):
     """QueryUpgradedConsensusStateResponse is the response type for the Query/UpgradedConsensusState
     RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -125,14 +131,15 @@
         *,
         upgraded_consensus_state: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["upgraded_consensus_state", b"upgraded_consensus_state"]) -> None: ...
 
 global___QueryUpgradedConsensusStateResponse = QueryUpgradedConsensusStateResponse
 
+@typing_extensions.final
 class QueryModuleVersionsRequest(google.protobuf.message.Message):
     """QueryModuleVersionsRequest is the request type for the Query/ModuleVersions
     RPC method.
 
     Since: cosmos-sdk 0.43
     """
 
@@ -149,14 +156,15 @@
         *,
         module_name: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["module_name", b"module_name"]) -> None: ...
 
 global___QueryModuleVersionsRequest = QueryModuleVersionsRequest
 
+@typing_extensions.final
 class QueryModuleVersionsResponse(google.protobuf.message.Message):
     """QueryModuleVersionsResponse is the response type for the Query/ModuleVersions
     RPC method.
 
     Since: cosmos-sdk 0.43
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/upgrade/v1beta1/upgrade_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Plan(google.protobuf.message.Message):
     """Plan specifies information about a planned upgrade and when it should occur."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TIME_FIELD_NUMBER: builtins.int
@@ -65,14 +66,15 @@
         upgraded_client_state: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["time", b"time", "upgraded_client_state", b"upgraded_client_state"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "info", b"info", "name", b"name", "time", b"time", "upgraded_client_state", b"upgraded_client_state"]) -> None: ...
 
 global___Plan = Plan
 
+@typing_extensions.final
 class SoftwareUpgradeProposal(google.protobuf.message.Message):
     """SoftwareUpgradeProposal is a gov Content type for initiating a software
     upgrade.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -91,14 +93,15 @@
         plan: global___Plan | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["plan", b"plan"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "plan", b"plan", "title", b"title"]) -> None: ...
 
 global___SoftwareUpgradeProposal = SoftwareUpgradeProposal
 
+@typing_extensions.final
 class CancelSoftwareUpgradeProposal(google.protobuf.message.Message):
     """CancelSoftwareUpgradeProposal is a gov Content type for cancelling a software
     upgrade.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -112,14 +115,15 @@
         title: builtins.str = ...,
         description: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "title", b"title"]) -> None: ...
 
 global___CancelSoftwareUpgradeProposal = CancelSoftwareUpgradeProposal
 
+@typing_extensions.final
 class ModuleVersion(google.protobuf.message.Message):
     """ModuleVersion specifies a module and its consensus version.
 
     Since: cosmos-sdk 0.43
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateVestingAccount(google.protobuf.message.Message):
     """MsgCreateVestingAccount defines a message that enables creating a vesting
     account.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -45,25 +46,27 @@
         end_time: builtins.int = ...,
         delayed: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "delayed", b"delayed", "end_time", b"end_time", "from_address", b"from_address", "to_address", b"to_address"]) -> None: ...
 
 global___MsgCreateVestingAccount = MsgCreateVestingAccount
 
+@typing_extensions.final
 class MsgCreateVestingAccountResponse(google.protobuf.message.Message):
     """MsgCreateVestingAccountResponse defines the Msg/CreateVestingAccount response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgCreateVestingAccountResponse = MsgCreateVestingAccountResponse
 
+@typing_extensions.final
 class MsgCreateClawbackVestingAccount(google.protobuf.message.Message):
     """MsgCreateClawbackVestingAccount defines a message that enables creating a ClawbackVestingAccount."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FROM_ADDRESS_FIELD_NUMBER: builtins.int
     TO_ADDRESS_FIELD_NUMBER: builtins.int
@@ -102,27 +105,29 @@
         vesting_periods: collections.abc.Iterable[cosmos.vesting.v1beta1.vesting_pb2.Period] | None = ...,
         merge: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["from_address", b"from_address", "lockup_periods", b"lockup_periods", "merge", b"merge", "start_time", b"start_time", "to_address", b"to_address", "vesting_periods", b"vesting_periods"]) -> None: ...
 
 global___MsgCreateClawbackVestingAccount = MsgCreateClawbackVestingAccount
 
+@typing_extensions.final
 class MsgCreateClawbackVestingAccountResponse(google.protobuf.message.Message):
     """MsgCreateClawbackVestingAccountResponse defines the
     MsgCreateClawbackVestingAccount response type.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgCreateClawbackVestingAccountResponse = MsgCreateClawbackVestingAccountResponse
 
+@typing_extensions.final
 class MsgClawback(google.protobuf.message.Message):
     """MsgClawback defines a message that removes unvested tokens from a
     ClawbackVestingAccount.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -145,14 +150,15 @@
         address: builtins.str = ...,
         dest_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "dest_address", b"dest_address", "funder_address", b"funder_address"]) -> None: ...
 
 global___MsgClawback = MsgClawback
 
+@typing_extensions.final
 class MsgClawbackResponse(google.protobuf.message.Message):
     """MsgClawbackResponse defines the MsgClawback response type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos/vesting/v1beta1/vesting_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class BaseVestingAccount(google.protobuf.message.Message):
     """BaseVestingAccount implements the VestingAccount interface. It contains all
     the necessary fields needed for any vesting account implementation.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -49,14 +50,15 @@
         end_time: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_account", b"base_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_account", b"base_account", "delegated_free", b"delegated_free", "delegated_vesting", b"delegated_vesting", "end_time", b"end_time", "original_vesting", b"original_vesting"]) -> None: ...
 
 global___BaseVestingAccount = BaseVestingAccount
 
+@typing_extensions.final
 class ContinuousVestingAccount(google.protobuf.message.Message):
     """ContinuousVestingAccount implements the VestingAccount interface. It
     continuously vests by unlocking coins linearly with respect to time.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -72,14 +74,15 @@
         start_time: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account", "start_time", b"start_time"]) -> None: ...
 
 global___ContinuousVestingAccount = ContinuousVestingAccount
 
+@typing_extensions.final
 class DelayedVestingAccount(google.protobuf.message.Message):
     """DelayedVestingAccount implements the VestingAccount interface. It vests all
     coins after a specific time, but non prior. In other words, it keeps them
     locked until a specified time.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -93,14 +96,15 @@
         base_vesting_account: global___BaseVestingAccount | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> None: ...
 
 global___DelayedVestingAccount = DelayedVestingAccount
 
+@typing_extensions.final
 class Period(google.protobuf.message.Message):
     """Period defines a length of time and amount of coins that will vest."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LENGTH_FIELD_NUMBER: builtins.int
     AMOUNT_FIELD_NUMBER: builtins.int
@@ -113,14 +117,15 @@
         length: builtins.int = ...,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "length", b"length"]) -> None: ...
 
 global___Period = Period
 
+@typing_extensions.final
 class PeriodicVestingAccount(google.protobuf.message.Message):
     """PeriodicVestingAccount implements the VestingAccount interface. It
     periodically vests by unlocking coins during each specified period.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -140,14 +145,15 @@
         vesting_periods: collections.abc.Iterable[global___Period] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account", "start_time", b"start_time", "vesting_periods", b"vesting_periods"]) -> None: ...
 
 global___PeriodicVestingAccount = PeriodicVestingAccount
 
+@typing_extensions.final
 class PermanentLockedAccount(google.protobuf.message.Message):
     """PermanentLockedAccount implements the VestingAccount interface. It does
     not ever release coins, locking them indefinitely. Coins in this account can
     still be used for delegating and for governance votes even while locked.
 
     Since: cosmos-sdk 0.43
     """
@@ -163,14 +169,15 @@
         base_vesting_account: global___BaseVestingAccount | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_vesting_account", b"base_vesting_account"]) -> None: ...
 
 global___PermanentLockedAccount = PermanentLockedAccount
 
+@typing_extensions.final
 class ClawbackVestingAccount(google.protobuf.message.Message):
     """ClawbackVestingAccount implements the VestingAccount interface. It provides
     an account that can hold contributions subject to "lockup" (like a
     PeriodicVestingAccount), or vesting which is subject to clawback
     of unvested tokens, or a combination (tokens vest, but are still locked).
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/cosmos_proto/cosmos_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/cosmos_proto/cosmos_pb2.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/gogoproto/gogo_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Http(google.protobuf.message.Message):
     """Defines the HTTP configuration for an API service. It contains a list of
     [HttpRule][google.api.HttpRule], each specifying the mapping of an RPC method
     to one or more HTTP REST API methods.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -59,14 +60,15 @@
         rules: collections.abc.Iterable[global___HttpRule] | None = ...,
         fully_decode_reserved_expansion: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fully_decode_reserved_expansion", b"fully_decode_reserved_expansion", "rules", b"rules"]) -> None: ...
 
 global___Http = Http
 
+@typing_extensions.final
 class HttpRule(google.protobuf.message.Message):
     """`HttpRule` defines the mapping of an RPC method to one or more HTTP
     REST API methods. The mapping specifies how different portions of the RPC
     request message are mapped to URL path, URL query parameters, and
     HTTP request body. The mapping is typically specified as an
     `google.api.http` annotation on the RPC method,
     see "google/api/annotations.proto" for details.
@@ -350,14 +352,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["custom", b"custom", "delete", b"delete", "get", b"get", "patch", b"patch", "pattern", b"pattern", "post", b"post", "put", b"put"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["additional_bindings", b"additional_bindings", "body", b"body", "custom", b"custom", "delete", b"delete", "get", b"get", "patch", b"patch", "pattern", b"pattern", "post", b"post", "put", b"put", "response_body", b"response_body", "selector", b"selector"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["pattern", b"pattern"]) -> typing_extensions.Literal["get", "put", "post", "delete", "patch", "custom"] | None: ...
 
 global___HttpRule = HttpRule
 
+@typing_extensions.final
 class CustomHttpPattern(google.protobuf.message.Message):
     """A custom pattern is used for defining custom HTTP verb."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KIND_FIELD_NUMBER: builtins.int
     PATH_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/http_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class HttpBody(google.protobuf.message.Message):
     """Message that represents an arbitrary HTTP body. It should only be used for
     payload formats that can't be represented as JSON, such as raw binary or
     an HTML page.
 
 
     This message can be used both in streaming and non-streaming API methods in
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/api/httpbody_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Any(google.protobuf.message.Message, google.protobuf.internal.well_known_types.Any):
     """`Any` contains an arbitrary serialized protocol buffer message along with a
     URL that describes the type of the serialized message.
 
     Protobuf library provides support to pack/unpack Any values in the form
     of utility functions or additional generated methods of the Any type.
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/google_apis/protobuf/any_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/downtime_duration_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _Downtime:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _DowntimeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Downtime.ValueType], builtins.type):  # noqa: F821
+class _DowntimeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Downtime.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     DURATION_30S: _Downtime.ValueType  # 0
     DURATION_1M: _Downtime.ValueType  # 1
     DURATION_2M: _Downtime.ValueType  # 2
     DURATION_3M: _Downtime.ValueType  # 3
     DURATION_4M: _Downtime.ValueType  # 4
     DURATION_5M: _Downtime.ValueType  # 5
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/genesis_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisDowntimeEntry(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DURATION_FIELD_NUMBER: builtins.int
     LAST_DOWNTIME_FIELD_NUMBER: builtins.int
     duration: osmosis.downtime_detector.v1beta1.downtime_duration_pb2.Downtime.ValueType
     @property
@@ -33,14 +34,15 @@
         last_downtime: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["last_downtime", b"last_downtime"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "last_downtime", b"last_downtime"]) -> None: ...
 
 global___GenesisDowntimeEntry = GenesisDowntimeEntry
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the twap module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOWNTIMES_FIELD_NUMBER: builtins.int
     LAST_BLOCK_TIME_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class RecoveredSinceDowntimeOfLengthRequest(google.protobuf.message.Message):
     """Query for has it been at least $RECOVERY_DURATION units of time,
     since the chain has been down for $DOWNTIME_DURATION.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -35,14 +36,15 @@
         recovery: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["recovery", b"recovery"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["downtime", b"downtime", "recovery", b"recovery"]) -> None: ...
 
 global___RecoveredSinceDowntimeOfLengthRequest = RecoveredSinceDowntimeOfLengthRequest
 
+@typing_extensions.final
 class RecoveredSinceDowntimeOfLengthResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUCCESFULLY_RECOVERED_FIELD_NUMBER: builtins.int
     succesfully_recovered: builtins.bool
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/downtime_detector/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/genesis_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class EpochInfo(google.protobuf.message.Message):
     """EpochInfo is a struct that describes the data going into
     a timer defined by the x/epochs module.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -93,14 +94,15 @@
         current_epoch_start_height: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["current_epoch_start_time", b"current_epoch_start_time", "duration", b"duration", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["current_epoch", b"current_epoch", "current_epoch_start_height", b"current_epoch_start_height", "current_epoch_start_time", b"current_epoch_start_time", "duration", b"duration", "epoch_counting_started", b"epoch_counting_started", "identifier", b"identifier", "start_time", b"start_time"]) -> None: ...
 
 global___EpochInfo = EpochInfo
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the epochs module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EPOCHS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryEpochsInfoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryEpochsInfoRequest = QueryEpochsInfoRequest
 
+@typing_extensions.final
 class QueryEpochsInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EPOCHS_FIELD_NUMBER: builtins.int
     @property
     def epochs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.epochs.genesis_pb2.EpochInfo]: ...
     def __init__(
@@ -37,28 +39,30 @@
         *,
         epochs: collections.abc.Iterable[osmosis.epochs.genesis_pb2.EpochInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["epochs", b"epochs"]) -> None: ...
 
 global___QueryEpochsInfoResponse = QueryEpochsInfoResponse
 
+@typing_extensions.final
 class QueryCurrentEpochRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IDENTIFIER_FIELD_NUMBER: builtins.int
     identifier: builtins.str
     def __init__(
         self,
         *,
         identifier: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["identifier", b"identifier"]) -> None: ...
 
 global___QueryCurrentEpochRequest = QueryCurrentEpochRequest
 
+@typing_extensions.final
 class QueryCurrentEpochResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CURRENT_EPOCH_FIELD_NUMBER: builtins.int
     current_epoch: builtins.int
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/epochs/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/balancerPool_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class SmoothWeightChangeParams(google.protobuf.message.Message):
     """Parameters for changing the weights in a balancer pool smoothly from
     a start weight and end weight over a period of time.
     Currently, the only smooth change supported is linear changing between
     the two weights, but more types may be added in the future.
     When these parameters are set, the weight w(t) for pool time `t` is the
     following:
@@ -83,14 +84,15 @@
         target_pool_weights: collections.abc.Iterable[global___PoolAsset] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "initial_pool_weights", b"initial_pool_weights", "start_time", b"start_time", "target_pool_weights", b"target_pool_weights"]) -> None: ...
 
 global___SmoothWeightChangeParams = SmoothWeightChangeParams
 
+@typing_extensions.final
 class PoolParams(google.protobuf.message.Message):
     """PoolParams defined the parameters that will be managed by the pool
     governance in the future. This params are not managed by the chain
     governance. Instead they will be managed by the token holders of the pool.
     The pool's token holders are specified in future_pool_governor.
     """
 
@@ -111,14 +113,15 @@
         smooth_weight_change_params: global___SmoothWeightChangeParams | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["smooth_weight_change_params", b"smooth_weight_change_params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["exit_fee", b"exit_fee", "smooth_weight_change_params", b"smooth_weight_change_params", "swap_fee", b"swap_fee"]) -> None: ...
 
 global___PoolParams = PoolParams
 
+@typing_extensions.final
 class PoolAsset(google.protobuf.message.Message):
     """Pool asset is an internal struct that combines the amount of the
     token in the pool, and its balancer weight.
     This is an awkward packaging of data,
     and should be revisited in a future state migration.
     """
 
@@ -140,14 +143,15 @@
         weight: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["token", b"token"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["token", b"token", "weight", b"weight"]) -> None: ...
 
 global___PoolAsset = PoolAsset
 
+@typing_extensions.final
 class Pool(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     POOL_PARAMS_FIELD_NUMBER: builtins.int
     FUTURE_POOL_GOVERNOR_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateBalancerPool(google.protobuf.message.Message):
     """===================== MsgCreatePool"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_PARAMS_FIELD_NUMBER: builtins.int
@@ -41,14 +42,15 @@
         future_pool_governor: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pool_params", b"pool_params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["future_pool_governor", b"future_pool_governor", "pool_assets", b"pool_assets", "pool_params", b"pool_params", "sender", b"sender"]) -> None: ...
 
 global___MsgCreateBalancerPool = MsgCreateBalancerPool
 
+@typing_extensions.final
 class MsgCreateBalancerPoolResponse(google.protobuf.message.Message):
     """Returns the poolID"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/balancer/tx/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/stableswap_pool_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PoolParams(google.protobuf.message.Message):
     """PoolParams defined the parameters that will be managed by the pool
     governance in the future. This params are not managed by the chain
     governance. Instead they will be managed by the token holders of the pool.
     The pool's token holders are specified in future_pool_governor.
     """
 
@@ -36,14 +37,15 @@
         swap_fee: builtins.str = ...,
         exit_fee: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["exit_fee", b"exit_fee", "swap_fee", b"swap_fee"]) -> None: ...
 
 global___PoolParams = PoolParams
 
+@typing_extensions.final
 class Pool(google.protobuf.message.Message):
     """Pool is the stableswap Pool struct"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateStableswapPool(google.protobuf.message.Message):
     """===================== MsgCreatePool"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_PARAMS_FIELD_NUMBER: builtins.int
@@ -49,14 +50,15 @@
         scaling_factor_controller: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pool_params", b"pool_params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["future_pool_governor", b"future_pool_governor", "initial_pool_liquidity", b"initial_pool_liquidity", "pool_params", b"pool_params", "scaling_factor_controller", b"scaling_factor_controller", "scaling_factors", b"scaling_factors", "sender", b"sender"]) -> None: ...
 
 global___MsgCreateStableswapPool = MsgCreateStableswapPool
 
+@typing_extensions.final
 class MsgCreateStableswapPoolResponse(google.protobuf.message.Message):
     """Returns a poolID with custom poolName."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -65,14 +67,15 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___MsgCreateStableswapPoolResponse = MsgCreateStableswapPoolResponse
 
+@typing_extensions.final
 class MsgStableSwapAdjustScalingFactors(google.protobuf.message.Message):
     """Sender must be the pool's scaling_factor_governor in order for the tx to
     succeed. Adjusts stableswap scaling factors.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -90,14 +93,15 @@
         pool_id: builtins.int = ...,
         scaling_factors: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "scaling_factors", b"scaling_factors", "sender", b"sender"]) -> None: ...
 
 global___MsgStableSwapAdjustScalingFactors = MsgStableSwapAdjustScalingFactors
 
+@typing_extensions.final
 class MsgStableSwapAdjustScalingFactorsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/pool_models/stableswap/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/genesis_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the incentives module"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_CREATION_FEE_FIELD_NUMBER: builtins.int
     @property
@@ -31,14 +32,15 @@
         *,
         pool_creation_fee: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_creation_fee", b"pool_creation_fee"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the gamm module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOLS_FIELD_NUMBER: builtins.int
     NEXT_POOL_NUMBER_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryPoolRequest(google.protobuf.message.Message):
     """=============================== Pool"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -32,14 +33,15 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryPoolRequest = QueryPoolRequest
 
+@typing_extensions.final
 class QueryPoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_FIELD_NUMBER: builtins.int
     @property
     def pool(self) -> google.protobuf.any_pb2.Any: ...
     def __init__(
@@ -48,14 +50,15 @@
         pool: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pool", b"pool"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool", b"pool"]) -> None: ...
 
 global___QueryPoolResponse = QueryPoolResponse
 
+@typing_extensions.final
 class QueryPoolsRequest(google.protobuf.message.Message):
     """=============================== Pools"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
@@ -67,14 +70,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___QueryPoolsRequest = QueryPoolsRequest
 
+@typing_extensions.final
 class QueryPoolsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOLS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pools(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]: ...
@@ -88,39 +92,42 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "pools", b"pools"]) -> None: ...
 
 global___QueryPoolsResponse = QueryPoolsResponse
 
+@typing_extensions.final
 class QueryNumPoolsRequest(google.protobuf.message.Message):
     """=============================== NumPools"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryNumPoolsRequest = QueryNumPoolsRequest
 
+@typing_extensions.final
 class QueryNumPoolsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NUM_POOLS_FIELD_NUMBER: builtins.int
     num_pools: builtins.int
     def __init__(
         self,
         *,
         num_pools: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["num_pools", b"num_pools"]) -> None: ...
 
 global___QueryNumPoolsResponse = QueryNumPoolsResponse
 
+@typing_extensions.final
 class QueryPoolTypeRequest(google.protobuf.message.Message):
     """=============================== PoolType"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -129,28 +136,30 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryPoolTypeRequest = QueryPoolTypeRequest
 
+@typing_extensions.final
 class QueryPoolTypeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_TYPE_FIELD_NUMBER: builtins.int
     pool_type: builtins.str
     def __init__(
         self,
         *,
         pool_type: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_type", b"pool_type"]) -> None: ...
 
 global___QueryPoolTypeResponse = QueryPoolTypeResponse
 
+@typing_extensions.final
 class QueryCalcJoinPoolSharesRequest(google.protobuf.message.Message):
     """=============================== CalcJoinPoolShares"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     TOKENS_IN_FIELD_NUMBER: builtins.int
@@ -163,14 +172,15 @@
         pool_id: builtins.int = ...,
         tokens_in: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "tokens_in", b"tokens_in"]) -> None: ...
 
 global___QueryCalcJoinPoolSharesRequest = QueryCalcJoinPoolSharesRequest
 
+@typing_extensions.final
 class QueryCalcJoinPoolSharesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHARE_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     TOKENS_OUT_FIELD_NUMBER: builtins.int
     share_out_amount: builtins.str
     @property
@@ -181,14 +191,15 @@
         share_out_amount: builtins.str = ...,
         tokens_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["share_out_amount", b"share_out_amount", "tokens_out", b"tokens_out"]) -> None: ...
 
 global___QueryCalcJoinPoolSharesResponse = QueryCalcJoinPoolSharesResponse
 
+@typing_extensions.final
 class QueryCalcExitPoolCoinsFromSharesRequest(google.protobuf.message.Message):
     """=============================== CalcExitPoolCoinsFromShares"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     SHARE_IN_AMOUNT_FIELD_NUMBER: builtins.int
@@ -200,14 +211,15 @@
         pool_id: builtins.int = ...,
         share_in_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "share_in_amount", b"share_in_amount"]) -> None: ...
 
 global___QueryCalcExitPoolCoinsFromSharesRequest = QueryCalcExitPoolCoinsFromSharesRequest
 
+@typing_extensions.final
 class QueryCalcExitPoolCoinsFromSharesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKENS_OUT_FIELD_NUMBER: builtins.int
     @property
     def tokens_out(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -215,14 +227,15 @@
         *,
         tokens_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["tokens_out", b"tokens_out"]) -> None: ...
 
 global___QueryCalcExitPoolCoinsFromSharesResponse = QueryCalcExitPoolCoinsFromSharesResponse
 
+@typing_extensions.final
 class QueryPoolParamsRequest(google.protobuf.message.Message):
     """=============================== PoolParams"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -231,14 +244,15 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryPoolParamsRequest = QueryPoolParamsRequest
 
+@typing_extensions.final
 class QueryPoolParamsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
     def params(self) -> google.protobuf.any_pb2.Any: ...
     def __init__(
@@ -247,14 +261,15 @@
         params: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryPoolParamsResponse = QueryPoolParamsResponse
 
+@typing_extensions.final
 class QueryTotalPoolLiquidityRequest(google.protobuf.message.Message):
     """=============================== PoolLiquidity"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -263,14 +278,15 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryTotalPoolLiquidityRequest = QueryTotalPoolLiquidityRequest
 
+@typing_extensions.final
 class QueryTotalPoolLiquidityResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIQUIDITY_FIELD_NUMBER: builtins.int
     @property
     def liquidity(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -278,14 +294,15 @@
         *,
         liquidity: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["liquidity", b"liquidity"]) -> None: ...
 
 global___QueryTotalPoolLiquidityResponse = QueryTotalPoolLiquidityResponse
 
+@typing_extensions.final
 class QueryTotalSharesRequest(google.protobuf.message.Message):
     """=============================== TotalShares"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -294,14 +311,15 @@
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryTotalSharesRequest = QueryTotalSharesRequest
 
+@typing_extensions.final
 class QueryTotalSharesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_SHARES_FIELD_NUMBER: builtins.int
     @property
     def total_shares(self) -> cosmos.base.v1beta1.coin_pb2.Coin: ...
     def __init__(
@@ -310,14 +328,15 @@
         total_shares: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["total_shares", b"total_shares"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["total_shares", b"total_shares"]) -> None: ...
 
 global___QueryTotalSharesResponse = QueryTotalSharesResponse
 
+@typing_extensions.final
 class QueryCalcJoinPoolNoSwapSharesRequest(google.protobuf.message.Message):
     """=============================== CalcJoinPoolNoSwapShares"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     TOKENS_IN_FIELD_NUMBER: builtins.int
@@ -330,14 +349,15 @@
         pool_id: builtins.int = ...,
         tokens_in: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "tokens_in", b"tokens_in"]) -> None: ...
 
 global___QueryCalcJoinPoolNoSwapSharesRequest = QueryCalcJoinPoolNoSwapSharesRequest
 
+@typing_extensions.final
 class QueryCalcJoinPoolNoSwapSharesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKENS_OUT_FIELD_NUMBER: builtins.int
     SHARES_OUT_FIELD_NUMBER: builtins.int
     @property
     def tokens_out(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
@@ -348,14 +368,15 @@
         tokens_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
         shares_out: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["shares_out", b"shares_out", "tokens_out", b"tokens_out"]) -> None: ...
 
 global___QueryCalcJoinPoolNoSwapSharesResponse = QueryCalcJoinPoolNoSwapSharesResponse
 
+@typing_extensions.final
 class QuerySpotPriceRequest(google.protobuf.message.Message):
     """QuerySpotPriceRequest defines the gRPC request structure for a SpotPrice
     query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -372,14 +393,15 @@
         base_asset_denom: builtins.str = ...,
         quote_asset_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset_denom", b"base_asset_denom", "pool_id", b"pool_id", "quote_asset_denom", b"quote_asset_denom"]) -> None: ...
 
 global___QuerySpotPriceRequest = QuerySpotPriceRequest
 
+@typing_extensions.final
 class QueryPoolsWithFilterRequest(google.protobuf.message.Message):
     """=============================== PoolsWithFilter"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MIN_LIQUIDITY_FIELD_NUMBER: builtins.int
     POOL_TYPE_FIELD_NUMBER: builtins.int
@@ -399,14 +421,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["min_liquidity", b"min_liquidity", "pagination", b"pagination", "pool_type", b"pool_type"]) -> None: ...
 
 global___QueryPoolsWithFilterRequest = QueryPoolsWithFilterRequest
 
+@typing_extensions.final
 class QueryPoolsWithFilterResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOLS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pools(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]: ...
@@ -420,14 +443,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "pools", b"pools"]) -> None: ...
 
 global___QueryPoolsWithFilterResponse = QueryPoolsWithFilterResponse
 
+@typing_extensions.final
 class QuerySpotPriceResponse(google.protobuf.message.Message):
     """QuerySpotPriceResponse defines the gRPC response structure for a SpotPrice
     query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -439,14 +463,15 @@
         *,
         spot_price: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["spot_price", b"spot_price"]) -> None: ...
 
 global___QuerySpotPriceResponse = QuerySpotPriceResponse
 
+@typing_extensions.final
 class QuerySwapExactAmountInRequest(google.protobuf.message.Message):
     """=============================== EstimateSwapExactAmountIn"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -466,28 +491,30 @@
         token_in: builtins.str = ...,
         routes: collections.abc.Iterable[osmosis.gamm.v1beta1.tx_pb2.SwapAmountInRoute] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "routes", b"routes", "sender", b"sender", "token_in", b"token_in"]) -> None: ...
 
 global___QuerySwapExactAmountInRequest = QuerySwapExactAmountInRequest
 
+@typing_extensions.final
 class QuerySwapExactAmountInResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     token_out_amount: builtins.str
     def __init__(
         self,
         *,
         token_out_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_out_amount", b"token_out_amount"]) -> None: ...
 
 global___QuerySwapExactAmountInResponse = QuerySwapExactAmountInResponse
 
+@typing_extensions.final
 class QuerySwapExactAmountOutRequest(google.protobuf.message.Message):
     """=============================== EstimateSwapExactAmountOut"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -507,37 +534,40 @@
         routes: collections.abc.Iterable[osmosis.gamm.v1beta1.tx_pb2.SwapAmountOutRoute] | None = ...,
         token_out: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "routes", b"routes", "sender", b"sender", "token_out", b"token_out"]) -> None: ...
 
 global___QuerySwapExactAmountOutRequest = QuerySwapExactAmountOutRequest
 
+@typing_extensions.final
 class QuerySwapExactAmountOutResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_IN_AMOUNT_FIELD_NUMBER: builtins.int
     token_in_amount: builtins.str
     def __init__(
         self,
         *,
         token_in_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_in_amount", b"token_in_amount"]) -> None: ...
 
 global___QuerySwapExactAmountOutResponse = QuerySwapExactAmountOutResponse
 
+@typing_extensions.final
 class QueryTotalLiquidityRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryTotalLiquidityRequest = QueryTotalLiquidityRequest
 
+@typing_extensions.final
 class QueryTotalLiquidityResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LIQUIDITY_FIELD_NUMBER: builtins.int
     @property
     def liquidity(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgJoinPool(google.protobuf.message.Message):
     """===================== MsgJoinPool
     This is really MsgJoinPoolNoSwap
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -41,14 +42,15 @@
         share_out_amount: builtins.str = ...,
         token_in_maxs: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_out_amount", b"share_out_amount", "token_in_maxs", b"token_in_maxs"]) -> None: ...
 
 global___MsgJoinPool = MsgJoinPool
 
+@typing_extensions.final
 class MsgJoinPoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHARE_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     TOKEN_IN_FIELD_NUMBER: builtins.int
     share_out_amount: builtins.str
     @property
@@ -59,14 +61,15 @@
         share_out_amount: builtins.str = ...,
         token_in: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["share_out_amount", b"share_out_amount", "token_in", b"token_in"]) -> None: ...
 
 global___MsgJoinPoolResponse = MsgJoinPoolResponse
 
+@typing_extensions.final
 class MsgExitPool(google.protobuf.message.Message):
     """===================== MsgExitPool"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -85,14 +88,15 @@
         share_in_amount: builtins.str = ...,
         token_out_mins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_in_amount", b"share_in_amount", "token_out_mins", b"token_out_mins"]) -> None: ...
 
 global___MsgExitPool = MsgExitPool
 
+@typing_extensions.final
 class MsgExitPoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_OUT_FIELD_NUMBER: builtins.int
     @property
     def token_out(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -100,14 +104,15 @@
         *,
         token_out: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> None: ...
 
 global___MsgExitPoolResponse = MsgExitPoolResponse
 
+@typing_extensions.final
 class SwapAmountInRoute(google.protobuf.message.Message):
     """===================== MsgSwapExactAmountIn"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     TOKEN_OUT_DENOM_FIELD_NUMBER: builtins.int
@@ -119,14 +124,15 @@
         pool_id: builtins.int = ...,
         token_out_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "token_out_denom", b"token_out_denom"]) -> None: ...
 
 global___SwapAmountInRoute = SwapAmountInRoute
 
+@typing_extensions.final
 class MsgSwapExactAmountIn(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     ROUTES_FIELD_NUMBER: builtins.int
     TOKEN_IN_FIELD_NUMBER: builtins.int
     TOKEN_OUT_MIN_AMOUNT_FIELD_NUMBER: builtins.int
@@ -145,28 +151,30 @@
         token_out_min_amount: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["token_in", b"token_in"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["routes", b"routes", "sender", b"sender", "token_in", b"token_in", "token_out_min_amount", b"token_out_min_amount"]) -> None: ...
 
 global___MsgSwapExactAmountIn = MsgSwapExactAmountIn
 
+@typing_extensions.final
 class MsgSwapExactAmountInResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     token_out_amount: builtins.str
     def __init__(
         self,
         *,
         token_out_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_out_amount", b"token_out_amount"]) -> None: ...
 
 global___MsgSwapExactAmountInResponse = MsgSwapExactAmountInResponse
 
+@typing_extensions.final
 class SwapAmountOutRoute(google.protobuf.message.Message):
     """===================== MsgSwapExactAmountOut"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     TOKEN_IN_DENOM_FIELD_NUMBER: builtins.int
@@ -178,14 +186,15 @@
         pool_id: builtins.int = ...,
         token_in_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "token_in_denom", b"token_in_denom"]) -> None: ...
 
 global___SwapAmountOutRoute = SwapAmountOutRoute
 
+@typing_extensions.final
 class MsgSwapExactAmountOut(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     ROUTES_FIELD_NUMBER: builtins.int
     TOKEN_IN_MAX_AMOUNT_FIELD_NUMBER: builtins.int
     TOKEN_OUT_FIELD_NUMBER: builtins.int
@@ -204,28 +213,30 @@
         token_out: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["routes", b"routes", "sender", b"sender", "token_in_max_amount", b"token_in_max_amount", "token_out", b"token_out"]) -> None: ...
 
 global___MsgSwapExactAmountOut = MsgSwapExactAmountOut
 
+@typing_extensions.final
 class MsgSwapExactAmountOutResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_IN_AMOUNT_FIELD_NUMBER: builtins.int
     token_in_amount: builtins.str
     def __init__(
         self,
         *,
         token_in_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_in_amount", b"token_in_amount"]) -> None: ...
 
 global___MsgSwapExactAmountOutResponse = MsgSwapExactAmountOutResponse
 
+@typing_extensions.final
 class MsgJoinSwapExternAmountIn(google.protobuf.message.Message):
     """===================== MsgJoinSwapExternAmountIn
     TODO: Rename to MsgJoinSwapExactAmountIn
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -252,28 +263,30 @@
         share_out_min_amount: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["token_in", b"token_in"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_out_min_amount", b"share_out_min_amount", "token_in", b"token_in"]) -> None: ...
 
 global___MsgJoinSwapExternAmountIn = MsgJoinSwapExternAmountIn
 
+@typing_extensions.final
 class MsgJoinSwapExternAmountInResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHARE_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     share_out_amount: builtins.str
     def __init__(
         self,
         *,
         share_out_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["share_out_amount", b"share_out_amount"]) -> None: ...
 
 global___MsgJoinSwapExternAmountInResponse = MsgJoinSwapExternAmountInResponse
 
+@typing_extensions.final
 class MsgJoinSwapShareAmountOut(google.protobuf.message.Message):
     """===================== MsgJoinSwapShareAmountOut"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -294,28 +307,30 @@
         share_out_amount: builtins.str = ...,
         token_in_max_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_out_amount", b"share_out_amount", "token_in_denom", b"token_in_denom", "token_in_max_amount", b"token_in_max_amount"]) -> None: ...
 
 global___MsgJoinSwapShareAmountOut = MsgJoinSwapShareAmountOut
 
+@typing_extensions.final
 class MsgJoinSwapShareAmountOutResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_IN_AMOUNT_FIELD_NUMBER: builtins.int
     token_in_amount: builtins.str
     def __init__(
         self,
         *,
         token_in_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_in_amount", b"token_in_amount"]) -> None: ...
 
 global___MsgJoinSwapShareAmountOutResponse = MsgJoinSwapShareAmountOutResponse
 
+@typing_extensions.final
 class MsgExitSwapShareAmountIn(google.protobuf.message.Message):
     """===================== MsgExitSwapShareAmountIn"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -336,28 +351,30 @@
         share_in_amount: builtins.str = ...,
         token_out_min_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_in_amount", b"share_in_amount", "token_out_denom", b"token_out_denom", "token_out_min_amount", b"token_out_min_amount"]) -> None: ...
 
 global___MsgExitSwapShareAmountIn = MsgExitSwapShareAmountIn
 
+@typing_extensions.final
 class MsgExitSwapShareAmountInResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOKEN_OUT_AMOUNT_FIELD_NUMBER: builtins.int
     token_out_amount: builtins.str
     def __init__(
         self,
         *,
         token_out_amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["token_out_amount", b"token_out_amount"]) -> None: ...
 
 global___MsgExitSwapShareAmountInResponse = MsgExitSwapShareAmountInResponse
 
+@typing_extensions.final
 class MsgExitSwapExternAmountOut(google.protobuf.message.Message):
     """===================== MsgExitSwapExternAmountOut"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     POOL_ID_FIELD_NUMBER: builtins.int
@@ -377,14 +394,15 @@
         share_in_max_amount: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["token_out", b"token_out"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender", "share_in_max_amount", b"share_in_max_amount", "token_out", b"token_out"]) -> None: ...
 
 global___MsgExitSwapExternAmountOut = MsgExitSwapExternAmountOut
 
+@typing_extensions.final
 class MsgExitSwapExternAmountOutResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHARE_IN_AMOUNT_FIELD_NUMBER: builtins.int
     share_in_amount: builtins.str
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,53 +11,53 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.JoinPool = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/JoinPool',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/JoinPool',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.FromString,
+        )
         self.ExitPool = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/ExitPool',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/ExitPool',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.FromString,
+        )
         self.SwapExactAmountIn = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/SwapExactAmountIn',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/SwapExactAmountIn',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.FromString,
+        )
         self.SwapExactAmountOut = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/SwapExactAmountOut',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/SwapExactAmountOut',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.FromString,
+        )
         self.JoinSwapExternAmountIn = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/JoinSwapExternAmountIn',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/JoinSwapExternAmountIn',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.FromString,
+        )
         self.JoinSwapShareAmountOut = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/JoinSwapShareAmountOut',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/JoinSwapShareAmountOut',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.FromString,
+        )
         self.ExitSwapExternAmountOut = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/ExitSwapExternAmountOut',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/ExitSwapExternAmountOut',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.FromString,
+        )
         self.ExitSwapShareAmountIn = channel.unary_unary(
-                '/osmosis.gamm.v1beta1.Msg/ExitSwapShareAmountIn',
-                request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.SerializeToString,
-                response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.FromString,
-                )
+            '/osmosis.gamm.v1beta1.Msg/ExitSwapShareAmountIn',
+            request_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.SerializeToString,
+            response_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.FromString,
+        )
 
 
 class MsgServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def JoinPool(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -106,192 +106,193 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_MsgServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'JoinPool': grpc.unary_unary_rpc_method_handler(
-                    servicer.JoinPool,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.SerializeToString,
-            ),
-            'ExitPool': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExitPool,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.SerializeToString,
-            ),
-            'SwapExactAmountIn': grpc.unary_unary_rpc_method_handler(
-                    servicer.SwapExactAmountIn,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.SerializeToString,
-            ),
-            'SwapExactAmountOut': grpc.unary_unary_rpc_method_handler(
-                    servicer.SwapExactAmountOut,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.SerializeToString,
-            ),
-            'JoinSwapExternAmountIn': grpc.unary_unary_rpc_method_handler(
-                    servicer.JoinSwapExternAmountIn,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.SerializeToString,
-            ),
-            'JoinSwapShareAmountOut': grpc.unary_unary_rpc_method_handler(
-                    servicer.JoinSwapShareAmountOut,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.SerializeToString,
-            ),
-            'ExitSwapExternAmountOut': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExitSwapExternAmountOut,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.SerializeToString,
-            ),
-            'ExitSwapShareAmountIn': grpc.unary_unary_rpc_method_handler(
-                    servicer.ExitSwapShareAmountIn,
-                    request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.FromString,
-                    response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.SerializeToString,
-            ),
+        'JoinPool': grpc.unary_unary_rpc_method_handler(
+            servicer.JoinPool,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.SerializeToString,
+        ),
+        'ExitPool': grpc.unary_unary_rpc_method_handler(
+            servicer.ExitPool,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.SerializeToString,
+        ),
+        'SwapExactAmountIn': grpc.unary_unary_rpc_method_handler(
+            servicer.SwapExactAmountIn,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.SerializeToString,
+        ),
+        'SwapExactAmountOut': grpc.unary_unary_rpc_method_handler(
+            servicer.SwapExactAmountOut,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.SerializeToString,
+        ),
+        'JoinSwapExternAmountIn': grpc.unary_unary_rpc_method_handler(
+            servicer.JoinSwapExternAmountIn,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.SerializeToString,
+        ),
+        'JoinSwapShareAmountOut': grpc.unary_unary_rpc_method_handler(
+            servicer.JoinSwapShareAmountOut,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.SerializeToString,
+        ),
+        'ExitSwapExternAmountOut': grpc.unary_unary_rpc_method_handler(
+            servicer.ExitSwapExternAmountOut,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.SerializeToString,
+        ),
+        'ExitSwapShareAmountIn': grpc.unary_unary_rpc_method_handler(
+            servicer.ExitSwapShareAmountIn,
+            request_deserializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.FromString,
+            response_serializer=osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'osmosis.gamm.v1beta1.Msg', rpc_method_handlers)
+        'osmosis.gamm.v1beta1.Msg', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
-
  # This class is part of an EXPERIMENTAL API.
+
+
 class Msg(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def JoinPool(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                 target,
+                 options=(),
+                 channel_credentials=None,
+                 call_credentials=None,
+                 insecure=False,
+                 compression=None,
+                 wait_for_ready=None,
+                 timeout=None,
+                 metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/JoinPool',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPool.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinPoolResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExitPool(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                 target,
+                 options=(),
+                 channel_credentials=None,
+                 call_credentials=None,
+                 insecure=False,
+                 compression=None,
+                 wait_for_ready=None,
+                 timeout=None,
+                 metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/ExitPool',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPool.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitPoolResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SwapExactAmountIn(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                          target,
+                          options=(),
+                          channel_credentials=None,
+                          call_credentials=None,
+                          insecure=False,
+                          compression=None,
+                          wait_for_ready=None,
+                          timeout=None,
+                          metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/SwapExactAmountIn',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountIn.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountInResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SwapExactAmountOut(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                           target,
+                           options=(),
+                           channel_credentials=None,
+                           call_credentials=None,
+                           insecure=False,
+                           compression=None,
+                           wait_for_ready=None,
+                           timeout=None,
+                           metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/SwapExactAmountOut',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOut.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgSwapExactAmountOutResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def JoinSwapExternAmountIn(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                               target,
+                               options=(),
+                               channel_credentials=None,
+                               call_credentials=None,
+                               insecure=False,
+                               compression=None,
+                               wait_for_ready=None,
+                               timeout=None,
+                               metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/JoinSwapExternAmountIn',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountIn.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapExternAmountInResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def JoinSwapShareAmountOut(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                               target,
+                               options=(),
+                               channel_credentials=None,
+                               call_credentials=None,
+                               insecure=False,
+                               compression=None,
+                               wait_for_ready=None,
+                               timeout=None,
+                               metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/JoinSwapShareAmountOut',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOut.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgJoinSwapShareAmountOutResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExitSwapExternAmountOut(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                                target,
+                                options=(),
+                                channel_credentials=None,
+                                call_credentials=None,
+                                insecure=False,
+                                compression=None,
+                                wait_for_ready=None,
+                                timeout=None,
+                                metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/ExitSwapExternAmountOut',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOut.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapExternAmountOutResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ExitSwapShareAmountIn(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
+                              target,
+                              options=(),
+                              channel_credentials=None,
+                              call_credentials=None,
+                              insecure=False,
+                              compression=None,
+                              wait_for_ready=None,
+                              timeout=None,
+                              metadata=None):
         return grpc.experimental.unary_unary(request, target, '/osmosis.gamm.v1beta1.Msg/ExitSwapShareAmountIn',
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.SerializeToString,
-            osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountIn.SerializeToString,
+                                             osmosis_dot_gamm_dot_v1beta1_dot_tx__pb2.MsgExitSwapShareAmountInResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QuerySpotPriceRequest(google.protobuf.message.Message):
     """QuerySpotPriceRequest defines the gRPC request structure for a SpotPrice
     query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -34,14 +35,15 @@
         base_asset_denom: builtins.str = ...,
         quote_asset_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset_denom", b"base_asset_denom", "pool_id", b"pool_id", "quote_asset_denom", b"quote_asset_denom"]) -> None: ...
 
 global___QuerySpotPriceRequest = QuerySpotPriceRequest
 
+@typing_extensions.final
 class QuerySpotPriceResponse(google.protobuf.message.Message):
     """QuerySpotPriceResponse defines the gRPC response structure for a SpotPrice
     query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/gamm/v2/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/genesis_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the ibc-rate-limit module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/params_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the parameters for the ibc-rate-limit module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTRACT_ADDRESS_FIELD_NUMBER: builtins.int
     contract_address: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ParamsRequest(google.protobuf.message.Message):
     """ParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ParamsRequest = ParamsRequest
 
+@typing_extensions.final
 class ParamsResponse(google.protobuf.message.Message):
     """aramsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/ibc_rate_limit/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/gauge_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/gauge_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Gauge(google.protobuf.message.Message):
     """Gauge is an object that stores and distributes yields to recipients who
     satisfy certain conditions. Currently gauges support conditions around the
     duration for which a given denom is locked.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -82,14 +83,15 @@
         distributed_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["distribute_to", b"distribute_to", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "distribute_to", b"distribute_to", "distributed_coins", b"distributed_coins", "filled_epochs", b"filled_epochs", "id", b"id", "is_perpetual", b"is_perpetual", "num_epochs_paid_over", b"num_epochs_paid_over", "start_time", b"start_time"]) -> None: ...
 
 global___Gauge = Gauge
 
+@typing_extensions.final
 class LockableDurationsInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKABLE_DURATIONS_FIELD_NUMBER: builtins.int
     @property
     def lockable_durations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.duration_pb2.Duration]:
         """List of incentivised durations that gauges will pay out to"""
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/genesis_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the incentives module's various parameters when first
     initialized
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/params_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the incentives module"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISTR_EPOCH_IDENTIFIER_FIELD_NUMBER: builtins.int
     distr_epoch_identifier: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ModuleToDistributeCoinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ModuleToDistributeCoinsRequest = ModuleToDistributeCoinsRequest
 
+@typing_extensions.final
 class ModuleToDistributeCoinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
         """Coins that have yet to be distributed"""
@@ -41,14 +43,15 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___ModuleToDistributeCoinsResponse = ModuleToDistributeCoinsResponse
 
+@typing_extensions.final
 class GaugeByIDRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     id: builtins.int
     """Gague ID being queried"""
     def __init__(
@@ -56,14 +59,15 @@
         *,
         id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
 
 global___GaugeByIDRequest = GaugeByIDRequest
 
+@typing_extensions.final
 class GaugeByIDResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GAUGE_FIELD_NUMBER: builtins.int
     @property
     def gauge(self) -> osmosis.incentives.gauge_pb2.Gauge:
         """Gauge that corresponds to provided gague ID"""
@@ -73,14 +77,15 @@
         gauge: osmosis.incentives.gauge_pb2.Gauge | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["gauge", b"gauge"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["gauge", b"gauge"]) -> None: ...
 
 global___GaugeByIDResponse = GaugeByIDResponse
 
+@typing_extensions.final
 class GaugesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pagination(self) -> cosmos.base.query.v1beta1.pagination_pb2.PageRequest:
         """Pagination defines pagination for the request"""
@@ -90,14 +95,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___GaugesRequest = GaugesRequest
 
+@typing_extensions.final
 class GaugesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]:
@@ -112,14 +118,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "pagination", b"pagination"]) -> None: ...
 
 global___GaugesResponse = GaugesResponse
 
+@typing_extensions.final
 class ActiveGaugesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pagination(self) -> cosmos.base.query.v1beta1.pagination_pb2.PageRequest:
         """Pagination defines pagination for the request"""
@@ -129,14 +136,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___ActiveGaugesRequest = ActiveGaugesRequest
 
+@typing_extensions.final
 class ActiveGaugesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]:
@@ -151,14 +159,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "pagination", b"pagination"]) -> None: ...
 
 global___ActiveGaugesResponse = ActiveGaugesResponse
 
+@typing_extensions.final
 class ActiveGaugesPerDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     denom: builtins.str
     """Desired denom when querying active gagues"""
@@ -172,14 +181,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "pagination", b"pagination"]) -> None: ...
 
 global___ActiveGaugesPerDenomRequest = ActiveGaugesPerDenomRequest
 
+@typing_extensions.final
 class ActiveGaugesPerDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]:
@@ -194,14 +204,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "pagination", b"pagination"]) -> None: ...
 
 global___ActiveGaugesPerDenomResponse = ActiveGaugesPerDenomResponse
 
+@typing_extensions.final
 class UpcomingGaugesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pagination(self) -> cosmos.base.query.v1beta1.pagination_pb2.PageRequest:
         """Pagination defines pagination for the request"""
@@ -211,14 +222,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___UpcomingGaugesRequest = UpcomingGaugesRequest
 
+@typing_extensions.final
 class UpcomingGaugesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]:
@@ -233,14 +245,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "pagination", b"pagination"]) -> None: ...
 
 global___UpcomingGaugesResponse = UpcomingGaugesResponse
 
+@typing_extensions.final
 class UpcomingGaugesPerDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     denom: builtins.str
     """Filter for upcoming gagues that match specific denom"""
@@ -254,14 +267,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "pagination", b"pagination"]) -> None: ...
 
 global___UpcomingGaugesPerDenomRequest = UpcomingGaugesPerDenomRequest
 
+@typing_extensions.final
 class UpcomingGaugesPerDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     UPCOMING_GAUGES_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def upcoming_gauges(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]:
@@ -276,14 +290,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination", "upcoming_gauges", b"upcoming_gauges"]) -> None: ...
 
 global___UpcomingGaugesPerDenomResponse = UpcomingGaugesPerDenomResponse
 
+@typing_extensions.final
 class RewardsEstRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     LOCK_IDS_FIELD_NUMBER: builtins.int
     END_EPOCH_FIELD_NUMBER: builtins.int
     owner: builtins.str
@@ -302,14 +317,15 @@
         lock_ids: collections.abc.Iterable[builtins.int] | None = ...,
         end_epoch: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["end_epoch", b"end_epoch", "lock_ids", b"lock_ids", "owner", b"owner"]) -> None: ...
 
 global___RewardsEstRequest = RewardsEstRequest
 
+@typing_extensions.final
 class RewardsEstResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]:
         """Estimated coin rewards that will be recieved at provided address
@@ -320,23 +336,25 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___RewardsEstResponse = RewardsEstResponse
 
+@typing_extensions.final
 class QueryLockableDurationsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryLockableDurationsRequest = QueryLockableDurationsRequest
 
+@typing_extensions.final
 class QueryLockableDurationsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKABLE_DURATIONS_FIELD_NUMBER: builtins.int
     @property
     def lockable_durations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.duration_pb2.Duration]:
         """Time durations that users can lock coins for in order to recieve rewards"""
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateGauge(google.protobuf.message.Message):
     """MsgCreateGauge creates a gague to distribute rewards to users"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_PERPETUAL_FIELD_NUMBER: builtins.int
     OWNER_FIELD_NUMBER: builtins.int
@@ -65,23 +66,25 @@
         num_epochs_paid_over: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["distribute_to", b"distribute_to", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "distribute_to", b"distribute_to", "is_perpetual", b"is_perpetual", "num_epochs_paid_over", b"num_epochs_paid_over", "owner", b"owner", "start_time", b"start_time"]) -> None: ...
 
 global___MsgCreateGauge = MsgCreateGauge
 
+@typing_extensions.final
 class MsgCreateGaugeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgCreateGaugeResponse = MsgCreateGaugeResponse
 
+@typing_extensions.final
 class MsgAddToGauge(google.protobuf.message.Message):
     """MsgAddToGauge adds coins to a previously created gauge"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     GAUGE_ID_FIELD_NUMBER: builtins.int
@@ -100,14 +103,15 @@
         gauge_id: builtins.int = ...,
         rewards: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["gauge_id", b"gauge_id", "owner", b"owner", "rewards", b"rewards"]) -> None: ...
 
 global___MsgAddToGauge = MsgAddToGauge
 
+@typing_extensions.final
 class MsgAddToGaugeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/incentives/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/genesis_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the lockup module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LAST_LOCK_ID_FIELD_NUMBER: builtins.int
     LOCKS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/lock_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/lock_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _LockQueryType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _LockQueryTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_LockQueryType.ValueType], builtins.type):  # noqa: F821
+class _LockQueryTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_LockQueryType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     ByDuration: _LockQueryType.ValueType  # 0
     ByTime: _LockQueryType.ValueType  # 1
 
 class LockQueryType(_LockQueryType, metaclass=_LockQueryTypeEnumTypeWrapper):
     """LockQueryType defines the type of the lock query that can
     either be by duration or start time of the lock.
     """
 
 ByDuration: LockQueryType.ValueType  # 0
 ByTime: LockQueryType.ValueType  # 1
 global___LockQueryType = LockQueryType
 
+@typing_extensions.final
 class PeriodLock(google.protobuf.message.Message):
     """PeriodLock is a single lock unit by period defined by the x/lockup module.
     It's a record of a locked coin at a specific time. It stores owner, duration,
     unlock time and the number of coins locked. A state of a period lock is
     created upon lock creation, and deleted once the lock has been matured after
     the `duration` has passed since unbonding started.
     """
@@ -87,14 +88,15 @@
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration", "end_time", b"end_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID", "coins", b"coins", "duration", b"duration", "end_time", b"end_time", "owner", b"owner"]) -> None: ...
 
 global___PeriodLock = PeriodLock
 
+@typing_extensions.final
 class QueryCondition(google.protobuf.message.Message):
     """QueryCondition is a struct used for querying locks upon different conditions.
     Duration field and timestamp fields could be optional, depending on the
     LockQueryType.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -128,14 +130,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration", "timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "duration", b"duration", "lock_query_type", b"lock_query_type", "timestamp", b"timestamp"]) -> None: ...
 
 global___QueryCondition = QueryCondition
 
+@typing_extensions.final
 class SyntheticLock(google.protobuf.message.Message):
     """SyntheticLock is creating virtual lockup where new denom is combination of
     original denom and synthetic suffix. At the time of synthetic lockup creation
     and deletion, accumulation store is also being updated and on querier side,
     they can query as freely as native lockup.
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/params_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FORCE_UNLOCK_ALLOWED_ADDRESSES_FIELD_NUMBER: builtins.int
     @property
     def force_unlock_allowed_addresses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ModuleBalanceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ModuleBalanceRequest = ModuleBalanceRequest
 
+@typing_extensions.final
 class ModuleBalanceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -41,23 +43,25 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___ModuleBalanceResponse = ModuleBalanceResponse
 
+@typing_extensions.final
 class ModuleLockedAmountRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ModuleLockedAmountRequest = ModuleLockedAmountRequest
 
+@typing_extensions.final
 class ModuleLockedAmountResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -65,28 +69,30 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___ModuleLockedAmountResponse = ModuleLockedAmountResponse
 
+@typing_extensions.final
 class AccountUnlockableCoinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     owner: builtins.str
     def __init__(
         self,
         *,
         owner: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner"]) -> None: ...
 
 global___AccountUnlockableCoinsRequest = AccountUnlockableCoinsRequest
 
+@typing_extensions.final
 class AccountUnlockableCoinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -94,28 +100,30 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___AccountUnlockableCoinsResponse = AccountUnlockableCoinsResponse
 
+@typing_extensions.final
 class AccountUnlockingCoinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     owner: builtins.str
     def __init__(
         self,
         *,
         owner: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner"]) -> None: ...
 
 global___AccountUnlockingCoinsRequest = AccountUnlockingCoinsRequest
 
+@typing_extensions.final
 class AccountUnlockingCoinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -123,28 +131,30 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___AccountUnlockingCoinsResponse = AccountUnlockingCoinsResponse
 
+@typing_extensions.final
 class AccountLockedCoinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     owner: builtins.str
     def __init__(
         self,
         *,
         owner: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner"]) -> None: ...
 
 global___AccountLockedCoinsRequest = AccountLockedCoinsRequest
 
+@typing_extensions.final
 class AccountLockedCoinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COINS_FIELD_NUMBER: builtins.int
     @property
     def coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -152,14 +162,15 @@
         *,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins"]) -> None: ...
 
 global___AccountLockedCoinsResponse = AccountLockedCoinsResponse
 
+@typing_extensions.final
 class AccountLockedPastTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -171,14 +182,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner", "timestamp", b"timestamp"]) -> None: ...
 
 global___AccountLockedPastTimeRequest = AccountLockedPastTimeRequest
 
+@typing_extensions.final
 class AccountLockedPastTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -186,14 +198,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedPastTimeResponse = AccountLockedPastTimeResponse
 
+@typing_extensions.final
 class AccountLockedPastTimeNotUnlockingOnlyRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -205,14 +218,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner", "timestamp", b"timestamp"]) -> None: ...
 
 global___AccountLockedPastTimeNotUnlockingOnlyRequest = AccountLockedPastTimeNotUnlockingOnlyRequest
 
+@typing_extensions.final
 class AccountLockedPastTimeNotUnlockingOnlyResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -220,14 +234,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedPastTimeNotUnlockingOnlyResponse = AccountLockedPastTimeNotUnlockingOnlyResponse
 
+@typing_extensions.final
 class AccountUnlockedBeforeTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -239,14 +254,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner", "timestamp", b"timestamp"]) -> None: ...
 
 global___AccountUnlockedBeforeTimeRequest = AccountUnlockedBeforeTimeRequest
 
+@typing_extensions.final
 class AccountUnlockedBeforeTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -254,14 +270,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountUnlockedBeforeTimeResponse = AccountUnlockedBeforeTimeResponse
 
+@typing_extensions.final
 class AccountLockedPastTimeDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     owner: builtins.str
@@ -276,14 +293,15 @@
         denom: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "owner", b"owner", "timestamp", b"timestamp"]) -> None: ...
 
 global___AccountLockedPastTimeDenomRequest = AccountLockedPastTimeDenomRequest
 
+@typing_extensions.final
 class AccountLockedPastTimeDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -291,14 +309,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedPastTimeDenomResponse = AccountLockedPastTimeDenomResponse
 
+@typing_extensions.final
 class LockedDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     denom: builtins.str
     @property
@@ -310,42 +329,45 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "duration", b"duration"]) -> None: ...
 
 global___LockedDenomRequest = LockedDenomRequest
 
+@typing_extensions.final
 class LockedDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AMOUNT_FIELD_NUMBER: builtins.int
     amount: builtins.str
     def __init__(
         self,
         *,
         amount: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> None: ...
 
 global___LockedDenomResponse = LockedDenomResponse
 
+@typing_extensions.final
 class LockedRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCK_ID_FIELD_NUMBER: builtins.int
     lock_id: builtins.int
     def __init__(
         self,
         *,
         lock_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id"]) -> None: ...
 
 global___LockedRequest = LockedRequest
 
+@typing_extensions.final
 class LockedResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCK_FIELD_NUMBER: builtins.int
     @property
     def lock(self) -> osmosis.lockup.lock_pb2.PeriodLock: ...
     def __init__(
@@ -354,28 +376,30 @@
         lock: osmosis.lockup.lock_pb2.PeriodLock | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["lock", b"lock"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock", b"lock"]) -> None: ...
 
 global___LockedResponse = LockedResponse
 
+@typing_extensions.final
 class SyntheticLockupsByLockupIDRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCK_ID_FIELD_NUMBER: builtins.int
     lock_id: builtins.int
     def __init__(
         self,
         *,
         lock_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id"]) -> None: ...
 
 global___SyntheticLockupsByLockupIDRequest = SyntheticLockupsByLockupIDRequest
 
+@typing_extensions.final
 class SyntheticLockupsByLockupIDResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SYNTHETIC_LOCKS_FIELD_NUMBER: builtins.int
     @property
     def synthetic_locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.SyntheticLock]: ...
     def __init__(
@@ -383,14 +407,15 @@
         *,
         synthetic_locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.SyntheticLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["synthetic_locks", b"synthetic_locks"]) -> None: ...
 
 global___SyntheticLockupsByLockupIDResponse = SyntheticLockupsByLockupIDResponse
 
+@typing_extensions.final
 class AccountLockedLongerDurationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -402,14 +427,15 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___AccountLockedLongerDurationRequest = AccountLockedLongerDurationRequest
 
+@typing_extensions.final
 class AccountLockedLongerDurationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -417,14 +443,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedLongerDurationResponse = AccountLockedLongerDurationResponse
 
+@typing_extensions.final
 class AccountLockedDurationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -436,14 +463,15 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___AccountLockedDurationRequest = AccountLockedDurationRequest
 
+@typing_extensions.final
 class AccountLockedDurationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -451,14 +479,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedDurationResponse = AccountLockedDurationResponse
 
+@typing_extensions.final
 class AccountLockedLongerDurationNotUnlockingOnlyRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     owner: builtins.str
     @property
@@ -470,14 +499,15 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___AccountLockedLongerDurationNotUnlockingOnlyRequest = AccountLockedLongerDurationNotUnlockingOnlyRequest
 
+@typing_extensions.final
 class AccountLockedLongerDurationNotUnlockingOnlyResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -485,14 +515,15 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedLongerDurationNotUnlockingOnlyResponse = AccountLockedLongerDurationNotUnlockingOnlyResponse
 
+@typing_extensions.final
 class AccountLockedLongerDurationDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     owner: builtins.str
@@ -507,14 +538,15 @@
         denom: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___AccountLockedLongerDurationDenomRequest = AccountLockedLongerDurationDenomRequest
 
+@typing_extensions.final
 class AccountLockedLongerDurationDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKS_FIELD_NUMBER: builtins.int
     @property
     def locks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -522,23 +554,25 @@
         *,
         locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["locks", b"locks"]) -> None: ...
 
 global___AccountLockedLongerDurationDenomResponse = AccountLockedLongerDurationDenomResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
     def params(self) -> osmosis.lockup.params_pb2.Params: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgLockTokens(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     COINS_FIELD_NUMBER: builtins.int
     owner: builtins.str
@@ -38,42 +39,45 @@
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___MsgLockTokens = MsgLockTokens
 
+@typing_extensions.final
 class MsgLockTokensResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     ID: builtins.int
     def __init__(
         self,
         *,
         ID: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID"]) -> None: ...
 
 global___MsgLockTokensResponse = MsgLockTokensResponse
 
+@typing_extensions.final
 class MsgBeginUnlockingAll(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     owner: builtins.str
     def __init__(
         self,
         *,
         owner: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["owner", b"owner"]) -> None: ...
 
 global___MsgBeginUnlockingAll = MsgBeginUnlockingAll
 
+@typing_extensions.final
 class MsgBeginUnlockingAllResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     UNLOCKS_FIELD_NUMBER: builtins.int
     @property
     def unlocks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.lockup.lock_pb2.PeriodLock]: ...
     def __init__(
@@ -81,14 +85,15 @@
         *,
         unlocks: collections.abc.Iterable[osmosis.lockup.lock_pb2.PeriodLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["unlocks", b"unlocks"]) -> None: ...
 
 global___MsgBeginUnlockingAllResponse = MsgBeginUnlockingAllResponse
 
+@typing_extensions.final
 class MsgBeginUnlocking(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OWNER_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     COINS_FIELD_NUMBER: builtins.int
     owner: builtins.str
@@ -103,28 +108,30 @@
         ID: builtins.int = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID", "coins", b"coins", "owner", b"owner"]) -> None: ...
 
 global___MsgBeginUnlocking = MsgBeginUnlocking
 
+@typing_extensions.final
 class MsgBeginUnlockingResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUCCESS_FIELD_NUMBER: builtins.int
     success: builtins.bool
     def __init__(
         self,
         *,
         success: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["success", b"success"]) -> None: ...
 
 global___MsgBeginUnlockingResponse = MsgBeginUnlockingResponse
 
+@typing_extensions.final
 class MsgExtendLockup(google.protobuf.message.Message):
     """MsgExtendLockup extends the existing lockup's duration.
     The new duration is longer than the original.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -146,28 +153,30 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID", "duration", b"duration", "owner", b"owner"]) -> None: ...
 
 global___MsgExtendLockup = MsgExtendLockup
 
+@typing_extensions.final
 class MsgExtendLockupResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUCCESS_FIELD_NUMBER: builtins.int
     success: builtins.bool
     def __init__(
         self,
         *,
         success: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["success", b"success"]) -> None: ...
 
 global___MsgExtendLockupResponse = MsgExtendLockupResponse
 
+@typing_extensions.final
 class MsgForceUnlock(google.protobuf.message.Message):
     """MsgForceUnlock unlocks locks immediately for
     addresses registered via governance.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -186,14 +195,15 @@
         ID: builtins.int = ...,
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID", "coins", b"coins", "owner", b"owner"]) -> None: ...
 
 global___MsgForceUnlock = MsgForceUnlock
 
+@typing_extensions.final
 class MsgForceUnlockResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUCCESS_FIELD_NUMBER: builtins.int
     success: builtins.bool
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/lockup/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/genesis_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the mint module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINTER_FIELD_NUMBER: builtins.int
     PARAMS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/mint_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Minter(google.protobuf.message.Message):
     """Minter represents the minting state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EPOCH_PROVISIONS_FIELD_NUMBER: builtins.int
     epoch_provisions: builtins.str
@@ -29,14 +30,15 @@
         *,
         epoch_provisions: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["epoch_provisions", b"epoch_provisions"]) -> None: ...
 
 global___Minter = Minter
 
+@typing_extensions.final
 class WeightedAddress(google.protobuf.message.Message):
     """WeightedAddress represents an address with a weight assigned to it.
     The weight is used to determine the proportion of the total minted
     tokens to be minted to the address.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -51,14 +53,15 @@
         address: builtins.str = ...,
         weight: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "weight", b"weight"]) -> None: ...
 
 global___WeightedAddress = WeightedAddress
 
+@typing_extensions.final
 class DistributionProportions(google.protobuf.message.Message):
     """DistributionProportions defines the distribution proportions of the minted
     denom. In other words, defines which stakeholders will receive the minted
     denoms and how much.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -91,14 +94,15 @@
         developer_rewards: builtins.str = ...,
         community_pool: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["community_pool", b"community_pool", "developer_rewards", b"developer_rewards", "pool_incentives", b"pool_incentives", "staking", b"staking"]) -> None: ...
 
 global___DistributionProportions = DistributionProportions
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the x/mint module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINT_DENOM_FIELD_NUMBER: builtins.int
     GENESIS_EPOCH_PROVISIONS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -41,27 +43,29 @@
         params: osmosis.mint.v1beta1.mint_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryEpochProvisionsRequest(google.protobuf.message.Message):
     """QueryEpochProvisionsRequest is the request type for the
     Query/EpochProvisions RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryEpochProvisionsRequest = QueryEpochProvisionsRequest
 
+@typing_extensions.final
 class QueryEpochProvisionsResponse(google.protobuf.message.Message):
     """QueryEpochProvisionsResponse is the response type for the
     Query/EpochProvisions RPC method.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/mint/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/genesis_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the pool incentives module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     LOCKABLE_DURATIONS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/gov_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ReplacePoolIncentivesProposal(google.protobuf.message.Message):
     """ReplacePoolIncentivesProposal is a gov Content type for updating the pool
     incentives. If a ReplacePoolIncentivesProposal passes, the proposal’s records
     override the existing DistrRecords set in the module. Each record has a
     specified gauge id and weight, and the incentives are distributed to each
     gauge according to weight/total_weight. The incentives are put in the fee
     pool and it is allocated to gauges and community pool by the DistrRecords
@@ -43,14 +44,15 @@
         description: builtins.str = ...,
         records: collections.abc.Iterable[osmosis.pool_incentives.v1beta1.incentives_pb2.DistrRecord] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "records", b"records", "title", b"title"]) -> None: ...
 
 global___ReplacePoolIncentivesProposal = ReplacePoolIncentivesProposal
 
+@typing_extensions.final
 class UpdatePoolIncentivesProposal(google.protobuf.message.Message):
     """UpdatePoolIncentivesProposal is a gov Content type for updating the pool
     incentives. If a UpdatePoolIncentivesProposal passes, all the DistrRecords
     in the proposals are edited. An existing DistrRecord is not overriden unless
     explicitly included in the proposal.
     This differs from an ReplacePoolIncentivesProposal because it only does an
     in place update of the DistrRecords for gauges explicitly mentioned in the
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/incentives_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINTED_DENOM_FIELD_NUMBER: builtins.int
     minted_denom: builtins.str
     """minted_denom is the denomination of the coin expected to be minted by the
     minting module. Pool-incentives module doesn’t actually mint the coin
@@ -32,14 +33,15 @@
         *,
         minted_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["minted_denom", b"minted_denom"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class LockableDurationsInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKABLE_DURATIONS_FIELD_NUMBER: builtins.int
     @property
     def lockable_durations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.duration_pb2.Duration]: ...
     def __init__(
@@ -47,14 +49,15 @@
         *,
         lockable_durations: collections.abc.Iterable[google.protobuf.duration_pb2.Duration] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lockable_durations", b"lockable_durations"]) -> None: ...
 
 global___LockableDurationsInfo = LockableDurationsInfo
 
+@typing_extensions.final
 class DistrInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_WEIGHT_FIELD_NUMBER: builtins.int
     RECORDS_FIELD_NUMBER: builtins.int
     total_weight: builtins.str
     @property
@@ -65,14 +68,15 @@
         total_weight: builtins.str = ...,
         records: collections.abc.Iterable[global___DistrRecord] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["records", b"records", "total_weight", b"total_weight"]) -> None: ...
 
 global___DistrInfo = DistrInfo
 
+@typing_extensions.final
 class DistrRecord(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GAUGE_ID_FIELD_NUMBER: builtins.int
     WEIGHT_FIELD_NUMBER: builtins.int
     gauge_id: builtins.int
     weight: builtins.str
@@ -82,14 +86,15 @@
         gauge_id: builtins.int = ...,
         weight: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["gauge_id", b"gauge_id", "weight", b"weight"]) -> None: ...
 
 global___DistrRecord = DistrRecord
 
+@typing_extensions.final
 class PoolToGauge(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     GAUGE_ID_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -104,14 +109,15 @@
         duration: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "gauge_id", b"gauge_id", "pool_id", b"pool_id"]) -> None: ...
 
 global___PoolToGauge = PoolToGauge
 
+@typing_extensions.final
 class PoolToGauges(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_TO_GAUGE_FIELD_NUMBER: builtins.int
     @property
     def pool_to_gauge(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PoolToGauge]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -15,31 +15,34 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryGaugeIdsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
     def __init__(
         self,
         *,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id"]) -> None: ...
 
 global___QueryGaugeIdsRequest = QueryGaugeIdsRequest
 
+@typing_extensions.final
 class QueryGaugeIdsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
     class GaugeIdWithDuration(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         GAUGE_ID_FIELD_NUMBER: builtins.int
         DURATION_FIELD_NUMBER: builtins.int
         GAUGE_INCENTIVE_PERCENTAGE_FIELD_NUMBER: builtins.int
         gauge_id: builtins.int
@@ -64,23 +67,25 @@
         *,
         gauge_ids_with_duration: collections.abc.Iterable[global___QueryGaugeIdsResponse.GaugeIdWithDuration] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["gauge_ids_with_duration", b"gauge_ids_with_duration"]) -> None: ...
 
 global___QueryGaugeIdsResponse = QueryGaugeIdsResponse
 
+@typing_extensions.final
 class QueryDistrInfoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryDistrInfoRequest = QueryDistrInfoRequest
 
+@typing_extensions.final
 class QueryDistrInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISTR_INFO_FIELD_NUMBER: builtins.int
     @property
     def distr_info(self) -> osmosis.pool_incentives.v1beta1.incentives_pb2.DistrInfo: ...
     def __init__(
@@ -89,23 +94,25 @@
         distr_info: osmosis.pool_incentives.v1beta1.incentives_pb2.DistrInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["distr_info", b"distr_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["distr_info", b"distr_info"]) -> None: ...
 
 global___QueryDistrInfoResponse = QueryDistrInfoResponse
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
     def params(self) -> osmosis.pool_incentives.v1beta1.incentives_pb2.Params: ...
     def __init__(
@@ -114,23 +121,25 @@
         params: osmosis.pool_incentives.v1beta1.incentives_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryLockableDurationsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryLockableDurationsRequest = QueryLockableDurationsRequest
 
+@typing_extensions.final
 class QueryLockableDurationsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCKABLE_DURATIONS_FIELD_NUMBER: builtins.int
     @property
     def lockable_durations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.duration_pb2.Duration]: ...
     def __init__(
@@ -138,23 +147,25 @@
         *,
         lockable_durations: collections.abc.Iterable[google.protobuf.duration_pb2.Duration] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lockable_durations", b"lockable_durations"]) -> None: ...
 
 global___QueryLockableDurationsResponse = QueryLockableDurationsResponse
 
+@typing_extensions.final
 class QueryIncentivizedPoolsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryIncentivizedPoolsRequest = QueryIncentivizedPoolsRequest
 
+@typing_extensions.final
 class IncentivizedPool(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     LOCKABLE_DURATION_FIELD_NUMBER: builtins.int
     GAUGE_ID_FIELD_NUMBER: builtins.int
     pool_id: builtins.int
@@ -169,14 +180,15 @@
         gauge_id: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["lockable_duration", b"lockable_duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["gauge_id", b"gauge_id", "lockable_duration", b"lockable_duration", "pool_id", b"pool_id"]) -> None: ...
 
 global___IncentivizedPool = IncentivizedPool
 
+@typing_extensions.final
 class QueryIncentivizedPoolsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INCENTIVIZED_POOLS_FIELD_NUMBER: builtins.int
     @property
     def incentivized_pools(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IncentivizedPool]: ...
     def __init__(
@@ -184,23 +196,25 @@
         *,
         incentivized_pools: collections.abc.Iterable[global___IncentivizedPool] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["incentivized_pools", b"incentivized_pools"]) -> None: ...
 
 global___QueryIncentivizedPoolsResponse = QueryIncentivizedPoolsResponse
 
+@typing_extensions.final
 class QueryExternalIncentiveGaugesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryExternalIncentiveGaugesRequest = QueryExternalIncentiveGaugesRequest
 
+@typing_extensions.final
 class QueryExternalIncentiveGaugesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     @property
     def data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.incentives.gauge_pb2.Gauge]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/pool_incentives/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/sumtree/v1beta1/tree_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Node(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHILDREN_FIELD_NUMBER: builtins.int
     @property
     def children(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Child]: ...
     def __init__(
@@ -27,14 +28,15 @@
         *,
         children: collections.abc.Iterable[global___Child] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["children", b"children"]) -> None: ...
 
 global___Node = Node
 
+@typing_extensions.final
 class Child(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     ACCUMULATION_FIELD_NUMBER: builtins.int
     index: builtins.bytes
     accumulation: builtins.str
@@ -44,14 +46,15 @@
         index: builtins.bytes = ...,
         accumulation: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["accumulation", b"accumulation", "index", b"index"]) -> None: ...
 
 global___Child = Child
 
+@typing_extensions.final
 class Leaf(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LEAF_FIELD_NUMBER: builtins.int
     @property
     def leaf(self) -> global___Child: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/genesis_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     SUPERFLUID_ASSETS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/params_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the superfluid module"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MINIMUM_RISK_FACTOR_FIELD_NUMBER: builtins.int
     minimum_risk_factor: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
     def params(self) -> osmosis.superfluid.params_pb2.Params:
         """params defines the parameters of the module."""
@@ -44,51 +46,55 @@
         params: osmosis.superfluid.params_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class AssetTypeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
     def __init__(
         self,
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___AssetTypeRequest = AssetTypeRequest
 
+@typing_extensions.final
 class AssetTypeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ASSET_TYPE_FIELD_NUMBER: builtins.int
     asset_type: osmosis.superfluid.superfluid_pb2.SuperfluidAssetType.ValueType
     def __init__(
         self,
         *,
         asset_type: osmosis.superfluid.superfluid_pb2.SuperfluidAssetType.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["asset_type", b"asset_type"]) -> None: ...
 
 global___AssetTypeResponse = AssetTypeResponse
 
+@typing_extensions.final
 class AllAssetsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___AllAssetsRequest = AllAssetsRequest
 
+@typing_extensions.final
 class AllAssetsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ASSETS_FIELD_NUMBER: builtins.int
     @property
     def assets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.superfluid.superfluid_pb2.SuperfluidAsset]: ...
     def __init__(
@@ -96,28 +102,30 @@
         *,
         assets: collections.abc.Iterable[osmosis.superfluid.superfluid_pb2.SuperfluidAsset] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["assets", b"assets"]) -> None: ...
 
 global___AllAssetsResponse = AllAssetsResponse
 
+@typing_extensions.final
 class AssetMultiplierRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
     def __init__(
         self,
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___AssetMultiplierRequest = AssetMultiplierRequest
 
+@typing_extensions.final
 class AssetMultiplierResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OSMO_EQUIVALENT_MULTIPLIER_FIELD_NUMBER: builtins.int
     @property
     def osmo_equivalent_multiplier(self) -> osmosis.superfluid.superfluid_pb2.OsmoEquivalentMultiplierRecord: ...
     def __init__(
@@ -126,14 +134,15 @@
         osmo_equivalent_multiplier: osmosis.superfluid.superfluid_pb2.OsmoEquivalentMultiplierRecord | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["osmo_equivalent_multiplier", b"osmo_equivalent_multiplier"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["osmo_equivalent_multiplier", b"osmo_equivalent_multiplier"]) -> None: ...
 
 global___AssetMultiplierResponse = AssetMultiplierResponse
 
+@typing_extensions.final
 class SuperfluidIntermediaryAccountInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     VAL_ADDR_FIELD_NUMBER: builtins.int
     GAUGE_ID_FIELD_NUMBER: builtins.int
     ADDRESS_FIELD_NUMBER: builtins.int
@@ -149,14 +158,15 @@
         gauge_id: builtins.int = ...,
         address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "denom", b"denom", "gauge_id", b"gauge_id", "val_addr", b"val_addr"]) -> None: ...
 
 global___SuperfluidIntermediaryAccountInfo = SuperfluidIntermediaryAccountInfo
 
+@typing_extensions.final
 class AllIntermediaryAccountsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def pagination(self) -> cosmos.base.query.v1beta1.pagination_pb2.PageRequest: ...
     def __init__(
@@ -165,14 +175,15 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageRequest | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> None: ...
 
 global___AllIntermediaryAccountsRequest = AllIntermediaryAccountsRequest
 
+@typing_extensions.final
 class AllIntermediaryAccountsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCOUNTS_FIELD_NUMBER: builtins.int
     PAGINATION_FIELD_NUMBER: builtins.int
     @property
     def accounts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SuperfluidIntermediaryAccountInfo]: ...
@@ -185,28 +196,30 @@
         pagination: cosmos.base.query.v1beta1.pagination_pb2.PageResponse | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pagination", b"pagination"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["accounts", b"accounts", "pagination", b"pagination"]) -> None: ...
 
 global___AllIntermediaryAccountsResponse = AllIntermediaryAccountsResponse
 
+@typing_extensions.final
 class ConnectedIntermediaryAccountRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOCK_ID_FIELD_NUMBER: builtins.int
     lock_id: builtins.int
     def __init__(
         self,
         *,
         lock_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id"]) -> None: ...
 
 global___ConnectedIntermediaryAccountRequest = ConnectedIntermediaryAccountRequest
 
+@typing_extensions.final
 class ConnectedIntermediaryAccountResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACCOUNT_FIELD_NUMBER: builtins.int
     @property
     def account(self) -> global___SuperfluidIntermediaryAccountInfo: ...
     def __init__(
@@ -215,28 +228,30 @@
         account: global___SuperfluidIntermediaryAccountInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["account", b"account"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["account", b"account"]) -> None: ...
 
 global___ConnectedIntermediaryAccountResponse = ConnectedIntermediaryAccountResponse
 
+@typing_extensions.final
 class QueryTotalDelegationByValidatorForDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
     def __init__(
         self,
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryTotalDelegationByValidatorForDenomRequest = QueryTotalDelegationByValidatorForDenomRequest
 
+@typing_extensions.final
 class QueryTotalDelegationByValidatorForDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ASSETS_FIELD_NUMBER: builtins.int
     @property
     def assets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Delegations]: ...
     def __init__(
@@ -244,14 +259,15 @@
         *,
         assets: collections.abc.Iterable[global___Delegations] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["assets", b"assets"]) -> None: ...
 
 global___QueryTotalDelegationByValidatorForDenomResponse = QueryTotalDelegationByValidatorForDenomResponse
 
+@typing_extensions.final
 class Delegations(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VAL_ADDR_FIELD_NUMBER: builtins.int
     AMOUNT_SFSD_FIELD_NUMBER: builtins.int
     OSMO_EQUIVALENT_FIELD_NUMBER: builtins.int
     val_addr: builtins.str
@@ -264,37 +280,40 @@
         amount_sfsd: builtins.str = ...,
         osmo_equivalent: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount_sfsd", b"amount_sfsd", "osmo_equivalent", b"osmo_equivalent", "val_addr", b"val_addr"]) -> None: ...
 
 global___Delegations = Delegations
 
+@typing_extensions.final
 class TotalSuperfluidDelegationsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___TotalSuperfluidDelegationsRequest = TotalSuperfluidDelegationsRequest
 
+@typing_extensions.final
 class TotalSuperfluidDelegationsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_DELEGATIONS_FIELD_NUMBER: builtins.int
     total_delegations: builtins.str
     def __init__(
         self,
         *,
         total_delegations: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["total_delegations", b"total_delegations"]) -> None: ...
 
 global___TotalSuperfluidDelegationsResponse = TotalSuperfluidDelegationsResponse
 
+@typing_extensions.final
 class SuperfluidDelegationAmountRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDRESS_FIELD_NUMBER: builtins.int
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     delegator_address: builtins.str
@@ -307,14 +326,15 @@
         validator_address: builtins.str = ...,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "denom", b"denom", "validator_address", b"validator_address"]) -> None: ...
 
 global___SuperfluidDelegationAmountRequest = SuperfluidDelegationAmountRequest
 
+@typing_extensions.final
 class SuperfluidDelegationAmountResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AMOUNT_FIELD_NUMBER: builtins.int
     @property
     def amount(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -322,28 +342,30 @@
         *,
         amount: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> None: ...
 
 global___SuperfluidDelegationAmountResponse = SuperfluidDelegationAmountResponse
 
+@typing_extensions.final
 class SuperfluidDelegationsByDelegatorRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDRESS_FIELD_NUMBER: builtins.int
     delegator_address: builtins.str
     def __init__(
         self,
         *,
         delegator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address"]) -> None: ...
 
 global___SuperfluidDelegationsByDelegatorRequest = SuperfluidDelegationsByDelegatorRequest
 
+@typing_extensions.final
 class SuperfluidDelegationsByDelegatorResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUPERFLUID_DELEGATION_RECORDS_FIELD_NUMBER: builtins.int
     TOTAL_DELEGATED_COINS_FIELD_NUMBER: builtins.int
     TOTAL_EQUIVALENT_STAKED_AMOUNT_FIELD_NUMBER: builtins.int
     @property
@@ -360,14 +382,15 @@
         total_equivalent_staked_amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["total_equivalent_staked_amount", b"total_equivalent_staked_amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["superfluid_delegation_records", b"superfluid_delegation_records", "total_delegated_coins", b"total_delegated_coins", "total_equivalent_staked_amount", b"total_equivalent_staked_amount"]) -> None: ...
 
 global___SuperfluidDelegationsByDelegatorResponse = SuperfluidDelegationsByDelegatorResponse
 
+@typing_extensions.final
 class SuperfluidUndelegationsByDelegatorRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDRESS_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     delegator_address: builtins.str
     denom: builtins.str
@@ -377,14 +400,15 @@
         delegator_address: builtins.str = ...,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address", "denom", b"denom"]) -> None: ...
 
 global___SuperfluidUndelegationsByDelegatorRequest = SuperfluidUndelegationsByDelegatorRequest
 
+@typing_extensions.final
 class SuperfluidUndelegationsByDelegatorResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUPERFLUID_DELEGATION_RECORDS_FIELD_NUMBER: builtins.int
     TOTAL_UNDELEGATED_COINS_FIELD_NUMBER: builtins.int
     SYNTHETIC_LOCKS_FIELD_NUMBER: builtins.int
     @property
@@ -400,14 +424,15 @@
         total_undelegated_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
         synthetic_locks: collections.abc.Iterable[osmosis.lockup.lock_pb2.SyntheticLock] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["superfluid_delegation_records", b"superfluid_delegation_records", "synthetic_locks", b"synthetic_locks", "total_undelegated_coins", b"total_undelegated_coins"]) -> None: ...
 
 global___SuperfluidUndelegationsByDelegatorResponse = SuperfluidUndelegationsByDelegatorResponse
 
+@typing_extensions.final
 class SuperfluidDelegationsByValidatorDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     validator_address: builtins.str
     denom: builtins.str
@@ -417,14 +442,15 @@
         validator_address: builtins.str = ...,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "validator_address", b"validator_address"]) -> None: ...
 
 global___SuperfluidDelegationsByValidatorDenomRequest = SuperfluidDelegationsByValidatorDenomRequest
 
+@typing_extensions.final
 class SuperfluidDelegationsByValidatorDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUPERFLUID_DELEGATION_RECORDS_FIELD_NUMBER: builtins.int
     @property
     def superfluid_delegation_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.superfluid.superfluid_pb2.SuperfluidDelegationRecord]: ...
     def __init__(
@@ -432,14 +458,15 @@
         *,
         superfluid_delegation_records: collections.abc.Iterable[osmosis.superfluid.superfluid_pb2.SuperfluidDelegationRecord] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["superfluid_delegation_records", b"superfluid_delegation_records"]) -> None: ...
 
 global___SuperfluidDelegationsByValidatorDenomResponse = SuperfluidDelegationsByValidatorDenomResponse
 
+@typing_extensions.final
 class EstimateSuperfluidDelegatedAmountByValidatorDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
     DENOM_FIELD_NUMBER: builtins.int
     validator_address: builtins.str
     denom: builtins.str
@@ -449,14 +476,15 @@
         validator_address: builtins.str = ...,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "validator_address", b"validator_address"]) -> None: ...
 
 global___EstimateSuperfluidDelegatedAmountByValidatorDenomRequest = EstimateSuperfluidDelegatedAmountByValidatorDenomRequest
 
+@typing_extensions.final
 class EstimateSuperfluidDelegatedAmountByValidatorDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_DELEGATED_COINS_FIELD_NUMBER: builtins.int
     @property
     def total_delegated_coins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[cosmos.base.v1beta1.coin_pb2.Coin]: ...
     def __init__(
@@ -464,28 +492,30 @@
         *,
         total_delegated_coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["total_delegated_coins", b"total_delegated_coins"]) -> None: ...
 
 global___EstimateSuperfluidDelegatedAmountByValidatorDenomResponse = EstimateSuperfluidDelegatedAmountByValidatorDenomResponse
 
+@typing_extensions.final
 class QueryTotalDelegationByDelegatorRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DELEGATOR_ADDRESS_FIELD_NUMBER: builtins.int
     delegator_address: builtins.str
     def __init__(
         self,
         *,
         delegator_address: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegator_address", b"delegator_address"]) -> None: ...
 
 global___QueryTotalDelegationByDelegatorRequest = QueryTotalDelegationByDelegatorRequest
 
+@typing_extensions.final
 class QueryTotalDelegationByDelegatorResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUPERFLUID_DELEGATION_RECORDS_FIELD_NUMBER: builtins.int
     DELEGATION_RESPONSE_FIELD_NUMBER: builtins.int
     TOTAL_DELEGATED_COINS_FIELD_NUMBER: builtins.int
     TOTAL_EQUIVALENT_STAKED_AMOUNT_FIELD_NUMBER: builtins.int
@@ -506,23 +536,25 @@
         total_equivalent_staked_amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["total_equivalent_staked_amount", b"total_equivalent_staked_amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegation_response", b"delegation_response", "superfluid_delegation_records", b"superfluid_delegation_records", "total_delegated_coins", b"total_delegated_coins", "total_equivalent_staked_amount", b"total_equivalent_staked_amount"]) -> None: ...
 
 global___QueryTotalDelegationByDelegatorResponse = QueryTotalDelegationByDelegatorResponse
 
+@typing_extensions.final
 class QueryUnpoolWhitelistRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryUnpoolWhitelistRequest = QueryUnpoolWhitelistRequest
 
+@typing_extensions.final
 class QueryUnpoolWhitelistResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_IDS_FIELD_NUMBER: builtins.int
     @property
     def pool_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/superfluid_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _SuperfluidAssetType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _SuperfluidAssetTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SuperfluidAssetType.ValueType], builtins.type):  # noqa: F821
+class _SuperfluidAssetTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SuperfluidAssetType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SuperfluidAssetTypeNative: _SuperfluidAssetType.ValueType  # 0
     SuperfluidAssetTypeLPShare: _SuperfluidAssetType.ValueType  # 1
     """SuperfluidAssetTypeLendingShare = 2; // for now not exist"""
 
 class SuperfluidAssetType(_SuperfluidAssetType, metaclass=_SuperfluidAssetTypeEnumTypeWrapper):
     """SuperfluidAssetType indicates whether the superfluid asset is
@@ -35,14 +35,15 @@
     """
 
 SuperfluidAssetTypeNative: SuperfluidAssetType.ValueType  # 0
 SuperfluidAssetTypeLPShare: SuperfluidAssetType.ValueType  # 1
 """SuperfluidAssetTypeLendingShare = 2; // for now not exist"""
 global___SuperfluidAssetType = SuperfluidAssetType
 
+@typing_extensions.final
 class SuperfluidAsset(google.protobuf.message.Message):
     """SuperfluidAsset stores the pair of superfluid asset type and denom pair"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     ASSET_TYPE_FIELD_NUMBER: builtins.int
@@ -57,14 +58,15 @@
         denom: builtins.str = ...,
         asset_type: global___SuperfluidAssetType.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["asset_type", b"asset_type", "denom", b"denom"]) -> None: ...
 
 global___SuperfluidAsset = SuperfluidAsset
 
+@typing_extensions.final
 class SuperfluidIntermediaryAccount(google.protobuf.message.Message):
     """SuperfluidIntermediaryAccount takes the role of intermediary between LP token
     and OSMO tokens for superfluid staking. The intermediary account is the
     actual account responsible for delegation, not the validator account itself.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -84,14 +86,15 @@
         val_addr: builtins.str = ...,
         gauge_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "gauge_id", b"gauge_id", "val_addr", b"val_addr"]) -> None: ...
 
 global___SuperfluidIntermediaryAccount = SuperfluidIntermediaryAccount
 
+@typing_extensions.final
 class OsmoEquivalentMultiplierRecord(google.protobuf.message.Message):
     """The Osmo-Equivalent-Multiplier Record for epoch N refers to the osmo worth we
     treat an LP share as having, for all of epoch N. Eventually this is intended
     to be set as the Time-weighted-average-osmo-backing for the entire duration
     of epoch N-1. (Thereby locking whats in use for epoch N as based on the prior
     epochs rewards) However for now, this is not the TWAP but instead the spot
     price at the boundary. For different types of assets in the future, it could
@@ -114,14 +117,15 @@
         denom: builtins.str = ...,
         multiplier: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "epoch_number", b"epoch_number", "multiplier", b"multiplier"]) -> None: ...
 
 global___OsmoEquivalentMultiplierRecord = OsmoEquivalentMultiplierRecord
 
+@typing_extensions.final
 class SuperfluidDelegationRecord(google.protobuf.message.Message):
     """SuperfluidDelegationRecord is a struct used to indicate superfluid
     delegations of an account in the state machine in a user friendly form.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -144,14 +148,15 @@
         equivalent_staked_amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["delegation_amount", b"delegation_amount", "equivalent_staked_amount", b"equivalent_staked_amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["delegation_amount", b"delegation_amount", "delegator_address", b"delegator_address", "equivalent_staked_amount", b"equivalent_staked_amount", "validator_address", b"validator_address"]) -> None: ...
 
 global___SuperfluidDelegationRecord = SuperfluidDelegationRecord
 
+@typing_extensions.final
 class LockIdIntermediaryAccountConnection(google.protobuf.message.Message):
     """LockIdIntermediaryAccountConnection is a struct used to indicate the
     relationship between the underlying lock id and superfluid delegation done
     via lp shares.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -166,14 +171,15 @@
         lock_id: builtins.int = ...,
         intermediary_account: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["intermediary_account", b"intermediary_account", "lock_id", b"lock_id"]) -> None: ...
 
 global___LockIdIntermediaryAccountConnection = LockIdIntermediaryAccountConnection
 
+@typing_extensions.final
 class UnpoolWhitelistedPools(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IDS_FIELD_NUMBER: builtins.int
     @property
     def ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgSuperfluidDelegate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     LOCK_ID_FIELD_NUMBER: builtins.int
     VAL_ADDR_FIELD_NUMBER: builtins.int
     sender: builtins.str
@@ -33,23 +34,25 @@
         lock_id: builtins.int = ...,
         val_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id", "sender", b"sender", "val_addr", b"val_addr"]) -> None: ...
 
 global___MsgSuperfluidDelegate = MsgSuperfluidDelegate
 
+@typing_extensions.final
 class MsgSuperfluidDelegateResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgSuperfluidDelegateResponse = MsgSuperfluidDelegateResponse
 
+@typing_extensions.final
 class MsgSuperfluidUndelegate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     LOCK_ID_FIELD_NUMBER: builtins.int
     sender: builtins.str
     lock_id: builtins.int
@@ -59,23 +62,25 @@
         sender: builtins.str = ...,
         lock_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id", "sender", b"sender"]) -> None: ...
 
 global___MsgSuperfluidUndelegate = MsgSuperfluidUndelegate
 
+@typing_extensions.final
 class MsgSuperfluidUndelegateResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgSuperfluidUndelegateResponse = MsgSuperfluidUndelegateResponse
 
+@typing_extensions.final
 class MsgSuperfluidUnbondLock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SENDER_FIELD_NUMBER: builtins.int
     LOCK_ID_FIELD_NUMBER: builtins.int
     sender: builtins.str
     lock_id: builtins.int
@@ -85,23 +90,25 @@
         sender: builtins.str = ...,
         lock_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["lock_id", b"lock_id", "sender", b"sender"]) -> None: ...
 
 global___MsgSuperfluidUnbondLock = MsgSuperfluidUnbondLock
 
+@typing_extensions.final
 class MsgSuperfluidUnbondLockResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgSuperfluidUnbondLockResponse = MsgSuperfluidUnbondLockResponse
 
+@typing_extensions.final
 class MsgLockAndSuperfluidDelegate(google.protobuf.message.Message):
     """message MsgSuperfluidRedelegate {
       string sender = 1 [ (gogoproto.moretags) = "yaml:\\"sender\\"" ];
       uint64 lock_id = 2;
       string new_val_addr = 3;
     }
     message MsgSuperfluidRedelegateResponse {}
@@ -127,28 +134,30 @@
         coins: collections.abc.Iterable[cosmos.base.v1beta1.coin_pb2.Coin] | None = ...,
         val_addr: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["coins", b"coins", "sender", b"sender", "val_addr", b"val_addr"]) -> None: ...
 
 global___MsgLockAndSuperfluidDelegate = MsgLockAndSuperfluidDelegate
 
+@typing_extensions.final
 class MsgLockAndSuperfluidDelegateResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     ID: builtins.int
     def __init__(
         self,
         *,
         ID: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["ID", b"ID"]) -> None: ...
 
 global___MsgLockAndSuperfluidDelegateResponse = MsgLockAndSuperfluidDelegateResponse
 
+@typing_extensions.final
 class MsgUnPoolWhitelistedPool(google.protobuf.message.Message):
     """MsgUnPoolWhitelistedPool Unpools every lock the sender has, that is
     associated with pool pool_id. If pool_id is not approved for unpooling by
     governance, this is a no-op. Unpooling takes the locked gamm shares, and runs
     "ExitPool" on it, to get the constituent tokens. e.g. z gamm/pool/1 tokens
     ExitPools into constituent tokens x uatom, y uosmo. Then it creates a new
     lock for every constituent token, with the duration associated with the lock.
@@ -168,14 +177,15 @@
         sender: builtins.str = ...,
         pool_id: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pool_id", b"pool_id", "sender", b"sender"]) -> None: ...
 
 global___MsgUnPoolWhitelistedPool = MsgUnPoolWhitelistedPool
 
+@typing_extensions.final
 class MsgUnPoolWhitelistedPoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXITED_LOCK_IDS_FIELD_NUMBER: builtins.int
     @property
     def exited_lock_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/superfluid/v1beta1/gov_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class SetSuperfluidAssetsProposal(google.protobuf.message.Message):
     """SetSuperfluidAssetsProposal is a gov Content type to update the superfluid
     assets
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -38,14 +39,15 @@
         description: builtins.str = ...,
         assets: collections.abc.Iterable[osmosis.superfluid.superfluid_pb2.SuperfluidAsset] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["assets", b"assets", "description", b"description", "title", b"title"]) -> None: ...
 
 global___SetSuperfluidAssetsProposal = SetSuperfluidAssetsProposal
 
+@typing_extensions.final
 class RemoveSuperfluidAssetsProposal(google.protobuf.message.Message):
     """RemoveSuperfluidAssetsProposal is a gov Content type to remove the superfluid
     assets by denom
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -63,14 +65,15 @@
         description: builtins.str = ...,
         superfluid_asset_denoms: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "superfluid_asset_denoms", b"superfluid_asset_denoms", "title", b"title"]) -> None: ...
 
 global___RemoveSuperfluidAssetsProposal = RemoveSuperfluidAssetsProposal
 
+@typing_extensions.final
 class UpdateUnpoolWhiteListProposal(google.protobuf.message.Message):
     """UpdateUnpoolWhiteListProposal is a gov Content type to update the
     allowed list of pool ids.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/authorityMetadata_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class DenomAuthorityMetadata(google.protobuf.message.Message):
     """DenomAuthorityMetadata specifies metadata for addresses that have specific
     capabilities over a token factory denom. Right now there is only one Admin
     permission, but is planned to be extended to the future.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/genesis_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the tokenfactory module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     FACTORY_DENOMS_FIELD_NUMBER: builtins.int
@@ -37,14 +38,15 @@
         factory_denoms: collections.abc.Iterable[global___GenesisDenom] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["factory_denoms", b"factory_denoms", "params", b"params"]) -> None: ...
 
 global___GenesisState = GenesisState
 
+@typing_extensions.final
 class GenesisDenom(google.protobuf.message.Message):
     """GenesisDenom defines a tokenfactory denom that is defined within genesis
     state. The structure contains DenomAuthorityMetadata which defines the
     denom's admin.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/params_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params defines the parameters for the tokenfactory module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_CREATION_FEE_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryParamsRequest(google.protobuf.message.Message):
     """QueryParamsRequest is the request type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryParamsRequest = QueryParamsRequest
 
+@typing_extensions.final
 class QueryParamsResponse(google.protobuf.message.Message):
     """QueryParamsResponse is the response type for the Query/Params RPC method."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
@@ -44,14 +46,15 @@
         params: osmosis.tokenfactory.v1beta1.params_pb2.Params | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["params", b"params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["params", b"params"]) -> None: ...
 
 global___QueryParamsResponse = QueryParamsResponse
 
+@typing_extensions.final
 class QueryDenomAuthorityMetadataRequest(google.protobuf.message.Message):
     """QueryDenomAuthorityMetadataRequest defines the request structure for the
     DenomAuthorityMetadata gRPC query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -62,14 +65,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryDenomAuthorityMetadataRequest = QueryDenomAuthorityMetadataRequest
 
+@typing_extensions.final
 class QueryDenomAuthorityMetadataResponse(google.protobuf.message.Message):
     """QueryDenomAuthorityMetadataResponse defines the response structure for the
     DenomAuthorityMetadata gRPC query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -82,14 +86,15 @@
         authority_metadata: osmosis.tokenfactory.v1beta1.authorityMetadata_pb2.DenomAuthorityMetadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["authority_metadata", b"authority_metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["authority_metadata", b"authority_metadata"]) -> None: ...
 
 global___QueryDenomAuthorityMetadataResponse = QueryDenomAuthorityMetadataResponse
 
+@typing_extensions.final
 class QueryDenomsFromCreatorRequest(google.protobuf.message.Message):
     """QueryDenomsFromCreatorRequest defines the request structure for the
     DenomsFromCreator gRPC query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -100,14 +105,15 @@
         *,
         creator: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["creator", b"creator"]) -> None: ...
 
 global___QueryDenomsFromCreatorRequest = QueryDenomsFromCreatorRequest
 
+@typing_extensions.final
 class QueryDenomsFromCreatorResponse(google.protobuf.message.Message):
     """QueryDenomsFromCreatorRequest defines the response structure for the
     DenomsFromCreator gRPC query.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class MsgCreateDenom(google.protobuf.message.Message):
     """MsgCreateDenom defines the message structure for the CreateDenom gRPC service
     method. It allows an account to create a new denom. It requires a sender
     address and a sub denomination. The (sender_address, sub_denomination) tuple
     must be unique and cannot be re-used.
 
     The resulting denom created is defined as
@@ -41,14 +42,15 @@
         sender: builtins.str = ...,
         subdenom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["sender", b"sender", "subdenom", b"subdenom"]) -> None: ...
 
 global___MsgCreateDenom = MsgCreateDenom
 
+@typing_extensions.final
 class MsgCreateDenomResponse(google.protobuf.message.Message):
     """MsgCreateDenomResponse is the return value of MsgCreateDenom
     It returns the full string of the newly created denom
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -59,14 +61,15 @@
         *,
         new_token_denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["new_token_denom", b"new_token_denom"]) -> None: ...
 
 global___MsgCreateDenomResponse = MsgCreateDenomResponse
 
+@typing_extensions.final
 class MsgMint(google.protobuf.message.Message):
     """MsgMint is the sdk.Msg type for allowing an admin account to mint
     more of a token.  For now, we only support minting to the sender account
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -82,23 +85,25 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "sender", b"sender"]) -> None: ...
 
 global___MsgMint = MsgMint
 
+@typing_extensions.final
 class MsgMintResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgMintResponse = MsgMintResponse
 
+@typing_extensions.final
 class MsgBurn(google.protobuf.message.Message):
     """MsgBurn is the sdk.Msg type for allowing an admin account to burn
     a token.  For now, we only support burning from the sender account.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -114,23 +119,25 @@
         amount: cosmos.base.v1beta1.coin_pb2.Coin | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["amount", b"amount"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["amount", b"amount", "sender", b"sender"]) -> None: ...
 
 global___MsgBurn = MsgBurn
 
+@typing_extensions.final
 class MsgBurnResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgBurnResponse = MsgBurnResponse
 
+@typing_extensions.final
 class MsgChangeAdmin(google.protobuf.message.Message):
     """MsgChangeAdmin is the sdk.Msg type for allowing an admin account to reassign
     adminship of a denom to a new account
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -147,27 +154,29 @@
         denom: builtins.str = ...,
         new_admin: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom", "new_admin", b"new_admin", "sender", b"sender"]) -> None: ...
 
 global___MsgChangeAdmin = MsgChangeAdmin
 
+@typing_extensions.final
 class MsgChangeAdminResponse(google.protobuf.message.Message):
     """MsgChangeAdminResponse defines the response structure for an executed
     MsgChangeAdmin message.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___MsgChangeAdminResponse = MsgChangeAdminResponse
 
+@typing_extensions.final
 class MsgSetDenomMetadata(google.protobuf.message.Message):
     """message MsgForceTransferResponse {}
 
     MsgSetDenomMetadata is the sdk.Msg type for allowing an admin account to set
     the denom's bank metadata
     """
 
@@ -185,14 +194,15 @@
         metadata: cosmos.bank.v1beta1.bank_pb2.Metadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["metadata", b"metadata", "sender", b"sender"]) -> None: ...
 
 global___MsgSetDenomMetadata = MsgSetDenomMetadata
 
+@typing_extensions.final
 class MsgSetDenomMetadataResponse(google.protobuf.message.Message):
     """MsgSetDenomMetadataResponse defines the response structure for an executed
     MsgSetDenomMetadata message.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/tokenfactory/v1beta1/tx_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/genesis_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Params(google.protobuf.message.Message):
     """Params holds parameters for the twap module"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PRUNE_EPOCH_IDENTIFIER_FIELD_NUMBER: builtins.int
     RECORD_HISTORY_KEEP_PERIOD_FIELD_NUMBER: builtins.int
@@ -35,14 +36,15 @@
         record_history_keep_period: google.protobuf.duration_pb2.Duration | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["record_history_keep_period", b"record_history_keep_period"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["prune_epoch_identifier", b"prune_epoch_identifier", "record_history_keep_period", b"record_history_keep_period"]) -> None: ...
 
 global___Params = Params
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the twap module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TWAPS_FIELD_NUMBER: builtins.int
     PARAMS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ArithmeticTwapRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     BASE_ASSET_FIELD_NUMBER: builtins.int
     QUOTE_ASSET_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
@@ -41,28 +42,30 @@
         end_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset", b"base_asset", "end_time", b"end_time", "pool_id", b"pool_id", "quote_asset", b"quote_asset", "start_time", b"start_time"]) -> None: ...
 
 global___ArithmeticTwapRequest = ArithmeticTwapRequest
 
+@typing_extensions.final
 class ArithmeticTwapResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ARITHMETIC_TWAP_FIELD_NUMBER: builtins.int
     arithmetic_twap: builtins.str
     def __init__(
         self,
         *,
         arithmetic_twap: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["arithmetic_twap", b"arithmetic_twap"]) -> None: ...
 
 global___ArithmeticTwapResponse = ArithmeticTwapResponse
 
+@typing_extensions.final
 class ArithmeticTwapToNowRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     BASE_ASSET_FIELD_NUMBER: builtins.int
     QUOTE_ASSET_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
@@ -80,28 +83,30 @@
         start_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset", b"base_asset", "pool_id", b"pool_id", "quote_asset", b"quote_asset", "start_time", b"start_time"]) -> None: ...
 
 global___ArithmeticTwapToNowRequest = ArithmeticTwapToNowRequest
 
+@typing_extensions.final
 class ArithmeticTwapToNowResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ARITHMETIC_TWAP_FIELD_NUMBER: builtins.int
     arithmetic_twap: builtins.str
     def __init__(
         self,
         *,
         arithmetic_twap: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["arithmetic_twap", b"arithmetic_twap"]) -> None: ...
 
 global___ArithmeticTwapToNowResponse = ArithmeticTwapToNowResponse
 
+@typing_extensions.final
 class GeometricTwapRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     BASE_ASSET_FIELD_NUMBER: builtins.int
     QUOTE_ASSET_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
@@ -123,28 +128,30 @@
         end_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["end_time", b"end_time", "start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset", b"base_asset", "end_time", b"end_time", "pool_id", b"pool_id", "quote_asset", b"quote_asset", "start_time", b"start_time"]) -> None: ...
 
 global___GeometricTwapRequest = GeometricTwapRequest
 
+@typing_extensions.final
 class GeometricTwapResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GEOMETRIC_TWAP_FIELD_NUMBER: builtins.int
     geometric_twap: builtins.str
     def __init__(
         self,
         *,
         geometric_twap: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["geometric_twap", b"geometric_twap"]) -> None: ...
 
 global___GeometricTwapResponse = GeometricTwapResponse
 
+@typing_extensions.final
 class GeometricTwapToNowRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOL_ID_FIELD_NUMBER: builtins.int
     BASE_ASSET_FIELD_NUMBER: builtins.int
     QUOTE_ASSET_FIELD_NUMBER: builtins.int
     START_TIME_FIELD_NUMBER: builtins.int
@@ -162,37 +169,40 @@
         start_time: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["start_time", b"start_time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_asset", b"base_asset", "pool_id", b"pool_id", "quote_asset", b"quote_asset", "start_time", b"start_time"]) -> None: ...
 
 global___GeometricTwapToNowRequest = GeometricTwapToNowRequest
 
+@typing_extensions.final
 class GeometricTwapToNowResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GEOMETRIC_TWAP_FIELD_NUMBER: builtins.int
     geometric_twap: builtins.str
     def __init__(
         self,
         *,
         geometric_twap: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["geometric_twap", b"geometric_twap"]) -> None: ...
 
 global___GeometricTwapToNowResponse = GeometricTwapToNowResponse
 
+@typing_extensions.final
 class ParamsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ParamsRequest = ParamsRequest
 
+@typing_extensions.final
 class ParamsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMS_FIELD_NUMBER: builtins.int
     @property
     def params(self) -> osmosis.twap.v1beta1.genesis_pb2.Params: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/twap/v1beta1/twap_record_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class TwapRecord(google.protobuf.message.Message):
     """A TWAP record should be indexed in state by pool_id, (asset pair), timestamp
     The asset pair assets should be lexicographically sorted.
     Technically (pool_id, asset_0_denom, asset_1_denom, height) do not need to
     appear in the struct however we view this as the wrong performance tradeoff
     given SDK today. Would rather we optimize for readability and correctness,
     than an optimal state storage format. The system bottleneck is elsewhere for
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/feetoken_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class FeeToken(google.protobuf.message.Message):
     """FeeToken is a struct that specifies a coin denom, and pool ID pair.
     This marks the token as eligible for use as a tx fee asset in Osmosis.
     Its price in osmo is derived through looking at the provided pool ID.
     The pool ID must have osmo as one of its assets.
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/genesis_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class GenesisState(google.protobuf.message.Message):
     """GenesisState defines the txfees module's genesis state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASEDENOM_FIELD_NUMBER: builtins.int
     FEETOKENS_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/gov_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class UpdateFeeTokenProposal(google.protobuf.message.Message):
     """UpdateFeeTokenProposal is a gov Content type for adding a new whitelisted fee
     token. It must specify a denom along with gamm pool ID to use as a spot price
     calculator. It can be used to add a new denom to the whitelist It can also be
     used to update the Pool to associate with the denom. If Pool ID is set to 0,
     it will remove the denom from the whitelisted set.
     """
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class QueryFeeTokensRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryFeeTokensRequest = QueryFeeTokensRequest
 
+@typing_extensions.final
 class QueryFeeTokensResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FEE_TOKENS_FIELD_NUMBER: builtins.int
     @property
     def fee_tokens(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[osmosis.txfees.v1beta1.feetoken_pb2.FeeToken]: ...
     def __init__(
@@ -37,14 +39,15 @@
         *,
         fee_tokens: collections.abc.Iterable[osmosis.txfees.v1beta1.feetoken_pb2.FeeToken] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["fee_tokens", b"fee_tokens"]) -> None: ...
 
 global___QueryFeeTokensResponse = QueryFeeTokensResponse
 
+@typing_extensions.final
 class QueryDenomSpotPriceRequest(google.protobuf.message.Message):
     """QueryDenomSpotPriceRequest defines grpc request structure for querying spot
     price for the specified tx fee denom
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -55,14 +58,15 @@
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryDenomSpotPriceRequest = QueryDenomSpotPriceRequest
 
+@typing_extensions.final
 class QueryDenomSpotPriceResponse(google.protobuf.message.Message):
     """QueryDenomSpotPriceRequest defines grpc response structure for querying spot
     price for the specified tx fee denom
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -76,51 +80,55 @@
         poolID: builtins.int = ...,
         spot_price: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["poolID", b"poolID", "spot_price", b"spot_price"]) -> None: ...
 
 global___QueryDenomSpotPriceResponse = QueryDenomSpotPriceResponse
 
+@typing_extensions.final
 class QueryDenomPoolIdRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DENOM_FIELD_NUMBER: builtins.int
     denom: builtins.str
     def __init__(
         self,
         *,
         denom: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["denom", b"denom"]) -> None: ...
 
 global___QueryDenomPoolIdRequest = QueryDenomPoolIdRequest
 
+@typing_extensions.final
 class QueryDenomPoolIdResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     POOLID_FIELD_NUMBER: builtins.int
     poolID: builtins.int
     def __init__(
         self,
         *,
         poolID: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["poolID", b"poolID"]) -> None: ...
 
 global___QueryDenomPoolIdResponse = QueryDenomPoolIdResponse
 
+@typing_extensions.final
 class QueryBaseDenomRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___QueryBaseDenomRequest = QueryBaseDenomRequest
 
+@typing_extensions.final
 class QueryBaseDenomResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_DENOM_FIELD_NUMBER: builtins.int
     base_denom: builtins.str
     def __init__(
         self,
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/osmosis/txfees/v1beta1/query_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -23,42 +23,43 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _CheckTxType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _CheckTxTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CheckTxType.ValueType], builtins.type):  # noqa: F821
+class _CheckTxTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CheckTxType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     NEW: _CheckTxType.ValueType  # 0
     RECHECK: _CheckTxType.ValueType  # 1
 
 class CheckTxType(_CheckTxType, metaclass=_CheckTxTypeEnumTypeWrapper): ...
 
 NEW: CheckTxType.ValueType  # 0
 RECHECK: CheckTxType.ValueType  # 1
 global___CheckTxType = CheckTxType
 
 class _EvidenceType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _EvidenceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_EvidenceType.ValueType], builtins.type):  # noqa: F821
+class _EvidenceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_EvidenceType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _EvidenceType.ValueType  # 0
     DUPLICATE_VOTE: _EvidenceType.ValueType  # 1
     LIGHT_CLIENT_ATTACK: _EvidenceType.ValueType  # 2
 
 class EvidenceType(_EvidenceType, metaclass=_EvidenceTypeEnumTypeWrapper): ...
 
 UNKNOWN: EvidenceType.ValueType  # 0
 DUPLICATE_VOTE: EvidenceType.ValueType  # 1
 LIGHT_CLIENT_ATTACK: EvidenceType.ValueType  # 2
 global___EvidenceType = EvidenceType
 
+@typing_extensions.final
 class Request(google.protobuf.message.Message):
     """----------------------------------------
     Request types
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -128,37 +129,40 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["apply_snapshot_chunk", b"apply_snapshot_chunk", "begin_block", b"begin_block", "check_tx", b"check_tx", "commit", b"commit", "deliver_tx", b"deliver_tx", "echo", b"echo", "end_block", b"end_block", "flush", b"flush", "info", b"info", "init_chain", b"init_chain", "list_snapshots", b"list_snapshots", "load_snapshot_chunk", b"load_snapshot_chunk", "offer_snapshot", b"offer_snapshot", "query", b"query", "set_option", b"set_option", "value", b"value"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["apply_snapshot_chunk", b"apply_snapshot_chunk", "begin_block", b"begin_block", "check_tx", b"check_tx", "commit", b"commit", "deliver_tx", b"deliver_tx", "echo", b"echo", "end_block", b"end_block", "flush", b"flush", "info", b"info", "init_chain", b"init_chain", "list_snapshots", b"list_snapshots", "load_snapshot_chunk", b"load_snapshot_chunk", "offer_snapshot", b"offer_snapshot", "query", b"query", "set_option", b"set_option", "value", b"value"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["value", b"value"]) -> typing_extensions.Literal["echo", "flush", "info", "set_option", "init_chain", "query", "begin_block", "check_tx", "deliver_tx", "end_block", "commit", "list_snapshots", "offer_snapshot", "load_snapshot_chunk", "apply_snapshot_chunk"] | None: ...
 
 global___Request = Request
 
+@typing_extensions.final
 class RequestEcho(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MESSAGE_FIELD_NUMBER: builtins.int
     message: builtins.str
     def __init__(
         self,
         *,
         message: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["message", b"message"]) -> None: ...
 
 global___RequestEcho = RequestEcho
 
+@typing_extensions.final
 class RequestFlush(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___RequestFlush = RequestFlush
 
+@typing_extensions.final
 class RequestInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VERSION_FIELD_NUMBER: builtins.int
     BLOCK_VERSION_FIELD_NUMBER: builtins.int
     P2P_VERSION_FIELD_NUMBER: builtins.int
     version: builtins.str
@@ -171,14 +175,15 @@
         block_version: builtins.int = ...,
         p2p_version: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_version", b"block_version", "p2p_version", b"p2p_version", "version", b"version"]) -> None: ...
 
 global___RequestInfo = RequestInfo
 
+@typing_extensions.final
 class RequestSetOption(google.protobuf.message.Message):
     """nondeterministic"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
@@ -190,14 +195,15 @@
         key: builtins.str = ...,
         value: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
 global___RequestSetOption = RequestSetOption
 
+@typing_extensions.final
 class RequestInitChain(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIME_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
     CONSENSUS_PARAMS_FIELD_NUMBER: builtins.int
     VALIDATORS_FIELD_NUMBER: builtins.int
@@ -223,14 +229,15 @@
         initial_height: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["consensus_params", b"consensus_params", "time", b"time"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_state_bytes", b"app_state_bytes", "chain_id", b"chain_id", "consensus_params", b"consensus_params", "initial_height", b"initial_height", "time", b"time", "validators", b"validators"]) -> None: ...
 
 global___RequestInitChain = RequestInitChain
 
+@typing_extensions.final
 class RequestQuery(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     PATH_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
     PROVE_FIELD_NUMBER: builtins.int
@@ -246,14 +253,15 @@
         height: builtins.int = ...,
         prove: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "height", b"height", "path", b"path", "prove", b"prove"]) -> None: ...
 
 global___RequestQuery = RequestQuery
 
+@typing_extensions.final
 class RequestBeginBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HASH_FIELD_NUMBER: builtins.int
     HEADER_FIELD_NUMBER: builtins.int
     LAST_COMMIT_INFO_FIELD_NUMBER: builtins.int
     BYZANTINE_VALIDATORS_FIELD_NUMBER: builtins.int
@@ -273,14 +281,15 @@
         byzantine_validators: collections.abc.Iterable[global___Evidence] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["header", b"header", "last_commit_info", b"last_commit_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["byzantine_validators", b"byzantine_validators", "hash", b"hash", "header", b"header", "last_commit_info", b"last_commit_info"]) -> None: ...
 
 global___RequestBeginBlock = RequestBeginBlock
 
+@typing_extensions.final
 class RequestCheckTx(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TX_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     tx: builtins.bytes
     type: global___CheckTxType.ValueType
@@ -290,62 +299,67 @@
         tx: builtins.bytes = ...,
         type: global___CheckTxType.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["tx", b"tx", "type", b"type"]) -> None: ...
 
 global___RequestCheckTx = RequestCheckTx
 
+@typing_extensions.final
 class RequestDeliverTx(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TX_FIELD_NUMBER: builtins.int
     tx: builtins.bytes
     def __init__(
         self,
         *,
         tx: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["tx", b"tx"]) -> None: ...
 
 global___RequestDeliverTx = RequestDeliverTx
 
+@typing_extensions.final
 class RequestEndBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     height: builtins.int
     def __init__(
         self,
         *,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height"]) -> None: ...
 
 global___RequestEndBlock = RequestEndBlock
 
+@typing_extensions.final
 class RequestCommit(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___RequestCommit = RequestCommit
 
+@typing_extensions.final
 class RequestListSnapshots(google.protobuf.message.Message):
     """lists available snapshots"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___RequestListSnapshots = RequestListSnapshots
 
+@typing_extensions.final
 class RequestOfferSnapshot(google.protobuf.message.Message):
     """offers a snapshot to the application"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SNAPSHOT_FIELD_NUMBER: builtins.int
     APP_HASH_FIELD_NUMBER: builtins.int
@@ -361,14 +375,15 @@
         app_hash: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["snapshot", b"snapshot"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_hash", b"app_hash", "snapshot", b"snapshot"]) -> None: ...
 
 global___RequestOfferSnapshot = RequestOfferSnapshot
 
+@typing_extensions.final
 class RequestLoadSnapshotChunk(google.protobuf.message.Message):
     """loads a snapshot chunk"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     FORMAT_FIELD_NUMBER: builtins.int
@@ -383,14 +398,15 @@
         format: builtins.int = ...,
         chunk: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["chunk", b"chunk", "format", b"format", "height", b"height"]) -> None: ...
 
 global___RequestLoadSnapshotChunk = RequestLoadSnapshotChunk
 
+@typing_extensions.final
 class RequestApplySnapshotChunk(google.protobuf.message.Message):
     """Applies a snapshot chunk"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     CHUNK_FIELD_NUMBER: builtins.int
@@ -405,14 +421,15 @@
         chunk: builtins.bytes = ...,
         sender: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["chunk", b"chunk", "index", b"index", "sender", b"sender"]) -> None: ...
 
 global___RequestApplySnapshotChunk = RequestApplySnapshotChunk
 
+@typing_extensions.final
 class Response(google.protobuf.message.Message):
     """----------------------------------------
     Response types
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -486,14 +503,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["apply_snapshot_chunk", b"apply_snapshot_chunk", "begin_block", b"begin_block", "check_tx", b"check_tx", "commit", b"commit", "deliver_tx", b"deliver_tx", "echo", b"echo", "end_block", b"end_block", "exception", b"exception", "flush", b"flush", "info", b"info", "init_chain", b"init_chain", "list_snapshots", b"list_snapshots", "load_snapshot_chunk", b"load_snapshot_chunk", "offer_snapshot", b"offer_snapshot", "query", b"query", "set_option", b"set_option", "value", b"value"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["apply_snapshot_chunk", b"apply_snapshot_chunk", "begin_block", b"begin_block", "check_tx", b"check_tx", "commit", b"commit", "deliver_tx", b"deliver_tx", "echo", b"echo", "end_block", b"end_block", "exception", b"exception", "flush", b"flush", "info", b"info", "init_chain", b"init_chain", "list_snapshots", b"list_snapshots", "load_snapshot_chunk", b"load_snapshot_chunk", "offer_snapshot", b"offer_snapshot", "query", b"query", "set_option", b"set_option", "value", b"value"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["value", b"value"]) -> typing_extensions.Literal["exception", "echo", "flush", "info", "set_option", "init_chain", "query", "begin_block", "check_tx", "deliver_tx", "end_block", "commit", "list_snapshots", "offer_snapshot", "load_snapshot_chunk", "apply_snapshot_chunk"] | None: ...
 
 global___Response = Response
 
+@typing_extensions.final
 class ResponseException(google.protobuf.message.Message):
     """nondeterministic"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_FIELD_NUMBER: builtins.int
     error: builtins.str
@@ -502,37 +520,40 @@
         *,
         error: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["error", b"error"]) -> None: ...
 
 global___ResponseException = ResponseException
 
+@typing_extensions.final
 class ResponseEcho(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MESSAGE_FIELD_NUMBER: builtins.int
     message: builtins.str
     def __init__(
         self,
         *,
         message: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["message", b"message"]) -> None: ...
 
 global___ResponseEcho = ResponseEcho
 
+@typing_extensions.final
 class ResponseFlush(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ResponseFlush = ResponseFlush
 
+@typing_extensions.final
 class ResponseInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     APP_VERSION_FIELD_NUMBER: builtins.int
     LAST_BLOCK_HEIGHT_FIELD_NUMBER: builtins.int
@@ -551,14 +572,15 @@
         last_block_height: builtins.int = ...,
         last_block_app_hash: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_version", b"app_version", "data", b"data", "last_block_app_hash", b"last_block_app_hash", "last_block_height", b"last_block_height", "version", b"version"]) -> None: ...
 
 global___ResponseInfo = ResponseInfo
 
+@typing_extensions.final
 class ResponseSetOption(google.protobuf.message.Message):
     """nondeterministic"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
@@ -574,14 +596,15 @@
         log: builtins.str = ...,
         info: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "info", b"info", "log", b"log"]) -> None: ...
 
 global___ResponseSetOption = ResponseSetOption
 
+@typing_extensions.final
 class ResponseInitChain(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONSENSUS_PARAMS_FIELD_NUMBER: builtins.int
     VALIDATORS_FIELD_NUMBER: builtins.int
     APP_HASH_FIELD_NUMBER: builtins.int
     @property
@@ -597,14 +620,15 @@
         app_hash: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["consensus_params", b"consensus_params"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_hash", b"app_hash", "consensus_params", b"consensus_params", "validators", b"validators"]) -> None: ...
 
 global___ResponseInitChain = ResponseInitChain
 
+@typing_extensions.final
 class ResponseQuery(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
     INFO_FIELD_NUMBER: builtins.int
     INDEX_FIELD_NUMBER: builtins.int
@@ -641,14 +665,15 @@
         codespace: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["proof_ops", b"proof_ops"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "codespace", b"codespace", "height", b"height", "index", b"index", "info", b"info", "key", b"key", "log", b"log", "proof_ops", b"proof_ops", "value", b"value"]) -> None: ...
 
 global___ResponseQuery = ResponseQuery
 
+@typing_extensions.final
 class ResponseBeginBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVENTS_FIELD_NUMBER: builtins.int
     @property
     def events(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Event]: ...
     def __init__(
@@ -656,14 +681,15 @@
         *,
         events: collections.abc.Iterable[global___Event] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["events", b"events"]) -> None: ...
 
 global___ResponseBeginBlock = ResponseBeginBlock
 
+@typing_extensions.final
 class ResponseCheckTx(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
     INFO_FIELD_NUMBER: builtins.int
@@ -694,14 +720,15 @@
         events: collections.abc.Iterable[global___Event] | None = ...,
         codespace: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "codespace", b"codespace", "data", b"data", "events", b"events", "gas_used", b"gas_used", "gas_wanted", b"gas_wanted", "info", b"info", "log", b"log"]) -> None: ...
 
 global___ResponseCheckTx = ResponseCheckTx
 
+@typing_extensions.final
 class ResponseDeliverTx(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CODE_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     LOG_FIELD_NUMBER: builtins.int
     INFO_FIELD_NUMBER: builtins.int
@@ -732,14 +759,15 @@
         events: collections.abc.Iterable[global___Event] | None = ...,
         codespace: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "codespace", b"codespace", "data", b"data", "events", b"events", "gas_used", b"gas_used", "gas_wanted", b"gas_wanted", "info", b"info", "log", b"log"]) -> None: ...
 
 global___ResponseDeliverTx = ResponseDeliverTx
 
+@typing_extensions.final
 class ResponseEndBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_UPDATES_FIELD_NUMBER: builtins.int
     CONSENSUS_PARAM_UPDATES_FIELD_NUMBER: builtins.int
     EVENTS_FIELD_NUMBER: builtins.int
     @property
@@ -756,14 +784,15 @@
         events: collections.abc.Iterable[global___Event] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["consensus_param_updates", b"consensus_param_updates"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["consensus_param_updates", b"consensus_param_updates", "events", b"events", "validator_updates", b"validator_updates"]) -> None: ...
 
 global___ResponseEndBlock = ResponseEndBlock
 
+@typing_extensions.final
 class ResponseCommit(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     RETAIN_HEIGHT_FIELD_NUMBER: builtins.int
     data: builtins.bytes
     """reserve 1"""
@@ -774,14 +803,15 @@
         data: builtins.bytes = ...,
         retain_height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "retain_height", b"retain_height"]) -> None: ...
 
 global___ResponseCommit = ResponseCommit
 
+@typing_extensions.final
 class ResponseListSnapshots(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SNAPSHOTS_FIELD_NUMBER: builtins.int
     @property
     def snapshots(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Snapshot]: ...
     def __init__(
@@ -789,14 +819,15 @@
         *,
         snapshots: collections.abc.Iterable[global___Snapshot] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["snapshots", b"snapshots"]) -> None: ...
 
 global___ResponseListSnapshots = ResponseListSnapshots
 
+@typing_extensions.final
 class ResponseOfferSnapshot(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Result:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -836,28 +867,30 @@
         *,
         result: global___ResponseOfferSnapshot.Result.ValueType = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
 
 global___ResponseOfferSnapshot = ResponseOfferSnapshot
 
+@typing_extensions.final
 class ResponseLoadSnapshotChunk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHUNK_FIELD_NUMBER: builtins.int
     chunk: builtins.bytes
     def __init__(
         self,
         *,
         chunk: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["chunk", b"chunk"]) -> None: ...
 
 global___ResponseLoadSnapshotChunk = ResponseLoadSnapshotChunk
 
+@typing_extensions.final
 class ResponseApplySnapshotChunk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Result:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -907,14 +940,15 @@
         refetch_chunks: collections.abc.Iterable[builtins.int] | None = ...,
         reject_senders: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["refetch_chunks", b"refetch_chunks", "reject_senders", b"reject_senders", "result", b"result"]) -> None: ...
 
 global___ResponseApplySnapshotChunk = ResponseApplySnapshotChunk
 
+@typing_extensions.final
 class ConsensusParams(google.protobuf.message.Message):
     """----------------------------------------
     Misc.
 
     ConsensusParams contains all consensus-relevant parameters
     that can be adjusted by the abci app
     """
@@ -942,14 +976,15 @@
         version: tendermint.types.params_pb2.VersionParams | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block", b"block", "evidence", b"evidence", "validator", b"validator", "version", b"version"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block", b"block", "evidence", b"evidence", "validator", b"validator", "version", b"version"]) -> None: ...
 
 global___ConsensusParams = ConsensusParams
 
+@typing_extensions.final
 class BlockParams(google.protobuf.message.Message):
     """BlockParams contains limits on the block size."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_BYTES_FIELD_NUMBER: builtins.int
     MAX_GAS_FIELD_NUMBER: builtins.int
@@ -963,14 +998,15 @@
         max_bytes: builtins.int = ...,
         max_gas: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["max_bytes", b"max_bytes", "max_gas", b"max_gas"]) -> None: ...
 
 global___BlockParams = BlockParams
 
+@typing_extensions.final
 class LastCommitInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ROUND_FIELD_NUMBER: builtins.int
     VOTES_FIELD_NUMBER: builtins.int
     round: builtins.int
     @property
@@ -981,14 +1017,15 @@
         round: builtins.int = ...,
         votes: collections.abc.Iterable[global___VoteInfo] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["round", b"round", "votes", b"votes"]) -> None: ...
 
 global___LastCommitInfo = LastCommitInfo
 
+@typing_extensions.final
 class Event(google.protobuf.message.Message):
     """Event allows application developers to attach additional information to
     ResponseBeginBlock, ResponseEndBlock, ResponseCheckTx and ResponseDeliverTx.
     Later, transactions may be queried using these events.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -1004,14 +1041,15 @@
         type: builtins.str = ...,
         attributes: collections.abc.Iterable[global___EventAttribute] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["attributes", b"attributes", "type", b"type"]) -> None: ...
 
 global___Event = Event
 
+@typing_extensions.final
 class EventAttribute(google.protobuf.message.Message):
     """EventAttribute is a single key-value pair, associated with an event."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
@@ -1027,14 +1065,15 @@
         value: builtins.bytes = ...,
         index: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["index", b"index", "key", b"key", "value", b"value"]) -> None: ...
 
 global___EventAttribute = EventAttribute
 
+@typing_extensions.final
 class TxResult(google.protobuf.message.Message):
     """TxResult contains results of executing the transaction.
 
     One usage is indexing transaction results.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -1057,14 +1096,15 @@
         result: global___ResponseDeliverTx | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["result", b"result"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "index", b"index", "result", b"result", "tx", b"tx"]) -> None: ...
 
 global___TxResult = TxResult
 
+@typing_extensions.final
 class Validator(google.protobuf.message.Message):
     """----------------------------------------
     Blockchain Types
 
     Validator
     """
 
@@ -1084,14 +1124,15 @@
         address: builtins.bytes = ...,
         power: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "power", b"power"]) -> None: ...
 
 global___Validator = Validator
 
+@typing_extensions.final
 class ValidatorUpdate(google.protobuf.message.Message):
     """ValidatorUpdate"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PUB_KEY_FIELD_NUMBER: builtins.int
     POWER_FIELD_NUMBER: builtins.int
@@ -1105,14 +1146,15 @@
         power: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pub_key", b"pub_key"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["power", b"power", "pub_key", b"pub_key"]) -> None: ...
 
 global___ValidatorUpdate = ValidatorUpdate
 
+@typing_extensions.final
 class VoteInfo(google.protobuf.message.Message):
     """VoteInfo"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATOR_FIELD_NUMBER: builtins.int
     SIGNED_LAST_BLOCK_FIELD_NUMBER: builtins.int
@@ -1126,14 +1168,15 @@
         signed_last_block: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["validator", b"validator"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["signed_last_block", b"signed_last_block", "validator", b"validator"]) -> None: ...
 
 global___VoteInfo = VoteInfo
 
+@typing_extensions.final
 class Evidence(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_FIELD_NUMBER: builtins.int
     VALIDATOR_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
     TIME_FIELD_NUMBER: builtins.int
@@ -1162,14 +1205,15 @@
         total_voting_power: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["time", b"time", "validator", b"validator"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "time", b"time", "total_voting_power", b"total_voting_power", "type", b"type", "validator", b"validator"]) -> None: ...
 
 global___Evidence = Evidence
 
+@typing_extensions.final
 class Snapshot(google.protobuf.message.Message):
     """----------------------------------------
     State Sync Types
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/abci/types_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/keys_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/keys_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class PublicKey(google.protobuf.message.Message):
     """PublicKey defines the keys available for use with Tendermint Validators"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ED25519_FIELD_NUMBER: builtins.int
     SECP256K1_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/crypto/proof_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/crypto/proof_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Proof(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_FIELD_NUMBER: builtins.int
     INDEX_FIELD_NUMBER: builtins.int
     LEAF_HASH_FIELD_NUMBER: builtins.int
     AUNTS_FIELD_NUMBER: builtins.int
@@ -36,14 +37,15 @@
         leaf_hash: builtins.bytes = ...,
         aunts: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["aunts", b"aunts", "index", b"index", "leaf_hash", b"leaf_hash", "total", b"total"]) -> None: ...
 
 global___Proof = Proof
 
+@typing_extensions.final
 class ValueOp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     PROOF_FIELD_NUMBER: builtins.int
     key: builtins.bytes
     """Encoded in ProofOp.Key."""
@@ -57,14 +59,15 @@
         proof: global___Proof | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["proof", b"proof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "proof", b"proof"]) -> None: ...
 
 global___ValueOp = ValueOp
 
+@typing_extensions.final
 class DominoOp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     INPUT_FIELD_NUMBER: builtins.int
     OUTPUT_FIELD_NUMBER: builtins.int
     key: builtins.str
@@ -77,14 +80,15 @@
         input: builtins.str = ...,
         output: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["input", b"input", "key", b"key", "output", b"output"]) -> None: ...
 
 global___DominoOp = DominoOp
 
+@typing_extensions.final
 class ProofOp(google.protobuf.message.Message):
     """ProofOp defines an operation used for calculating Merkle root
     The data could be arbitrary format, providing nessecary data
     for example neighbouring node hash
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -102,14 +106,15 @@
         key: builtins.bytes = ...,
         data: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "key", b"key", "type", b"type"]) -> None: ...
 
 global___ProofOp = ProofOp
 
+@typing_extensions.final
 class ProofOps(google.protobuf.message.Message):
     """ProofOps is Merkle proof defined by the list of ProofOps"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPS_FIELD_NUMBER: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/libs/bits/types_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/libs/bits/types_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class BitArray(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BITS_FIELD_NUMBER: builtins.int
     ELEMS_FIELD_NUMBER: builtins.int
     bits: builtins.int
     @property
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/p2p/types_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/p2p/types_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class NetAddress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     IP_FIELD_NUMBER: builtins.int
     PORT_FIELD_NUMBER: builtins.int
     id: builtins.str
@@ -30,14 +31,15 @@
         ip: builtins.str = ...,
         port: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "ip", b"ip", "port", b"port"]) -> None: ...
 
 global___NetAddress = NetAddress
 
+@typing_extensions.final
 class ProtocolVersion(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     P2P_FIELD_NUMBER: builtins.int
     BLOCK_FIELD_NUMBER: builtins.int
     APP_FIELD_NUMBER: builtins.int
     p2p: builtins.int
@@ -50,14 +52,15 @@
         block: builtins.int = ...,
         app: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["app", b"app", "block", b"block", "p2p", b"p2p"]) -> None: ...
 
 global___ProtocolVersion = ProtocolVersion
 
+@typing_extensions.final
 class DefaultNodeInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PROTOCOL_VERSION_FIELD_NUMBER: builtins.int
     DEFAULT_NODE_ID_FIELD_NUMBER: builtins.int
     LISTEN_ADDR_FIELD_NUMBER: builtins.int
     NETWORK_FIELD_NUMBER: builtins.int
@@ -88,14 +91,15 @@
         other: global___DefaultNodeInfoOther | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["other", b"other", "protocol_version", b"protocol_version"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["channels", b"channels", "default_node_id", b"default_node_id", "listen_addr", b"listen_addr", "moniker", b"moniker", "network", b"network", "other", b"other", "protocol_version", b"protocol_version", "version", b"version"]) -> None: ...
 
 global___DefaultNodeInfo = DefaultNodeInfo
 
+@typing_extensions.final
 class DefaultNodeInfoOther(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TX_INDEX_FIELD_NUMBER: builtins.int
     RPC_ADDRESS_FIELD_NUMBER: builtins.int
     tx_index: builtins.str
     rpc_address: builtins.str
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/block_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/block_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Block(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEADER_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     EVIDENCE_FIELD_NUMBER: builtins.int
     LAST_COMMIT_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/evidence_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/evidence_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class Evidence(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DUPLICATE_VOTE_EVIDENCE_FIELD_NUMBER: builtins.int
     LIGHT_CLIENT_ATTACK_EVIDENCE_FIELD_NUMBER: builtins.int
     @property
     def duplicate_vote_evidence(self) -> global___DuplicateVoteEvidence: ...
@@ -36,14 +37,15 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["duplicate_vote_evidence", b"duplicate_vote_evidence", "light_client_attack_evidence", b"light_client_attack_evidence", "sum", b"sum"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["duplicate_vote_evidence", b"duplicate_vote_evidence", "light_client_attack_evidence", b"light_client_attack_evidence", "sum", b"sum"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["sum", b"sum"]) -> typing_extensions.Literal["duplicate_vote_evidence", "light_client_attack_evidence"] | None: ...
 
 global___Evidence = Evidence
 
+@typing_extensions.final
 class DuplicateVoteEvidence(google.protobuf.message.Message):
     """DuplicateVoteEvidence contains evidence of a validator signed two conflicting votes."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VOTE_A_FIELD_NUMBER: builtins.int
     VOTE_B_FIELD_NUMBER: builtins.int
@@ -68,14 +70,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp", "vote_a", b"vote_a", "vote_b", b"vote_b"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp", "total_voting_power", b"total_voting_power", "validator_power", b"validator_power", "vote_a", b"vote_a", "vote_b", b"vote_b"]) -> None: ...
 
 global___DuplicateVoteEvidence = DuplicateVoteEvidence
 
+@typing_extensions.final
 class LightClientAttackEvidence(google.protobuf.message.Message):
     """LightClientAttackEvidence contains evidence of a set of validators attempting to mislead a light client."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFLICTING_BLOCK_FIELD_NUMBER: builtins.int
     COMMON_HEIGHT_FIELD_NUMBER: builtins.int
@@ -100,14 +103,15 @@
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["conflicting_block", b"conflicting_block", "timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["byzantine_validators", b"byzantine_validators", "common_height", b"common_height", "conflicting_block", b"conflicting_block", "timestamp", b"timestamp", "total_voting_power", b"total_voting_power"]) -> None: ...
 
 global___LightClientAttackEvidence = LightClientAttackEvidence
 
+@typing_extensions.final
 class EvidenceList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EVIDENCE_FIELD_NUMBER: builtins.int
     @property
     def evidence(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Evidence]: ...
     def __init__(
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/params_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/params_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ConsensusParams(google.protobuf.message.Message):
     """ConsensusParams contains consensus critical parameters that determine the
     validity of blocks.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -45,14 +46,15 @@
         version: global___VersionParams | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block", b"block", "evidence", b"evidence", "validator", b"validator", "version", b"version"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block", b"block", "evidence", b"evidence", "validator", b"validator", "version", b"version"]) -> None: ...
 
 global___ConsensusParams = ConsensusParams
 
+@typing_extensions.final
 class BlockParams(google.protobuf.message.Message):
     """BlockParams contains limits on the block size."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_BYTES_FIELD_NUMBER: builtins.int
     MAX_GAS_FIELD_NUMBER: builtins.int
@@ -78,14 +80,15 @@
         max_gas: builtins.int = ...,
         time_iota_ms: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["max_bytes", b"max_bytes", "max_gas", b"max_gas", "time_iota_ms", b"time_iota_ms"]) -> None: ...
 
 global___BlockParams = BlockParams
 
+@typing_extensions.final
 class EvidenceParams(google.protobuf.message.Message):
     """EvidenceParams determine how we handle evidence of malfeasance."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_AGE_NUM_BLOCKS_FIELD_NUMBER: builtins.int
     MAX_AGE_DURATION_FIELD_NUMBER: builtins.int
@@ -117,14 +120,15 @@
         max_bytes: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["max_age_duration", b"max_age_duration"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["max_age_duration", b"max_age_duration", "max_age_num_blocks", b"max_age_num_blocks", "max_bytes", b"max_bytes"]) -> None: ...
 
 global___EvidenceParams = EvidenceParams
 
+@typing_extensions.final
 class ValidatorParams(google.protobuf.message.Message):
     """ValidatorParams restrict the public key types validators can use.
     NOTE: uses ABCI pubkey naming, not Amino names.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -136,14 +140,15 @@
         *,
         pub_key_types: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["pub_key_types", b"pub_key_types"]) -> None: ...
 
 global___ValidatorParams = ValidatorParams
 
+@typing_extensions.final
 class VersionParams(google.protobuf.message.Message):
     """VersionParams contains the ABCI application version."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APP_VERSION_FIELD_NUMBER: builtins.int
     app_version: builtins.int
@@ -152,14 +157,15 @@
         *,
         app_version: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_version", b"app_version"]) -> None: ...
 
 global___VersionParams = VersionParams
 
+@typing_extensions.final
 class HashedParams(google.protobuf.message.Message):
     """HashedParams is a subset of ConsensusParams.
 
     It is hashed into the Header.ConsensusHash.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/types_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/types_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _BlockIDFlag:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _BlockIDFlagEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BlockIDFlag.ValueType], builtins.type):  # noqa: F821
+class _BlockIDFlagEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_BlockIDFlag.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     BLOCK_ID_FLAG_UNKNOWN: _BlockIDFlag.ValueType  # 0
     BLOCK_ID_FLAG_ABSENT: _BlockIDFlag.ValueType  # 1
     BLOCK_ID_FLAG_COMMIT: _BlockIDFlag.ValueType  # 2
     BLOCK_ID_FLAG_NIL: _BlockIDFlag.ValueType  # 3
 
 class BlockIDFlag(_BlockIDFlag, metaclass=_BlockIDFlagEnumTypeWrapper):
@@ -42,15 +42,15 @@
 BLOCK_ID_FLAG_NIL: BlockIDFlag.ValueType  # 3
 global___BlockIDFlag = BlockIDFlag
 
 class _SignedMsgType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _SignedMsgTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignedMsgType.ValueType], builtins.type):  # noqa: F821
+class _SignedMsgTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SignedMsgType.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SIGNED_MSG_TYPE_UNKNOWN: _SignedMsgType.ValueType  # 0
     SIGNED_MSG_TYPE_PREVOTE: _SignedMsgType.ValueType  # 1
     """Votes"""
     SIGNED_MSG_TYPE_PRECOMMIT: _SignedMsgType.ValueType  # 2
     SIGNED_MSG_TYPE_PROPOSAL: _SignedMsgType.ValueType  # 32
     """Proposals"""
@@ -62,14 +62,15 @@
 SIGNED_MSG_TYPE_PREVOTE: SignedMsgType.ValueType  # 1
 """Votes"""
 SIGNED_MSG_TYPE_PRECOMMIT: SignedMsgType.ValueType  # 2
 SIGNED_MSG_TYPE_PROPOSAL: SignedMsgType.ValueType  # 32
 """Proposals"""
 global___SignedMsgType = SignedMsgType
 
+@typing_extensions.final
 class PartSetHeader(google.protobuf.message.Message):
     """PartsetHeader"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
@@ -81,14 +82,15 @@
         total: builtins.int = ...,
         hash: builtins.bytes = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["hash", b"hash", "total", b"total"]) -> None: ...
 
 global___PartSetHeader = PartSetHeader
 
+@typing_extensions.final
 class Part(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INDEX_FIELD_NUMBER: builtins.int
     BYTES_FIELD_NUMBER: builtins.int
     PROOF_FIELD_NUMBER: builtins.int
     index: builtins.int
@@ -103,14 +105,15 @@
         proof: tendermint.crypto.proof_pb2.Proof | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["proof", b"proof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["bytes", b"bytes", "index", b"index", "proof", b"proof"]) -> None: ...
 
 global___Part = Part
 
+@typing_extensions.final
 class BlockID(google.protobuf.message.Message):
     """BlockID"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HASH_FIELD_NUMBER: builtins.int
     PART_SET_HEADER_FIELD_NUMBER: builtins.int
@@ -124,14 +127,15 @@
         part_set_header: global___PartSetHeader | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["part_set_header", b"part_set_header"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["hash", b"hash", "part_set_header", b"part_set_header"]) -> None: ...
 
 global___BlockID = BlockID
 
+@typing_extensions.final
 class Header(google.protobuf.message.Message):
     """--------------------------------
 
     Header defines the structure of a Tendermint block header.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -203,14 +207,15 @@
         proposer_address: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["last_block_id", b"last_block_id", "time", b"time", "version", b"version"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["app_hash", b"app_hash", "chain_id", b"chain_id", "consensus_hash", b"consensus_hash", "data_hash", b"data_hash", "evidence_hash", b"evidence_hash", "height", b"height", "last_block_id", b"last_block_id", "last_commit_hash", b"last_commit_hash", "last_results_hash", b"last_results_hash", "next_validators_hash", b"next_validators_hash", "proposer_address", b"proposer_address", "time", b"time", "validators_hash", b"validators_hash", "version", b"version"]) -> None: ...
 
 global___Header = Header
 
+@typing_extensions.final
 class Data(google.protobuf.message.Message):
     """Data contains the set of transactions included in the block"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TXS_FIELD_NUMBER: builtins.int
     @property
@@ -224,14 +229,15 @@
         *,
         txs: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["txs", b"txs"]) -> None: ...
 
 global___Data = Data
 
+@typing_extensions.final
 class Vote(google.protobuf.message.Message):
     """Vote represents a prevote, precommit, or commit vote from validators for
     consensus.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -267,14 +273,15 @@
         signature: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "height", b"height", "round", b"round", "signature", b"signature", "timestamp", b"timestamp", "type", b"type", "validator_address", b"validator_address", "validator_index", b"validator_index"]) -> None: ...
 
 global___Vote = Vote
 
+@typing_extensions.final
 class Commit(google.protobuf.message.Message):
     """Commit contains the evidence that a block was committed by a set of validators."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEIGHT_FIELD_NUMBER: builtins.int
     ROUND_FIELD_NUMBER: builtins.int
@@ -295,14 +302,15 @@
         signatures: collections.abc.Iterable[global___CommitSig] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block_id", b"block_id"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "height", b"height", "round", b"round", "signatures", b"signatures"]) -> None: ...
 
 global___Commit = Commit
 
+@typing_extensions.final
 class CommitSig(google.protobuf.message.Message):
     """CommitSig is a part of the Vote included in a Commit."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_ID_FLAG_FIELD_NUMBER: builtins.int
     VALIDATOR_ADDRESS_FIELD_NUMBER: builtins.int
@@ -322,14 +330,15 @@
         signature: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_id_flag", b"block_id_flag", "signature", b"signature", "timestamp", b"timestamp", "validator_address", b"validator_address"]) -> None: ...
 
 global___CommitSig = CommitSig
 
+@typing_extensions.final
 class Proposal(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
     ROUND_FIELD_NUMBER: builtins.int
     POL_ROUND_FIELD_NUMBER: builtins.int
@@ -357,14 +366,15 @@
         signature: builtins.bytes = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "timestamp", b"timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "height", b"height", "pol_round", b"pol_round", "round", b"round", "signature", b"signature", "timestamp", b"timestamp", "type", b"type"]) -> None: ...
 
 global___Proposal = Proposal
 
+@typing_extensions.final
 class SignedHeader(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEADER_FIELD_NUMBER: builtins.int
     COMMIT_FIELD_NUMBER: builtins.int
     @property
     def header(self) -> global___Header: ...
@@ -377,14 +387,15 @@
         commit: global___Commit | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["commit", b"commit", "header", b"header"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["commit", b"commit", "header", b"header"]) -> None: ...
 
 global___SignedHeader = SignedHeader
 
+@typing_extensions.final
 class LightBlock(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SIGNED_HEADER_FIELD_NUMBER: builtins.int
     VALIDATOR_SET_FIELD_NUMBER: builtins.int
     @property
     def signed_header(self) -> global___SignedHeader: ...
@@ -397,14 +408,15 @@
         validator_set: tendermint.types.validator_pb2.ValidatorSet | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["signed_header", b"signed_header", "validator_set", b"validator_set"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["signed_header", b"signed_header", "validator_set", b"validator_set"]) -> None: ...
 
 global___LightBlock = LightBlock
 
+@typing_extensions.final
 class BlockMeta(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BLOCK_ID_FIELD_NUMBER: builtins.int
     BLOCK_SIZE_FIELD_NUMBER: builtins.int
     HEADER_FIELD_NUMBER: builtins.int
     NUM_TXS_FIELD_NUMBER: builtins.int
@@ -423,14 +435,15 @@
         num_txs: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "header", b"header"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["block_id", b"block_id", "block_size", b"block_size", "header", b"header", "num_txs", b"num_txs"]) -> None: ...
 
 global___BlockMeta = BlockMeta
 
+@typing_extensions.final
 class TxProof(google.protobuf.message.Message):
     """TxProof represents a Merkle proof of the presence of a transaction in the Merkle tree."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ROOT_HASH_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/types/validator_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/types/validator_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class ValidatorSet(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALIDATORS_FIELD_NUMBER: builtins.int
     PROPOSER_FIELD_NUMBER: builtins.int
     TOTAL_VOTING_POWER_FIELD_NUMBER: builtins.int
     @property
@@ -36,14 +37,15 @@
         total_voting_power: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["proposer", b"proposer"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["proposer", b"proposer", "total_voting_power", b"total_voting_power", "validators", b"validators"]) -> None: ...
 
 global___ValidatorSet = ValidatorSet
 
+@typing_extensions.final
 class Validator(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     PUB_KEY_FIELD_NUMBER: builtins.int
     VOTING_POWER_FIELD_NUMBER: builtins.int
     PROPOSER_PRIORITY_FIELD_NUMBER: builtins.int
@@ -61,14 +63,15 @@
         proposer_priority: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["pub_key", b"pub_key"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["address", b"address", "proposer_priority", b"proposer_priority", "pub_key", b"pub_key", "voting_power", b"voting_power"]) -> None: ...
 
 global___Validator = Validator
 
+@typing_extensions.final
 class SimpleValidator(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PUB_KEY_FIELD_NUMBER: builtins.int
     VOTING_POWER_FIELD_NUMBER: builtins.int
     @property
     def pub_key(self) -> tendermint.crypto.keys_pb2.PublicKey: ...
```

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2.py` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosis_proto/proto/tendermint/version/types_pb2.pyi` & `osmosispy-0.0.9/osmosis_proto/proto/tendermint/version/types_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+@typing_extensions.final
 class App(google.protobuf.message.Message):
     """App includes the protocol and software version for the application.
     This information is included in ResponseInfo. The App.Protocol can be
     updated in ResponseEndBlock.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -32,14 +33,15 @@
         protocol: builtins.int = ...,
         software: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["protocol", b"protocol", "software", b"software"]) -> None: ...
 
 global___App = App
 
+@typing_extensions.final
 class Consensus(google.protobuf.message.Message):
     """Consensus captures the consensus rules for processing a block in the blockchain,
     including all blockchain data structures and the rules of the application's
     state transition machine.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `osmosispy-0.0.8/osmosispy/__init__.py` & `osmosispy-0.0.9/osmosispy/__init__.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/grpc_client.py` & `osmosispy-0.0.9/osmosispy/grpc_client.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/pytypes/common.py` & `osmosispy-0.0.9/osmosispy/pytypes/common.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/pytypes/event.py` & `osmosispy-0.0.9/osmosispy/pytypes/event.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/pytypes/network.py` & `osmosispy-0.0.9/osmosispy/pytypes/network.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/pytypes/tx_resp.py` & `osmosispy-0.0.9/osmosispy/pytypes/tx_resp.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/sdk.py` & `osmosispy-0.0.9/osmosispy/sdk.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/trading_client/binance.py` & `osmosispy-0.0.9/osmosispy/trading_client/binance.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/trading_client/client.py` & `osmosispy-0.0.9/osmosispy/trading_client/client.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/trading_client/osmosis.py` & `osmosispy-0.0.9/osmosispy/trading_client/osmosis.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/tx.py` & `osmosispy-0.0.9/osmosispy/tx.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/utils.py` & `osmosispy-0.0.9/osmosispy/utils.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/osmosispy/wallet.py` & `osmosispy-0.0.9/osmosispy/wallet.py`

 * *Files identical despite different names*

### Comparing `osmosispy-0.0.8/pyproject.toml` & `osmosispy-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "osmosispy"
-version = "0.0.8"
+version = "0.0.9"
 description = "Osmosis Python SDK"
 packages = [
     { include = "osmosispy" },
     { include = "osmosis_proto" },
 ]
 authors = ["sbneo2022"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "3.11.2"
 grpcio = "1.51.1"
 grpcio-tools = "1.51.1"
 protobuf = "4.21.12"
 types-protobuf = "4.21.0.2"
 mypy-protobuf = "3.4.0"
 bech32 = "1.2.0"
 asyncio = "3.4.3"
```

### Comparing `osmosispy-0.0.8/PKG-INFO` & `osmosispy-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: osmosispy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Osmosis Python SDK
 License: MIT
 Author: sbneo2022
-Requires-Python: >=3.11,<4.0
+Requires-Python: ==3.11.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (==3.4.3)
 Requires-Dist: bech32 (==1.2.0)
 Requires-Dist: binance-connector (>=2.0.0,<3.0.0)
 Requires-Dist: bip32 (==3.4)
 Requires-Dist: ecdsa (==0.18.0)
 Requires-Dist: grpcio (==1.51.1)
 Requires-Dist: grpcio-tools (==1.51.1)
```

