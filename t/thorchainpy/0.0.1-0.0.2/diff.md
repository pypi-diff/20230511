# Comparing `tmp/thorchainpy-0.0.1.tar.gz` & `tmp/thorchainpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thorchainpy-0.0.1.tar", max compression
+gzip compressed data, was "thorchainpy-0.0.2.tar", max compression
```

## Comparing `thorchainpy-0.0.1.tar` & `thorchainpy-0.0.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
--rw-r--r--   0        0        0      656 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      156 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/__init__.py
--rw-r--r--   0        0        0       47 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/borrowers/__init__.py
--rw-r--r--   0        0        0     3365 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/borrowers/borrower.py
--rw-r--r--   0        0        0     4974 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/borrowers/borrowers.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/health/__init__.py
--rw-r--r--   0        0        0     3322 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/health/ping.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/invariants/__init__.py
--rw-r--r--   0        0        0     4784 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/invariants/invariant.py
--rw-r--r--   0        0        0     4345 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/invariants/invariants.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/liquidity_providers/__init__.py
--rw-r--r--   0        0        0     3397 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/liquidity_providers/liquidity_provider.py
--rw-r--r--   0        0        0     5294 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/liquidity_providers/liquidity_providers.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/__init__.py
--rw-r--r--   0        0        0     4291 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/mimir.py
--rw-r--r--   0        0        0     4293 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_admin.py
--rw-r--r--   0        0        0     4452 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_key.py
--rw-r--r--   0        0        0     4941 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_node.py
--rw-r--r--   0        0        0     4327 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_nodes.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/__init__.py
--rw-r--r--   0        0        0     4836 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/ban.py
--rw-r--r--   0        0        0     4411 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/constants.py
--rw-r--r--   0        0        0     4899 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/inbound_addresses.py
--rw-r--r--   0        0        0     4674 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/lastblock.py
--rw-r--r--   0        0        0     5039 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/lastblock_chain.py
--rw-r--r--   0        0        0     4291 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/network.py
--rw-r--r--   0        0        0     4221 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/ragnarok.py
--rw-r--r--   0        0        0     4643 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/network/version.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/nodes/__init__.py
--rw-r--r--   0        0        0     3161 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/nodes/node.py
--rw-r--r--   0        0        0     4574 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/nodes/nodes.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/pol/__init__.py
--rw-r--r--   0        0        0     4303 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/pol/pol.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/pools/__init__.py
--rw-r--r--   0        0        0     3059 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/pools/pool.py
--rw-r--r--   0        0        0     4530 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/pools/pools.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/queue/__init__.py
--rw-r--r--   0        0        0     4219 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/queue/queue.py
--rw-r--r--   0        0        0     4708 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/queue/queue_outbound.py
--rw-r--r--   0        0        0     4589 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/queue/queue_scheduled.py
--rw-r--r--   0        0        0     4541 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/queue/queue_swap.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/quote/__init__.py
--rw-r--r--   0        0        0     5688 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/quote/quotesaverdeposit.py
--rw-r--r--   0        0        0     6559 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/quote/quotesaverwithdraw.py
--rw-r--r--   0        0        0    10103 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/quote/quoteswap.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/savers/__init__.py
--rw-r--r--   0        0        0     3372 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/savers/saver.py
--rw-r--r--   0        0        0     4882 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/savers/savers.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/thornames/__init__.py
--rw-r--r--   0        0        0     4890 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/thornames/thorname.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/__init__.py
--rw-r--r--   0        0        0     4944 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/tx.py
--rw-r--r--   0        0        0     4992 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/tx_signers.py
--rw-r--r--   0        0        0     4936 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/tx_signers_old.py
--rw-r--r--   0        0        0     4972 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/tx_stages.py
--rw-r--r--   0        0        0     4928 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/transactions/tx_status.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/tss/__init__.py
--rw-r--r--   0        0        0     4385 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/tss/keysign.py
--rw-r--r--   0        0        0     5306 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/tss/keysign_pubkey.py
--rw-r--r--   0        0        0     4363 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/tss/metrics.py
--rw-r--r--   0        0        0     5434 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/tss/metrics_keygen.py
--rw-r--r--   0        0        0        0 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/vaults/__init__.py
--rw-r--r--   0        0        0     4499 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/vaults/asgard.py
--rw-r--r--   0        0        0     3212 2023-03-31 22:33:39.756862 thorchainpy-0.0.1/thorchainpy/api/vaults/vault.py
--rw-r--r--   0        0        0     4376 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/api/vaults/vault_pubkeys.py
--rw-r--r--   0        0        0     4514 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/api/vaults/yggdrasil.py
--rw-r--r--   0        0        0     2817 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/client.py
--rw-r--r--   0        0        0      470 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/errors.py
--rw-r--r--   0        0        0     5223 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/__init__.py
--rw-r--r--   0        0        0     2287 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/ban_response.py
--rw-r--r--   0        0        0     3059 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/borrower.py
--rw-r--r--   0        0        0     1846 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/coin.py
--rw-r--r--   0        0        0     4137 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/constants_response.py
--rw-r--r--   0        0        0     1295 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/constants_response_bool_values.py
--rw-r--r--   0        0        0     1287 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/constants_response_int_64_values.py
--rw-r--r--   0        0        0     1302 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/constants_response_string_values.py
--rw-r--r--   0        0        0     6485 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/inbound_address.py
--rw-r--r--   0        0        0     1929 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/invariant_response.py
--rw-r--r--   0        0        0     1684 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/invariants_response.py
--rw-r--r--   0        0        0     2447 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/keygen_metric.py
--rw-r--r--   0        0        0     1835 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/keygen_metric_node_keygen_metric.py
--rw-r--r--   0        0        0     2351 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/keysign_response.py
--rw-r--r--   0        0        0     2383 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/keysign_response_keysign_info.py
--rw-r--r--   0        0        0     2060 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/last_block.py
--rw-r--r--   0        0        0     6051 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/liquidity_provider.py
--rw-r--r--   0        0        0     4664 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/liquidity_provider_summary.py
--rw-r--r--   0        0        0     3260 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/metrics_response.py
--rw-r--r--   0        0        0     2576 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/metrics_response_keysign_metrics.py
--rw-r--r--   0        0        0     2216 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/mimir_nodes_response.py
--rw-r--r--   0        0        0     1998 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/mimir_nodes_response_mimir_vote.py
--rw-r--r--   0        0        0     1241 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/mimir_response.py
--rw-r--r--   0        0        0     5434 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/msg_swap.py
--rw-r--r--   0        0        0     4378 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/network_response.py
--rw-r--r--   0        0        0     8533 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node.py
--rw-r--r--   0        0        0     1583 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_chain_height.py
--rw-r--r--   0        0        0     2638 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_node_bond_providers.py
--rw-r--r--   0        0        0     1897 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_node_bond_providers_node_bond_provider.py
--rw-r--r--   0        0        0     1820 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_node_jail.py
--rw-r--r--   0        0        0     1850 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_node_preflight_status.py
--rw-r--r--   0        0        0     1989 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_node_pub_key_set.py
--rw-r--r--   0        0        0      219 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/node_status.py
--rw-r--r--   0        0        0     7359 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/observed_tx.py
--rw-r--r--   0        0        0      169 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/observed_tx_status.py
--rw-r--r--   0        0        0     1442 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/ping_ping.py
--rw-r--r--   0        0        0     2572 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/pol_response.py
--rw-r--r--   0        0        0     5718 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/pool.py
--rw-r--r--   0        0        0     2158 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/queue_response.py
--rw-r--r--   0        0        0     1779 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/quote_fees.py
--rw-r--r--   0        0        0     5883 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/quote_saver_deposit_response.py
--rw-r--r--   0        0        0     5505 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/quote_saver_withdraw_response.py
--rw-r--r--   0        0        0     6581 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/quote_swap_response.py
--rw-r--r--   0        0        0     3437 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/saver.py
--rw-r--r--   0        0        0     3106 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/thorname.py
--rw-r--r--   0        0        0     1787 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/thorname_alias.py
--rw-r--r--   0        0        0     2309 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tss_keysign_metric.py
--rw-r--r--   0        0        0     1731 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tss_metric.py
--rw-r--r--   0        0        0     3697 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx.py
--rw-r--r--   0        0        0     5186 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_details_response.py
--rw-r--r--   0        0        0     4289 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_out_item.py
--rw-r--r--   0        0        0     3677 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_response.py
--rw-r--r--   0        0        0     5186 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_signers_response.py
--rw-r--r--   0        0        0     6679 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response.py
--rw-r--r--   0        0        0     4335 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_confirmation_counted.py
--rw-r--r--   0        0        0     1610 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_finalised.py
--rw-r--r--   0        0        0     1932 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_observed.py
--rw-r--r--   0        0        0     2649 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_outbound_delay.py
--rw-r--r--   0        0        0     2695 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_outbound_signed.py
--rw-r--r--   0        0        0     1597 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_swap_finalised.py
--rw-r--r--   0        0        0     4079 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_status_response.py
--rw-r--r--   0        0        0     2267 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/tx_status_response_planned_out_txs_item.py
--rw-r--r--   0        0        0     6907 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault.py
--rw-r--r--   0        0        0     1782 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault_address.py
--rw-r--r--   0        0        0     2114 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault_info.py
--rw-r--r--   0        0        0     2429 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault_pubkeys_response.py
--rw-r--r--   0        0        0     1766 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault_router.py
--rw-r--r--   0        0        0      184 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/vault_type.py
--rw-r--r--   0        0        0     1822 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/models/version_response.py
--rw-r--r--   0        0        0       25 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/py.typed
--rw-r--r--   0        0        0      974 2023-03-31 22:33:39.760862 thorchainpy-0.0.1/thorchainpy/types.py
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 thorchainpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      656 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/borrowers/__init__.py
+-rw-r--r--   0        0        0     3365 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/borrowers/borrower.py
+-rw-r--r--   0        0        0     4974 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/borrowers/borrowers.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/health/__init__.py
+-rw-r--r--   0        0        0     3322 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/health/ping.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/invariants/__init__.py
+-rw-r--r--   0        0        0     4784 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/invariants/invariant.py
+-rw-r--r--   0        0        0     4345 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/invariants/invariants.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/liquidity_providers/__init__.py
+-rw-r--r--   0        0        0     3397 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/liquidity_providers/liquidity_provider.py
+-rw-r--r--   0        0        0     5294 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/liquidity_providers/liquidity_providers.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/__init__.py
+-rw-r--r--   0        0        0     4291 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/mimir.py
+-rw-r--r--   0        0        0     4293 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_admin.py
+-rw-r--r--   0        0        0     4452 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_key.py
+-rw-r--r--   0        0        0     4941 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_node.py
+-rw-r--r--   0        0        0     4327 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_nodes.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/__init__.py
+-rw-r--r--   0        0        0     4836 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/ban.py
+-rw-r--r--   0        0        0     4411 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/constants.py
+-rw-r--r--   0        0        0     4899 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/inbound_addresses.py
+-rw-r--r--   0        0        0     4674 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/lastblock.py
+-rw-r--r--   0        0        0     5039 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/lastblock_chain.py
+-rw-r--r--   0        0        0     4291 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/network.py
+-rw-r--r--   0        0        0     4221 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/ragnarok.py
+-rw-r--r--   0        0        0     4643 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/network/version.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/nodes/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/nodes/node.py
+-rw-r--r--   0        0        0     4574 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/nodes/nodes.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/pol/__init__.py
+-rw-r--r--   0        0        0     4303 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/pol/pol.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/pools/__init__.py
+-rw-r--r--   0        0        0     3059 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/pools/pool.py
+-rw-r--r--   0        0        0     4530 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/pools/pools.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/queue/__init__.py
+-rw-r--r--   0        0        0     4219 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/queue/queue.py
+-rw-r--r--   0        0        0     4708 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/queue/queue_outbound.py
+-rw-r--r--   0        0        0     4589 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/queue/queue_scheduled.py
+-rw-r--r--   0        0        0     4541 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/queue/queue_swap.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/quote/__init__.py
+-rw-r--r--   0        0        0     5688 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/quote/quotesaverdeposit.py
+-rw-r--r--   0        0        0     6559 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/quote/quotesaverwithdraw.py
+-rw-r--r--   0        0        0    10103 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/quote/quoteswap.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/savers/__init__.py
+-rw-r--r--   0        0        0     3372 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/savers/saver.py
+-rw-r--r--   0        0        0     4882 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/savers/savers.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/thornames/__init__.py
+-rw-r--r--   0        0        0     4890 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/thornames/thorname.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/tx.py
+-rw-r--r--   0        0        0     4992 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/tx_signers.py
+-rw-r--r--   0        0        0     4936 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/tx_signers_old.py
+-rw-r--r--   0        0        0     4972 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/tx_stages.py
+-rw-r--r--   0        0        0     4928 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/transactions/tx_status.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/tss/__init__.py
+-rw-r--r--   0        0        0     4385 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/tss/keysign.py
+-rw-r--r--   0        0        0     5306 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/tss/keysign_pubkey.py
+-rw-r--r--   0        0        0     4363 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/tss/metrics.py
+-rw-r--r--   0        0        0     5434 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/tss/metrics_keygen.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/vaults/__init__.py
+-rw-r--r--   0        0        0     4499 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/vaults/asgard.py
+-rw-r--r--   0        0        0     3212 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/vaults/vault.py
+-rw-r--r--   0        0        0     4376 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/vaults/vault_pubkeys.py
+-rw-r--r--   0        0        0     4514 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/api/vaults/yggdrasil.py
+-rw-r--r--   0        0        0     2817 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/client.py
+-rw-r--r--   0        0        0      470 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/errors.py
+-rw-r--r--   0        0        0     5223 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/__init__.py
+-rw-r--r--   0        0        0     2287 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/ban_response.py
+-rw-r--r--   0        0        0     3059 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/borrower.py
+-rw-r--r--   0        0        0     1846 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/coin.py
+-rw-r--r--   0        0        0     4137 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/constants_response.py
+-rw-r--r--   0        0        0     1295 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/constants_response_bool_values.py
+-rw-r--r--   0        0        0     1287 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/constants_response_int_64_values.py
+-rw-r--r--   0        0        0     1302 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/constants_response_string_values.py
+-rw-r--r--   0        0        0     6485 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/inbound_address.py
+-rw-r--r--   0        0        0     1929 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/invariant_response.py
+-rw-r--r--   0        0        0     1684 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/invariants_response.py
+-rw-r--r--   0        0        0     2447 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/keygen_metric.py
+-rw-r--r--   0        0        0     1835 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/keygen_metric_node_keygen_metric.py
+-rw-r--r--   0        0        0     2351 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/keysign_response.py
+-rw-r--r--   0        0        0     2383 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/keysign_response_keysign_info.py
+-rw-r--r--   0        0        0     2060 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/last_block.py
+-rw-r--r--   0        0        0     6051 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/liquidity_provider.py
+-rw-r--r--   0        0        0     4664 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/liquidity_provider_summary.py
+-rw-r--r--   0        0        0     3260 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/metrics_response.py
+-rw-r--r--   0        0        0     2576 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/metrics_response_keysign_metrics.py
+-rw-r--r--   0        0        0     2216 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/mimir_nodes_response.py
+-rw-r--r--   0        0        0     1998 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/mimir_nodes_response_mimir_vote.py
+-rw-r--r--   0        0        0     1241 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/mimir_response.py
+-rw-r--r--   0        0        0     5434 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/msg_swap.py
+-rw-r--r--   0        0        0     4378 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/network_response.py
+-rw-r--r--   0        0        0     8533 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/node.py
+-rw-r--r--   0        0        0     1583 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/node_chain_height.py
+-rw-r--r--   0        0        0     2638 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/node_node_bond_providers.py
+-rw-r--r--   0        0        0     1897 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/node_node_bond_providers_node_bond_provider.py
+-rw-r--r--   0        0        0     1820 2023-05-11 15:23:38.106665 thorchainpy-0.0.2/thorchainpy/models/node_node_jail.py
+-rw-r--r--   0        0        0     1850 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/node_node_preflight_status.py
+-rw-r--r--   0        0        0     1989 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/node_node_pub_key_set.py
+-rw-r--r--   0        0        0      219 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/node_status.py
+-rw-r--r--   0        0        0     7359 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/observed_tx.py
+-rw-r--r--   0        0        0      169 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/observed_tx_status.py
+-rw-r--r--   0        0        0     1442 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/ping_ping.py
+-rw-r--r--   0        0        0     2572 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/pol_response.py
+-rw-r--r--   0        0        0     5718 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/pool.py
+-rw-r--r--   0        0        0     2158 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/queue_response.py
+-rw-r--r--   0        0        0     1779 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/quote_fees.py
+-rw-r--r--   0        0        0     5883 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/quote_saver_deposit_response.py
+-rw-r--r--   0        0        0     5505 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/quote_saver_withdraw_response.py
+-rw-r--r--   0        0        0     6581 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/quote_swap_response.py
+-rw-r--r--   0        0        0     3437 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/saver.py
+-rw-r--r--   0        0        0     3106 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/thorname.py
+-rw-r--r--   0        0        0     1787 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/thorname_alias.py
+-rw-r--r--   0        0        0     2309 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tss_keysign_metric.py
+-rw-r--r--   0        0        0     1731 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tss_metric.py
+-rw-r--r--   0        0        0     3697 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx.py
+-rw-r--r--   0        0        0     5186 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_details_response.py
+-rw-r--r--   0        0        0     4289 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_out_item.py
+-rw-r--r--   0        0        0     3677 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_response.py
+-rw-r--r--   0        0        0     5186 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_signers_response.py
+-rw-r--r--   0        0        0     6679 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response.py
+-rw-r--r--   0        0        0     4335 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_confirmation_counted.py
+-rw-r--r--   0        0        0     1610 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_finalised.py
+-rw-r--r--   0        0        0     1932 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_observed.py
+-rw-r--r--   0        0        0     2649 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_outbound_delay.py
+-rw-r--r--   0        0        0     2695 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_outbound_signed.py
+-rw-r--r--   0        0        0     1597 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_swap_finalised.py
+-rw-r--r--   0        0        0     4079 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_status_response.py
+-rw-r--r--   0        0        0     2267 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/tx_status_response_planned_out_txs_item.py
+-rw-r--r--   0        0        0     6907 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault.py
+-rw-r--r--   0        0        0     1782 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault_address.py
+-rw-r--r--   0        0        0     2114 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault_info.py
+-rw-r--r--   0        0        0     2429 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault_pubkeys_response.py
+-rw-r--r--   0        0        0     1766 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault_router.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/vault_type.py
+-rw-r--r--   0        0        0     1822 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/models/version_response.py
+-rw-r--r--   0        0        0       25 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/py.typed
+-rw-r--r--   0        0        0      974 2023-05-11 15:23:38.110664 thorchainpy-0.0.2/thorchainpy/types.py
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 thorchainpy-0.0.2/PKG-INFO
```

### Comparing `thorchainpy-0.0.1/pyproject.toml` & `thorchainpy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thorchainpy"
-version = "0.0.1"
+version = "0.0.2"
 description = "Thorchain Python SDK"
 packages = [
     { include = "thorchainpy" },
 ]
 authors = ["sbneo2022"]
 license = "MIT"
```

### Comparing `thorchainpy-0.0.1/thorchainpy/api/borrowers/borrower.py` & `thorchainpy-0.0.2/thorchainpy/api/borrowers/borrower.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/borrowers/borrowers.py` & `thorchainpy-0.0.2/thorchainpy/api/borrowers/borrowers.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/health/ping.py` & `thorchainpy-0.0.2/thorchainpy/api/health/ping.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/invariants/invariant.py` & `thorchainpy-0.0.2/thorchainpy/api/invariants/invariant.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/invariants/invariants.py` & `thorchainpy-0.0.2/thorchainpy/api/invariants/invariants.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/liquidity_providers/liquidity_provider.py` & `thorchainpy-0.0.2/thorchainpy/api/liquidity_providers/liquidity_provider.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/liquidity_providers/liquidity_providers.py` & `thorchainpy-0.0.2/thorchainpy/api/liquidity_providers/liquidity_providers.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/mimir/mimir.py` & `thorchainpy-0.0.2/thorchainpy/api/mimir/mimir.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_admin.py` & `thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_admin.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_key.py` & `thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_key.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_node.py` & `thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_node.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/mimir/mimir_nodes.py` & `thorchainpy-0.0.2/thorchainpy/api/mimir/mimir_nodes.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/ban.py` & `thorchainpy-0.0.2/thorchainpy/api/network/ban.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/constants.py` & `thorchainpy-0.0.2/thorchainpy/api/network/constants.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/inbound_addresses.py` & `thorchainpy-0.0.2/thorchainpy/api/network/inbound_addresses.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/lastblock.py` & `thorchainpy-0.0.2/thorchainpy/api/network/lastblock.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/lastblock_chain.py` & `thorchainpy-0.0.2/thorchainpy/api/network/lastblock_chain.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/network.py` & `thorchainpy-0.0.2/thorchainpy/api/network/network.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/ragnarok.py` & `thorchainpy-0.0.2/thorchainpy/api/network/ragnarok.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/network/version.py` & `thorchainpy-0.0.2/thorchainpy/api/network/version.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/nodes/node.py` & `thorchainpy-0.0.2/thorchainpy/api/nodes/node.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/nodes/nodes.py` & `thorchainpy-0.0.2/thorchainpy/api/nodes/nodes.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/pol/pol.py` & `thorchainpy-0.0.2/thorchainpy/api/pol/pol.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/pools/pool.py` & `thorchainpy-0.0.2/thorchainpy/api/pools/pool.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/pools/pools.py` & `thorchainpy-0.0.2/thorchainpy/api/pools/pools.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/queue/queue.py` & `thorchainpy-0.0.2/thorchainpy/api/queue/queue.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/queue/queue_outbound.py` & `thorchainpy-0.0.2/thorchainpy/api/queue/queue_outbound.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/queue/queue_scheduled.py` & `thorchainpy-0.0.2/thorchainpy/api/queue/queue_scheduled.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/queue/queue_swap.py` & `thorchainpy-0.0.2/thorchainpy/api/queue/queue_swap.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/quote/quotesaverdeposit.py` & `thorchainpy-0.0.2/thorchainpy/api/quote/quotesaverdeposit.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/quote/quotesaverwithdraw.py` & `thorchainpy-0.0.2/thorchainpy/api/quote/quotesaverwithdraw.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/quote/quoteswap.py` & `thorchainpy-0.0.2/thorchainpy/api/quote/quoteswap.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/savers/saver.py` & `thorchainpy-0.0.2/thorchainpy/api/savers/saver.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/savers/savers.py` & `thorchainpy-0.0.2/thorchainpy/api/savers/savers.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/thornames/thorname.py` & `thorchainpy-0.0.2/thorchainpy/api/thornames/thorname.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/transactions/tx.py` & `thorchainpy-0.0.2/thorchainpy/api/transactions/tx.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/transactions/tx_signers.py` & `thorchainpy-0.0.2/thorchainpy/api/transactions/tx_signers.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/transactions/tx_signers_old.py` & `thorchainpy-0.0.2/thorchainpy/api/transactions/tx_signers_old.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/transactions/tx_stages.py` & `thorchainpy-0.0.2/thorchainpy/api/transactions/tx_stages.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/transactions/tx_status.py` & `thorchainpy-0.0.2/thorchainpy/api/transactions/tx_status.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/tss/keysign.py` & `thorchainpy-0.0.2/thorchainpy/api/tss/keysign.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/tss/keysign_pubkey.py` & `thorchainpy-0.0.2/thorchainpy/api/tss/keysign_pubkey.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/tss/metrics.py` & `thorchainpy-0.0.2/thorchainpy/api/tss/metrics.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/tss/metrics_keygen.py` & `thorchainpy-0.0.2/thorchainpy/api/tss/metrics_keygen.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/vaults/asgard.py` & `thorchainpy-0.0.2/thorchainpy/api/vaults/asgard.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/vaults/vault.py` & `thorchainpy-0.0.2/thorchainpy/api/vaults/vault.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/vaults/vault_pubkeys.py` & `thorchainpy-0.0.2/thorchainpy/api/vaults/vault_pubkeys.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/api/vaults/yggdrasil.py` & `thorchainpy-0.0.2/thorchainpy/api/vaults/yggdrasil.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/client.py` & `thorchainpy-0.0.2/thorchainpy/client.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/__init__.py` & `thorchainpy-0.0.2/thorchainpy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/ban_response.py` & `thorchainpy-0.0.2/thorchainpy/models/ban_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/borrower.py` & `thorchainpy-0.0.2/thorchainpy/models/borrower.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/coin.py` & `thorchainpy-0.0.2/thorchainpy/models/coin.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/constants_response.py` & `thorchainpy-0.0.2/thorchainpy/models/constants_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/constants_response_bool_values.py` & `thorchainpy-0.0.2/thorchainpy/models/constants_response_bool_values.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/constants_response_int_64_values.py` & `thorchainpy-0.0.2/thorchainpy/models/constants_response_int_64_values.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/constants_response_string_values.py` & `thorchainpy-0.0.2/thorchainpy/models/constants_response_string_values.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/inbound_address.py` & `thorchainpy-0.0.2/thorchainpy/models/inbound_address.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/invariant_response.py` & `thorchainpy-0.0.2/thorchainpy/models/invariant_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/invariants_response.py` & `thorchainpy-0.0.2/thorchainpy/models/invariants_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/keygen_metric.py` & `thorchainpy-0.0.2/thorchainpy/models/keygen_metric.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/keygen_metric_node_keygen_metric.py` & `thorchainpy-0.0.2/thorchainpy/models/keygen_metric_node_keygen_metric.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/keysign_response.py` & `thorchainpy-0.0.2/thorchainpy/models/keysign_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/keysign_response_keysign_info.py` & `thorchainpy-0.0.2/thorchainpy/models/keysign_response_keysign_info.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/last_block.py` & `thorchainpy-0.0.2/thorchainpy/models/last_block.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/liquidity_provider.py` & `thorchainpy-0.0.2/thorchainpy/models/liquidity_provider.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/liquidity_provider_summary.py` & `thorchainpy-0.0.2/thorchainpy/models/liquidity_provider_summary.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/metrics_response.py` & `thorchainpy-0.0.2/thorchainpy/models/metrics_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/metrics_response_keysign_metrics.py` & `thorchainpy-0.0.2/thorchainpy/models/metrics_response_keysign_metrics.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/mimir_nodes_response.py` & `thorchainpy-0.0.2/thorchainpy/models/mimir_nodes_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/mimir_nodes_response_mimir_vote.py` & `thorchainpy-0.0.2/thorchainpy/models/mimir_nodes_response_mimir_vote.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/mimir_response.py` & `thorchainpy-0.0.2/thorchainpy/models/mimir_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/msg_swap.py` & `thorchainpy-0.0.2/thorchainpy/models/msg_swap.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/network_response.py` & `thorchainpy-0.0.2/thorchainpy/models/network_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node.py` & `thorchainpy-0.0.2/thorchainpy/models/node.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_chain_height.py` & `thorchainpy-0.0.2/thorchainpy/models/node_chain_height.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_node_bond_providers.py` & `thorchainpy-0.0.2/thorchainpy/models/node_node_bond_providers.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_node_bond_providers_node_bond_provider.py` & `thorchainpy-0.0.2/thorchainpy/models/node_node_bond_providers_node_bond_provider.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_node_jail.py` & `thorchainpy-0.0.2/thorchainpy/models/node_node_jail.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_node_preflight_status.py` & `thorchainpy-0.0.2/thorchainpy/models/node_node_preflight_status.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/node_node_pub_key_set.py` & `thorchainpy-0.0.2/thorchainpy/models/node_node_pub_key_set.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/observed_tx.py` & `thorchainpy-0.0.2/thorchainpy/models/observed_tx.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/ping_ping.py` & `thorchainpy-0.0.2/thorchainpy/models/ping_ping.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/pol_response.py` & `thorchainpy-0.0.2/thorchainpy/models/pol_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/pool.py` & `thorchainpy-0.0.2/thorchainpy/models/pool.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/queue_response.py` & `thorchainpy-0.0.2/thorchainpy/models/queue_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/quote_fees.py` & `thorchainpy-0.0.2/thorchainpy/models/quote_fees.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/quote_saver_deposit_response.py` & `thorchainpy-0.0.2/thorchainpy/models/quote_saver_deposit_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/quote_saver_withdraw_response.py` & `thorchainpy-0.0.2/thorchainpy/models/quote_saver_withdraw_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/quote_swap_response.py` & `thorchainpy-0.0.2/thorchainpy/models/quote_swap_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/saver.py` & `thorchainpy-0.0.2/thorchainpy/models/saver.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/thorname.py` & `thorchainpy-0.0.2/thorchainpy/models/thorname.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/thorname_alias.py` & `thorchainpy-0.0.2/thorchainpy/models/thorname_alias.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tss_keysign_metric.py` & `thorchainpy-0.0.2/thorchainpy/models/tss_keysign_metric.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tss_metric.py` & `thorchainpy-0.0.2/thorchainpy/models/tss_metric.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx.py` & `thorchainpy-0.0.2/thorchainpy/models/tx.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_details_response.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_details_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_out_item.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_out_item.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_response.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_signers_response.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_signers_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_confirmation_counted.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_confirmation_counted.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_finalised.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_finalised.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_inbound_observed.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_inbound_observed.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_outbound_delay.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_outbound_delay.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_outbound_signed.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_outbound_signed.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_stages_response_swap_finalised.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_stages_response_swap_finalised.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_status_response.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_status_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/tx_status_response_planned_out_txs_item.py` & `thorchainpy-0.0.2/thorchainpy/models/tx_status_response_planned_out_txs_item.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/vault.py` & `thorchainpy-0.0.2/thorchainpy/models/vault.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/vault_address.py` & `thorchainpy-0.0.2/thorchainpy/models/vault_address.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/vault_info.py` & `thorchainpy-0.0.2/thorchainpy/models/vault_info.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/vault_pubkeys_response.py` & `thorchainpy-0.0.2/thorchainpy/models/vault_pubkeys_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/vault_router.py` & `thorchainpy-0.0.2/thorchainpy/models/vault_router.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/models/version_response.py` & `thorchainpy-0.0.2/thorchainpy/models/version_response.py`

 * *Files identical despite different names*

### Comparing `thorchainpy-0.0.1/thorchainpy/types.py` & `thorchainpy-0.0.2/thorchainpy/types.py`

 * *Files identical despite different names*

