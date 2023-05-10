# Comparing `tmp/thirdweb_sdk-3.0.2a2.tar.gz` & `tmp/thirdweb_sdk-3.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thirdweb_sdk-3.0.2a2.tar", max compression
+gzip compressed data, was "thirdweb_sdk-3.0.2a3.tar", max compression
```

## Comparing `thirdweb_sdk-3.0.2a2.tar` & `thirdweb_sdk-3.0.2a3.tar`

### file list

```diff
@@ -1,353 +1,353 @@
--rw-r--r--   0        0        0    10942 2023-03-13 04:51:11.285705 thirdweb_sdk-3.0.2a2/LICENSE
--rw-r--r--   0        0        0     5877 2023-03-21 02:20:09.125450 thirdweb_sdk-3.0.2a2/README.md
--rw-r--r--   0        0        0     2644 2023-03-21 21:16:13.019746 thirdweb_sdk-3.0.2a2/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 04:51:11.293180 thirdweb_sdk-3.0.2a2/thirdweb/.DS_Store
--rw-r--r--   0        0        0       30 2023-03-13 04:51:11.293237 thirdweb_sdk-3.0.2a2/thirdweb/__init__.py
--rw-r--r--   0        0        0    20818 2023-03-21 21:10:18.158812 thirdweb_sdk-3.0.2a2/thirdweb/abi/__init__.py
--rw-r--r--   0        0        0    85792 2023-03-21 21:08:52.826421 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc1155.py
--rw-r--r--   0        0        0    68008 2023-03-21 21:09:50.028064 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc1155_claimable.py
--rw-r--r--   0        0        0    80026 2023-03-21 21:09:19.039328 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc20.py
--rw-r--r--   0        0        0    59394 2023-03-21 21:08:55.454225 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc20_claimable.py
--rw-r--r--   0        0        0    80078 2023-03-21 21:08:32.955064 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc721.py
--rw-r--r--   0        0        0    64449 2023-03-21 21:09:23.692826 thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc721_claimable.py
--rw-r--r--   0        0        0     9165 2023-03-21 21:09:23.112408 thirdweb_sdk-3.0.2a2/thirdweb/abi/app_u_r_i.py
--rw-r--r--   0        0        0     8936 2023-03-21 21:09:53.181526 thirdweb_sdk-3.0.2a2/thirdweb/abi/batch_mint_metadata.py
--rw-r--r--   0        0        0     3300 2023-03-21 21:09:34.778001 thirdweb_sdk-3.0.2a2/thirdweb/abi/context.py
--rw-r--r--   0        0        0     9470 2023-03-21 21:08:40.342165 thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata.py
--rw-r--r--   0        0        0     9520 2023-03-21 21:09:33.589642 thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata_logic.py
--rw-r--r--   0        0        0     6115 2023-03-21 21:10:05.425680 thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata_storage.py
--rw-r--r--   0        0        0    90485 2023-03-21 21:09:55.752398 thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_publisher.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:09:40.498905 thirdweb_sdk-3.0.2a2/thirdweb/abi/counters.py
--rw-r--r--   0        0        0     5790 2023-03-21 21:09:58.916669 thirdweb_sdk-3.0.2a2/thirdweb/abi/currency_transfer_lib.py
--rw-r--r--   0        0        0    12320 2023-03-21 21:09:51.216590 thirdweb_sdk-3.0.2a2/thirdweb/abi/default_operator_filterer.py
--rw-r--r--   0        0        0    10109 2023-03-21 21:09:04.207780 thirdweb_sdk-3.0.2a2/thirdweb/abi/default_operator_filterer_upgradeable.py
--rw-r--r--   0        0        0    21950 2023-03-21 21:08:58.109378 thirdweb_sdk-3.0.2a2/thirdweb/abi/delayed_reveal.py
--rw-r--r--   0        0        0    76514 2023-03-21 21:10:12.220098 thirdweb_sdk-3.0.2a2/thirdweb/abi/direct_listings_logic.py
--rw-r--r--   0        0        0     6079 2023-03-21 21:09:09.925710 thirdweb_sdk-3.0.2a2/thirdweb/abi/direct_listings_storage.py
--rw-r--r--   0        0        0    41239 2023-03-21 21:09:56.213129 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop.py
--rw-r--r--   0        0        0    46630 2023-03-21 21:09:12.134631 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop1155.py
--rw-r--r--   0        0        0   229869 2023-03-21 21:09:14.349826 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc1155.py
--rw-r--r--   0        0        0   206478 2023-03-21 21:08:49.095573 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc20.py
--rw-r--r--   0        0        0   243271 2023-03-21 21:08:32.298958 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc721.py
--rw-r--r--   0        0        0    33157 2023-03-21 21:09:24.135217 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_single_phase.py
--rw-r--r--   0        0        0    37416 2023-03-21 21:08:11.342793 thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_single_phase1155.py
--rw-r--r--   0        0        0   241058 2023-03-21 21:10:01.145783 thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc1155_v2.py
--rw-r--r--   0        0        0   226555 2023-03-21 21:10:07.308443 thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc20_v2.py
--rw-r--r--   0        0        0   249102 2023-03-21 21:08:45.180881 thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc721_v3.py
--rw-r--r--   0        0        0    43296 2023-03-21 21:10:02.988282 thirdweb_sdk-3.0.2a2/thirdweb/abi/dropsinglephase1155_v1.py
--rw-r--r--   0        0        0    38914 2023-03-21 21:09:21.406116 thirdweb_sdk-3.0.2a2/thirdweb/abi/dropsinglephase_v1.py
--rw-r--r--   0        0        0     3442 2023-03-21 21:09:27.330388 thirdweb_sdk-3.0.2a2/thirdweb/abi/e_i_p712_chainless_domain.py
--rw-r--r--   0        0        0     3284 2023-03-21 21:09:42.232778 thirdweb_sdk-3.0.2a2/thirdweb/abi/ecdsa.py
--rw-r--r--   0        0        0   156536 2023-03-21 21:09:47.953246 thirdweb_sdk-3.0.2a2/thirdweb/abi/edition_stake.py
--rw-r--r--   0        0        0     3292 2023-03-21 21:08:57.701782 thirdweb_sdk-3.0.2a2/thirdweb/abi/eip712.py
--rw-r--r--   0        0        0    64754 2023-03-21 21:08:29.322475 thirdweb_sdk-3.0.2a2/thirdweb/abi/english_auctions_logic.py
--rw-r--r--   0        0        0     6097 2023-03-21 21:08:56.748251 thirdweb_sdk-3.0.2a2/thirdweb/abi/english_auctions_storage.py
--rw-r--r--   0        0        0     3378 2023-03-21 21:08:15.565330 thirdweb_sdk-3.0.2a2/thirdweb/abi/enumerable_set.py
--rw-r--r--   0        0        0    43189 2023-03-21 21:09:50.869568 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155.py
--rw-r--r--   0        0        0   115583 2023-03-21 21:09:39.910365 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_base.py
--rw-r--r--   0        0        0   139620 2023-03-21 21:09:55.030334 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_delayed_reveal.py
--rw-r--r--   0        0        0   170049 2023-03-21 21:09:30.695787 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_drop.py
--rw-r--r--   0        0        0    18760 2023-03-21 21:08:36.055900 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_holder.py
--rw-r--r--   0        0        0   121380 2023-03-21 21:09:34.469034 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_lazy_mint.py
--rw-r--r--   0        0        0   112914 2023-03-21 21:09:07.116023 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_preset_upgradeable.py
--rw-r--r--   0        0        0    18357 2023-03-21 21:09:11.649006 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_receiver.py
--rw-r--r--   0        0        0   134633 2023-03-21 21:09:58.313669 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_signature_mint.py
--rw-r--r--   0        0        0     6858 2023-03-21 21:08:59.421204 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc165.py
--rw-r--r--   0        0        0     6039 2023-03-21 21:08:39.763908 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1967_proxy.py
--rw-r--r--   0        0        0     5644 2023-03-21 21:09:40.801785 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1967_upgrade.py
--rw-r--r--   0        0        0    39698 2023-03-21 21:10:05.887107 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20.py
--rw-r--r--   0        0        0    72167 2023-03-21 21:09:15.008808 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_base.py
--rw-r--r--   0        0        0   104921 2023-03-21 21:09:26.648481 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_drop.py
--rw-r--r--   0        0        0   136778 2023-03-21 21:09:06.224555 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_drop_vote.py
--rw-r--r--   0        0        0    50917 2023-03-21 21:09:53.719532 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_permit.py
--rw-r--r--   0        0        0    90382 2023-03-21 21:09:04.935832 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_signature_mint.py
--rw-r--r--   0        0        0   122210 2023-03-21 21:10:14.156593 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_signature_mint_vote.py
--rw-r--r--   0        0        0   103909 2023-03-21 21:10:11.196981 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_vote.py
--rw-r--r--   0        0        0    82607 2023-03-21 21:08:08.709909 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_votes.py
--rw-r--r--   0        0        0     6811 2023-03-21 21:08:35.394687 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context.py
--rw-r--r--   0        0        0     7980 2023-03-21 21:08:43.703650 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_consumer.py
--rw-r--r--   0        0        0     6856 2023-03-21 21:08:25.980022 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_logic.py
--rw-r--r--   0        0        0     6079 2023-03-21 21:09:19.363783 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_storage.py
--rw-r--r--   0        0        0     7631 2023-03-21 21:09:01.457912 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable.py
--rw-r--r--   0        0        0     6955 2023-03-21 21:10:18.120247 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable_logic.py
--rw-r--r--   0        0        0     6282 2023-03-21 21:09:16.164432 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable_storage.py
--rw-r--r--   0        0        0    53696 2023-03-21 21:08:53.384176 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_a_upgradeable.py
--rw-r--r--   0        0        0   119717 2023-03-21 21:10:04.187429 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_base.py
--rw-r--r--   0        0        0   142298 2023-03-21 21:08:22.609407 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_delayed_reveal.py
--rw-r--r--   0        0        0   169717 2023-03-21 21:10:17.785418 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_drop.py
--rw-r--r--   0        0        0     8931 2023-03-21 21:09:57.029679 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_holder.py
--rw-r--r--   0        0        0   124064 2023-03-21 21:08:30.495068 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_lazy_mint.py
--rw-r--r--   0        0        0   182421 2023-03-21 21:08:18.454287 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_multiwrap.py
--rw-r--r--   0        0        0   138584 2023-03-21 21:08:27.767685 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_signature_mint.py
--rw-r--r--   0        0        0    52988 2023-03-21 21:08:17.199277 thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721a.py
--rw-r--r--   0        0        0     3300 2023-03-21 21:09:45.796279 thirdweb_sdk-3.0.2a2/thirdweb/abi/fee_type.py
--rw-r--r--   0        0        0    11166 2023-03-21 21:09:28.994626 thirdweb_sdk-3.0.2a2/thirdweb/abi/forwarder_consumer.py
--rw-r--r--   0        0        0    26106 2023-03-21 21:09:07.796858 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc1155.py
--rw-r--r--   0        0        0    10788 2023-03-21 21:09:41.161880 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc1155_claimable.py
--rw-r--r--   0        0        0    25450 2023-03-21 21:10:11.604943 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc20.py
--rw-r--r--   0        0        0    10033 2023-03-21 21:08:52.164274 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc20_claimable.py
--rw-r--r--   0        0        0    25497 2023-03-21 21:08:11.703586 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc721.py
--rw-r--r--   0        0        0    10043 2023-03-21 21:09:24.787850 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc721_claimable.py
--rw-r--r--   0        0        0     9175 2023-03-21 21:09:54.058430 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_app_u_r_i.py
--rw-r--r--   0        0        0     5661 2023-03-21 21:09:17.821503 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_beacon.py
--rw-r--r--   0        0        0    11588 2023-03-21 21:08:59.104045 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc1155.py
--rw-r--r--   0        0        0     9891 2023-03-21 21:08:51.568867 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc20.py
--rw-r--r--   0        0        0     6533 2023-03-21 21:09:45.510156 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc721.py
--rw-r--r--   0        0        0     3394 2023-03-21 21:09:02.361163 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_condition.py
--rw-r--r--   0        0        0     3474 2023-03-21 21:08:50.934488 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_condition_multi_phase.py
--rw-r--r--   0        0        0    10930 2023-03-21 21:08:21.017658 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_conditions_single_phase.py
--rw-r--r--   0        0        0    13127 2023-03-21 21:09:16.528243 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claimable_erc1155.py
--rw-r--r--   0        0        0    11876 2023-03-21 21:08:58.752286 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claimable_erc721.py
--rw-r--r--   0        0        0     7811 2023-03-21 21:08:38.694409 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_context.py
--rw-r--r--   0        0        0    23449 2023-03-21 21:10:16.706004 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_deployer.py
--rw-r--r--   0        0        0     8413 2023-03-21 21:09:25.867177 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_factory.py
--rw-r--r--   0        0        0     9480 2023-03-21 21:09:43.016186 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_metadata.py
--rw-r--r--   0        0        0    44219 2023-03-21 21:08:12.767691 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_publisher.py
--rw-r--r--   0        0        0    11835 2023-03-21 21:08:45.862693 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_delayed_reveal.py
--rw-r--r--   0        0        0    15264 2023-03-21 21:09:12.496261 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_delayed_reveal_deprecated.py
--rw-r--r--   0        0        0    57624 2023-03-21 21:08:06.836542 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_direct_listings.py
--rw-r--r--   0        0        0    20142 2023-03-21 21:10:12.961703 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop.py
--rw-r--r--   0        0        0    21722 2023-03-21 21:10:01.846865 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop1155.py
--rw-r--r--   0        0        0     3426 2023-03-21 21:09:43.300962 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_claim_condition.py
--rw-r--r--   0        0        0    60183 2023-03-21 21:09:27.877982 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc1155.py
--rw-r--r--   0        0        0    43180 2023-03-21 21:09:20.624859 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc20.py
--rw-r--r--   0        0        0    66414 2023-03-21 21:08:49.682350 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc721.py
--rw-r--r--   0        0        0    20224 2023-03-21 21:08:33.319295 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_single_phase.py
--rw-r--r--   0        0        0    21804 2023-03-21 21:08:33.957556 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_single_phase1155.py
--rw-r--r--   0        0        0    11373 2023-03-21 21:09:29.617976 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_edition_stake.py
--rw-r--r--   0        0        0    55894 2023-03-21 21:09:03.239311 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_english_auctions.py
--rw-r--r--   0        0        0     5838 2023-03-21 21:09:48.758369 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_enumerable.py
--rw-r--r--   0        0        0     6466 2023-03-21 21:09:17.503662 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_metadata.py
--rw-r--r--   0        0        0    18366 2023-03-21 21:08:25.684910 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_receiver.py
--rw-r--r--   0        0        0     6575 2023-03-21 21:09:49.433466 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_supply.py
--rw-r--r--   0        0        0     5815 2023-03-21 21:10:10.412497 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1822_proxiable.py
--rw-r--r--   0        0        0     9937 2023-03-21 21:09:46.908158 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc20_metadata.py
--rw-r--r--   0        0        0    14843 2023-03-21 21:10:12.600494 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc20_permit.py
--rw-r--r--   0        0        0     6820 2023-03-21 21:08:21.322696 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc2771_context.py
--rw-r--r--   0        0        0    10336 2023-03-21 21:10:02.166521 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_enumerable.py
--rw-r--r--   0        0        0    10879 2023-03-21 21:09:20.960681 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_metadata.py
--rw-r--r--   0        0        0     8622 2023-03-21 21:08:35.699659 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_receiver.py
--rw-r--r--   0        0        0     5733 2023-03-21 21:09:00.575249 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_supply.py
--rw-r--r--   0        0        0     7383 2023-03-21 21:09:38.542929 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_fee_tier_placement_extension.py
--rw-r--r--   0        0        0     9333 2023-03-21 21:09:16.856426 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_lazy_mint.py
--rw-r--r--   0        0        0     9955 2023-03-21 21:08:26.876718 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_lazy_mint_with_tier.py
--rw-r--r--   0        0        0    68265 2023-03-21 21:08:50.285543 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_marketplace.py
--rw-r--r--   0        0        0     8961 2023-03-21 21:08:25.055553 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc1155.py
--rw-r--r--   0        0        0     7682 2023-03-21 21:08:37.368837 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc20.py
--rw-r--r--   0        0        0     7691 2023-03-21 21:08:20.336604 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc721.py
--rw-r--r--   0        0        0     6643 2023-03-21 21:08:29.639130 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_multicall.py
--rw-r--r--   0        0        0    15555 2023-03-21 21:09:45.188257 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_multiwrap.py
--rw-r--r--   0        0        0    11286 2023-03-21 21:09:15.357126 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_n_f_t_stake.py
--rw-r--r--   0        0        0    32749 2023-03-21 21:08:40.742755 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_offers.py
--rw-r--r--   0        0        0    94730 2023-03-21 21:09:25.529235 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_operator_filter_registry.py
--rw-r--r--   0        0        0     9845 2023-03-21 21:09:17.194955 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_operator_filter_toggle.py
--rw-r--r--   0        0        0     9391 2023-03-21 21:08:13.089909 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_ownable.py
--rw-r--r--   0        0        0    19897 2023-03-21 21:08:24.749487 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_pack.py
--rw-r--r--   0        0        0    31414 2023-03-21 21:09:20.150610 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_pack_v_r_f_direct.py
--rw-r--r--   0        0        0    23527 2023-03-21 21:08:28.786000 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_permissions.py
--rw-r--r--   0        0        0    30461 2023-03-21 21:09:28.318670 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_permissions_enumerable.py
--rw-r--r--   0        0        0    11346 2023-03-21 21:09:52.012179 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_platform_fee.py
--rw-r--r--   0        0        0    15146 2023-03-21 21:08:06.021657 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_plugin_map.py
--rw-r--r--   0        0        0     9980 2023-03-21 21:08:28.093834 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_primary_sale.py
--rw-r--r--   0        0        0    27471 2023-03-21 21:09:12.927559 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_router.py
--rw-r--r--   0        0        0    27105 2023-03-21 21:09:33.262167 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_royalty.py
--rw-r--r--   0        0        0     9998 2023-03-21 21:09:32.834376 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_action.py
--rw-r--r--   0        0        0    16148 2023-03-21 21:08:24.386449 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc1155.py
--rw-r--r--   0        0        0    15154 2023-03-21 21:09:50.382906 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc20.py
--rw-r--r--   0        0        0    15923 2023-03-21 21:10:13.306912 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc721.py
--rw-r--r--   0        0        0    27313 2023-03-21 21:08:23.744026 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking1155.py
--rw-r--r--   0        0        0    19685 2023-03-21 21:09:00.260631 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking20.py
--rw-r--r--   0        0        0    18920 2023-03-21 21:09:02.741026 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking721.py
--rw-r--r--   0        0        0     7095 2023-03-21 21:08:09.021380 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_fee.py
--rw-r--r--   0        0        0    26206 2023-03-21 21:10:14.906955 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_multichain_registry.py
--rw-r--r--   0        0        0    21103 2023-03-21 21:08:47.779452 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_registry.py
--rw-r--r--   0        0        0    13067 2023-03-21 21:08:50.637838 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_thirdweb_contract.py
--rw-r--r--   0        0        0     3370 2023-03-21 21:09:18.109490 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_bundle.py
--rw-r--r--   0        0        0    53182 2023-03-21 21:09:52.846792 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc1155.py
--rw-r--r--   0        0        0    46867 2023-03-21 21:08:14.962462 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc20.py
--rw-r--r--   0        0        0    58484 2023-03-21 21:09:01.140567 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc721.py
--rw-r--r--   0        0        0    11351 2023-03-21 21:10:14.507583 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_stake.py
--rw-r--r--   0        0        0    27443 2023-03-21 21:09:41.596621 thirdweb_sdk-3.0.2a2/thirdweb/abi/i_votes.py
--rw-r--r--   0        0        0     3418 2023-03-21 21:08:22.898138 thirdweb_sdk-3.0.2a2/thirdweb/abi/iclaimcondition_v1.py
--rw-r--r--   0        0        0     3450 2023-03-21 21:09:01.745494 thirdweb_sdk-3.0.2a2/thirdweb/abi/idropclaimcondition_v2.py
--rw-r--r--   0        0        0    61520 2023-03-21 21:10:16.312733 thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc1155_v2.py
--rw-r--r--   0        0        0    44262 2023-03-21 21:09:15.846242 thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc20_v2.py
--rw-r--r--   0        0        0    67599 2023-03-21 21:08:57.394509 thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc721_v3.py
--rw-r--r--   0        0        0    21795 2023-03-21 21:10:02.535793 thirdweb_sdk-3.0.2a2/thirdweb/abi/idropsinglephase1155_v1.py
--rw-r--r--   0        0        0    20215 2023-03-21 21:08:30.866300 thirdweb_sdk-3.0.2a2/thirdweb/abi/idropsinglephase_v1.py
--rw-r--r--   0        0        0    31974 2023-03-21 21:08:23.339715 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc1155.py
--rw-r--r--   0        0        0     6867 2023-03-21 21:08:21.620170 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc165.py
--rw-r--r--   0        0        0    24799 2023-03-21 21:10:08.101108 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc20.py
--rw-r--r--   0        0        0    10953 2023-03-21 21:08:26.561893 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc2981.py
--rw-r--r--   0        0        0    39092 2023-03-21 21:09:59.670318 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc721.py
--rw-r--r--   0        0        0    49418 2023-03-21 21:10:15.744637 thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc721a.py
--rw-r--r--   0        0        0     3362 2023-03-21 21:08:33.598331 thirdweb_sdk-3.0.2a2/thirdweb/abi/init_storage.py
--rw-r--r--   0        0        0     4108 2023-03-21 21:08:51.849966 thirdweb_sdk-3.0.2a2/thirdweb/abi/initializable.py
--rw-r--r--   0        0        0    13842 2023-03-21 21:09:05.298641 thirdweb_sdk-3.0.2a2/thirdweb/abi/isignatureminterc721_v1.py
--rw-r--r--   0        0        0    11782 2023-03-21 21:09:57.371637 thirdweb_sdk-3.0.2a2/thirdweb/abi/iweth.py
--rw-r--r--   0        0        0    14519 2023-03-21 21:10:09.145892 thirdweb_sdk-3.0.2a2/thirdweb/abi/lazy_mint.py
--rw-r--r--   0        0        0    19969 2023-03-21 21:09:27.034492 thirdweb_sdk-3.0.2a2/thirdweb/abi/lazy_mint_with_tier.py
--rw-r--r--   0        0        0   156959 2023-03-21 21:09:09.311269 thirdweb_sdk-3.0.2a2/thirdweb/abi/marketplace.py
--rw-r--r--   0        0        0   117081 2023-03-21 21:08:43.377369 thirdweb_sdk-3.0.2a2/thirdweb/abi/marketplace_v3.py
--rw-r--r--   0        0        0     3276 2023-03-21 21:08:24.042491 thirdweb_sdk-3.0.2a2/thirdweb/abi/math.py
--rw-r--r--   0        0        0     3362 2023-03-21 21:08:15.836006 thirdweb_sdk-3.0.2a2/thirdweb/abi/merkle_proof.py
--rw-r--r--   0        0        0     9839 2023-03-21 21:08:20.678273 thirdweb_sdk-3.0.2a2/thirdweb/abi/mock.py
--rw-r--r--   0        0        0     8147 2023-03-21 21:08:35.095946 thirdweb_sdk-3.0.2a2/thirdweb/abi/mock_contract.py
--rw-r--r--   0        0        0    43400 2023-03-21 21:09:56.694280 thirdweb_sdk-3.0.2a2/thirdweb/abi/mock_contract_publisher.py
--rw-r--r--   0        0        0     6634 2023-03-21 21:10:09.467119 thirdweb_sdk-3.0.2a2/thirdweb/abi/multicall.py
--rw-r--r--   0        0        0   188886 2023-03-21 21:08:08.030741 thirdweb_sdk-3.0.2a2/thirdweb/abi/multiwrap.py
--rw-r--r--   0        0        0   127828 2023-03-21 21:10:05.102285 thirdweb_sdk-3.0.2a2/thirdweb/abi/n_f_t_stake.py
--rw-r--r--   0        0        0    41556 2023-03-21 21:09:08.244100 thirdweb_sdk-3.0.2a2/thirdweb/abi/offers_logic.py
--rw-r--r--   0        0        0     5890 2023-03-21 21:08:58.420071 thirdweb_sdk-3.0.2a2/thirdweb/abi/offers_storage.py
--rw-r--r--   0        0        0     9837 2023-03-21 21:08:15.292128 thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filter_toggle.py
--rw-r--r--   0        0        0    12250 2023-03-21 21:08:45.537192 thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filterer.py
--rw-r--r--   0        0        0    10025 2023-03-21 21:09:24.458347 thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filterer_upgradeable.py
--rw-r--r--   0        0        0     9381 2023-03-21 21:10:03.317386 thirdweb_sdk-3.0.2a2/thirdweb/abi/ownable.py
--rw-r--r--   0        0        0   189507 2023-03-21 21:08:10.601424 thirdweb_sdk-3.0.2a2/thirdweb/abi/pack.py
--rw-r--r--   0        0        0   192431 2023-03-21 21:09:31.958711 thirdweb_sdk-3.0.2a2/thirdweb/abi/pack_v_r_f_direct.py
--rw-r--r--   0        0        0    42973 2023-03-21 21:09:39.029359 thirdweb_sdk-3.0.2a2/thirdweb/abi/payment_splitter_upgradeable.py
--rw-r--r--   0        0        0    29535 2023-03-21 21:08:09.430315 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions.py
--rw-r--r--   0        0        0    36480 2023-03-21 21:09:21.872069 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable.py
--rw-r--r--   0        0        0    36540 2023-03-21 21:09:42.685789 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable_logic.py
--rw-r--r--   0        0        0     6205 2023-03-21 21:09:29.299239 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable_storage.py
--rw-r--r--   0        0        0    29595 2023-03-21 21:08:37.779099 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_logic.py
--rw-r--r--   0        0        0     5980 2023-03-21 21:10:01.481488 thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_storage.py
--rw-r--r--   0        0        0    11336 2023-03-21 21:10:07.692903 thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee.py
--rw-r--r--   0        0        0    11386 2023-03-21 21:08:36.640452 thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee_logic.py
--rw-r--r--   0        0        0     5985 2023-03-21 21:08:47.395169 thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee_storage.py
--rw-r--r--   0        0        0    15127 2023-03-21 21:09:41.949341 thirdweb_sdk-3.0.2a2/thirdweb/abi/plugin_map.py
--rw-r--r--   0        0        0     9970 2023-03-21 21:08:10.928311 thirdweb_sdk-3.0.2a2/thirdweb/abi/primary_sale.py
--rw-r--r--   0        0        0     3400 2023-03-21 21:08:39.467301 thirdweb_sdk-3.0.2a2/thirdweb/abi/proxy.py
--rw-r--r--   0        0        0     6116 2023-03-21 21:09:52.313980 thirdweb_sdk-3.0.2a2/thirdweb/abi/proxy_for_upgradeable.py
--rw-r--r--   0        0        0     3394 2023-03-21 21:09:18.390581 thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard.py
--rw-r--r--   0        0        0     3434 2023-03-21 21:08:25.328015 thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_logic.py
--rw-r--r--   0        0        0     6097 2023-03-21 21:08:51.241047 thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_storage.py
--rw-r--r--   0        0        0     4225 2023-03-21 21:09:36.287555 thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_upgradeable.py
--rw-r--r--   0        0        0    38781 2023-03-21 21:09:51.679791 thirdweb_sdk-3.0.2a2/thirdweb/abi/router.py
--rw-r--r--   0        0        0    39070 2023-03-21 21:08:59.885461 thirdweb_sdk-3.0.2a2/thirdweb/abi/router_immutable.py
--rw-r--r--   0        0        0     5890 2023-03-21 21:08:53.692550 thirdweb_sdk-3.0.2a2/thirdweb/abi/router_storage.py
--rw-r--r--   0        0        0    27102 2023-03-21 21:08:37.053809 thirdweb_sdk-3.0.2a2/thirdweb/abi/royalty.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:08:16.116731 thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_cast.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:09:07.411738 thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_erc20.py
--rw-r--r--   0        0        0     3308 2023-03-21 21:08:42.541800 thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_math.py
--rw-r--r--   0        0        0     9992 2023-03-21 21:08:06.333519 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_action.py
--rw-r--r--   0        0        0    10824 2023-03-21 21:08:28.406656 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_action_upgradeable.py
--rw-r--r--   0        0        0   231932 2023-03-21 21:08:19.956367 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_drop.py
--rw-r--r--   0        0        0    16142 2023-03-21 21:09:28.670178 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc1155.py
--rw-r--r--   0        0        0    16979 2023-03-21 21:09:19.723980 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc1155_upgradeable.py
--rw-r--r--   0        0        0    15148 2023-03-21 21:08:55.805549 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc20.py
--rw-r--r--   0        0        0    15983 2023-03-21 21:09:43.645432 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc20_upgradeable.py
--rw-r--r--   0        0        0    15917 2023-03-21 21:09:49.109778 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc721.py
--rw-r--r--   0        0        0    16753 2023-03-21 21:10:15.245507 thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc721_upgradeable.py
--rw-r--r--   0        0        0   237737 2023-03-21 21:08:14.448220 thirdweb_sdk-3.0.2a2/thirdweb/abi/signaturedrop_v4.py
--rw-r--r--   0        0        0    42531 2023-03-21 21:09:32.484424 thirdweb_sdk-3.0.2a2/thirdweb/abi/soulbound_erc721_a.py
--rw-r--r--   0        0        0   101885 2023-03-21 21:09:46.568630 thirdweb_sdk-3.0.2a2/thirdweb/abi/split.py
--rw-r--r--   0        0        0    72420 2023-03-21 21:08:05.682227 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155.py
--rw-r--r--   0        0        0   111245 2023-03-21 21:08:41.517848 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155_base.py
--rw-r--r--   0        0        0    73314 2023-03-21 21:08:56.422298 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155_upgradeable.py
--rw-r--r--   0        0        0    49004 2023-03-21 21:09:36.783300 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20.py
--rw-r--r--   0        0        0    72923 2023-03-21 21:08:38.370233 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20_base.py
--rw-r--r--   0        0        0    49928 2023-03-21 21:08:39.184022 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20_upgradeable.py
--rw-r--r--   0        0        0    50405 2023-03-21 21:08:16.628311 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721.py
--rw-r--r--   0        0        0    85256 2023-03-21 21:10:08.769380 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721_base.py
--rw-r--r--   0        0        0    51319 2023-03-21 21:08:05.087710 thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721_upgradeable.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:08:40.031617 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_address.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:08:26.250272 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_bit_maps.py
--rw-r--r--   0        0        0    89887 2023-03-21 21:08:42.249889 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_factory.py
--rw-r--r--   0        0        0    75523 2023-03-21 21:08:12.312353 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_fee.py
--rw-r--r--   0        0        0    67405 2023-03-21 21:09:03.862533 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry.py
--rw-r--r--   0        0        0    37213 2023-03-21 21:09:48.429865 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_logic.py
--rw-r--r--   0        0        0    75392 2023-03-21 21:10:10.097915 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_router.py
--rw-r--r--   0        0        0     6169 2023-03-21 21:09:37.112500 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_storage.py
--rw-r--r--   0        0        0     3738 2023-03-21 21:09:58.614997 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_proxy.py
--rw-r--r--   0        0        0    59703 2023-03-21 21:08:34.777306 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_registry.py
--rw-r--r--   0        0        0     3378 2023-03-21 21:08:34.224832 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_storage_slot.py
--rw-r--r--   0        0        0     3316 2023-03-21 21:09:09.623398 thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_strings.py
--rw-r--r--   0        0        0   206242 2023-03-21 21:09:11.247290 thirdweb_sdk-3.0.2a2/thirdweb/abi/tiered_drop.py
--rw-r--r--   0        0        0    15273 2023-03-21 21:09:38.226378 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_bundle.py
--rw-r--r--   0        0        0   182279 2023-03-21 21:09:35.982389 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc1155.py
--rw-r--r--   0        0        0   176744 2023-03-21 21:08:54.858300 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc20.py
--rw-r--r--   0        0        0   185235 2023-03-21 21:08:47.076267 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc721.py
--rw-r--r--   0        0        0   118802 2023-03-21 21:09:22.761817 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_stake.py
--rw-r--r--   0        0        0    35792 2023-03-21 21:09:37.864038 thirdweb_sdk-3.0.2a2/thirdweb/abi/token_store.py
--rw-r--r--   0        0        0    15519 2023-03-21 21:09:02.087865 thirdweb_sdk-3.0.2a2/thirdweb/abi/upgradeable.py
--rw-r--r--   0        0        0   180710 2023-03-21 21:09:44.839464 thirdweb_sdk-3.0.2a2/thirdweb/abi/vote_erc20.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298098 thirdweb_sdk-3.0.2a2/thirdweb/common/__init__.py
--rw-r--r--   0        0        0     4797 2023-03-13 04:51:11.298195 thirdweb_sdk-3.0.2a2/thirdweb/common/claim_conditions.py
--rw-r--r--   0        0        0     4039 2023-03-13 04:51:11.298272 thirdweb_sdk-3.0.2a2/thirdweb/common/currency.py
--rw-r--r--   0        0        0     2706 2023-03-13 04:51:11.298342 thirdweb_sdk-3.0.2a2/thirdweb/common/error.py
--rw-r--r--   0        0        0     3962 2023-03-21 02:20:09.125984 thirdweb_sdk-3.0.2a2/thirdweb/common/feature_detection.py
--rw-r--r--   0        0        0     4696 2023-03-13 04:51:11.298476 thirdweb_sdk-3.0.2a2/thirdweb/common/marketplace.py
--rw-r--r--   0        0        0     4657 2023-03-13 04:51:11.298549 thirdweb_sdk-3.0.2a2/thirdweb/common/merkle_tree.py
--rw-r--r--   0        0        0     2699 2023-03-13 04:51:11.298625 thirdweb_sdk-3.0.2a2/thirdweb/common/nft.py
--rw-r--r--   0        0        0     1241 2023-03-13 04:51:11.298693 thirdweb_sdk-3.0.2a2/thirdweb/common/sign.py
--rw-r--r--   0        0        0      287 2023-03-13 04:51:11.298753 thirdweb_sdk-3.0.2a2/thirdweb/common/signature_minting.py
--rw-r--r--   0        0        0     2552 2023-03-13 04:51:11.298824 thirdweb_sdk-3.0.2a2/thirdweb/common/snapshots.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298891 thirdweb_sdk-3.0.2a2/thirdweb/constants/__init__.py
--rw-r--r--   0        0        0     3044 2023-03-13 04:51:11.298995 thirdweb_sdk-3.0.2a2/thirdweb/constants/addresses.py
--rw-r--r--   0        0        0      284 2023-03-13 04:51:11.299055 thirdweb_sdk-3.0.2a2/thirdweb/constants/chains.py
--rw-r--r--   0        0        0      182 2023-03-13 04:51:11.299107 thirdweb_sdk-3.0.2a2/thirdweb/constants/contract.py
--rw-r--r--   0        0        0     2457 2023-03-13 04:51:11.299165 thirdweb_sdk-3.0.2a2/thirdweb/constants/currency.py
--rw-r--r--   0        0        0      190 2023-03-13 04:51:11.299216 thirdweb_sdk-3.0.2a2/thirdweb/constants/events.py
--rw-r--r--   0        0        0      983 2023-03-13 04:51:11.299284 thirdweb_sdk-3.0.2a2/thirdweb/constants/role.py
--rw-r--r--   0        0        0      544 2023-03-13 04:51:11.299350 thirdweb_sdk-3.0.2a2/thirdweb/constants/rpc.py
--rw-r--r--   0        0        0     1518 2023-03-13 04:51:11.299410 thirdweb_sdk-3.0.2a2/thirdweb/constants/urls.py
--rw-r--r--   0        0        0      254 2023-03-13 04:51:11.299504 thirdweb_sdk-3.0.2a2/thirdweb/contracts/__init__.py
--rw-r--r--   0        0        0     8728 2023-03-21 19:42:41.604041 thirdweb_sdk-3.0.2a2/thirdweb/contracts/custom.py
--rw-r--r--   0        0        0     9658 2023-03-21 02:20:09.126457 thirdweb_sdk-3.0.2a2/thirdweb/contracts/edition.py
--rw-r--r--   0        0        0     8591 2023-03-21 02:20:09.126668 thirdweb_sdk-3.0.2a2/thirdweb/contracts/edition_drop.py
--rw-r--r--   0        0        0     1680 2023-03-13 04:51:11.299821 thirdweb_sdk-3.0.2a2/thirdweb/contracts/maps.py
--rw-r--r--   0        0        0    12583 2023-03-13 04:51:11.299938 thirdweb_sdk-3.0.2a2/thirdweb/contracts/marketplace.py
--rw-r--r--   0        0        0    12181 2023-03-21 02:20:09.126891 thirdweb_sdk-3.0.2a2/thirdweb/contracts/multiwrap.py
--rw-r--r--   0        0        0     8646 2023-03-21 02:20:09.127098 thirdweb_sdk-3.0.2a2/thirdweb/contracts/nft_collection.py
--rw-r--r--   0        0        0    12048 2023-03-21 02:20:09.127310 thirdweb_sdk-3.0.2a2/thirdweb/contracts/nft_drop.py
--rw-r--r--   0        0        0     6305 2023-03-21 02:20:09.127530 thirdweb_sdk-3.0.2a2/thirdweb/contracts/token.py
--rw-r--r--   0        0        0       29 2023-03-13 04:51:11.300414 thirdweb_sdk-3.0.2a2/thirdweb/core/__init__.py
--rw-r--r--   0        0        0       54 2023-03-13 04:51:11.300500 thirdweb_sdk-3.0.2a2/thirdweb/core/auth/__init__.py
--rw-r--r--   0        0        0    13845 2023-03-13 04:51:11.300598 thirdweb_sdk-3.0.2a2/thirdweb/core/auth/wallet_authenticator.py
--rw-r--r--   0        0        0        0 2023-03-13 04:51:11.300659 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/__init__.py
--rw-r--r--   0        0        0     1318 2023-03-13 04:51:11.300732 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/base_contract.py
--rw-r--r--   0        0        0     4014 2023-03-13 04:51:11.300801 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_deployer.py
--rw-r--r--   0        0        0     3358 2023-03-13 04:51:11.300864 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_events.py
--rw-r--r--   0        0        0     1638 2023-03-13 04:51:11.300923 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_metadata.py
--rw-r--r--   0        0        0     1419 2023-03-13 04:51:11.300983 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_platform_fee.py
--rw-r--r--   0        0        0     3292 2023-03-13 04:51:11.301051 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_roles.py
--rw-r--r--   0        0        0     3229 2023-03-13 04:51:11.301115 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_royalty.py
--rw-r--r--   0        0        0     1051 2023-03-13 04:51:11.301175 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_sales.py
--rw-r--r--   0        0        0     5077 2023-03-13 04:51:11.301253 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_wrapper.py
--rw-r--r--   0        0        0     2361 2023-03-13 04:51:11.301333 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/drop_claim_conditions.py
--rw-r--r--   0        0        0     2722 2023-03-13 04:51:11.301386 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/drop_erc1155_claim_conditions.py
--rw-r--r--   0        0        0     7510 2023-03-21 02:20:09.127796 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_1155.py
--rw-r--r--   0        0        0     8047 2023-03-13 04:51:11.301549 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_1155_signature_minting.py
--rw-r--r--   0        0        0     1270 2023-03-21 19:42:41.604472 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_1155_standard.py
--rw-r--r--   0        0        0     8842 2023-03-21 19:42:39.047953 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_20.py
--rw-r--r--   0        0        0     6733 2023-03-13 04:51:11.301730 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_20_signature_minting.py
--rw-r--r--   0        0        0     1263 2023-03-21 19:42:41.604726 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_20_standard.py
--rw-r--r--   0        0        0     7064 2023-03-21 02:20:09.128346 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_721.py
--rw-r--r--   0        0        0     7822 2023-03-13 04:51:11.301886 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_721_signature_minting.py
--rw-r--r--   0        0        0     1352 2023-03-21 19:42:41.604974 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_721_standard.py
--rw-r--r--   0        0        0     6575 2023-03-13 04:51:11.301958 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/factory.py
--rw-r--r--   0        0        0     9265 2023-03-13 04:51:11.302042 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/ipfs_storage.py
--rw-r--r--   0        0        0    11102 2023-03-13 04:51:11.302151 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/marketplace_auction.py
--rw-r--r--   0        0        0    12104 2023-03-13 04:51:11.302217 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/marketplace_direct.py
--rw-r--r--   0        0        0     2764 2023-03-13 04:51:11.302278 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/provider_handler.py
--rw-r--r--   0        0        0     1257 2023-03-13 04:51:11.302340 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/registry.py
--rw-r--r--   0        0        0     4780 2023-03-13 04:51:11.302405 thirdweb_sdk-3.0.2a2/thirdweb/core/classes/sharded_merkle_tree.py
--rw-r--r--   0        0        0     3227 2023-03-13 04:51:11.302500 thirdweb_sdk-3.0.2a2/thirdweb/core/helpers/storage.py
--rw-r--r--   0        0        0     7739 2023-03-13 04:51:11.302575 thirdweb_sdk-3.0.2a2/thirdweb/core/sdk.py
--rw-r--r--   0        0        0      254 2023-03-13 04:51:11.302670 thirdweb_sdk-3.0.2a2/thirdweb/types/__init__.py
--rw-r--r--   0        0        0     1482 2023-03-13 04:51:11.302742 thirdweb_sdk-3.0.2a2/thirdweb/types/auth.py
--rw-r--r--   0        0        0     1758 2023-03-13 04:51:11.302808 thirdweb_sdk-3.0.2a2/thirdweb/types/contract.py
--rw-r--r--   0        0        0     3111 2023-03-13 04:51:11.302929 thirdweb_sdk-3.0.2a2/thirdweb/types/contracts/claim_conditions.py
--rw-r--r--   0        0        0     5664 2023-03-13 04:51:11.303002 thirdweb_sdk-3.0.2a2/thirdweb/types/contracts/signature.py
--rw-r--r--   0        0        0      528 2023-03-13 04:51:11.303061 thirdweb_sdk-3.0.2a2/thirdweb/types/currency.py
--rw-r--r--   0        0        0      578 2023-03-13 04:51:11.303126 thirdweb_sdk-3.0.2a2/thirdweb/types/events.py
--rw-r--r--   0        0        0     2519 2023-03-13 04:51:11.303186 thirdweb_sdk-3.0.2a2/thirdweb/types/marketplace.py
--rw-r--r--   0        0        0      945 2023-03-13 04:51:11.303247 thirdweb_sdk-3.0.2a2/thirdweb/types/multiwrap.py
--rw-r--r--   0        0        0     3574 2023-03-13 04:51:11.303318 thirdweb_sdk-3.0.2a2/thirdweb/types/nft.py
--rw-r--r--   0        0        0     1084 2023-03-13 04:51:11.303390 thirdweb_sdk-3.0.2a2/thirdweb/types/sdk.py
--rw-r--r--   0        0        0      243 2023-03-13 04:51:11.303500 thirdweb_sdk-3.0.2a2/thirdweb/types/settings/__init__.py
--rw-r--r--   0        0        0     4111 2023-03-13 04:51:11.303569 thirdweb_sdk-3.0.2a2/thirdweb/types/settings/metadata.py
--rw-r--r--   0        0        0      215 2023-03-13 04:51:11.303629 thirdweb_sdk-3.0.2a2/thirdweb/types/storage.py
--rw-r--r--   0        0        0      334 2023-03-13 04:51:11.303692 thirdweb_sdk-3.0.2a2/thirdweb/types/tx.py
--rw-r--r--   0        0        0     6696 1970-01-01 00:00:00.000000 thirdweb_sdk-3.0.2a2/PKG-INFO
+-rw-r--r--   0        0        0    10942 2023-03-13 04:51:11.285705 thirdweb_sdk-3.0.2a3/LICENSE
+-rw-r--r--   0        0        0     5877 2023-03-21 02:20:09.125450 thirdweb_sdk-3.0.2a3/README.md
+-rw-r--r--   0        0        0     2644 2023-05-10 22:38:23.444106 thirdweb_sdk-3.0.2a3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 04:51:11.293180 thirdweb_sdk-3.0.2a3/thirdweb/.DS_Store
+-rw-r--r--   0        0        0       30 2023-03-13 04:51:11.293237 thirdweb_sdk-3.0.2a3/thirdweb/__init__.py
+-rw-r--r--   0        0        0    20818 2023-03-21 21:23:13.236831 thirdweb_sdk-3.0.2a3/thirdweb/abi/__init__.py
+-rw-r--r--   0        0        0    85792 2023-03-21 21:23:13.237140 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc1155.py
+-rw-r--r--   0        0        0    68008 2023-03-21 21:23:13.237423 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc1155_claimable.py
+-rw-r--r--   0        0        0    80026 2023-03-21 21:23:13.237714 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc20.py
+-rw-r--r--   0        0        0    59394 2023-03-21 21:23:13.237980 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc20_claimable.py
+-rw-r--r--   0        0        0    80078 2023-03-21 21:23:13.238277 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc721.py
+-rw-r--r--   0        0        0    64449 2023-03-21 21:23:13.238530 thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc721_claimable.py
+-rw-r--r--   0        0        0     9165 2023-03-21 21:23:13.238692 thirdweb_sdk-3.0.2a3/thirdweb/abi/app_u_r_i.py
+-rw-r--r--   0        0        0     8936 2023-03-21 21:23:13.238839 thirdweb_sdk-3.0.2a3/thirdweb/abi/batch_mint_metadata.py
+-rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.238969 thirdweb_sdk-3.0.2a3/thirdweb/abi/context.py
+-rw-r--r--   0        0        0     9470 2023-03-21 21:23:13.239125 thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata.py
+-rw-r--r--   0        0        0     9520 2023-03-21 21:23:13.239295 thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata_logic.py
+-rw-r--r--   0        0        0     6115 2023-03-21 21:23:13.239442 thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata_storage.py
+-rw-r--r--   0        0        0    90485 2023-03-21 21:23:13.239903 thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_publisher.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.240119 thirdweb_sdk-3.0.2a3/thirdweb/abi/counters.py
+-rw-r--r--   0        0        0     5790 2023-03-21 21:23:13.240283 thirdweb_sdk-3.0.2a3/thirdweb/abi/currency_transfer_lib.py
+-rw-r--r--   0        0        0    12320 2023-03-21 21:23:13.240459 thirdweb_sdk-3.0.2a3/thirdweb/abi/default_operator_filterer.py
+-rw-r--r--   0        0        0    10109 2023-03-21 21:23:13.240627 thirdweb_sdk-3.0.2a3/thirdweb/abi/default_operator_filterer_upgradeable.py
+-rw-r--r--   0        0        0    21950 2023-03-21 21:23:13.240845 thirdweb_sdk-3.0.2a3/thirdweb/abi/delayed_reveal.py
+-rw-r--r--   0        0        0    76514 2023-03-21 21:23:13.241162 thirdweb_sdk-3.0.2a3/thirdweb/abi/direct_listings_logic.py
+-rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.241334 thirdweb_sdk-3.0.2a3/thirdweb/abi/direct_listings_storage.py
+-rw-r--r--   0        0        0    41239 2023-03-21 21:23:13.241551 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop.py
+-rw-r--r--   0        0        0    46630 2023-03-21 21:23:13.241777 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop1155.py
+-rw-r--r--   0        0        0   229869 2023-03-21 21:23:13.242485 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc1155.py
+-rw-r--r--   0        0        0   206478 2023-03-21 21:23:13.243046 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc20.py
+-rw-r--r--   0        0        0   243271 2023-03-21 21:23:13.243687 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc721.py
+-rw-r--r--   0        0        0    33157 2023-03-21 21:23:13.243907 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_single_phase.py
+-rw-r--r--   0        0        0    37416 2023-03-21 21:23:13.244123 thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_single_phase1155.py
+-rw-r--r--   0        0        0   241058 2023-03-21 21:23:13.244635 thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc1155_v2.py
+-rw-r--r--   0        0        0   226555 2023-03-21 21:23:13.245160 thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc20_v2.py
+-rw-r--r--   0        0        0   249102 2023-03-21 21:23:13.245721 thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc721_v3.py
+-rw-r--r--   0        0        0    43296 2023-03-21 21:23:13.245944 thirdweb_sdk-3.0.2a3/thirdweb/abi/dropsinglephase1155_v1.py
+-rw-r--r--   0        0        0    38914 2023-03-21 21:23:13.246156 thirdweb_sdk-3.0.2a3/thirdweb/abi/dropsinglephase_v1.py
+-rw-r--r--   0        0        0     3442 2023-03-21 21:23:13.246326 thirdweb_sdk-3.0.2a3/thirdweb/abi/e_i_p712_chainless_domain.py
+-rw-r--r--   0        0        0     3284 2023-03-21 21:23:13.246467 thirdweb_sdk-3.0.2a3/thirdweb/abi/ecdsa.py
+-rw-r--r--   0        0        0   156536 2023-03-21 21:23:13.246871 thirdweb_sdk-3.0.2a3/thirdweb/abi/edition_stake.py
+-rw-r--r--   0        0        0     3292 2023-03-21 21:23:13.247008 thirdweb_sdk-3.0.2a3/thirdweb/abi/eip712.py
+-rw-r--r--   0        0        0    64754 2023-03-21 21:23:13.247249 thirdweb_sdk-3.0.2a3/thirdweb/abi/english_auctions_logic.py
+-rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.247424 thirdweb_sdk-3.0.2a3/thirdweb/abi/english_auctions_storage.py
+-rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.247600 thirdweb_sdk-3.0.2a3/thirdweb/abi/enumerable_set.py
+-rw-r--r--   0        0        0    43189 2023-03-21 21:23:13.247814 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155.py
+-rw-r--r--   0        0        0   115583 2023-03-21 21:23:13.248175 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_base.py
+-rw-r--r--   0        0        0   139620 2023-03-21 21:23:13.248544 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_delayed_reveal.py
+-rw-r--r--   0        0        0   170049 2023-03-21 21:23:13.248978 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_drop.py
+-rw-r--r--   0        0        0    18760 2023-03-21 21:23:13.249150 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_holder.py
+-rw-r--r--   0        0        0   121380 2023-03-21 21:23:13.249486 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_lazy_mint.py
+-rw-r--r--   0        0        0   112914 2023-03-21 21:23:13.249801 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_preset_upgradeable.py
+-rw-r--r--   0        0        0    18357 2023-03-21 21:23:13.249969 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_receiver.py
+-rw-r--r--   0        0        0   134633 2023-03-21 21:23:13.250319 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_signature_mint.py
+-rw-r--r--   0        0        0     6858 2023-03-21 21:23:13.250859 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc165.py
+-rw-r--r--   0        0        0     6039 2023-03-21 21:23:13.251003 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1967_proxy.py
+-rw-r--r--   0        0        0     5644 2023-03-21 21:23:13.251135 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1967_upgrade.py
+-rw-r--r--   0        0        0    39698 2023-03-21 21:23:13.251312 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20.py
+-rw-r--r--   0        0        0    72167 2023-03-21 21:23:13.251539 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_base.py
+-rw-r--r--   0        0        0   104921 2023-03-21 21:23:13.251834 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_drop.py
+-rw-r--r--   0        0        0   136778 2023-03-21 21:23:13.252201 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_drop_vote.py
+-rw-r--r--   0        0        0    50917 2023-03-21 21:23:13.252406 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_permit.py
+-rw-r--r--   0        0        0    90382 2023-03-21 21:23:13.252677 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_signature_mint.py
+-rw-r--r--   0        0        0   122210 2023-03-21 21:23:13.253003 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_signature_mint_vote.py
+-rw-r--r--   0        0        0   103909 2023-03-21 21:23:13.253295 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_vote.py
+-rw-r--r--   0        0        0    82607 2023-03-21 21:23:13.253572 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_votes.py
+-rw-r--r--   0        0        0     6811 2023-03-21 21:23:13.253736 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context.py
+-rw-r--r--   0        0        0     7980 2023-03-21 21:23:13.253881 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_consumer.py
+-rw-r--r--   0        0        0     6856 2023-03-21 21:23:13.254037 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_logic.py
+-rw-r--r--   0        0        0     6079 2023-03-21 21:23:13.254191 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_storage.py
+-rw-r--r--   0        0        0     7631 2023-03-21 21:23:13.254332 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable.py
+-rw-r--r--   0        0        0     6955 2023-03-21 21:23:13.254489 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable_logic.py
+-rw-r--r--   0        0        0     6282 2023-03-21 21:23:13.254610 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable_storage.py
+-rw-r--r--   0        0        0    53696 2023-03-21 21:23:13.254828 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_a_upgradeable.py
+-rw-r--r--   0        0        0   119717 2023-03-21 21:23:13.255136 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_base.py
+-rw-r--r--   0        0        0   142298 2023-03-21 21:23:13.255489 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_delayed_reveal.py
+-rw-r--r--   0        0        0   169717 2023-03-21 21:23:13.255907 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_drop.py
+-rw-r--r--   0        0        0     8931 2023-03-21 21:23:13.256062 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_holder.py
+-rw-r--r--   0        0        0   124064 2023-03-21 21:23:13.256406 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_lazy_mint.py
+-rw-r--r--   0        0        0   182421 2023-03-21 21:23:13.256821 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_multiwrap.py
+-rw-r--r--   0        0        0   138584 2023-03-21 21:23:13.257156 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_signature_mint.py
+-rw-r--r--   0        0        0    52988 2023-03-21 21:23:13.257362 thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721a.py
+-rw-r--r--   0        0        0     3300 2023-03-21 21:23:13.257494 thirdweb_sdk-3.0.2a3/thirdweb/abi/fee_type.py
+-rw-r--r--   0        0        0    11166 2023-03-21 21:23:13.257651 thirdweb_sdk-3.0.2a3/thirdweb/abi/forwarder_consumer.py
+-rw-r--r--   0        0        0    26106 2023-03-21 21:23:13.257810 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc1155.py
+-rw-r--r--   0        0        0    10788 2023-03-21 21:23:13.257985 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc1155_claimable.py
+-rw-r--r--   0        0        0    25450 2023-03-21 21:23:13.258153 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc20.py
+-rw-r--r--   0        0        0    10033 2023-03-21 21:23:13.258293 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc20_claimable.py
+-rw-r--r--   0        0        0    25497 2023-03-21 21:23:13.258455 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc721.py
+-rw-r--r--   0        0        0    10043 2023-03-21 21:23:13.258592 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc721_claimable.py
+-rw-r--r--   0        0        0     9175 2023-03-21 21:23:13.258726 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_app_u_r_i.py
+-rw-r--r--   0        0        0     5661 2023-03-21 21:23:13.258854 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_beacon.py
+-rw-r--r--   0        0        0    11588 2023-03-21 21:23:13.258998 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc1155.py
+-rw-r--r--   0        0        0     9891 2023-03-21 21:23:13.259133 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc20.py
+-rw-r--r--   0        0        0     6533 2023-03-21 21:23:13.259256 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc721.py
+-rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.259376 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_condition.py
+-rw-r--r--   0        0        0     3474 2023-03-21 21:23:13.259510 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_condition_multi_phase.py
+-rw-r--r--   0        0        0    10930 2023-03-21 21:23:13.259648 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_conditions_single_phase.py
+-rw-r--r--   0        0        0    13127 2023-03-21 21:23:13.259788 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claimable_erc1155.py
+-rw-r--r--   0        0        0    11876 2023-03-21 21:23:13.259913 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claimable_erc721.py
+-rw-r--r--   0        0        0     7811 2023-03-21 21:23:13.260053 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_context.py
+-rw-r--r--   0        0        0    23449 2023-03-21 21:23:13.260235 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_deployer.py
+-rw-r--r--   0        0        0     8413 2023-03-21 21:23:13.260387 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_factory.py
+-rw-r--r--   0        0        0     9480 2023-03-21 21:23:13.260521 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_metadata.py
+-rw-r--r--   0        0        0    44219 2023-03-21 21:23:13.260712 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_publisher.py
+-rw-r--r--   0        0        0    11835 2023-03-21 21:23:13.260853 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_delayed_reveal.py
+-rw-r--r--   0        0        0    15264 2023-03-21 21:23:13.260989 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_delayed_reveal_deprecated.py
+-rw-r--r--   0        0        0    57624 2023-03-21 21:23:13.261211 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_direct_listings.py
+-rw-r--r--   0        0        0    20142 2023-03-21 21:23:13.261365 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop.py
+-rw-r--r--   0        0        0    21722 2023-03-21 21:23:13.261543 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop1155.py
+-rw-r--r--   0        0        0     3426 2023-03-21 21:23:13.261696 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_claim_condition.py
+-rw-r--r--   0        0        0    60183 2023-03-21 21:23:13.261901 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc1155.py
+-rw-r--r--   0        0        0    43180 2023-03-21 21:23:13.262090 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc20.py
+-rw-r--r--   0        0        0    66414 2023-03-21 21:23:13.262347 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc721.py
+-rw-r--r--   0        0        0    20224 2023-03-21 21:23:13.262510 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_single_phase.py
+-rw-r--r--   0        0        0    21804 2023-03-21 21:23:13.262667 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_single_phase1155.py
+-rw-r--r--   0        0        0    11373 2023-03-21 21:23:13.262807 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_edition_stake.py
+-rw-r--r--   0        0        0    55894 2023-03-21 21:23:13.263009 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_english_auctions.py
+-rw-r--r--   0        0        0     5838 2023-03-21 21:23:13.263163 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_enumerable.py
+-rw-r--r--   0        0        0     6466 2023-03-21 21:23:13.263300 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_metadata.py
+-rw-r--r--   0        0        0    18366 2023-03-21 21:23:13.263446 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_receiver.py
+-rw-r--r--   0        0        0     6575 2023-03-21 21:23:13.263588 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_supply.py
+-rw-r--r--   0        0        0     5815 2023-03-21 21:23:13.263713 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1822_proxiable.py
+-rw-r--r--   0        0        0     9937 2023-03-21 21:23:13.263831 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc20_metadata.py
+-rw-r--r--   0        0        0    14843 2023-03-21 21:23:13.263957 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc20_permit.py
+-rw-r--r--   0        0        0     6820 2023-03-21 21:23:13.264083 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc2771_context.py
+-rw-r--r--   0        0        0    10336 2023-03-21 21:23:13.264227 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_enumerable.py
+-rw-r--r--   0        0        0    10879 2023-03-21 21:23:13.264362 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_metadata.py
+-rw-r--r--   0        0        0     8622 2023-03-21 21:23:13.264491 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_receiver.py
+-rw-r--r--   0        0        0     5733 2023-03-21 21:23:13.264619 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_supply.py
+-rw-r--r--   0        0        0     7383 2023-03-21 21:23:13.264746 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_fee_tier_placement_extension.py
+-rw-r--r--   0        0        0     9333 2023-03-21 21:23:13.264861 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_lazy_mint.py
+-rw-r--r--   0        0        0     9955 2023-03-21 21:23:13.264991 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_lazy_mint_with_tier.py
+-rw-r--r--   0        0        0    68265 2023-03-21 21:23:13.265206 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_marketplace.py
+-rw-r--r--   0        0        0     8961 2023-03-21 21:23:13.265364 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc1155.py
+-rw-r--r--   0        0        0     7682 2023-03-21 21:23:13.265488 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc20.py
+-rw-r--r--   0        0        0     7691 2023-03-21 21:23:13.265603 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc721.py
+-rw-r--r--   0        0        0     6643 2023-03-21 21:23:13.265712 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_multicall.py
+-rw-r--r--   0        0        0    15555 2023-03-21 21:23:13.265837 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_multiwrap.py
+-rw-r--r--   0        0        0    11286 2023-03-21 21:23:13.265950 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_n_f_t_stake.py
+-rw-r--r--   0        0        0    32749 2023-03-21 21:23:13.266098 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_offers.py
+-rw-r--r--   0        0        0    94730 2023-03-21 21:23:13.266342 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_operator_filter_registry.py
+-rw-r--r--   0        0        0     9845 2023-03-21 21:23:13.266490 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_operator_filter_toggle.py
+-rw-r--r--   0        0        0     9391 2023-03-21 21:23:13.266630 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_ownable.py
+-rw-r--r--   0        0        0    19897 2023-03-21 21:23:13.266769 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_pack.py
+-rw-r--r--   0        0        0    31414 2023-03-21 21:23:13.266928 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_pack_v_r_f_direct.py
+-rw-r--r--   0        0        0    23527 2023-03-21 21:23:13.267072 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_permissions.py
+-rw-r--r--   0        0        0    30461 2023-03-21 21:23:13.267260 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_permissions_enumerable.py
+-rw-r--r--   0        0        0    11346 2023-03-21 21:23:13.267463 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_platform_fee.py
+-rw-r--r--   0        0        0    15146 2023-03-21 21:23:13.267593 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_plugin_map.py
+-rw-r--r--   0        0        0     9980 2023-03-21 21:23:13.267723 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_primary_sale.py
+-rw-r--r--   0        0        0    27471 2023-03-21 21:23:13.267868 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_router.py
+-rw-r--r--   0        0        0    27105 2023-03-21 21:23:13.268058 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_royalty.py
+-rw-r--r--   0        0        0     9998 2023-03-21 21:23:13.268194 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_action.py
+-rw-r--r--   0        0        0    16148 2023-03-21 21:23:13.268332 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc1155.py
+-rw-r--r--   0        0        0    15154 2023-03-21 21:23:13.268485 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc20.py
+-rw-r--r--   0        0        0    15923 2023-03-21 21:23:13.268633 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc721.py
+-rw-r--r--   0        0        0    27313 2023-03-21 21:23:13.268779 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking1155.py
+-rw-r--r--   0        0        0    19685 2023-03-21 21:23:13.268918 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking20.py
+-rw-r--r--   0        0        0    18920 2023-03-21 21:23:13.269054 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking721.py
+-rw-r--r--   0        0        0     7095 2023-03-21 21:23:13.269185 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_fee.py
+-rw-r--r--   0        0        0    26206 2023-03-21 21:23:13.269336 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_multichain_registry.py
+-rw-r--r--   0        0        0    21103 2023-03-21 21:23:13.269504 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_registry.py
+-rw-r--r--   0        0        0    13067 2023-03-21 21:23:13.269651 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_thirdweb_contract.py
+-rw-r--r--   0        0        0     3370 2023-03-21 21:23:13.269761 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_bundle.py
+-rw-r--r--   0        0        0    53182 2023-03-21 21:23:13.270402 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc1155.py
+-rw-r--r--   0        0        0    46867 2023-03-21 21:23:13.270660 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc20.py
+-rw-r--r--   0        0        0    58484 2023-03-21 21:23:13.271450 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc721.py
+-rw-r--r--   0        0        0    11351 2023-03-21 21:23:13.271592 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_stake.py
+-rw-r--r--   0        0        0    27443 2023-03-21 21:23:13.271753 thirdweb_sdk-3.0.2a3/thirdweb/abi/i_votes.py
+-rw-r--r--   0        0        0     3418 2023-03-21 21:23:13.271870 thirdweb_sdk-3.0.2a3/thirdweb/abi/iclaimcondition_v1.py
+-rw-r--r--   0        0        0     3450 2023-03-21 21:23:13.271980 thirdweb_sdk-3.0.2a3/thirdweb/abi/idropclaimcondition_v2.py
+-rw-r--r--   0        0        0    61520 2023-03-21 21:23:13.272188 thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc1155_v2.py
+-rw-r--r--   0        0        0    44262 2023-03-21 21:23:13.272388 thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc20_v2.py
+-rw-r--r--   0        0        0    67599 2023-03-21 21:23:13.272611 thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc721_v3.py
+-rw-r--r--   0        0        0    21795 2023-03-21 21:23:13.272779 thirdweb_sdk-3.0.2a3/thirdweb/abi/idropsinglephase1155_v1.py
+-rw-r--r--   0        0        0    20215 2023-03-21 21:23:13.272932 thirdweb_sdk-3.0.2a3/thirdweb/abi/idropsinglephase_v1.py
+-rw-r--r--   0        0        0    31974 2023-03-21 21:23:13.273101 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc1155.py
+-rw-r--r--   0        0        0     6867 2023-03-21 21:23:13.273333 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc165.py
+-rw-r--r--   0        0        0    24799 2023-03-21 21:23:13.273460 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc20.py
+-rw-r--r--   0        0        0    10953 2023-03-21 21:23:13.273598 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc2981.py
+-rw-r--r--   0        0        0    39092 2023-03-21 21:23:13.273809 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc721.py
+-rw-r--r--   0        0        0    49418 2023-03-21 21:23:13.274000 thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc721a.py
+-rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.274132 thirdweb_sdk-3.0.2a3/thirdweb/abi/init_storage.py
+-rw-r--r--   0        0        0     4108 2023-03-21 21:23:13.274281 thirdweb_sdk-3.0.2a3/thirdweb/abi/initializable.py
+-rw-r--r--   0        0        0    13842 2023-03-21 21:23:13.274439 thirdweb_sdk-3.0.2a3/thirdweb/abi/isignatureminterc721_v1.py
+-rw-r--r--   0        0        0    11782 2023-03-21 21:23:13.274565 thirdweb_sdk-3.0.2a3/thirdweb/abi/iweth.py
+-rw-r--r--   0        0        0    14519 2023-03-21 21:23:13.274700 thirdweb_sdk-3.0.2a3/thirdweb/abi/lazy_mint.py
+-rw-r--r--   0        0        0    19969 2023-03-21 21:23:13.274856 thirdweb_sdk-3.0.2a3/thirdweb/abi/lazy_mint_with_tier.py
+-rw-r--r--   0        0        0   156959 2023-03-21 21:23:13.275265 thirdweb_sdk-3.0.2a3/thirdweb/abi/marketplace.py
+-rw-r--r--   0        0        0   117081 2023-03-21 21:23:13.275601 thirdweb_sdk-3.0.2a3/thirdweb/abi/marketplace_v3.py
+-rw-r--r--   0        0        0     3276 2023-03-21 21:23:13.275761 thirdweb_sdk-3.0.2a3/thirdweb/abi/math.py
+-rw-r--r--   0        0        0     3362 2023-03-21 21:23:13.275902 thirdweb_sdk-3.0.2a3/thirdweb/abi/merkle_proof.py
+-rw-r--r--   0        0        0     9839 2023-03-21 21:23:13.276042 thirdweb_sdk-3.0.2a3/thirdweb/abi/mock.py
+-rw-r--r--   0        0        0     8147 2023-03-21 21:23:13.276190 thirdweb_sdk-3.0.2a3/thirdweb/abi/mock_contract.py
+-rw-r--r--   0        0        0    43400 2023-03-21 21:23:13.276392 thirdweb_sdk-3.0.2a3/thirdweb/abi/mock_contract_publisher.py
+-rw-r--r--   0        0        0     6634 2023-03-21 21:23:13.276550 thirdweb_sdk-3.0.2a3/thirdweb/abi/multicall.py
+-rw-r--r--   0        0        0   188886 2023-03-21 21:23:13.277020 thirdweb_sdk-3.0.2a3/thirdweb/abi/multiwrap.py
+-rw-r--r--   0        0        0   127828 2023-03-21 21:23:13.277343 thirdweb_sdk-3.0.2a3/thirdweb/abi/n_f_t_stake.py
+-rw-r--r--   0        0        0    41556 2023-03-21 21:23:13.277556 thirdweb_sdk-3.0.2a3/thirdweb/abi/offers_logic.py
+-rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.277742 thirdweb_sdk-3.0.2a3/thirdweb/abi/offers_storage.py
+-rw-r--r--   0        0        0     9837 2023-03-21 21:23:13.277906 thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filter_toggle.py
+-rw-r--r--   0        0        0    12250 2023-03-21 21:23:13.278071 thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filterer.py
+-rw-r--r--   0        0        0    10025 2023-03-21 21:23:13.278242 thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filterer_upgradeable.py
+-rw-r--r--   0        0        0     9381 2023-03-21 21:23:13.278404 thirdweb_sdk-3.0.2a3/thirdweb/abi/ownable.py
+-rw-r--r--   0        0        0   189507 2023-03-21 21:23:13.278843 thirdweb_sdk-3.0.2a3/thirdweb/abi/pack.py
+-rw-r--r--   0        0        0   192431 2023-03-21 21:23:13.279296 thirdweb_sdk-3.0.2a3/thirdweb/abi/pack_v_r_f_direct.py
+-rw-r--r--   0        0        0    42973 2023-03-21 21:23:13.279504 thirdweb_sdk-3.0.2a3/thirdweb/abi/payment_splitter_upgradeable.py
+-rw-r--r--   0        0        0    29535 2023-03-21 21:23:13.279694 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions.py
+-rw-r--r--   0        0        0    36480 2023-03-21 21:23:13.279895 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable.py
+-rw-r--r--   0        0        0    36540 2023-03-21 21:23:13.280089 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable_logic.py
+-rw-r--r--   0        0        0     6205 2023-03-21 21:23:13.280250 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable_storage.py
+-rw-r--r--   0        0        0    29595 2023-03-21 21:23:13.280415 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_logic.py
+-rw-r--r--   0        0        0     5980 2023-03-21 21:23:13.280568 thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_storage.py
+-rw-r--r--   0        0        0    11336 2023-03-21 21:23:13.280726 thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee.py
+-rw-r--r--   0        0        0    11386 2023-03-21 21:23:13.280882 thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee_logic.py
+-rw-r--r--   0        0        0     5985 2023-03-21 21:23:13.281049 thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee_storage.py
+-rw-r--r--   0        0        0    15127 2023-03-21 21:23:13.281212 thirdweb_sdk-3.0.2a3/thirdweb/abi/plugin_map.py
+-rw-r--r--   0        0        0     9970 2023-03-21 21:23:13.281363 thirdweb_sdk-3.0.2a3/thirdweb/abi/primary_sale.py
+-rw-r--r--   0        0        0     3400 2023-03-21 21:23:13.281512 thirdweb_sdk-3.0.2a3/thirdweb/abi/proxy.py
+-rw-r--r--   0        0        0     6116 2023-03-21 21:23:13.281669 thirdweb_sdk-3.0.2a3/thirdweb/abi/proxy_for_upgradeable.py
+-rw-r--r--   0        0        0     3394 2023-03-21 21:23:13.281808 thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard.py
+-rw-r--r--   0        0        0     3434 2023-03-21 21:23:13.281960 thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_logic.py
+-rw-r--r--   0        0        0     6097 2023-03-21 21:23:13.282103 thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_storage.py
+-rw-r--r--   0        0        0     4225 2023-03-21 21:23:13.282265 thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_upgradeable.py
+-rw-r--r--   0        0        0    38781 2023-03-21 21:23:13.282466 thirdweb_sdk-3.0.2a3/thirdweb/abi/router.py
+-rw-r--r--   0        0        0    39070 2023-03-21 21:23:13.282675 thirdweb_sdk-3.0.2a3/thirdweb/abi/router_immutable.py
+-rw-r--r--   0        0        0     5890 2023-03-21 21:23:13.282818 thirdweb_sdk-3.0.2a3/thirdweb/abi/router_storage.py
+-rw-r--r--   0        0        0    27102 2023-03-21 21:23:13.282994 thirdweb_sdk-3.0.2a3/thirdweb/abi/royalty.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283141 thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_cast.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.283262 thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_erc20.py
+-rw-r--r--   0        0        0     3308 2023-03-21 21:23:13.283384 thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_math.py
+-rw-r--r--   0        0        0     9992 2023-03-21 21:23:13.283531 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_action.py
+-rw-r--r--   0        0        0    10824 2023-03-21 21:23:13.283687 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_action_upgradeable.py
+-rw-r--r--   0        0        0   231932 2023-03-21 21:23:13.284160 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_drop.py
+-rw-r--r--   0        0        0    16142 2023-03-21 21:23:13.284389 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc1155.py
+-rw-r--r--   0        0        0    16979 2023-03-21 21:23:13.284556 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc1155_upgradeable.py
+-rw-r--r--   0        0        0    15148 2023-03-21 21:23:13.284777 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc20.py
+-rw-r--r--   0        0        0    15983 2023-03-21 21:23:13.284942 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc20_upgradeable.py
+-rw-r--r--   0        0        0    15917 2023-03-21 21:23:13.285134 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc721.py
+-rw-r--r--   0        0        0    16753 2023-03-21 21:23:13.285291 thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc721_upgradeable.py
+-rw-r--r--   0        0        0   237737 2023-03-21 21:23:13.285730 thirdweb_sdk-3.0.2a3/thirdweb/abi/signaturedrop_v4.py
+-rw-r--r--   0        0        0    42531 2023-03-21 21:23:13.285946 thirdweb_sdk-3.0.2a3/thirdweb/abi/soulbound_erc721_a.py
+-rw-r--r--   0        0        0   101885 2023-03-21 21:23:13.286193 thirdweb_sdk-3.0.2a3/thirdweb/abi/split.py
+-rw-r--r--   0        0        0    72420 2023-03-21 21:23:13.286430 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155.py
+-rw-r--r--   0        0        0   111245 2023-03-21 21:23:13.286697 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155_base.py
+-rw-r--r--   0        0        0    73314 2023-03-21 21:23:13.286919 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155_upgradeable.py
+-rw-r--r--   0        0        0    49004 2023-03-21 21:23:13.287115 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20.py
+-rw-r--r--   0        0        0    72923 2023-03-21 21:23:13.287329 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20_base.py
+-rw-r--r--   0        0        0    49928 2023-03-21 21:23:13.287516 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20_upgradeable.py
+-rw-r--r--   0        0        0    50405 2023-03-21 21:23:13.287702 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721.py
+-rw-r--r--   0        0        0    85256 2023-03-21 21:23:13.287922 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721_base.py
+-rw-r--r--   0        0        0    51319 2023-03-21 21:23:13.288130 thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721_upgradeable.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288248 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_address.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.288348 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_bit_maps.py
+-rw-r--r--   0        0        0    89887 2023-03-21 21:23:13.288497 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_factory.py
+-rw-r--r--   0        0        0    75523 2023-03-21 21:23:13.288703 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_fee.py
+-rw-r--r--   0        0        0    67405 2023-03-21 21:23:13.288905 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry.py
+-rw-r--r--   0        0        0    37213 2023-03-21 21:23:13.289082 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_logic.py
+-rw-r--r--   0        0        0    75392 2023-03-21 21:23:13.289301 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_router.py
+-rw-r--r--   0        0        0     6169 2023-03-21 21:23:13.289435 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_storage.py
+-rw-r--r--   0        0        0     3738 2023-03-21 21:23:13.289536 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_proxy.py
+-rw-r--r--   0        0        0    59703 2023-03-21 21:23:13.289758 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_registry.py
+-rw-r--r--   0        0        0     3378 2023-03-21 21:23:13.289874 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_storage_slot.py
+-rw-r--r--   0        0        0     3316 2023-03-21 21:23:13.289982 thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_strings.py
+-rw-r--r--   0        0        0   206242 2023-03-21 21:23:13.290372 thirdweb_sdk-3.0.2a3/thirdweb/abi/tiered_drop.py
+-rw-r--r--   0        0        0    15273 2023-03-21 21:23:13.290500 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_bundle.py
+-rw-r--r--   0        0        0   182279 2023-03-21 21:23:13.290887 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc1155.py
+-rw-r--r--   0        0        0   176744 2023-03-21 21:23:13.291274 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc20.py
+-rw-r--r--   0        0        0   185235 2023-03-21 21:23:13.291683 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc721.py
+-rw-r--r--   0        0        0   118802 2023-03-21 21:23:13.291949 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_stake.py
+-rw-r--r--   0        0        0    35792 2023-03-21 21:23:13.292111 thirdweb_sdk-3.0.2a3/thirdweb/abi/token_store.py
+-rw-r--r--   0        0        0    15519 2023-03-21 21:23:13.292243 thirdweb_sdk-3.0.2a3/thirdweb/abi/upgradeable.py
+-rw-r--r--   0        0        0   180710 2023-03-21 21:23:13.292582 thirdweb_sdk-3.0.2a3/thirdweb/abi/vote_erc20.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298098 thirdweb_sdk-3.0.2a3/thirdweb/common/__init__.py
+-rw-r--r--   0        0        0     4797 2023-03-13 04:51:11.298195 thirdweb_sdk-3.0.2a3/thirdweb/common/claim_conditions.py
+-rw-r--r--   0        0        0     4039 2023-03-13 04:51:11.298272 thirdweb_sdk-3.0.2a3/thirdweb/common/currency.py
+-rw-r--r--   0        0        0     2706 2023-03-13 04:51:11.298342 thirdweb_sdk-3.0.2a3/thirdweb/common/error.py
+-rw-r--r--   0        0        0     3962 2023-03-21 02:20:09.125984 thirdweb_sdk-3.0.2a3/thirdweb/common/feature_detection.py
+-rw-r--r--   0        0        0     4696 2023-03-13 04:51:11.298476 thirdweb_sdk-3.0.2a3/thirdweb/common/marketplace.py
+-rw-r--r--   0        0        0     4657 2023-03-13 04:51:11.298549 thirdweb_sdk-3.0.2a3/thirdweb/common/merkle_tree.py
+-rw-r--r--   0        0        0     2699 2023-03-13 04:51:11.298625 thirdweb_sdk-3.0.2a3/thirdweb/common/nft.py
+-rw-r--r--   0        0        0     1241 2023-03-13 04:51:11.298693 thirdweb_sdk-3.0.2a3/thirdweb/common/sign.py
+-rw-r--r--   0        0        0      287 2023-03-13 04:51:11.298753 thirdweb_sdk-3.0.2a3/thirdweb/common/signature_minting.py
+-rw-r--r--   0        0        0     2552 2023-03-13 04:51:11.298824 thirdweb_sdk-3.0.2a3/thirdweb/common/snapshots.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.298891 thirdweb_sdk-3.0.2a3/thirdweb/constants/__init__.py
+-rw-r--r--   0        0        0     3044 2023-03-13 04:51:11.298995 thirdweb_sdk-3.0.2a3/thirdweb/constants/addresses.py
+-rw-r--r--   0        0        0      284 2023-03-13 04:51:11.299055 thirdweb_sdk-3.0.2a3/thirdweb/constants/chains.py
+-rw-r--r--   0        0        0      182 2023-03-13 04:51:11.299107 thirdweb_sdk-3.0.2a3/thirdweb/constants/contract.py
+-rw-r--r--   0        0        0     2457 2023-03-13 04:51:11.299165 thirdweb_sdk-3.0.2a3/thirdweb/constants/currency.py
+-rw-r--r--   0        0        0      190 2023-03-13 04:51:11.299216 thirdweb_sdk-3.0.2a3/thirdweb/constants/events.py
+-rw-r--r--   0        0        0      983 2023-03-13 04:51:11.299284 thirdweb_sdk-3.0.2a3/thirdweb/constants/role.py
+-rw-r--r--   0        0        0      544 2023-03-13 04:51:11.299350 thirdweb_sdk-3.0.2a3/thirdweb/constants/rpc.py
+-rw-r--r--   0        0        0     1518 2023-03-13 04:51:11.299410 thirdweb_sdk-3.0.2a3/thirdweb/constants/urls.py
+-rw-r--r--   0        0        0      254 2023-03-13 04:51:11.299504 thirdweb_sdk-3.0.2a3/thirdweb/contracts/__init__.py
+-rw-r--r--   0        0        0     7736 2023-03-23 03:04:29.206870 thirdweb_sdk-3.0.2a3/thirdweb/contracts/custom.py
+-rw-r--r--   0        0        0     7869 2023-03-23 03:00:03.893613 thirdweb_sdk-3.0.2a3/thirdweb/contracts/edition.py
+-rw-r--r--   0        0        0     5786 2023-03-23 03:00:03.893922 thirdweb_sdk-3.0.2a3/thirdweb/contracts/edition_drop.py
+-rw-r--r--   0        0        0     1680 2023-03-13 04:51:11.299821 thirdweb_sdk-3.0.2a3/thirdweb/contracts/maps.py
+-rw-r--r--   0        0        0    12583 2023-03-22 00:51:09.363374 thirdweb_sdk-3.0.2a3/thirdweb/contracts/marketplace.py
+-rw-r--r--   0        0        0    12181 2023-03-21 02:20:09.126891 thirdweb_sdk-3.0.2a3/thirdweb/contracts/multiwrap.py
+-rw-r--r--   0        0        0     7456 2023-03-23 03:00:03.894216 thirdweb_sdk-3.0.2a3/thirdweb/contracts/nft_collection.py
+-rw-r--r--   0        0        0     8243 2023-03-23 03:00:03.894523 thirdweb_sdk-3.0.2a3/thirdweb/contracts/nft_drop.py
+-rw-r--r--   0        0        0     5787 2023-03-23 03:04:29.207062 thirdweb_sdk-3.0.2a3/thirdweb/contracts/token.py
+-rw-r--r--   0        0        0       29 2023-03-13 04:51:11.300414 thirdweb_sdk-3.0.2a3/thirdweb/core/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-13 04:51:11.300500 thirdweb_sdk-3.0.2a3/thirdweb/core/auth/__init__.py
+-rw-r--r--   0        0        0    13845 2023-03-13 04:51:11.300598 thirdweb_sdk-3.0.2a3/thirdweb/core/auth/wallet_authenticator.py
+-rw-r--r--   0        0        0        0 2023-03-13 04:51:11.300659 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/__init__.py
+-rw-r--r--   0        0        0     1318 2023-03-21 22:42:36.159881 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/base_contract.py
+-rw-r--r--   0        0        0     4014 2023-03-13 04:51:11.300801 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_deployer.py
+-rw-r--r--   0        0        0     3359 2023-03-23 03:04:29.207240 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_events.py
+-rw-r--r--   0        0        0     2110 2023-03-24 01:37:36.263013 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_metadata.py
+-rw-r--r--   0        0        0     1983 2023-03-24 01:37:36.263235 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_platform_fee.py
+-rw-r--r--   0        0        0     4275 2023-03-24 01:37:36.263461 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_roles.py
+-rw-r--r--   0        0        0     4231 2023-05-10 22:38:00.168091 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_royalty.py
+-rw-r--r--   0        0        0     1388 2023-03-24 01:37:36.263947 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_sales.py
+-rw-r--r--   0        0        0     5077 2023-03-21 22:42:35.046463 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_wrapper.py
+-rw-r--r--   0        0        0     2361 2023-03-13 04:51:11.301333 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/drop_claim_conditions.py
+-rw-r--r--   0        0        0     2722 2023-03-13 04:51:11.301386 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/drop_erc1155_claim_conditions.py
+-rw-r--r--   0        0        0    24253 2023-03-24 02:09:56.316705 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_1155.py
+-rw-r--r--   0        0        0     8047 2023-03-13 04:51:11.301549 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_1155_signature_minting.py
+-rw-r--r--   0        0        0     5534 2023-03-23 03:00:03.895228 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_1155_standard.py
+-rw-r--r--   0        0        0    11065 2023-03-24 01:37:36.264471 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_20.py
+-rw-r--r--   0        0        0     6733 2023-03-13 04:51:11.301730 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_20_signature_minting.py
+-rw-r--r--   0        0        0     6779 2023-03-23 03:00:03.895861 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_20_standard.py
+-rw-r--r--   0        0        0    23244 2023-03-24 01:37:46.685537 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_721.py
+-rw-r--r--   0        0        0     7822 2023-03-13 04:51:11.301886 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_721_signature_minting.py
+-rw-r--r--   0        0        0     5646 2023-03-23 03:00:03.896556 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_721_standard.py
+-rw-r--r--   0        0        0     6575 2023-03-13 04:51:11.301958 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/factory.py
+-rw-r--r--   0        0        0     9265 2023-03-13 04:51:11.302042 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/ipfs_storage.py
+-rw-r--r--   0        0        0    11102 2023-03-13 04:51:11.302151 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/marketplace_auction.py
+-rw-r--r--   0        0        0    12104 2023-03-13 04:51:11.302217 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/marketplace_direct.py
+-rw-r--r--   0        0        0     2764 2023-03-13 04:51:11.302278 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/provider_handler.py
+-rw-r--r--   0        0        0     1257 2023-03-13 04:51:11.302340 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/registry.py
+-rw-r--r--   0        0        0     4780 2023-03-13 04:51:11.302405 thirdweb_sdk-3.0.2a3/thirdweb/core/classes/sharded_merkle_tree.py
+-rw-r--r--   0        0        0     3227 2023-03-13 04:51:11.302500 thirdweb_sdk-3.0.2a3/thirdweb/core/helpers/storage.py
+-rw-r--r--   0        0        0     7739 2023-03-13 04:51:11.302575 thirdweb_sdk-3.0.2a3/thirdweb/core/sdk.py
+-rw-r--r--   0        0        0      254 2023-03-13 04:51:11.302670 thirdweb_sdk-3.0.2a3/thirdweb/types/__init__.py
+-rw-r--r--   0        0        0     1482 2023-03-13 04:51:11.302742 thirdweb_sdk-3.0.2a3/thirdweb/types/auth.py
+-rw-r--r--   0        0        0     1836 2023-03-23 03:00:03.896883 thirdweb_sdk-3.0.2a3/thirdweb/types/contract.py
+-rw-r--r--   0        0        0     3111 2023-03-13 04:51:11.302929 thirdweb_sdk-3.0.2a3/thirdweb/types/contracts/claim_conditions.py
+-rw-r--r--   0        0        0     5664 2023-03-13 04:51:11.303002 thirdweb_sdk-3.0.2a3/thirdweb/types/contracts/signature.py
+-rw-r--r--   0        0        0      528 2023-03-13 04:51:11.303061 thirdweb_sdk-3.0.2a3/thirdweb/types/currency.py
+-rw-r--r--   0        0        0      578 2023-03-13 04:51:11.303126 thirdweb_sdk-3.0.2a3/thirdweb/types/events.py
+-rw-r--r--   0        0        0     2519 2023-03-13 04:51:11.303186 thirdweb_sdk-3.0.2a3/thirdweb/types/marketplace.py
+-rw-r--r--   0        0        0      945 2023-03-13 04:51:11.303247 thirdweb_sdk-3.0.2a3/thirdweb/types/multiwrap.py
+-rw-r--r--   0        0        0     3574 2023-03-13 04:51:11.303318 thirdweb_sdk-3.0.2a3/thirdweb/types/nft.py
+-rw-r--r--   0        0        0     1084 2023-03-13 04:51:11.303390 thirdweb_sdk-3.0.2a3/thirdweb/types/sdk.py
+-rw-r--r--   0        0        0      329 2023-03-23 03:04:29.209187 thirdweb_sdk-3.0.2a3/thirdweb/types/settings/__init__.py
+-rw-r--r--   0        0        0     4111 2023-03-13 04:51:11.303569 thirdweb_sdk-3.0.2a3/thirdweb/types/settings/metadata.py
+-rw-r--r--   0        0        0      215 2023-03-13 04:51:11.303629 thirdweb_sdk-3.0.2a3/thirdweb/types/storage.py
+-rw-r--r--   0        0        0      334 2023-03-13 04:51:11.303692 thirdweb_sdk-3.0.2a3/thirdweb/types/tx.py
+-rw-r--r--   0        0        0     6696 1970-01-01 00:00:00.000000 thirdweb_sdk-3.0.2a3/PKG-INFO
```

### Comparing `thirdweb_sdk-3.0.2a2/LICENSE` & `thirdweb_sdk-3.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/README.md` & `thirdweb_sdk-3.0.2a3/README.md`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/pyproject.toml` & `thirdweb_sdk-3.0.2a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 authors = ["thirdweb <sdk@thirdweb.com>"]
 description = ""
 name = "thirdweb-sdk"
 packages = [
   {include = "thirdweb"},
 ]
 readme = "README.md"
-version = "3.0.2a2"
+version = "3.0.2a3"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1"
 dacite = "^1.6.0"
 mypy-extensions = "^0.4.3"
 thirdweb-contract-wrappers = "^2.0.4"
 web3 = "5.27.0"
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/.DS_Store` & `thirdweb_sdk-3.0.2a3/thirdweb/.DS_Store`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/__init__.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/__init__.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc1155_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc1155_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc20_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc20_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/airdrop_erc721_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/airdrop_erc721_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/app_u_r_i.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/app_u_r_i.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/batch_mint_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/batch_mint_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/context.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_metadata_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_metadata_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/contract_publisher.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/counters.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/counters.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/currency_transfer_lib.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/currency_transfer_lib.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/default_operator_filterer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/default_operator_filterer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/default_operator_filterer_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/default_operator_filterer_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/delayed_reveal.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/direct_listings_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/direct_listings_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/direct_listings_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/direct_listings_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_single_phase.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/drop_single_phase1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/drop_single_phase1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc1155_v2.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc1155_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc20_v2.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc20_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/droperc721_v3.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/droperc721_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/dropsinglephase1155_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/dropsinglephase1155_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/dropsinglephase_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/dropsinglephase_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/e_i_p712_chainless_domain.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/e_i_p712_chainless_domain.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ecdsa.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ecdsa.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/edition_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/edition_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/eip712.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/eip712.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/english_auctions_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/english_auctions_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/english_auctions_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/english_auctions_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/enumerable_set.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/enumerable_set.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_delayed_reveal.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_holder.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_holder.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_lazy_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_preset_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_preset_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_receiver.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1155_signature_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1155_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc165.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc165.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1967_proxy.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1967_proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc1967_upgrade.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc1967_upgrade.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_drop_vote.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_drop_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_permit.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_permit.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_signature_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_signature_mint_vote.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_signature_mint_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_vote.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_vote.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc20_votes.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc20_votes.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_consumer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_consumer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc2771_context_upgradeable_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc2771_context_upgradeable_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_a_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_a_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_delayed_reveal.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_holder.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_holder.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_lazy_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_multiwrap.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721_signature_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721_signature_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/erc721a.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/erc721a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/fee_type.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/fee_type.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/forwarder_consumer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/forwarder_consumer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc1155_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc1155_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc20_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc20_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_airdrop_erc721_claimable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_airdrop_erc721_claimable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_app_u_r_i.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_app_u_r_i.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_beacon.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_beacon.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_burnable_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_burnable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_condition.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_condition.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_condition_multi_phase.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_condition_multi_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claim_conditions_single_phase.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claim_conditions_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claimable_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claimable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_claimable_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_claimable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_context.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_deployer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_deployer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_factory.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_factory.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_contract_publisher.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_delayed_reveal.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_delayed_reveal.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_delayed_reveal_deprecated.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_delayed_reveal_deprecated.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_direct_listings.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_direct_listings.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_claim_condition.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_claim_condition.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_single_phase.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_single_phase.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_drop_single_phase1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_drop_single_phase1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_edition_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_edition_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_english_auctions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_english_auctions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_enumerable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_receiver.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1155_supply.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1155_supply.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc1822_proxiable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc1822_proxiable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc20_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc20_permit.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc20_permit.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc2771_context.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc2771_context.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_enumerable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_receiver.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_receiver.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_erc721_supply.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_erc721_supply.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_fee_tier_placement_extension.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_fee_tier_placement_extension.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_lazy_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_lazy_mint_with_tier.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_lazy_mint_with_tier.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_marketplace.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_mintable_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_mintable_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_multicall.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_multicall.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_multiwrap.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_n_f_t_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_n_f_t_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_offers.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_offers.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_operator_filter_registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_operator_filter_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_operator_filter_toggle.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_operator_filter_toggle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_ownable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_ownable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_pack.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_pack.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_pack_v_r_f_direct.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_pack_v_r_f_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_permissions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_permissions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_permissions_enumerable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_permissions_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_platform_fee.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_platform_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_plugin_map.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_plugin_map.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_primary_sale.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_primary_sale.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_router.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_royalty.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_royalty.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_action.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_action.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_signature_mint_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_signature_mint_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_staking721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_staking721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_fee.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_multichain_registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_multichain_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_t_w_registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_t_w_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_thirdweb_contract.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_thirdweb_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_bundle.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_bundle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_token_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_token_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/i_votes.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/i_votes.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/iclaimcondition_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/iclaimcondition_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idropclaimcondition_v2.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idropclaimcondition_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc1155_v2.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc1155_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc20_v2.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc20_v2.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idroperc721_v3.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idroperc721_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idropsinglephase1155_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idropsinglephase1155_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/idropsinglephase_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/idropsinglephase_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc165.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc165.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc2981.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc2981.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ierc721a.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ierc721a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/init_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/init_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/initializable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/initializable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/isignatureminterc721_v1.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/isignatureminterc721_v1.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/iweth.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/iweth.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/lazy_mint.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/lazy_mint.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/lazy_mint_with_tier.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/lazy_mint_with_tier.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/marketplace.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/marketplace_v3.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/marketplace_v3.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/math.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/math.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/merkle_proof.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/merkle_proof.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/mock.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/mock.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/mock_contract.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/mock_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/mock_contract_publisher.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/mock_contract_publisher.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/multicall.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/multicall.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/multiwrap.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/n_f_t_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/n_f_t_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/offers_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/offers_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/offers_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/offers_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filter_toggle.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filter_toggle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filterer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filterer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/operator_filterer_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/operator_filterer_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/ownable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/ownable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/pack.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/pack.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/pack_v_r_f_direct.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/pack_v_r_f_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/payment_splitter_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/payment_splitter_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_enumerable_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_enumerable_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/permissions_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/permissions_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/platform_fee_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/platform_fee_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/plugin_map.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/plugin_map.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/primary_sale.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/primary_sale.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/proxy.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/proxy_for_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/proxy_for_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/reentrancy_guard_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/reentrancy_guard_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/router.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/router_immutable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/router_immutable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/router_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/router_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/royalty.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/royalty.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_cast.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_cast.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/safe_math.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/safe_math.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_action.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_action.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_action_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_action_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc1155_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc1155_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc20_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc20_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signature_mint_erc721_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signature_mint_erc721_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/signaturedrop_v4.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/signaturedrop_v4.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/soulbound_erc721_a.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/soulbound_erc721_a.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/split.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/split.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking1155_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking1155_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking20_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking20_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721_base.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721_base.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/staking721_upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/staking721_upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_address.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_address.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_bit_maps.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_bit_maps.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_factory.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_factory.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_fee.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_fee.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_logic.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_logic.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_router.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_router.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_multichain_registry_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_multichain_registry_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_proxy.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_proxy.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_storage_slot.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_storage_slot.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/t_w_strings.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/t_w_strings.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/tiered_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/tiered_drop.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_bundle.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_bundle.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc1155.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc1155.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_erc721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_erc721.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_stake.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_stake.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/token_store.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/token_store.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/upgradeable.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/upgradeable.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/abi/vote_erc20.py` & `thirdweb_sdk-3.0.2a3/thirdweb/abi/vote_erc20.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/claim_conditions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/currency.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/error.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/error.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/feature_detection.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/feature_detection.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/marketplace.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/merkle_tree.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/nft.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/nft.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/sign.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/sign.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/common/snapshots.py` & `thirdweb_sdk-3.0.2a3/thirdweb/common/snapshots.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/constants/addresses.py` & `thirdweb_sdk-3.0.2a3/thirdweb/constants/addresses.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/constants/currency.py` & `thirdweb_sdk-3.0.2a3/thirdweb/constants/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/constants/role.py` & `thirdweb_sdk-3.0.2a3/thirdweb/constants/role.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/constants/rpc.py` & `thirdweb_sdk-3.0.2a3/thirdweb/constants/rpc.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/constants/urls.py` & `thirdweb_sdk-3.0.2a3/thirdweb/constants/urls.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/custom.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from web3 import Web3
 from web3.contract import ContractFunctions, ContractFunction
 from thirdweb.abi.token_erc1155 import TokenERC1155
 from thirdweb.abi.token_erc20 import TokenERC20
 from thirdweb.abi.token_erc721 import TokenERC721
 from thirdweb.common.error import NoSignerException
-from thirdweb.common.feature_detection import matches_interface
 from thirdweb.constants.role import ALL_ROLES
 from thirdweb.core.classes.base_contract import BaseContract
 from thirdweb.core.classes.contract_metadata import ContractMetadata
 from thirdweb.core.classes.contract_platform_fee import ContractPlatformFee
 from thirdweb.core.classes.contract_roles import ContractRoles
 from thirdweb.core.classes.contract_royalty import ContractRoyalty
 from thirdweb.core.classes.contract_sales import ContractPrimarySale
@@ -24,14 +23,15 @@
 from thirdweb.types.contract import ContractType
 from eth_account.account import LocalAccount
 from thirdweb.abi import (
     IPermissionsEnumerable,
     IRoyalty,
     IPrimarySale,
     IPlatformFee,
+    IContractMetadata,
 )
 
 from thirdweb.types.sdk import SDKOptions
 from thirdweb.types.settings.metadata import (
     CustomContractMetadata,
 )
 
@@ -87,14 +87,15 @@
         super().__init__(contract_wrapper)
 
         contract = provider.eth.contract(address=cast(Address, address), abi=abi)
         self.functions = contract.functions
 
         self._storage = storage
 
+        self.metadata = self._detect_metadata()
         self.roles = self._detect_roles()
         self.royalties = self._detect_royalties()
         self.sales = self._detect_primary_sales()
         self.platform_fee = self._detect_platform_fee()
 
         self.erc20 = self._detect_erc_20()
         self.erc721 = self._detect_erc_721()
@@ -147,74 +148,54 @@
 
             return provider.eth.wait_for_transaction_receipt(tx_hash)
 
     """
     INTERNAL FUNCTIONS
     """
 
-    def _detect_roles(self):
-        interface_to_match = self._get_interface_functions(IPermissionsEnumerable.abi())
+    def _detect_metadata(self):
+        contract_wrapper = self._get_contract_wrapper(IContractMetadata)
+        return ContractMetadata(
+            contract_wrapper,
+            self._storage,
+            CustomContractMetadata,
+        )
 
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(IPermissionsEnumerable)
-            return ContractRoles(contract_wrapper, ALL_ROLES)
-        return None
+    def _detect_roles(self):
+        contract_wrapper = self._get_contract_wrapper(IPermissionsEnumerable)
+        return ContractRoles(contract_wrapper, ALL_ROLES)
 
     def _detect_royalties(self):
-        interface_to_match = self._get_interface_functions(IRoyalty.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(IRoyalty)
-            metadata = ContractMetadata(
-                contract_wrapper,
-                self._storage,
-                CustomContractMetadata,
-            )
-            return ContractRoyalty(contract_wrapper, metadata)
-        return None
+        contract_wrapper = self._get_contract_wrapper(IRoyalty)
+        metadata = ContractMetadata(
+            contract_wrapper,
+            self._storage,
+            CustomContractMetadata,
+        )
+        return ContractRoyalty(contract_wrapper, metadata)
 
     def _detect_primary_sales(self):
-        interface_to_match = self._get_interface_functions(IPrimarySale.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(IPrimarySale)
-            return ContractPrimarySale(contract_wrapper)
-        return None
+        contract_wrapper = self._get_contract_wrapper(IPrimarySale)
+        return ContractPrimarySale(contract_wrapper)
 
     def _detect_platform_fee(self):
-        interface_to_match = self._get_interface_functions(IPlatformFee.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(IPlatformFee)
-            return ContractPlatformFee(contract_wrapper)
-        return None
+        contract_wrapper = self._get_contract_wrapper(IPlatformFee)
+        return ContractPlatformFee(contract_wrapper)
 
     def _detect_erc_20(self):
-        interface_to_match = self._get_interface_functions(TokenERC20.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(TokenERC20)
-            return ERC20(contract_wrapper, self._storage)
-        return None
+        contract_wrapper = self._get_contract_wrapper(TokenERC20)
+        return ERC20(contract_wrapper, self._storage)
 
     def _detect_erc_721(self):
-        interface_to_match = self._get_interface_functions(TokenERC721.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(TokenERC721)
-            return ERC721(contract_wrapper, self._storage)
-        return None
+        contract_wrapper = self._get_contract_wrapper(TokenERC721)
+        return ERC721(contract_wrapper, self._storage)
 
     def _detect_erc_1155(self):
-        interface_to_match = self._get_interface_functions(TokenERC1155.abi())
-
-        if matches_interface(self.functions, interface_to_match):
-            contract_wrapper = self._get_contract_wrapper(TokenERC1155)
-            return ERC1155(contract_wrapper, self._storage)
-        return None
+        contract_wrapper = self._get_contract_wrapper(TokenERC1155)
+        return ERC1155(contract_wrapper, self._storage)
 
     def _get_interface_functions(self, abi: str) -> ContractFunctions:
         return (
             self._contract_wrapper.get_provider()
             .eth.contract(
                 address=cast(
                     Address, self._contract_wrapper._contract_abi.contract_address
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/edition.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/edition.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,17 +90,15 @@
         """
         Mint a new NFT to the connected wallet
 
         :param metadata_with_supply: EditionMetadataInput for the NFT to mint
         :returns: receipt, id, and metadata of the mint
         """
 
-        return self.mint_to(
-            self._contract_wrapper.get_signer_address(), metadata_with_supply
-        )
+        return self._erc1155.mint(metadata_with_supply)
 
     def mint_to(
         self, to: str, metadata_with_supply: EditionMetadataInput
     ) -> TxResultWithId[EditionMetadata]:
         """
         Mint a new NFT to the specified wallet
 
@@ -125,73 +123,54 @@
         ```
 
         :param to: wallet address to mint the NFT to
         :param metadata_with_supply: EditionMetadataInput for the NFT to mint
         :returns: receipt, id, and metadata of the mint
         """
 
-        uri = upload_or_extract_uri(metadata_with_supply.metadata, self._storage)
-        receipt = self._contract_wrapper.send_transaction(
-            "mint_to", [to, int(MAX_INT, 16), uri, metadata_with_supply.supply]
-        )
-        events = self._contract_wrapper.get_events("TransferSingle", receipt)
-
-        if len(events) == 0:
-            raise Exception("No TransferSingle event found")
-
-        id = events[0].get("args").get("id")  # type: ignore
-
-        return TxResultWithId(receipt, id=id, data=lambda: self.get(id))
+        return self._erc1155.mint_to(to, metadata_with_supply)
 
     def mint_additional_supply(
         self, token_id: int, additional_supply: int
     ) -> TxResultWithId[EditionMetadata]:
         """
         Mint additional supply of a token to the connected wallet
 
         :param token_id: token ID to mint additional supply of
         :param additional_supply: additional supply to mint
         :returns: receipt, id, and metadata of the mint
         """
 
-        return self.mint_additional_supply_to(
-            self._contract_wrapper.get_signer_address(), token_id, additional_supply
-        )
+        return self._erc1155.mint_additional_supply(token_id, additional_supply)
 
     def mint_additional_supply_to(
         self, to: str, token_id: int, additional_supply: int
     ) -> TxResultWithId[EditionMetadata]:
         """
         Mint additional supply of a token to the specified wallet
 
         :param to: wallet address to mint additional supply to
         :param token_id: token ID to mint additional supply of
         :param additional_supply: additional supply to mint
         :returns: receipt, id, and metadata of the mint
         """
 
-        metadata = self._erc1155._get_token_metadata(token_id)
-        receipt = self._contract_wrapper.send_transaction(
-            "mint_to", [to, token_id, metadata.uri, additional_supply]
-        )
-        return TxResultWithId(receipt, id=token_id, data=lambda: self.get(token_id))
+        return self._erc1155.mint_additional_supply_to(to, token_id, additional_supply)
 
     def mint_batch(
         self, metadatas_with_supply: List[EditionMetadataInput]
     ) -> List[TxResultWithId[EditionMetadata]]:
         """
         Mint a batch of NFTs to the connected wallet
 
         :param metadatas_with_supply: list of EditionMetadataInput for the NFTs to mint
         :returns: receipts, ids, and metadatas of the mint
         """
 
-        return self.mint_batch_to(
-            self._contract_wrapper.get_signer_address(), metadatas_with_supply
-        )
+        return self._erc1155.mint_batch(metadatas_with_supply)
 
     def mint_batch_to(
         self, to: str, metadatas_with_supply: List[EditionMetadataInput]
     ) -> List[TxResultWithId[EditionMetadata]]:
         """
         Mint a batch of NFTs to the specified wallet
 
@@ -226,32 +205,8 @@
         ```
 
         :param to: wallet address to mint the NFTs to
         :param metadatas_with_supply: list of EditionMetadataInput for the NFTs to mint
         :returns: receipts, ids, and metadatas of the mint
         """
 
-        metadatas = [a.metadata for a in metadatas_with_supply]
-        supplies = [a.supply for a in metadatas_with_supply]
-        uris = upload_or_extract_uris(metadatas, self._storage)
-
-        encoded = []
-        interface = self._contract_wrapper.get_contract_interface()
-        for index, uri in enumerate(uris):
-            encoded.append(
-                interface.encodeABI(
-                    "mintTo", [to, int(MAX_INT, 16), uri, supplies[index]]
-                )
-            )
-
-        receipt = self._contract_wrapper.multi_call(encoded)
-        events = self._contract_wrapper.get_events("TokensMinted", receipt)
-
-        if len(events) == 0 and len(events) < len(metadatas):
-            raise Exception("No TokensMinted event found, minting failed")
-
-        results = []
-        for event in events:
-            id = event.get("args").get("tokenIdMinted")  # type: ignore
-            results.append(TxResultWithId(receipt, id=id, data=lambda: self.get(id)))
-
-        return results
+        return self._erc1155.mint_batch_to(to, metadatas_with_supply)
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/edition_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/edition_drop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from typing import Final, List, Optional
 
 from web3 import Web3
 from thirdweb.abi import DropERC1155
-from thirdweb.abi.drop_erc721 import IDropAllowlistProof
-from thirdweb.common.claim_conditions import prepare_claim
 from thirdweb.constants.role import Role
 from thirdweb.core.classes.contract_events import ContractEvents
 from thirdweb.core.classes.contract_metadata import ContractMetadata
 from thirdweb.core.classes.contract_platform_fee import ContractPlatformFee
 from thirdweb.core.classes.contract_roles import ContractRoles
 from thirdweb.core.classes.contract_royalty import ContractRoyalty
 from thirdweb.core.classes.contract_sales import ContractPrimarySale
 from thirdweb.core.classes.contract_wrapper import ContractWrapper
 from thirdweb.core.classes.erc_1155_standard import ERC1155Standard
 from thirdweb.core.classes.ipfs_storage import IpfsStorage
 from thirdweb.types.contract import ContractType
-from thirdweb.types.contracts.claim_conditions import ClaimVerification
 from thirdweb.types.nft import NFTMetadata, NFTMetadataInput
 from thirdweb.types.sdk import SDKOptions
 from thirdweb.types.settings.metadata import EditionDropContractMetadata
 from eth_account.account import LocalAccount
 from thirdweb.core.classes.drop_erc1155_claim_conditions import (
     DropERC1155ClaimConditions,
 )
-from zero_ex.contract_wrappers.tx_params import TxParams
 from thirdweb.types.tx import TxResultWithId
 from web3.eth import TxReceipt
 
 
 class EditionDrop(ERC1155Standard[DropERC1155]):
     """
     Setup a collection of NFTs with a customizable number of each NFT that are minted as users claim them.
@@ -119,49 +115,15 @@
         first_nft = txs[0].data()
         ```
 
         :param metadatas: List of NFT metadata inputs.
         :return: List of tx results with ids for created NFTs.
         """
 
-        start_file_number = (
-            self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
-        )
-        batch = self._storage.upload_metadata_batch(
-            [metadata.to_json() for metadata in metadatas],
-            start_file_number,
-            self._contract_wrapper._contract_abi.contract_address,
-            self._contract_wrapper.get_signer_address(),
-        )
-        base_uri = batch.base_uri
-
-        receipt = self._contract_wrapper.send_transaction(
-            "lazy_mint",
-            [
-                len(batch.metadata_uris),
-                base_uri if base_uri.endswith("/") else base_uri + "/",
-                Web3.toBytes(text=""),
-            ],
-        )
-
-        events = self._contract_wrapper.get_events("TokensLazyMinted", receipt)
-        start_index = events[0].get("args").get("startTokenId")  # type: ignore
-        ending_index = events[0].get("args").get("endTokenId")  # type: ignore
-        results = []
-
-        for id in range(start_index, ending_index + 1):
-            results.append(
-                TxResultWithId(
-                    receipt,
-                    id=id,
-                    data=lambda: self._erc1155._get_token_metadata(id),
-                )
-            )
-
-        return results
+        return self._erc1155.create_batch(metadatas)
 
     def claim_to(
         self,
         destination_address: str,
         token_id: int,
         quantity: int,
     ) -> TxReceipt:
@@ -182,71 +144,23 @@
         :param destination_address: Destination address to claim to.
         :param token_id: token ID of the token to claim.
         :param quantity: Number of NFTs to claim.
         :param proofs: List of merkle proofs.
         :return: tx receipt of the claim
         """
 
-        claim_verification = self._prepare_claim(token_id, quantity)
-        overrides: TxParams = TxParams(value=claim_verification.value)
-
-        proof = IDropAllowlistProof(
-            proof=claim_verification.proofs,
-            quantityLimitPerWallet=claim_verification.max_claimable,
-            pricePerToken=claim_verification.price_in_proof,
-            currency=claim_verification.currency_address_in_proof
-        )
-
-        return self._contract_wrapper.send_transaction(
-            "claim",
-            [
-                destination_address,
-                token_id,
-                quantity,
-                claim_verification.currency_address,
-                claim_verification.price,
-                proof,
-                "",
-            ],
-            overrides
-        )
+        return self._erc1155.claim_to(destination_address, token_id, quantity)
 
     def claim(
         self,
         token_id: int,
         quantity: int,
     ) -> TxReceipt:
         """
         Claim NFTs.
 
         :param quantity: Number of NFTs to claim.
         :param token_id: token ID of the token to claim.
         :param proofs: List of merkle proofs.
         :return: tx receipt of the claim
         """
-        return self.claim_to(
-            self._contract_wrapper.get_signer_address(),
-            token_id,
-            quantity,
-        )
-
-    """
-    INTERNAL FUNCTIONS
-    """
-
-    def _prepare_claim(
-        self,
-        token_id: int,
-        quantity: int,
-    ) -> ClaimVerification:
-        address_to_claim = self._contract_wrapper.get_signer_address()
-        active = self.claim_conditions.get_active(token_id)
-        merkle_metadata = self.metadata.get().merkle
-
-        return prepare_claim(
-            address_to_claim,
-            quantity,
-            active,
-            merkle_metadata,
-            self._contract_wrapper,
-            self._storage,
-        )
+        return self._erc1155.claim(token_id, quantity)
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/maps.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/maps.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/marketplace.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/multiwrap.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/nft_collection.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/nft_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
         Mint a new NFT to the connected wallet
 
         :param metadata: metadata of the NFT to mint
         :returns: receipt, id, and metadata for the mint
         """
 
-        return self.mint_to(self._contract_wrapper.get_signer_address(), metadata)
+        return self._erc721.mint(metadata)
 
     def mint_to(
         self, to: str, metadata: Union[NFTMetadataInput, str]
     ) -> TxResultWithId[NFTMetadataOwner]:
         """
         Mint a new NFT to the specified wallet
 
@@ -158,38 +158,27 @@
         ```
 
         :param to: wallet address to mint the NFT to
         :param metadata: metadata of the NFT to mint
         :returns: receipt, id, and metadata for the mint
         """
 
-        uri = upload_or_extract_uri(metadata, self._storage)
-        receipt = self._contract_wrapper.send_transaction("mint_to", [to, uri])
-        events = self._contract_wrapper.get_events("Transfer", receipt)
-
-        if len(events) == 0:
-            raise Exception("No Transfer event found")
-
-        id = events[0].get("args").get("tokenId")  # type: ignore
-
-        return TxResultWithId(receipt, id=id, data=lambda: self.get(id))
+        return self._erc721.mint_to(to, metadata)
 
     def mint_batch(
         self, metadatas: List[Union[NFTMetadataInput, str]]
     ) -> List[TxResultWithId[NFTMetadataOwner]]:
         """
         Mint a batch of new NFTs to the connected wallet
 
         :param metadatas: list of metadata of the NFTs to mint
         :returns: receipts, ids, and metadatas for each mint
         """
 
-        return self.mint_batch_to(
-            self._contract_wrapper.get_signer_address(), metadatas
-        )
+        return self._erc721.mint_batch(metadatas)
 
     def mint_batch_to(
         self, to: str, metadatas: List[Union[NFTMetadataInput, str]]
     ) -> List[TxResultWithId[NFTMetadataOwner]]:
         """
         Mint a batch of new NFTs to the specified wallet
 
@@ -218,26 +207,8 @@
         ```
 
         :param to: wallet address to mint the NFTs to
         :param metadatas: list of metadata of the NFTs to mint
         :returns: receipts, ids, and metadatas for each mint
         """
 
-        uris = upload_or_extract_uris(metadatas, self._storage)
-
-        encoded = []
-        interface = self._contract_wrapper.get_contract_interface()
-        for uri in uris:
-            encoded.append(interface.encodeABI("mintTo", [to, uri]))
-
-        receipt = self._contract_wrapper.multi_call(encoded)
-        events = self._contract_wrapper.get_events("TokensMinted", receipt)
-
-        if len(events) == 0 or len(events) < len(metadatas):
-            raise Exception("No TokensMinted event found, minting failed")
-
-        results = []
-        for event in events:
-            id = event.get("args").get("tokenIdMinted")  # type: ignore
-            results.append(TxResultWithId(receipt, id=id, data=lambda: self.get(id)))
-
-        return results
+        return self._erc721.mint_batch_to(to, metadatas)
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/nft_drop.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_20.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,367 +1,395 @@
-from typing import Final, List, Optional
-from thirdweb.abi import DropERC721
-from thirdweb.abi.drop_erc721 import IDropAllowlistProof
-from thirdweb.common.claim_conditions import prepare_claim
-from thirdweb.constants.role import Role
-from thirdweb.core.classes.contract_events import ContractEvents
-from thirdweb.core.classes.contract_metadata import ContractMetadata
-from thirdweb.core.classes.contract_platform_fee import ContractPlatformFee
-from thirdweb.core.classes.contract_roles import ContractRoles
-from thirdweb.core.classes.contract_royalty import ContractRoyalty
-from thirdweb.core.classes.contract_sales import ContractPrimarySale
+from typing import List
+from thirdweb.abi.token_erc20 import TokenERC20
+from thirdweb.common.currency import (
+    fetch_currency_metadata,
+    fetch_currency_value,
+    parse_units,
+)
+from thirdweb.constants.currency import ZERO_ADDRESS
+from thirdweb.constants.role import Role, get_role_hash
 from thirdweb.core.classes.contract_wrapper import ContractWrapper
-from thirdweb.core.classes.drop_claim_conditions import DropClaimConditions
-from thirdweb.core.classes.erc_721_standard import ERC721Standard
+from thirdweb.core.classes.base_contract import BaseContract
 from thirdweb.core.classes.ipfs_storage import IpfsStorage
-from thirdweb.types.contract import ContractType
-from thirdweb.types.contracts.claim_conditions import ClaimVerification
-from zero_ex.contract_wrappers.tx_params import TxParams
-from thirdweb.types.nft import (
-    NFTMetadata,
-    NFTMetadataInput,
-    NFTMetadataOwner,
-    QueryAllParams,
+from thirdweb.types.currency import (
+    Currency,
+    CurrencyValue,
+    Price,
+    PriceWei,
+    TokenAmount,
 )
-from thirdweb.types.sdk import SDKOptions
-from thirdweb.types.settings.metadata import NFTDropContractMetadata
-from eth_account.account import LocalAccount
-from web3 import Web3
+from web3.eth import TxReceipt
 
-from thirdweb.types.tx import TxResultWithId
 
+class ERC20(BaseContract[TokenERC20]):
+    _storage: IpfsStorage
 
-class NFTDrop(ERC721Standard[DropERC721]):
+    def __init__(
+        self,
+        contract_wrapper: ContractWrapper,
+        storage: IpfsStorage,
+    ):
+        super().__init__(contract_wrapper)
+        self._storage = storage
+
+    """
+    READ FUNCTIONS
     """
-    Setup a collection of one-of-one NFTs that are minted as users claim them.
 
-    ```python
-    from thirdweb import ThirdwebSDK
+    def get(self) -> Currency:
+        """
+        Get token metadata
 
-    # You can customize this to a supported network or your own RPC URL
-    network = "mumbai"
+        ```python
+        token = contract.erc20.get()
+        print(token)
+        ```
 
-    # Now we can create a new instance of the SDK
-    sdk = ThirdwebSDK(network)
+        :extension: ERC20
+        :returns: token metadata
+        """
 
-    # If you want to send transactions, you can instantiate the SDK with a private key instead:
-    #   sdk = ThirdwebSDK.from_private_key(PRIVATE_KEY, network)
+        return fetch_currency_metadata(
+            self._contract_wrapper.get_provider(), self.get_address()
+        )
 
-    contract = sdk.get_nft_drop("{{contract_address}}")
-    ```
-    """
+    def balance(self) -> CurrencyValue:
+        """
+        Get token balance
 
-    _abi_type = DropERC721
+        ```python
+        balance = contract.erc20.balance()
+        print(balance)
+        ```
 
-    contract_type: Final[ContractType] = ContractType.NFT_DROP
-    contract_roles: Final[List[Role]] = [Role.ADMIN, Role.MINTER, Role.TRANSFER]
+        :extension: ERC20
+        :returns: balance of the connected wallet
+        """
 
-    metadata: ContractMetadata[DropERC721, NFTDropContractMetadata]
-    roles: ContractRoles
-    primary_sale: ContractPrimarySale[DropERC721]
-    platform_fee: ContractPlatformFee[DropERC721]
-    royalty: ContractRoyalty[DropERC721]
-    claim_conditions: DropClaimConditions
-    events: ContractEvents[DropERC721]
+        return self.balance_of(self._contract_wrapper.get_signer_address())
 
-    def __init__(
-        self,
-        provider: Web3,
-        address: str,
-        storage: IpfsStorage,
-        signer: Optional[LocalAccount] = None,
-        options: SDKOptions = SDKOptions(),
-    ):
-        abi = DropERC721(provider, address)
-        contract_wrapper = ContractWrapper(abi, provider, signer, options)
-        super().__init__(contract_wrapper, storage)
+    def balance_of(self, address: str) -> CurrencyValue:
+        """
+        Get token balance of a specific wallet
 
-        self.metadata = ContractMetadata(
-            contract_wrapper, storage, NFTDropContractMetadata
-        )
-        self.roles = ContractRoles(contract_wrapper, self.contract_roles)
-        self.primary_sale = ContractPrimarySale(contract_wrapper)
-        self.platform_fee = ContractPlatformFee(contract_wrapper)
-        self.royalty = ContractRoyalty(contract_wrapper, self.metadata)
-        self.claim_conditions = DropClaimConditions(
-            self._contract_wrapper, self.metadata, self._storage
+        ```python
+        address = "{{wallet_address}}"
+        balance = contract.erc20.balance_of(address)
+        print(balance)
+        ```
+
+        :extension: ERC20
+        :param address: wallet address to check the balance of
+        :returns: balance of the specified wallet
+        """
+
+        return self._get_value(
+            self._contract_wrapper._contract_abi.balance_of.call(address)
         )
-        self.events = ContractEvents(contract_wrapper)
 
-    def get_owned(self, address: str = "") -> List[NFTMetadataOwner]:
+    def total_supply(self) -> CurrencyValue:
         """
-        Get the metadata of all tokens owned by a specific address
+        Get the total minted supply
 
         ```python
-        nfts = contract.get_owned("{{wallet_address}}")
-        print(nfts)
+        supply = contract.erc20.total_supply()
+        print(supply)
         ```
 
-        :param address: the address to get the metadata for
-        :return: the metadata of all tokens owned by the address
+        :extension: ERC20
+        :returns: total minted supply of the token
         """
 
-        token_ids = self.get_owned_token_ids(address)
-        return [self.get(token_id) for token_id in token_ids]
-
-    def get_owned_token_ids(self, address: str = "") -> List[int]:
-        """
-        Get the token IDs owned by a specific address
+        return self._get_value(self._contract_wrapper._contract_abi.total_supply.call())
 
-        :param address: the address to get the token IDs for
-        :return: the token IDs owned by the address
+    def allowance(self, spender: str) -> CurrencyValue:
         """
+        Get the allowance of a specific spender
 
-        owner = address if address else self._contract_wrapper.get_signer_address()
+        ```python
+        spender = "{{wallet_address}}"
+        allowance = contract.erc20.allowance(spender)
+        print(allowance)
+        ```
 
-        total_count = self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
-        token_ids = []
-        for i in range(total_count):
-            if self._contract_wrapper._contract_abi.owner_of.call(i).lower() == owner.lower():
-                token_ids.append(i)
+        :extension: ERC20
+        :param spender: wallet address to check the allowance of
+        :returns: allowance of the connected wallet
+        """
 
-        return token_ids
+        return self.allowance_of(self._contract_wrapper.get_signer_address(), spender)
 
-    def get_all_claimed(
-        self, query_params: QueryAllParams = QueryAllParams()
-    ) -> List[NFTMetadataOwner]:
+    def allowance_of(self, owner: str, spender: str) -> CurrencyValue:
         """
-        Get all claimed NFTs.
+        Get the allowance of a spender for a specific owner
 
         ```python
-        claimed_nfts = contract.get_all_claimed()
-        first_owner = claimed_nfts[0].owner
+        # Address of the wallet who owns the funds
+        address = "{{wallet_address}}"
+
+        # Address of the wallet to check the token allowance
+        spender = "0x..."
+
+        allowance = contract.erc20.allowance_of(address, spender)
+        print(allowance)
         ```
 
-        :param query_params: Query parameters.
-        :return: List of nft metadatas and owners for claimed nfts.
+        :extension: ERC20
+        :param owner: wallet address whose assets will be spent
+        :param spender: wallet address to check the allowance of
+        :returns: allowance of the specified spender for the specified owner
         """
 
-        max_id = min(
-            self._contract_wrapper._contract_abi.next_token_id_to_claim.call(),
-            query_params.start + query_params.count,
+        return self._get_value(
+            self._contract_wrapper._contract_abi.allowance.call(owner, spender)
         )
 
-        return [self.get(token_id) for token_id in range(query_params.start, max_id)]
-
-    def get_all_unclaimed(
-        self, query_params: QueryAllParams = QueryAllParams()
-    ) -> List[NFTMetadata]:
+    def is_transfer_restricted(self) -> bool:
         """
-        Get all unclaimed NFTs.
+        Check whether transfer is restricted for tokens in this module
 
         ```python
-        unclaimed_nfts = contract.get_all_unclaimed()
-        first_nft_name = unclaimed_nfts[0].name
+        is_restricted = contract.erc20.is_transfer_restricted()
+        print(is_restricted)
         ```
 
-        :param query_params: Query parameters.
-        :return: List of nft metadatas.
+        :returns: True if transfer is restricted, False otherwise
         """
 
-        max_id = min(
-            self._contract_wrapper._contract_abi.next_token_id_to_mint.call(),
-            query_params.start + query_params.count,
+        anyone_can_transfer = self._contract_wrapper._contract_abi.has_role.call(
+            get_role_hash(Role.TRANSFER), ZERO_ADDRESS
         )
-        unminted_id = self._contract_wrapper._contract_abi.next_token_id_to_claim.call()
 
-        return [
-            self._get_token_metadata(unminted_id + i)
-            for i in range(max_id - unminted_id)
-        ]
+        return not anyone_can_transfer
 
-    def total_claimed_supply(self) -> int:
+    """
+    WRITE FUNCTIONS
+    """
+
+    def mint(self, amount: Price) -> TxReceipt:
         """
-        Get the total number of NFTs claimed from this contract
+        Mint tokens
 
         ```python
-        total_claimed = contract.total_claimed_supply()
+        address = "{{wallet_address}}"
+        amount = 100
+
+        receipt = contract.erc20.mint(amount)
         ```
 
-        :return: Total number of NFTs claimed from this contract
+        :extension: ERC20Mintable
+        :param amount: amount of tokens to mint
+        :returns: transaction receipt of the mint
         """
-        return self._contract_wrapper._contract_abi.next_token_id_to_claim.call()
 
-    def total_unclaimed_supply(self) -> int:
+        return self.mint_to(self._contract_wrapper.get_signer_address(), amount)
+
+    def mint_to(self, to: str, amount: Price) -> TxReceipt:
         """
-        Get the total number of unclaimed NFTs in this contract
+        Mint tokens to a specific wallet
 
         ```python
-        total_unclaimed = contract.total_unclaimed_supply()
+        address = "{{wallet_address}}"
+        amount = 100
+
+        receipt = contract.erc20.mint_to(address, amount)
         ```
 
-        :return: Total number of unclaimed NFTs in this contract
+        :extension: ERC20Mintable
+        :param to: wallet address to mint tokens to
+        :param amount: amount of tokens to mint
+        :returns: transaction receipt of the mint
         """
-        return (
-            self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
-            - self.total_claimed_supply()
+
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction(
+            "mint_to", [to, amount_with_decimals]
         )
 
-    def create_batch(
-        self, metadatas: List[NFTMetadataInput]
-    ) -> List[TxResultWithId[NFTMetadata]]:
-        """
-        Create a batch of NFTs.
-
-        ```python
-        from thirdweb.types.nft import NFTMetadataInput
-
-        # You can customize this metadata however you like
-        metadatas = [
-            NFTMetadataInput.from_json({
-                "name": "Cool NFT",
-                "description": "This is a cool NFT",
-                "image": open("path/to/file.jpg", "rb"),
-            }),
-            NFTMetadataInput.from_json({
-                "name": "Cooler NFT",
-                "description": "This is a cooler NFT",
-                "image": open("path/to/file.jpg", "rb"),
-            }),
+    def mint_batch_to(self, args: List[TokenAmount]) -> TxReceipt:
+        """
+        Mint tokens to many wallets
+
+        ```python
+        from thirdweb.types.currency import TokenAmount
+
+        args = [
+            TokenAmount("{{wallet_address}}", 1),
+            TokenAmount("{{wallet_address}}", 2),
         ]
 
-        txs = contract.create_batch(metadatas)
-        first_token_id = txs[0].id
-        first_nft = txs[0].data()
+        :extension: ERC20BatchMintable
+        contract.erc20.mint_batch_to(args)
         ```
 
+        :param args: list of wallet addresses and amounts to mint
+        :returns: transaction receipt of the mint
+        """
 
-        :param metadatas: List of NFT metadata inputs.
-        :return: List of tx results with ids for created NFTs.
+        encoded = []
+        interface = self._contract_wrapper.get_contract_interface()
+        for arg in args:
+            encoded.append(
+                interface.encodeABI(
+                    "mintTo",
+                    [arg.to_address, parse_units(arg.amount, self.get().decimals)],
+                )
+            )
+        return self._contract_wrapper.multi_call(encoded)
+
+    def transfer(self, to: str, amount: Price) -> TxReceipt:
         """
+        Transfer tokens
 
-        start_file_number = (
-            self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
-        )
-        batch = self._storage.upload_metadata_batch(
-            [metadata.to_json() for metadata in metadatas],
-            start_file_number,
-            self._contract_wrapper._contract_abi.contract_address,
-            self._contract_wrapper.get_signer_address(),
-        )
-        base_uri = batch.base_uri
+        ```python
+        # Address to send tokens to
+        to = "0x...
 
-        receipt = self._contract_wrapper.send_transaction(
-            "lazy_mint",
-            [
-                len(batch.metadata_uris),
-                base_uri if base_uri.endswith("/") else base_uri + "/",
-                Web3.toBytes(text=""),
-            ],
-        )
+        # Amount of tokens to transfer
+        amount = 0.1
 
-        events = self._contract_wrapper.get_events("TokensLazyMinted", receipt)
-        start_index = events[0].get("args").get("startTokenId")  # type: ignore
-        ending_index = events[0].get("args").get("endTokenId")  # type: ignore
-        results = []
-
-        for id in range(start_index, ending_index + 1):
-            results.append(
-                TxResultWithId(
-                    receipt,
-                    id=id,
-                    data=lambda: self._get_token_metadata(id),
-                )
-            )
+        contract.erc20.transfer(to, amount)
+        ```
 
-        return results
+        :extension: ERC20
+        :param to: wallet address to transfer the tokens to
+        :param amount: amount of tokens to transfer
+        :returns: transaction receipt of the transfer
+        """
 
-    def claim_to(
-        self,
-        destination_address: str,
-        quantity: int,
-    ) -> List[TxResultWithId[NFTMetadata]]:
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction(
+            "transfer", [to, amount_with_decimals]
+        )
+
+    def transfer_from(self, fr: str, to: str, amount: Price) -> TxReceipt:
         """
-        Claim NFTs to a destination address.
+        Transfer tokens from a specific wallet
 
         ```python
-        address = {{wallet_address}}
-        quantity = 1
+        # Address to send tokens from
+        fr = "{{wallet_address}}"
+
+        # Address to send tokens to
+        to = "0x..."
 
-        tx = contract.claim_to(address, quantity)
-        receipt = tx.receipt
-        claimed_token_id = tx.id
-        claimed_nft = tx.data()
+        # Amount of tokens to transfer
+        amount = 0.1
+
+        contract.erc20.transfer_from(fr, to, amount)
         ```
 
-        :param destination_address: Destination address to claim to.
-        :param quantity: Number of NFTs to claim.
-        :param proofs: List of merkle proofs.
-        :return: List of tx results with ids for claimed NFTs.
+        :extension: ERC20
+        :param fr: wallet address to transfer the tokens from
+        :param to: wallet address to transfer the tokens to
+        :param amount: amount of tokens to transfer
+        :returns: transaction receipt of the transfer
         """
 
-        # TODO: OVERRIDES
-        claim_verification = self._prepare_claim(quantity)
-        overrides: TxParams = TxParams(value=claim_verification.value)
-
-        proof = IDropAllowlistProof(
-            proof=claim_verification.proofs,
-            quantityLimitPerWallet=claim_verification.max_claimable,
-            pricePerToken=claim_verification.price_in_proof,
-            currency=claim_verification.currency_address_in_proof
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction(
+            "transfer_from", [fr, to, amount_with_decimals]
         )
 
-        receipt = self._contract_wrapper.send_transaction(
-            "claim",
-            [
-                destination_address,
-                quantity,
-                claim_verification.currency_address,
-                claim_verification.price,
-                proof,
-                "",
-            ],
-            overrides
+    def set_allowance(self, spender: str, amount: Price) -> TxReceipt:
+        """
+        Approve a specific wallet to spend tokens
+
+        ```python
+        spender = "0x..."
+        amount = 100
+        contract.erc20.set_allowance(spender, amount)
+        ```
+
+        :extension: ERC20
+        :param spender: wallet address to set the allowance of
+        :param amount: amount to set the allowance to
+        :returns: transaction receipt of the allowance set
+        """
+
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction(
+            "approve", [spender, amount_with_decimals]
         )
 
-        events = self._contract_wrapper.get_events("TokensClaimed", receipt)
-        start_index = events[0].get("args").get("startTokenId")  # type: ignore
-        ending_index = start_index + quantity
-
-        results = []
-        for id in range(start_index, ending_index + 1):
-            results.append(
-                TxResultWithId(
-                    receipt,
-                    id=id,
-                    data=lambda: self._get_token_metadata(id),
-                )
+    def transfer_batch(self, args: List[TokenAmount]):
+        """
+        Transfer tokens to many wallets
+
+        ```python
+        from thirdweb.types.currency import TokenAmount
+
+        data = [
+            TokenAmount("{{wallet_address}}", 0.1),
+            TokenAmount("0x...", 0.2),
+        ]
+
+        contract.erc20.transfer_batch(data)
+        ```
+
+        :param args: list of token amounts and addressed to transfer to
+        :returns: transaction receipt of the transfers
+        """
+
+        encoded = []
+        interface = self._contract_wrapper.get_contract_interface()
+
+        for arg in args:
+            amount_with_decimals = self.normalize_amount(arg.amount)
+            encoded.append(
+                interface.encodeABI("transfer", [arg.to_address, amount_with_decimals])
             )
 
-        return results
+        return self._contract_wrapper.multi_call(encoded)
 
-    def claim(
-        self,
-        quantity: int,
-    ) -> List[TxResultWithId[NFTMetadata]]:
+    def burn(self, amount: Price) -> TxReceipt:
         """
-        Claim NFTs.
+        Burn tokens
+
+        ```python
+        amount = 0.1
+        contract.erc20.burn(amount)
+        ```
 
-        :param quantity: Number of NFTs to claim.
-        :param proofs: List of merkle proofs.
-        :return: List of tx results with ids for claimed NFTs.
-        """
-        return self.claim_to(
-            self._contract_wrapper.get_signer_address(),
-            quantity,
+        :extension: ERC20Burnable
+        :param amount: amount of tokens to burn
+        :returns: transaction receipt of the burn
+        """
+
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction("burn", [amount_with_decimals])
+
+    def burn_from(self, holder: str, amount: Price) -> TxReceipt:
+        """
+        Burn tokens from a specific wallet
+
+        ```python
+        holder = "{{wallet_address}}"
+        amount = 0.1
+        contract.erc20.burn_from(holder, amount)
+        ```
+
+        :extension: ERC20Burnable
+        :param holder: wallet address to burn the tokens from
+        :param amount: amount of tokens to burn
+        :returns: transaction receipt of the burn
+        """
+
+        amount_with_decimals = parse_units(amount, self.get().decimals)
+        return self._contract_wrapper.send_transaction(
+            "burn_from", [holder, amount_with_decimals]
         )
 
     """
     INTERNAL FUNCTIONS
     """
 
-    def _prepare_claim(
-        self,
-        quantity: int,
-    ) -> ClaimVerification:
-        address_to_claim = self._contract_wrapper.get_signer_address()
-        active = self.claim_conditions.get_active()
-        merkle_metadata = self.metadata.get().merkle
-
-        return prepare_claim(
-            address_to_claim,
-            quantity,
-            active,
-            merkle_metadata,
-            self._contract_wrapper,
-            self._storage,
+    def _get_value(self, value: PriceWei) -> CurrencyValue:
+        return fetch_currency_value(
+            self._contract_wrapper.get_provider(),
+            self.get_address(),
+            value,
         )
+
+    def normalize_amount(self, amount: Price) -> PriceWei:
+        decimals = self.get().decimals
+        return parse_units(amount, decimals)
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/contracts/token.py` & `thirdweb_sdk-3.0.2a3/thirdweb/contracts/token.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,33 +127,30 @@
         """
         Mint tokens to the connected wallet.
 
         :param amount: amount of tokens to mint
         :returns: transaction receipt of the mint
         """
 
-        return self.mint_to(self._contract_wrapper.get_signer_address(), amount)
+        return self._erc20.mint(amount)
 
     def mint_to(self, to: str, amount: Price) -> TxReceipt:
         """
         Mint tokens to a specified wallet.
 
         ```python
         contract.mint_to("{{wallet_address}}", 1)
         ```
 
         :param to: wallet address to mint tokens to
         :param amount: amount of tokens to mint
         :returns: transaction receipt of the mint
         """
 
-        amount_with_decimals = parse_units(amount, self.get().decimals)
-        return self._contract_wrapper.send_transaction(
-            "mint_to", [to, amount_with_decimals]
-        )
+        return self._erc20.mint_to(to, amount)
 
     def mint_batch_to(self, args: List[TokenAmount]) -> TxReceipt:
         """
         Mint tokens to a list of wallets.
 
         ```python
         from thirdweb.types.currency import TokenAmount
@@ -166,24 +163,15 @@
         contract.mint_batch_to(args)
         ```
 
         :param args: list of wallet addresses and amounts to mint
         :returns: transaction receipt of the mint
         """
 
-        encoded = []
-        interface = self._contract_wrapper.get_contract_interface()
-        for arg in args:
-            encoded.append(
-                interface.encodeABI(
-                    "mintTo",
-                    [arg.to_address, parse_units(arg.amount, self.get().decimals)],
-                )
-            )
-        return self._contract_wrapper.multi_call(encoded)
+        return self._erc20.mint_batch_to(args)
 
     def delegate_to(self, delegatee_address: str) -> TxReceipt:
         """
         Delegate the connected wallets tokens to a specified wallet.
 
         :param delegatee_address: wallet address to delegate tokens to
         :returns: transaction receipt of the delegation
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/auth/wallet_authenticator.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/auth/wallet_authenticator.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/base_contract.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/base_contract.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_deployer.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_deployer.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_events.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Callable, Dict, Generic, Tuple
 from thirdweb.constants.events import EventType
 from thirdweb.core.classes.contract_wrapper import ContractWrapper
 from thirdweb.types.contract import TContractABI
 from thirdweb.types.events import EventQueryOptions, TxEvent
 from web3.datastructures import AttributeDict
+
 class ContractEvents(Generic[TContractABI]):
     _contract_wrapper: ContractWrapper[TContractABI]
 
     def __init__(self, contract_wrapper: ContractWrapper[TContractABI]):
         self._contract_wrapper = contract_wrapper
 
     def add_transaction_listener(self, listener: Callable[[TxEvent], Any]):
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,47 @@
     ):
         self._contract_wrapper = contract_wrapper
         self._storage = storage
         self._schema = cast(TContractSchema, contract_schema)
 
     def get(self) -> TContractSchema:
         """
-        Get the metadata associated with this contract.
+        Get the contract metadata
 
+        ```python
+        metadata = contract.metadata.get()
+        print(metadata)
+        ```
+
+        :extension: ContractMetadata
         :returns: metadata associated with this contract
         """
 
         abi = self._contract_wrapper._contract_abi
         uri = abi.contract_uri.call()
         data = self._storage.get(uri)
         return cast(TContractSchema, self._schema.from_json(data))
 
     def set(self, metadata: TContractSchema) -> TxReceipt:
         """
-        Set the metadata associated with this contract.
+        Set the contract metadata
+
+        ```python
+        from thirdweb.types import ContractMetadataSchema
+
+        metadata = ContractMetadataSchema.from_json({
+            "name": "My Contract",
+            "description": "This is my contract!",
+            "image": open("path/to/file.jpg", "rb")
+        })
+
+        receipt = contract.metadata.set(metadata)
+        ```
 
+        :extension: ContractMetadata
         :param metadata: metadata to set
         :returns: transaction receipt of setting the metadata
         """
 
         uri = self._parse_and_upload_metadata(metadata.to_json())
         return self._contract_wrapper.send_transaction("set_contract_uri", [uri])
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_sales.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_sales.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,25 +8,38 @@
     _contract_wrapper: ContractWrapper[TPrimarySaleABI]
 
     def __init__(self, contract_wrapper: ContractWrapper[TPrimarySaleABI]):
         self._contract_wrapper = contract_wrapper
 
     def get_recipient(self) -> str:
         """
-        Get the primary sale recipient of this contract.
+        Get the contract primary sale recipient
 
+        ```python
+        primary_sale_recipient = contract.sales.get_recipient()
+        print(primary_sale_recipient)
+        ```
+
+        :extension: PrimarySale
         :returns: the address of the primary sale recipient.
         """
 
         return self._contract_wrapper._contract_abi.primary_sale_recipient.call()
 
     def set_recipient(self, recipient: str) -> TxReceipt:
         """
-        Set the primary sale recipient of this contract
+        Set the contract primary sale recipient
+
+        ```python
+        primary_sale_recipient = "{{wallet_address}}"
+
+        receipt = contract.sales.set_recipient(primary_sale_recipient)
+        ```
 
+        :extension: PrimarySale
         :param recipient: the address of the primary sale recipient.
         :returns: the transaction receipt.
         """
 
         return self._contract_wrapper.send_transaction(
             "set_primary_sale_recipient", [recipient]
         )
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/contract_wrapper.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/drop_claim_conditions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/drop_claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/drop_erc1155_claim_conditions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/drop_erc1155_claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_1155_signature_minting.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_1155_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_20_signature_minting.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_20_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_721.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/sdk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,223 +1,245 @@
-from typing import Generic, List
-from thirdweb.common.error import NotFoundException
-from thirdweb.common.nft import fetch_token_metadata
-from thirdweb.constants.currency import ZERO_ADDRESS
-from thirdweb.constants.role import Role, get_role_hash
-from thirdweb.core.classes.base_contract import BaseContract
-from thirdweb.core.classes.contract_wrapper import ContractWrapper
+from eth_account import Account
+from thirdweb.common.feature_detection import (
+    fetch_contract_metadata_from_address,
+)
+from thirdweb.constants.urls import get_provider_for_network
+from thirdweb.contracts import Marketplace
+from thirdweb.contracts.custom import CustomContract
+from thirdweb.contracts.edition_drop import EditionDrop
+from thirdweb.contracts.nft_drop import NFTDrop
+from thirdweb.contracts.multiwrap import Multiwrap
+from thirdweb.core.auth.wallet_authenticator import WalletAuthenticator
+from thirdweb.core.classes.contract_deployer import ContractDeployer
 from thirdweb.core.classes.ipfs_storage import IpfsStorage
-from thirdweb.types.contract import TERC721
-from thirdweb.types.nft import NFTMetadata, NFTMetadataOwner, QueryAllParams
-from web3.eth import TxReceipt
+from thirdweb.core.classes.provider_handler import ProviderHandler
+from thirdweb.contracts import Token, Edition, NFTCollection
 
+from eth_account.account import LocalAccount
+from typing import Any, Dict, Optional, Type, Union, cast
+from web3 import Web3
+
+from thirdweb.types.sdk import SDKOptions
+
+
+class ThirdwebSDK(ProviderHandler):
+    """
+    The main entry point for the Thirdweb SDK.
+    """
+
+    __contract_cache: Dict[
+        str,
+        Union[
+            NFTCollection,
+            Edition,
+            Token,
+            Marketplace,
+            NFTDrop,
+            EditionDrop,
+            Multiwrap,
+        ],
+    ] = {}
+    storage: IpfsStorage
+    auth: WalletAuthenticator
+    deployer: ContractDeployer
+
+    @staticmethod
+    def from_private_key(
+        private_key: str,
+        network: str,
+        options: SDKOptions = SDKOptions(),
+    ) -> "ThirdwebSDK":
+        signer = Account.from_key(private_key)
+        sdk = ThirdwebSDK(network, signer, options)
+        return sdk
 
-class ERC721(Generic[TERC721], BaseContract[TERC721]):
-    _storage: IpfsStorage
-
-    def __init__(self, contract_wrapper: ContractWrapper, storage: IpfsStorage):
-        super().__init__(contract_wrapper)
-        self._storage = storage
-
-    """
-    READ FUNCTIONS
-    """
-
-    def get(self, token_id: int) -> NFTMetadataOwner:
+    def __init__(
+        self,
+        network: str,
+        signer: Optional[LocalAccount] = None,
+        options: SDKOptions = SDKOptions(),
+        storage: IpfsStorage = IpfsStorage(),
+    ):
         """
-        Get metadata for a token
-
-        ```python
-        nft = contract.get(0)
-        print(nft)
-        ```
+        Initialize the thirdweb SDK.
 
-        :param token_id: token ID of the token to get the metadata for
-        :return: the metadata for the token and its owner
+        :param provider: web3 provider instance to use for getting on-chain data
+        :param signer: signer to use for sending transactions
+        :param options: optional SDK configuration options
+        :param storage: optional IPFS storage instance to use for storing data
         """
 
-        try:
-            owner = self.owner_of(token_id)
-        except:
-            owner = ZERO_ADDRESS
+        provider = get_provider_for_network(network)
+        super().__init__(provider, signer, options)
 
-        metadata = self._get_token_metadata(token_id)
-        return NFTMetadataOwner(metadata, owner)
+        self.auth = WalletAuthenticator(provider, signer, options)
+        self.deployer = ContractDeployer(provider, signer, options, storage)
+        self.storage = storage
 
-    def get_all(
-        self, query_params: QueryAllParams = QueryAllParams()
-    ) -> List[NFTMetadataOwner]:
+    def get_nft_collection(self, address: str) -> NFTCollection:
         """
-        Get the metadata of all tokens in the contract
-
-        ```python
-        nfts = contract.get_all()
-        print(nfts)
-        ```
+        Returns an NFT Collection contract SDK instance
 
-        :param query_params: optionally define a QueryAllParams instance to narrow the metadata query to specific tokens
-        :return: the metadata of all tokens in the contract
+        :param address: address of the NFT Collection contract
+        :returns: NFT Collection contract SDK instance
         """
 
-        max_id = min(query_params.start + query_params.count, self.get_total_count())
+        return cast(NFTCollection, self._get_contract(address, NFTCollection))
 
-        nfts = []
-        for token_id in range(query_params.start, max_id):
-            try:
-                nft = self.get(token_id)
-                nfts.append(nft)
-            except:
-                pass
-
-        return nfts
-
-    def get_total_count(self) -> int:
+    def get_edition(self, address: str) -> Edition:
         """
-        Get the total number of NFTs minted by this contract
+        Returns an Edition contract SDK instance
 
-        :return: the total number of NFTs minted by this contract
+        :param address: address of the Edition contract
+        :returns: Edition contract SDK instance
         """
 
-        return self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
+        return cast(Edition, self._get_contract(address, Edition))
 
-    def owner_of(self, token_id: int) -> str:
+    def get_token(self, address: str) -> Token:
         """
-        Get the owner of a token
+        Returns a Token contract SDK instance
 
-        :param token_id: the token ID of the token to get the owner of
-        :return: the owner of the token
+        :param address: address of the Token contract
+        :returns: Token contract SDK instance
         """
-        return self._contract_wrapper._contract_abi.owner_of.call(token_id)
 
-    def total_supply(
-        self,
-    ) -> int:
-        """
-        Get the total number of tokens in the contract
+        return cast(Token, self._get_contract(address, Token))
 
-        :return: the total number of tokens in the contract
+    def get_marketplace(self, address: str) -> Marketplace:
         """
-        return self._contract_wrapper._contract_abi.next_token_id_to_mint.call()
+        Returns a Marketplace contract SDK instance
 
-    def balance(
-        self,
-    ) -> int:
+        :param address: address of the Marketplace contract
+        :returns: Marketplace contract SDK instance
         """
-        Get the token balance of the connected wallet
 
-        :return: the token balance of the connected wallet
-        """
-
-        return self.balance_of(self._contract_wrapper.get_signer_address())
+        return cast(Marketplace, self._get_contract(address, Marketplace))
 
-    def balance_of(self, address: str) -> int:
+    def get_nft_drop(self, address: str) -> NFTDrop:
         """
-        Get the token balance of a specific address
+        Returns an NFT Drop contract SDK instance
 
-        ```python
-        balance = contract.balance_of("{{wallet_address}}")
-        print(balance)
-        ```
-
-        :param address: the address to get the token balance of
+        :param address: address of the NFT Drop contract
+        :returns: NFT Drop contract SDK instance
         """
 
-        return self._contract_wrapper._contract_abi.balance_of.call(address)
+        return cast(NFTDrop, self._get_contract(address, NFTDrop))
 
-    def is_transfer_restricted(
-        self,
-    ) -> bool:
+    def get_edition_drop(self, address: str) -> EditionDrop:
         """
-        Check if the contract is restricted to transfers only by admins
+        Returns an Edition Drop contract SDK instance
 
-        :return: True if the contract is restricted to transfers only by admins, False otherwise
+        :param address: address of the Edition Drop contract
+        :returns: Edition Drop contract SDK instance
         """
 
-        anyone_can_transfer = self._contract_wrapper._contract_abi.has_role.call(
-            get_role_hash(Role.TRANSFER), ZERO_ADDRESS
-        )
-
-        return not anyone_can_transfer
+        return cast(EditionDrop, self._get_contract(address, EditionDrop))
 
-    def is_approved(self, address: str, operator: str) -> bool:
+    def get_multiwrap(self, address: str) -> Multiwrap:
         """
-        Check whether an operator address is approved for all operations of a specific addresses assets
+        Returns a multiwrap contract SDK instance
 
-        :param address: the address whose assets are to be checked
-        :param operator: the address of the operator to check
-        :return: True if the operator is approved for all operations of the assets, False otherwise
+        :param address: address of the multiwrap contract
+        :returns: multiwrap contract SDK instance
         """
 
-        return self._contract_wrapper._contract_abi.is_approved_for_all.call(
-            address, operator
-        )
+        return cast(Multiwrap, self._get_contract(address, Multiwrap))
 
-    """
-    WRITE FUNCTIONS
-    """
+    def get_contract(self, address: str) -> CustomContract:
+        """
+        Returns a custom contract SDK instance
 
-    def transfer(self, to: str, token_id: int) -> TxReceipt:
+        :param address: address of the custom contract
+        :returns: custom contract SDK instance
         """
-        Transfer a specified token from the connected wallet to a specified address.
 
-        ```python
-        to = "{{wallet_address}}"
-        token_id = 0
+        if address in self.__contract_cache:
+            return cast(CustomContract, self.__contract_cache[address])
 
-        receipt = contract.transfer(to, token_id)
-        ```
+        try:
+            provider = self.get_provider()
+            abi = fetch_contract_metadata_from_address(address, provider, self.storage)
+            return self.get_contract_from_abi(address, abi)
+        except:
+            raise Exception(f"Error fetching ABI for this contract\n{address}")
 
-        :param to: wallet address to transfer the tokens to
-        :param token_id: the specific token ID to transfer
-        :returns: transaction receipt of the transfer
+    def get_contract_from_abi(self, address: str, abi: str) -> CustomContract:
         """
+        Returns a custom contract SDK instance given the contract ABI
 
-        fr = self._contract_wrapper.get_signer_address()
-        return self._contract_wrapper.send_transaction(
-            "safe_transfer_from1", [fr, to, token_id]
-        )
-
-    def burn(self, token_id: int) -> TxReceipt:
+        :param address: address of the custom contract
+        :param abi: abi of the custom contract
+        :returns: custom contract SDK instance
         """
-        Burn a specified token from the connected wallet.
 
-        :param token_id: token ID of the token to burn
-        :returns: transaction receipt of the burn
-        """
+        if address in self.__contract_cache:
+            return cast(CustomContract, self.__contract_cache[address])
 
-        return self._contract_wrapper.send_transaction("burn", [token_id])
+        provider = self.get_provider()
+        contract = CustomContract(
+            provider,
+            address,
+            abi,
+            self.storage,
+            self.get_signer(),
+            self.get_options(),
+        )
+        self.__contract_cache[address] = cast(Any, contract)
+        return contract
 
-    def set_approval_for_all(self, operator: str, approved: bool) -> TxReceipt:
+    def update_provider(self, provider: Web3):
         """
-        Set the approval of an operator for all operations of a specific address's assets
+        Update the provider instance used by the SDK.
 
-        :param operator: the address of the operator to set the approval for
-        :param approved: the address whos assets the operator is approved to manage
-        :returns: transaction receipt of the approval
+        :param provider: web3 provider instance to use for getting on-chain data
         """
 
-        return self._contract_wrapper.send_transaction(
-            "set_approval_for_all", [operator, approved]
-        )
+        super()._update_provider(provider)
+        self.auth._update_provider(provider)
+        self.deployer._update_provider(provider)
+
+        for contract in self.__contract_cache.values():
+            contract.on_provider_updated(provider)
 
-    def set_approval_for_token(self, operator: str, token_id: int) -> TxReceipt:
+    def update_signer(self, signer: Optional[LocalAccount] = None):
         """
-        Approve an operator for the NFT owner, which allows the operator to call transferFrom
-        or safeTransferFrom for the specified token.
+        Update the signer instance used by the SDK.
 
-        :param operator: the address of the operator to set the approval for
-        :param token_id: the specific token ID to set the approval for
-        :returns: transaction receipt of the approval
+        :param signer: signer to use for sending transactions
         """
-        return self._contract_wrapper.send_transaction("approve", [operator, token_id])
 
-    """
-    INTERNAL FUNCTIONS
-    """
+        super()._update_signer(signer)
+        self.auth._update_signer(signer)
+        self.deployer._update_signer(signer)
 
-    def _get_token_metadata(self, token_id: int) -> NFTMetadata:
-        token_uri = self._contract_wrapper._contract_abi.token_uri.call(token_id)
+        for contract in self.__contract_cache.values():
+            contract.on_signer_updated(signer)
 
-        if not token_uri:
-            raise NotFoundException(str(token_id))
+    def _get_contract(
+        self,
+        address: str,
+        contract_type: Union[
+            Type[NFTCollection],
+            Type[Edition],
+            Type[Token],
+            Type[Marketplace],
+            Type[NFTDrop],
+            Type[EditionDrop],
+            Type[Multiwrap],
+        ],
+    ) -> Union[
+        NFTCollection, Edition, Token, Marketplace, NFTDrop, EditionDrop, Multiwrap
+    ]:
+        if address in self.__contract_cache:
+            return self.__contract_cache[address]
+
+        contract = contract_type(
+            self.get_provider(),
+            address,
+            self.storage,
+            self.get_signer(),
+            self.get_options(),
+        )
 
-        return fetch_token_metadata(token_id, token_uri, self._storage)
+        self.__contract_cache[address] = contract
+        return contract
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/erc_721_signature_minting.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/erc_721_signature_minting.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/factory.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/factory.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/ipfs_storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/ipfs_storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/marketplace_auction.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/marketplace_auction.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/marketplace_direct.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/marketplace_direct.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/provider_handler.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/provider_handler.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/registry.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/registry.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/classes/sharded_merkle_tree.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/classes/sharded_merkle_tree.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/core/helpers/storage.py` & `thirdweb_sdk-3.0.2a3/thirdweb/core/helpers/storage.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/auth.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/auth.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/contract.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/contract.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
     IERC20,
     IERC721,
     IERC1155,
     DropERC721,
     DropERC1155,
     Multiwrap,
 )
+from thirdweb.abi.i_mintable_erc20 import IMintableERC20
 from thirdweb.types.settings.metadata import ContractMetadataSchema
 
-
 TContractABI = TypeVar(
     "TContractABI",
     bound=Union[
         TokenERC721,
         TokenERC1155,
         TokenERC20,
         Marketplace,
@@ -28,14 +28,15 @@
         IERC721,
         IERC1155,
         TWRegistry,
         TWFactory,
         DropERC721,
         DropERC1155,
         Multiwrap,
+        IMintableERC20
     ],
 )
 
 TERC721 = TypeVar("TERC721", bound=Union[TokenERC721, DropERC721, Multiwrap])
 TERC1155 = TypeVar("TERC1155", bound=Union[TokenERC1155, DropERC1155])
 
 TPrimarySaleABI = TypeVar(
@@ -66,15 +67,14 @@
         DropERC1155,
         Multiwrap,
     ],
 )
 
 TContractSchema = TypeVar("TContractSchema", bound=ContractMetadataSchema)
 
-
 class ContractType(Enum):
     NFT_COLLECTION = "nft-collection"
     EDITION = "edition"
     TOKEN = "token"
     MARKETPLACE = "marketplace"
     NFT_DROP = "nft-drop"
     EDITION_DROP = "edition-drop"
```

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/contracts/claim_conditions.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/contracts/claim_conditions.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/contracts/signature.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/contracts/signature.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/currency.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/currency.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/events.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/events.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/marketplace.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/marketplace.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/multiwrap.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/multiwrap.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/nft.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/nft.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/sdk.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/sdk.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/thirdweb/types/settings/metadata.py` & `thirdweb_sdk-3.0.2a3/thirdweb/types/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `thirdweb_sdk-3.0.2a2/PKG-INFO` & `thirdweb_sdk-3.0.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thirdweb-sdk
-Version: 3.0.2a2
+Version: 3.0.2a3
 Summary: 
 Author: thirdweb
 Author-email: sdk@thirdweb.com
 Requires-Python: >=3.7.1
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thirdweb-sdk Version: 3.0.2a2 Summary: Author:
+Metadata-Version: 2.1 Name: thirdweb-sdk Version: 3.0.2a3 Summary: Author:
 thirdweb Author-email: sdk@thirdweb.com Requires-Python: >=3.7.1 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: cbor2 (>=5.4.3,<6.0.0) Requires-Dist: dacite
 (>=1.6.0,<2.0.0) Requires-Dist: mypy-extensions (>=0.4.3,<0.5.0) Requires-Dist:
 pyee (>=9.0.4,<10.0.0) Requires-Dist: pymerkle (>=2.0.2,<3.0.0) Requires-Dist:
```

