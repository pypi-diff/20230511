# Comparing `tmp/lightspark-1.0.0.tar.gz` & `tmp/lightspark-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightspark-1.0.0.tar", last modified: Tue Apr 11 01:37:33 2023, max compression
+gzip compressed data, was "lightspark-1.1.0.tar", last modified: Thu May 11 01:10:18 2023, max compression
```

## Comparing `lightspark-1.0.0.tar` & `lightspark-1.1.0.tar`

### file list

```diff
@@ -1,114 +1,117 @@
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.574119 lightspark-1.0.0/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      355 2023-04-11 01:37:33.574119 lightspark-1.0.0/PKG-INFO
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      609 2023-04-11 01:22:43.000000 lightspark-1.0.0/README.md
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.570119 lightspark-1.0.0/lightspark/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     6429 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/__init__.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      185 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/exceptions.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    18945 2023-04-11 01:20:58.000000 lightspark-1.0.0/lightspark/lightspark_client.py
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.574119 lightspark-1.0.0/lightspark/objects/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    71959 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Account.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1925 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/AccountToApiTokensConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1307 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/AccountToChannelsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     2653 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/AccountToNodesConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     2053 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/AccountToPaymentRequestsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4712 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/AccountToTransactionsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1899 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ApiToken.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      782 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/BitcoinNetwork.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     5279 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/BlockchainBalance.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    13660 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Channel.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     5395 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ChannelClosingTransaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1351 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ChannelFees.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     5366 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ChannelOpeningTransaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1456 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ChannelStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     3668 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/ChannelToTransactionsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      736 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateApiTokenInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1448 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateApiTokenOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      828 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateInvoiceInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      659 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateInvoiceOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      393 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateNodeWalletAddressInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      898 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CreateNodeWalletAddressOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     5550 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CurrencyAmount.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1345 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/CurrencyUnit.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      371 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/DeleteApiTokenInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      668 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/DeleteApiTokenOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4573 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Deposit.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    45969 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Entity.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1654 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/FeeEstimate.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      429 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/FundNodeInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1134 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/FundNodeOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4484 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/GraphNode.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     3451 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Hop.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1752 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/HtlcAttemptFailureCode.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     6081 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/IncomingPayment.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     3001 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/IncomingPaymentAttempt.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      558 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/IncomingPaymentAttemptStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1555 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    10747 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Invoice.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     9364 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/InvoiceData.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      487 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/InvoiceType.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      962 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      851 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1324 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightningFeeEstimateOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    20160 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightningTransaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    20327 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightsparkNode.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      429 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightsparkNodePurpose.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      612 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightsparkNodeStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1983 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    13646 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Node.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1035 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/NodeAddress.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      512 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/NodeAddressType.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1499 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/NodeToAddressesConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    14387 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OnChainTransaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    16999 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OutgoingPayment.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     7538 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttempt.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      536 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1533 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1538 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      994 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PageInfo.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1158 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PayInvoiceInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      680 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PayInvoiceOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      684 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PaymentFailureReason.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    11545 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PaymentRequest.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    10106 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PaymentRequestData.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      402 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/PaymentRequestStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      842 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Permission.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1213 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/RequestWithdrawalInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      746 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/RequestWithdrawalOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      534 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/RichText.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     5504 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/RoutingTransaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      523 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/RoutingTransactionFailureReason.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      653 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Secret.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1095 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/SendPaymentInput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      687 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/SendPaymentOutput.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    31911 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Transaction.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      978 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/TransactionFailures.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      885 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/TransactionStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1632 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/TransactionType.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      432 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WebhookEventType.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4674 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/Withdrawal.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      438 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WithdrawalMode.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    10802 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WithdrawalRequest.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      449 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WithdrawalRequestStatus.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     2457 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     2457 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       75 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/__init__.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)    10333 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/objects/all_entities.py
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.574119 lightspark-1.0.0/lightspark/requests/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       75 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/requests/__init__.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      416 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/requests/encoder.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4304 2023-04-11 01:22:43.000000 lightspark-1.0.0/lightspark/requests/requester.py
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.574119 lightspark-1.0.0/lightspark/utils/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       75 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/utils/__init__.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     3673 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/utils/crypto.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     1146 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/utils/enums.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       22 2023-04-11 01:22:43.000000 lightspark-1.0.0/lightspark/version.py
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     2214 2023-04-10 23:43:15.000000 lightspark-1.0.0/lightspark/webhooks.py
-drwxrwxr-x   0 mgorven   (1000) mgorven   (1000)        0 2023-04-11 01:37:33.570119 lightspark-1.0.0/lightspark.egg-info/
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      355 2023-04-11 01:37:33.000000 lightspark-1.0.0/lightspark.egg-info/PKG-INFO
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)     4177 2023-04-11 01:37:33.000000 lightspark-1.0.0/lightspark.egg-info/SOURCES.txt
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)        1 2023-04-11 01:37:33.000000 lightspark-1.0.0/lightspark.egg-info/dependency_links.txt
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       22 2023-04-11 01:37:33.000000 lightspark-1.0.0/lightspark.egg-info/requires.txt
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       11 2023-04-11 01:37:33.000000 lightspark-1.0.0/lightspark.egg-info/top_level.txt
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)       81 2023-04-10 23:43:15.000000 lightspark-1.0.0/pyproject.toml
--rw-rw-r--   0 mgorven   (1000) mgorven   (1000)      596 2023-04-11 01:37:33.574119 lightspark-1.0.0/setup.cfg
--rwxrwxr-x   0 mgorven   (1000) mgorven   (1000)       62 2023-04-10 23:43:15.000000 lightspark-1.0.0/setup.py
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.146854 lightspark-1.1.0/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      395 2023-05-11 01:10:18.146911 lightspark-1.1.0/PKG-INFO
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      609 2023-05-11 00:23:23.000000 lightspark-1.1.0/README.md
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.128142 lightspark-1.1.0/lightspark/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     6608 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/__init__.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      185 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/exceptions.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    20130 2023-05-09 20:23:17.000000 lightspark-1.1.0/lightspark/lightspark_client.py
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.145543 lightspark-1.1.0/lightspark/objects/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    75427 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/Account.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1925 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/AccountToApiTokensConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1307 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/AccountToChannelsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     2653 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/AccountToNodesConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     2053 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/AccountToPaymentRequestsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4712 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/AccountToTransactionsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1882 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/AccountToWalletsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1899 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ApiToken.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     3442 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/Balances.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      782 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/BitcoinNetwork.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     5279 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/BlockchainBalance.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    13660 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Channel.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     5395 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ChannelClosingTransaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1351 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ChannelFees.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     5366 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ChannelOpeningTransaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1456 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ChannelStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     3668 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/ChannelToTransactionsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      736 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateApiTokenInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1448 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateApiTokenOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      828 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateInvoiceInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      659 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateInvoiceOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      393 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateNodeWalletAddressInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      898 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CreateNodeWalletAddressOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     5550 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CurrencyAmount.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1345 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/CurrencyUnit.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      371 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/DeleteApiTokenInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      668 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/DeleteApiTokenOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4573 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Deposit.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    48303 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/Entity.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1654 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/FeeEstimate.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      429 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/FundNodeInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1134 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/FundNodeOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4484 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/GraphNode.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     3451 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Hop.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1752 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/HtlcAttemptFailureCode.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     6081 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/IncomingPayment.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     3001 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/IncomingPaymentAttempt.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      558 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/IncomingPaymentAttemptStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1555 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    10747 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Invoice.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     9794 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/InvoiceData.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      487 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/InvoiceType.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      962 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      851 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightningFeeEstimateForNodeInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1324 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightningFeeEstimateOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    20160 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightningTransaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    20327 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightsparkNode.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      429 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightsparkNodePurpose.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      644 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightsparkNodeStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1983 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/LightsparkNodeToChannelsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    13646 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Node.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1035 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/NodeAddress.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      512 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/NodeAddressType.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1499 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/NodeToAddressesConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    14387 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OnChainTransaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    16999 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OutgoingPayment.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     7538 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttempt.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      536 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttemptStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1533 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1538 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      994 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PageInfo.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1158 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PayInvoiceInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      680 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PayInvoiceOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      684 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PaymentFailureReason.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    11545 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PaymentRequest.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    10106 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PaymentRequestData.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      402 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/PaymentRequestStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      842 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Permission.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1213 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/RequestWithdrawalInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      746 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/RequestWithdrawalOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      534 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/RichText.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     5504 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/RoutingTransaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      523 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/RoutingTransactionFailureReason.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      653 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Secret.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1095 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/SendPaymentInput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      687 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/SendPaymentOutput.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    31911 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Transaction.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      978 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/TransactionFailures.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      885 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/TransactionStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1632 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/TransactionType.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     6123 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/Wallet.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      730 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WebhookEventType.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4674 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/Withdrawal.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      438 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WithdrawalMode.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    11626 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WithdrawalRequest.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      449 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WithdrawalRequestStatus.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     2457 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     2457 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       75 2023-05-06 01:38:44.000000 lightspark-1.1.0/lightspark/objects/__init__.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)    10653 2023-05-06 01:45:30.000000 lightspark-1.1.0/lightspark/objects/all_entities.py
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.146173 lightspark-1.1.0/lightspark/requests/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       75 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/requests/__init__.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      416 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/requests/encoder.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4311 2023-04-26 20:21:00.000000 lightspark-1.1.0/lightspark/requests/requester.py
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.146736 lightspark-1.1.0/lightspark/utils/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       75 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/utils/__init__.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     3673 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/utils/crypto.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     1146 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/utils/enums.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       22 2023-05-11 00:22:53.000000 lightspark-1.1.0/lightspark/version.py
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     2214 2023-04-10 22:06:34.000000 lightspark-1.1.0/lightspark/webhooks.py
+drwxr-xr-x   0 jeremyklein   (501) staff       (20)        0 2023-05-11 01:10:18.128962 lightspark-1.1.0/lightspark.egg-info/
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      395 2023-05-11 01:10:18.000000 lightspark-1.1.0/lightspark.egg-info/PKG-INFO
+-rw-r--r--   0 jeremyklein   (501) staff       (20)     4286 2023-05-11 01:10:18.000000 lightspark-1.1.0/lightspark.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremyklein   (501) staff       (20)        1 2023-05-11 01:10:18.000000 lightspark-1.1.0/lightspark.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       28 2023-05-11 01:10:18.000000 lightspark-1.1.0/lightspark.egg-info/requires.txt
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       11 2023-05-11 01:10:18.000000 lightspark-1.1.0/lightspark.egg-info/top_level.txt
+-rw-r--r--   0 jeremyklein   (501) staff       (20)       81 2023-04-10 22:06:34.000000 lightspark-1.1.0/pyproject.toml
+-rw-r--r--   0 jeremyklein   (501) staff       (20)      649 2023-05-11 01:10:18.147168 lightspark-1.1.0/setup.cfg
+-rwxr-xr-x   0 jeremyklein   (501) staff       (20)       62 2023-04-10 22:06:34.000000 lightspark-1.1.0/setup.py
```

### Comparing `lightspark-1.0.0/README.md` & `lightspark-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Lightspark Python SDK - v1.0.0
+# Lightspark Python SDK - v1.1.0
 
 The Lightspark Python SDK provides a convenient way to interact with the Lightspark services from applications written in the Python language.
 
 ## Documentation
 
 The documentation for this SDK (installation, usage, etc.) is available at https://app.lightspark.com/docs/sdk
```

### Comparing `lightspark-1.0.0/lightspark/__init__.py` & `lightspark-1.1.0/lightspark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from lightspark.objects.AccountToNodesConnection import AccountToNodesConnection
 from lightspark.objects.AccountToPaymentRequestsConnection import (
     AccountToPaymentRequestsConnection,
 )
 from lightspark.objects.AccountToTransactionsConnection import (
     AccountToTransactionsConnection,
 )
+from lightspark.objects.AccountToWalletsConnection import AccountToWalletsConnection
 from lightspark.objects.ApiToken import ApiToken
+from lightspark.objects.Balances import Balances
 from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.objects.BlockchainBalance import BlockchainBalance
 from lightspark.objects.Channel import Channel
 from lightspark.objects.ChannelClosingTransaction import ChannelClosingTransaction
 from lightspark.objects.ChannelFees import ChannelFees
 from lightspark.objects.ChannelOpeningTransaction import ChannelOpeningTransaction
 from lightspark.objects.ChannelStatus import ChannelStatus
@@ -97,14 +99,15 @@
 from lightspark.objects.Secret import Secret
 from lightspark.objects.SendPaymentInput import SendPaymentInput
 from lightspark.objects.SendPaymentOutput import SendPaymentOutput
 from lightspark.objects.Transaction import Transaction
 from lightspark.objects.TransactionFailures import TransactionFailures
 from lightspark.objects.TransactionStatus import TransactionStatus
 from lightspark.objects.TransactionType import TransactionType
+from lightspark.objects.Wallet import Wallet
 from lightspark.objects.WebhookEventType import WebhookEventType
 from lightspark.objects.Withdrawal import Withdrawal
 from lightspark.objects.WithdrawalMode import WithdrawalMode
 from lightspark.objects.WithdrawalRequest import WithdrawalRequest
 from lightspark.objects.WithdrawalRequestStatus import WithdrawalRequestStatus
 from lightspark.objects.WithdrawalRequestToChannelClosingTransactionsConnection import (
     WithdrawalRequestToChannelClosingTransactionsConnection,
```

### Comparing `lightspark-1.0.0/lightspark/lightspark_client.py` & `lightspark-1.1.0/lightspark/lightspark_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 import logging
 from dataclasses import dataclass
+from datetime import datetime, timedelta, timezone
 from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
 
+import jwt
+from cryptography.hazmat.primitives.asymmetric.ed448 import Ed448PrivateKey
+from cryptography.hazmat.primitives.serialization import (
+    Encoding,
+    NoEncryption,
+    PrivateFormat,
+    PublicFormat,
+)
 from lightspark.exceptions import LightsparkException
 from lightspark.objects.Account import FRAGMENT as AccountFragment
 from lightspark.objects.Account import Account
 from lightspark.objects.Account import from_json as Account_from_json
 from lightspark.objects.all_entities import get_entity
 from lightspark.objects.ApiToken import FRAGMENT as ApiTokenFragment
 from lightspark.objects.ApiToken import ApiToken
@@ -16,26 +25,26 @@
 from lightspark.objects.CurrencyAmount import FRAGMENT as CurrencyAmountFragment
 from lightspark.objects.CurrencyAmount import CurrencyAmount
 from lightspark.objects.CurrencyAmount import from_json as CurrencyAmount_from_json
 from lightspark.objects.Entity import Entity
 from lightspark.objects.FeeEstimate import FRAGMENT as FeeEstimateFragment
 from lightspark.objects.FeeEstimate import FeeEstimate
 from lightspark.objects.FeeEstimate import from_json as FeeEstimate_from_json
-from lightspark.objects.LightningFeeEstimateOutput import (
-    FRAGMENT as LightningFeeEstimateFragment,
-)
-from lightspark.objects.LightningFeeEstimateOutput import (
-    from_json as LightningFeeEstimateOutput_from_json,
-)
 from lightspark.objects.Invoice import FRAGMENT as InvoiceFragment
 from lightspark.objects.Invoice import Invoice
 from lightspark.objects.Invoice import from_json as Invoice_from_json
 from lightspark.objects.InvoiceData import FRAGMENT as InvoiceDataFragment
 from lightspark.objects.InvoiceData import from_json as InvoiceData_from_json
 from lightspark.objects.InvoiceType import InvoiceType
+from lightspark.objects.LightningFeeEstimateOutput import (
+    FRAGMENT as LightningFeeEstimateFragment,
+)
+from lightspark.objects.LightningFeeEstimateOutput import (
+    from_json as LightningFeeEstimateOutput_from_json,
+)
 from lightspark.objects.OutgoingPayment import FRAGMENT as OutgoingPaymentFragment
 from lightspark.objects.OutgoingPayment import OutgoingPayment
 from lightspark.objects.OutgoingPayment import from_json as OutgoingPayment_from_json
 from lightspark.objects.PaymentRequestData import PaymentRequestData
 from lightspark.objects.Permission import Permission
 from lightspark.objects.WithdrawalMode import WithdrawalMode
 from lightspark.objects.WithdrawalRequest import FRAGMENT as WithdrawalRequestFragment
@@ -213,14 +222,42 @@
             This JSON object can then be used to instantiate some of the python
             objects defined in the lightspark.objects.* modules, using the `from_json`
             function defined in each module.
         """
         logger.info("Executing arbitrary GraphQL request with document=%s", document)
         return self._requester.execute_graphql(query=document, variables=variables)
 
+    def generate_jwt_key(self) -> Tuple[str, str]:
+        key = Ed448PrivateKey.generate()
+        return (
+            key.public_key()
+            .public_bytes(Encoding.PEM, PublicFormat.SubjectPublicKeyInfo)
+            .decode(),
+            key.private_bytes(
+                Encoding.PEM, PrivateFormat.PKCS8, NoEncryption()
+            ).decode(),
+        )
+
+    def generate_wallet_jwt(
+        self,
+        private_key_pem: str,
+        third_party_id: str,
+        test_mode: bool = False,
+        duration: timedelta = timedelta(minutes=1),
+        algorithm: str = "EdDSA",
+    ) -> str:
+        payload = {
+            "aud": "https://api.lightspark.com",
+            "exp": datetime.now(timezone.utc) + duration,
+            "iat": datetime.now(timezone.utc),
+            "sub": third_party_id,
+            "test": test_mode,
+        }
+        return jwt.encode(payload, private_key_pem, algorithm)
+
     def get_current_account(
         self,
     ) -> Account:
         logger.info("Fetching current account.")
         json = self._requester.execute_graphql(
             f"""
 query GetCurrentAccount {{
```

### Comparing `lightspark-1.0.0/lightspark/objects/Account.py` & `lightspark-1.1.0/lightspark/objects/Account.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from .AccountToPaymentRequestsConnection import (
     from_json as AccountToPaymentRequestsConnection_from_json,
 )
 from .AccountToTransactionsConnection import AccountToTransactionsConnection
 from .AccountToTransactionsConnection import (
     from_json as AccountToTransactionsConnection_from_json,
 )
+from .AccountToWalletsConnection import AccountToWalletsConnection
+from .AccountToWalletsConnection import (
+    from_json as AccountToWalletsConnection_from_json,
+)
 from .BitcoinNetwork import BitcoinNetwork
 from .BlockchainBalance import BlockchainBalance
 from .BlockchainBalance import from_json as BlockchainBalance_from_json
 from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
 from .Entity import Entity
 from .TransactionFailures import TransactionFailures
@@ -765,14 +769,15 @@
                                     currency_amount_original_unit: original_unit
                                     currency_amount_preferred_currency_unit: preferred_currency_unit
                                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                                 }
                                 invoice_data_created_at: created_at
                                 invoice_data_expires_at: expires_at
+                                invoice_data_memo: memo
                                 invoice_data_destination: destination {
                                     __typename
                                     ... on GraphNode {
                                         __typename
                                         graph_node_id: id
                                         graph_node_created_at: created_at
                                         graph_node_updated_at: updated_at
@@ -885,15 +890,14 @@
                                             currency_amount_preferred_currency_unit: preferred_currency_unit
                                             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                                             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                                         }
                                         lightspark_node_status: status
                                     }
                                 }
-                                invoice_data_memo: memo
                             }
                         }
                         outgoing_payment_failure_reason: failure_reason
                         outgoing_payment_failure_message: failure_message {
                             __typename
                             rich_text_text: text
                         }
@@ -1030,14 +1034,15 @@
                                 currency_amount_original_unit: original_unit
                                 currency_amount_preferred_currency_unit: preferred_currency_unit
                                 currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                                 currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                             }
                             invoice_data_created_at: created_at
                             invoice_data_expires_at: expires_at
+                            invoice_data_memo: memo
                             invoice_data_destination: destination {
                                 __typename
                                 ... on GraphNode {
                                     __typename
                                     graph_node_id: id
                                     graph_node_created_at: created_at
                                     graph_node_updated_at: updated_at
@@ -1150,15 +1155,14 @@
                                         currency_amount_preferred_currency_unit: preferred_currency_unit
                                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                                     }
                                     lightspark_node_status: status
                                 }
                             }
-                            invoice_data_memo: memo
                         }
                         invoice_status: status
                         invoice_amount_paid: amount_paid {
                             __typename
                             currency_amount_original_value: original_value
                             currency_amount_original_unit: original_unit
                             currency_amount_preferred_currency_unit: preferred_currency_unit
@@ -1188,14 +1192,75 @@
                 "bitcoin_network": bitcoin_network,
                 "lightning_node_id": lightning_node_id,
             },
         )
         connection = json["entity"]["payment_requests"]
         return AccountToPaymentRequestsConnection_from_json(self.requester, connection)
 
+    def get_wallets(self, first: Optional[int] = None) -> AccountToWalletsConnection:
+        json = self.requester.execute_graphql(
+            """
+query FetchAccountToWalletsConnection($entity_id: ID!, $first: Int) {
+    entity(id: $entity_id) {
+        ... on Account {
+            wallets(, first: $first) {
+                __typename
+                account_to_wallets_connection_page_info: page_info {
+                    __typename
+                    page_info_has_next_page: has_next_page
+                    page_info_has_previous_page: has_previous_page
+                    page_info_start_cursor: start_cursor
+                    page_info_end_cursor: end_cursor
+                }
+                account_to_wallets_connection_count: count
+                account_to_wallets_connection_entities: entities {
+                    __typename
+                    wallet_id: id
+                    wallet_created_at: created_at
+                    wallet_updated_at: updated_at
+                    wallet_last_login_at: last_login_at
+                    wallet_balances: balances {
+                        __typename
+                        balances_owned_balance: owned_balance {
+                            __typename
+                            currency_amount_original_value: original_value
+                            currency_amount_original_unit: original_unit
+                            currency_amount_preferred_currency_unit: preferred_currency_unit
+                            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                        }
+                        balances_available_to_send_balance: available_to_send_balance {
+                            __typename
+                            currency_amount_original_value: original_value
+                            currency_amount_original_unit: original_unit
+                            currency_amount_preferred_currency_unit: preferred_currency_unit
+                            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                        }
+                        balances_available_to_withdraw_balance: available_to_withdraw_balance {
+                            __typename
+                            currency_amount_original_value: original_value
+                            currency_amount_original_unit: original_unit
+                            currency_amount_preferred_currency_unit: preferred_currency_unit
+                            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                        }
+                    }
+                    wallet_third_party_identifier: third_party_identifier
+                }
+            }
+        }
+    }
+}
+            """,
+            {"entity_id": self.id, "first": first},
+        )
+        connection = json["entity"]["wallets"]
+        return AccountToWalletsConnection_from_json(self.requester, connection)
+
 
 FRAGMENT = """
 fragment AccountFragment on Account {
     __typename
     account_id: id
     account_created_at: created_at
     account_updated_at: updated_at
```

### Comparing `lightspark-1.0.0/lightspark/objects/AccountToApiTokensConnection.py` & `lightspark-1.1.0/lightspark/objects/AccountToApiTokensConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/AccountToChannelsConnection.py` & `lightspark-1.1.0/lightspark/objects/AccountToChannelsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/AccountToNodesConnection.py` & `lightspark-1.1.0/lightspark/objects/AccountToNodesConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/AccountToPaymentRequestsConnection.py` & `lightspark-1.1.0/lightspark/objects/AccountToPaymentRequestsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/AccountToTransactionsConnection.py` & `lightspark-1.1.0/lightspark/objects/AccountToTransactionsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ApiToken.py` & `lightspark-1.1.0/lightspark/objects/ApiToken.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/BitcoinNetwork.py` & `lightspark-1.1.0/lightspark/objects/BitcoinNetwork.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/BlockchainBalance.py` & `lightspark-1.1.0/lightspark/objects/BlockchainBalance.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Channel.py` & `lightspark-1.1.0/lightspark/objects/Channel.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ChannelClosingTransaction.py` & `lightspark-1.1.0/lightspark/objects/ChannelClosingTransaction.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ChannelFees.py` & `lightspark-1.1.0/lightspark/objects/ChannelFees.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ChannelOpeningTransaction.py` & `lightspark-1.1.0/lightspark/objects/ChannelOpeningTransaction.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ChannelStatus.py` & `lightspark-1.1.0/lightspark/objects/ChannelStatus.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/ChannelToTransactionsConnection.py` & `lightspark-1.1.0/lightspark/objects/ChannelToTransactionsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CreateApiTokenInput.py` & `lightspark-1.1.0/lightspark/objects/CreateApiTokenInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CreateApiTokenOutput.py` & `lightspark-1.1.0/lightspark/objects/CreateApiTokenOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CreateInvoiceInput.py` & `lightspark-1.1.0/lightspark/objects/CreateInvoiceInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CreateInvoiceOutput.py` & `lightspark-1.1.0/lightspark/objects/CreateInvoiceOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CreateNodeWalletAddressOutput.py` & `lightspark-1.1.0/lightspark/objects/CreateNodeWalletAddressOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CurrencyAmount.py` & `lightspark-1.1.0/lightspark/objects/CurrencyAmount.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/CurrencyUnit.py` & `lightspark-1.1.0/lightspark/objects/CurrencyUnit.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/DeleteApiTokenOutput.py` & `lightspark-1.1.0/lightspark/objects/DeleteApiTokenOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Deposit.py` & `lightspark-1.1.0/lightspark/objects/Deposit.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Entity.py` & `lightspark-1.1.0/lightspark/objects/Entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,15 @@
                 currency_amount_original_unit: original_unit
                 currency_amount_preferred_currency_unit: preferred_currency_unit
                 currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                 currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
             }
             invoice_data_created_at: created_at
             invoice_data_expires_at: expires_at
+            invoice_data_memo: memo
             invoice_data_destination: destination {
                 __typename
                 ... on GraphNode {
                     __typename
                     graph_node_id: id
                     graph_node_created_at: created_at
                     graph_node_updated_at: updated_at
@@ -453,15 +454,14 @@
                         currency_amount_preferred_currency_unit: preferred_currency_unit
                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                     }
                     lightspark_node_status: status
                 }
             }
-            invoice_data_memo: memo
         }
         invoice_status: status
         invoice_amount_paid: amount_paid {
             __typename
             currency_amount_original_value: original_value
             currency_amount_original_unit: original_unit
             currency_amount_preferred_currency_unit: preferred_currency_unit
@@ -617,14 +617,15 @@
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
                 invoice_data_created_at: created_at
                 invoice_data_expires_at: expires_at
+                invoice_data_memo: memo
                 invoice_data_destination: destination {
                     __typename
                     ... on GraphNode {
                         __typename
                         graph_node_id: id
                         graph_node_created_at: created_at
                         graph_node_updated_at: updated_at
@@ -737,15 +738,14 @@
                             currency_amount_preferred_currency_unit: preferred_currency_unit
                             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                         }
                         lightspark_node_status: status
                     }
                 }
-                invoice_data_memo: memo
             }
         }
         outgoing_payment_failure_reason: failure_reason
         outgoing_payment_failure_message: failure_message {
             __typename
             rich_text_text: text
         }
@@ -811,14 +811,49 @@
         }
         routing_transaction_failure_message: failure_message {
             __typename
             rich_text_text: text
         }
         routing_transaction_failure_reason: failure_reason
     }
+    ... on Wallet {
+        __typename
+        wallet_id: id
+        wallet_created_at: created_at
+        wallet_updated_at: updated_at
+        wallet_last_login_at: last_login_at
+        wallet_balances: balances {
+            __typename
+            balances_owned_balance: owned_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            balances_available_to_send_balance: available_to_send_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            balances_available_to_withdraw_balance: available_to_withdraw_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+        }
+        wallet_third_party_identifier: third_party_identifier
+    }
     ... on Withdrawal {
         __typename
         withdrawal_id: id
         withdrawal_created_at: created_at
         withdrawal_updated_at: updated_at
         withdrawal_status: status
         withdrawal_resolved_at: resolved_at
@@ -856,14 +891,22 @@
             __typename
             currency_amount_original_value: original_value
             currency_amount_original_unit: original_unit
             currency_amount_preferred_currency_unit: preferred_currency_unit
             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
         }
+        withdrawal_request_estimated_amount: estimated_amount {
+            __typename
+            currency_amount_original_value: original_value
+            currency_amount_original_unit: original_unit
+            currency_amount_preferred_currency_unit: preferred_currency_unit
+            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+        }
         withdrawal_request_bitcoin_address: bitcoin_address
         withdrawal_request_withdrawal_mode: withdrawal_mode
         withdrawal_request_status: status
         withdrawal_request_completed_at: completed_at
         withdrawal_request_withdrawal: withdrawal {
             id
         }
```

### Comparing `lightspark-1.0.0/lightspark/objects/FeeEstimate.py` & `lightspark-1.1.0/lightspark/objects/FeeEstimate.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/FundNodeOutput.py` & `lightspark-1.1.0/lightspark/objects/FundNodeOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/GraphNode.py` & `lightspark-1.1.0/lightspark/objects/GraphNode.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Hop.py` & `lightspark-1.1.0/lightspark/objects/Hop.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/HtlcAttemptFailureCode.py` & `lightspark-1.1.0/lightspark/objects/HtlcAttemptFailureCode.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/IncomingPayment.py` & `lightspark-1.1.0/lightspark/objects/IncomingPayment.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/IncomingPaymentAttempt.py` & `lightspark-1.1.0/lightspark/objects/IncomingPaymentAttempt.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/IncomingPaymentAttemptStatus.py` & `lightspark-1.1.0/lightspark/objects/IncomingPaymentAttemptStatus.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py` & `lightspark-1.1.0/lightspark/objects/IncomingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Invoice.py` & `lightspark-1.1.0/lightspark/objects/Invoice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             currency_amount_original_unit: original_unit
             currency_amount_preferred_currency_unit: preferred_currency_unit
             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
         }
         invoice_data_created_at: created_at
         invoice_data_expires_at: expires_at
+        invoice_data_memo: memo
         invoice_data_destination: destination {
             __typename
             ... on GraphNode {
                 __typename
                 graph_node_id: id
                 graph_node_created_at: created_at
                 graph_node_updated_at: updated_at
@@ -180,15 +181,14 @@
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
                 lightspark_node_status: status
             }
         }
-        invoice_data_memo: memo
     }
     invoice_status: status
     invoice_amount_paid: amount_paid {
         __typename
         currency_amount_original_value: original_value
         currency_amount_original_unit: original_unit
         currency_amount_preferred_currency_unit: preferred_currency_unit
```

### Comparing `lightspark-1.0.0/lightspark/objects/InvoiceData.py` & `lightspark-1.1.0/lightspark/objects/PaymentRequestData.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,197 +1,196 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
-from datetime import datetime
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping
 
+from lightspark.exceptions import LightsparkException
 from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .BitcoinNetwork import BitcoinNetwork
-from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
-from .Node import Node
 from .Node import from_json as Node_from_json
-from .PaymentRequestData import PaymentRequestData
 
 
 @dataclass
-class InvoiceData(PaymentRequestData):
-    """This object represents the BOLT #11 invoice protocol for Lightning Payments. See https://github.com/lightning/bolts/blob/master/11-payment-encoding.md."""
+class PaymentRequestData:
+    """The interface of a payment request on the Lightning Network (a.k.a. Lightning Invoice)."""
 
     requester: Requester
 
     encoded_payment_request: str
 
     bitcoin_network: BitcoinNetwork
 
-    payment_hash: str
-
-    amount: CurrencyAmount
-
-    created_at: datetime
-
-    expires_at: datetime
-
-    destination: Node
-
-    memo: Optional[str]
-
     typename: str
 
 
 FRAGMENT = """
-fragment InvoiceDataFragment on InvoiceData {
+fragment PaymentRequestDataFragment on PaymentRequestData {
     __typename
-    invoice_data_encoded_payment_request: encoded_payment_request
-    invoice_data_bitcoin_network: bitcoin_network
-    invoice_data_payment_hash: payment_hash
-    invoice_data_amount: amount {
-        __typename
-        currency_amount_original_value: original_value
-        currency_amount_original_unit: original_unit
-        currency_amount_preferred_currency_unit: preferred_currency_unit
-        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-    }
-    invoice_data_created_at: created_at
-    invoice_data_expires_at: expires_at
-    invoice_data_destination: destination {
+    ... on InvoiceData {
         __typename
-        ... on GraphNode {
+        invoice_data_encoded_payment_request: encoded_payment_request
+        invoice_data_bitcoin_network: bitcoin_network
+        invoice_data_payment_hash: payment_hash
+        invoice_data_amount: amount {
             __typename
-            graph_node_id: id
-            graph_node_created_at: created_at
-            graph_node_updated_at: updated_at
-            graph_node_alias: alias
-            graph_node_bitcoin_network: bitcoin_network
-            graph_node_color: color
-            graph_node_conductivity: conductivity
-            graph_node_display_name: display_name
-            graph_node_public_key: public_key
+            currency_amount_original_value: original_value
+            currency_amount_original_unit: original_unit
+            currency_amount_preferred_currency_unit: preferred_currency_unit
+            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
         }
-        ... on LightsparkNode {
+        invoice_data_created_at: created_at
+        invoice_data_expires_at: expires_at
+        invoice_data_memo: memo
+        invoice_data_destination: destination {
             __typename
-            lightspark_node_id: id
-            lightspark_node_created_at: created_at
-            lightspark_node_updated_at: updated_at
-            lightspark_node_alias: alias
-            lightspark_node_bitcoin_network: bitcoin_network
-            lightspark_node_color: color
-            lightspark_node_conductivity: conductivity
-            lightspark_node_display_name: display_name
-            lightspark_node_public_key: public_key
-            lightspark_node_account: account {
-                id
+            ... on GraphNode {
+                __typename
+                graph_node_id: id
+                graph_node_created_at: created_at
+                graph_node_updated_at: updated_at
+                graph_node_alias: alias
+                graph_node_bitcoin_network: bitcoin_network
+                graph_node_color: color
+                graph_node_conductivity: conductivity
+                graph_node_display_name: display_name
+                graph_node_public_key: public_key
             }
-            lightspark_node_blockchain_balance: blockchain_balance {
+            ... on LightsparkNode {
                 __typename
-                blockchain_balance_total_balance: total_balance {
+                lightspark_node_id: id
+                lightspark_node_created_at: created_at
+                lightspark_node_updated_at: updated_at
+                lightspark_node_alias: alias
+                lightspark_node_bitcoin_network: bitcoin_network
+                lightspark_node_color: color
+                lightspark_node_conductivity: conductivity
+                lightspark_node_display_name: display_name
+                lightspark_node_public_key: public_key
+                lightspark_node_account: account {
+                    id
+                }
+                lightspark_node_blockchain_balance: blockchain_balance {
                     __typename
-                    currency_amount_original_value: original_value
-                    currency_amount_original_unit: original_unit
-                    currency_amount_preferred_currency_unit: preferred_currency_unit
-                    currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                    currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    blockchain_balance_total_balance: total_balance {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    blockchain_balance_confirmed_balance: confirmed_balance {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    blockchain_balance_unconfirmed_balance: unconfirmed_balance {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    blockchain_balance_locked_balance: locked_balance {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    blockchain_balance_required_reserve: required_reserve {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
+                    blockchain_balance_available_balance: available_balance {
+                        __typename
+                        currency_amount_original_value: original_value
+                        currency_amount_original_unit: original_unit
+                        currency_amount_preferred_currency_unit: preferred_currency_unit
+                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    }
                 }
-                blockchain_balance_confirmed_balance: confirmed_balance {
+                lightspark_node_encrypted_signing_private_key: encrypted_signing_private_key {
                     __typename
-                    currency_amount_original_value: original_value
-                    currency_amount_original_unit: original_unit
-                    currency_amount_preferred_currency_unit: preferred_currency_unit
-                    currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                    currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+                    secret_encrypted_value: encrypted_value
+                    secret_cipher: cipher
                 }
-                blockchain_balance_unconfirmed_balance: unconfirmed_balance {
+                lightspark_node_total_balance: total_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                blockchain_balance_locked_balance: locked_balance {
+                lightspark_node_total_local_balance: total_local_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                blockchain_balance_required_reserve: required_reserve {
+                lightspark_node_local_balance: local_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                blockchain_balance_available_balance: available_balance {
+                lightspark_node_purpose: purpose
+                lightspark_node_remote_balance: remote_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
+                lightspark_node_status: status
             }
-            lightspark_node_encrypted_signing_private_key: encrypted_signing_private_key {
-                __typename
-                secret_encrypted_value: encrypted_value
-                secret_cipher: cipher
-            }
-            lightspark_node_total_balance: total_balance {
-                __typename
-                currency_amount_original_value: original_value
-                currency_amount_original_unit: original_unit
-                currency_amount_preferred_currency_unit: preferred_currency_unit
-                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-            }
-            lightspark_node_total_local_balance: total_local_balance {
-                __typename
-                currency_amount_original_value: original_value
-                currency_amount_original_unit: original_unit
-                currency_amount_preferred_currency_unit: preferred_currency_unit
-                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-            }
-            lightspark_node_local_balance: local_balance {
-                __typename
-                currency_amount_original_value: original_value
-                currency_amount_original_unit: original_unit
-                currency_amount_preferred_currency_unit: preferred_currency_unit
-                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-            }
-            lightspark_node_purpose: purpose
-            lightspark_node_remote_balance: remote_balance {
-                __typename
-                currency_amount_original_value: original_value
-                currency_amount_original_unit: original_unit
-                currency_amount_preferred_currency_unit: preferred_currency_unit
-                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-            }
-            lightspark_node_status: status
         }
     }
-    invoice_data_memo: memo
 }
 """
 
 
-def from_json(requester: Requester, obj: Mapping[str, Any]) -> InvoiceData:
-    return InvoiceData(
-        requester=requester,
-        typename="InvoiceData",
-        encoded_payment_request=obj["invoice_data_encoded_payment_request"],
-        bitcoin_network=parse_enum(BitcoinNetwork, obj["invoice_data_bitcoin_network"]),
-        payment_hash=obj["invoice_data_payment_hash"],
-        amount=CurrencyAmount_from_json(requester, obj["invoice_data_amount"]),
-        created_at=obj["invoice_data_created_at"],
-        expires_at=obj["invoice_data_expires_at"],
-        destination=Node_from_json(requester, obj["invoice_data_destination"]),
-        memo=obj["invoice_data_memo"],
+def from_json(requester: Requester, obj: Mapping[str, Any]) -> PaymentRequestData:
+    if obj["__typename"] == "InvoiceData":
+        # pylint: disable=import-outside-toplevel
+        from lightspark.objects.InvoiceData import InvoiceData
+
+        return InvoiceData(
+            requester=requester,
+            typename="InvoiceData",
+            encoded_payment_request=obj["invoice_data_encoded_payment_request"],
+            bitcoin_network=parse_enum(
+                BitcoinNetwork, obj["invoice_data_bitcoin_network"]
+            ),
+            payment_hash=obj["invoice_data_payment_hash"],
+            amount=CurrencyAmount_from_json(requester, obj["invoice_data_amount"]),
+            created_at=obj["invoice_data_created_at"],
+            expires_at=obj["invoice_data_expires_at"],
+            memo=obj["invoice_data_memo"],
+            destination=Node_from_json(requester, obj["invoice_data_destination"]),
+        )
+    graphql_typename = obj["__typename"]
+    raise LightsparkException(
+        "UNKNOWN_INTERFACE",
+        f"Couldn't find a concrete type for interface PaymentRequestData corresponding to the typename={graphql_typename}",
     )
```

### Comparing `lightspark-1.0.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py` & `lightspark-1.1.0/lightspark/objects/LightningFeeEstimateForInvoiceInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/LightningFeeEstimateForNodeInput.py` & `lightspark-1.1.0/lightspark/objects/LightningFeeEstimateForNodeInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/LightningFeeEstimateOutput.py` & `lightspark-1.1.0/lightspark/objects/LightningFeeEstimateOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/LightningTransaction.py` & `lightspark-1.1.0/lightspark/objects/LightningTransaction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
                 invoice_data_created_at: created_at
                 invoice_data_expires_at: expires_at
+                invoice_data_memo: memo
                 invoice_data_destination: destination {
                     __typename
                     ... on GraphNode {
                         __typename
                         graph_node_id: id
                         graph_node_created_at: created_at
                         graph_node_updated_at: updated_at
@@ -241,15 +242,14 @@
                             currency_amount_preferred_currency_unit: preferred_currency_unit
                             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                         }
                         lightspark_node_status: status
                     }
                 }
-                invoice_data_memo: memo
             }
         }
         outgoing_payment_failure_reason: failure_reason
         outgoing_payment_failure_message: failure_message {
             __typename
             rich_text_text: text
         }
```

### Comparing `lightspark-1.0.0/lightspark/objects/LightsparkNode.py` & `lightspark-1.1.0/lightspark/objects/LightsparkNode.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/LightsparkNodeStatus.py` & `lightspark-1.1.0/lightspark/objects/LightsparkNodeStatus.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,9 +9,10 @@
     CREATED = "CREATED"
     DEPLOYED = "DEPLOYED"
     STARTED = "STARTED"
     SYNCING = "SYNCING"
     READY = "READY"
     STOPPED = "STOPPED"
     TERMINATED = "TERMINATED"
+    TERMINATING = "TERMINATING"
     WALLET_LOCKED = "WALLET_LOCKED"
     FAILED_TO_DEPLOY = "FAILED_TO_DEPLOY"
```

### Comparing `lightspark-1.0.0/lightspark/objects/LightsparkNodeToChannelsConnection.py` & `lightspark-1.1.0/lightspark/objects/LightsparkNodeToChannelsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Node.py` & `lightspark-1.1.0/lightspark/objects/Node.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/NodeAddress.py` & `lightspark-1.1.0/lightspark/objects/NodeAddress.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/NodeAddressType.py` & `lightspark-1.1.0/lightspark/objects/NodeAddressType.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/NodeToAddressesConnection.py` & `lightspark-1.1.0/lightspark/objects/NodeToAddressesConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/OnChainTransaction.py` & `lightspark-1.1.0/lightspark/objects/OnChainTransaction.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/OutgoingPayment.py` & `lightspark-1.1.0/lightspark/objects/OutgoingPayment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,15 @@
                 currency_amount_original_unit: original_unit
                 currency_amount_preferred_currency_unit: preferred_currency_unit
                 currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                 currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
             }
             invoice_data_created_at: created_at
             invoice_data_expires_at: expires_at
+            invoice_data_memo: memo
             invoice_data_destination: destination {
                 __typename
                 ... on GraphNode {
                     __typename
                     graph_node_id: id
                     graph_node_created_at: created_at
                     graph_node_updated_at: updated_at
@@ -287,15 +288,14 @@
                         currency_amount_preferred_currency_unit: preferred_currency_unit
                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                     }
                     lightspark_node_status: status
                 }
             }
-            invoice_data_memo: memo
         }
     }
     outgoing_payment_failure_reason: failure_reason
     outgoing_payment_failure_message: failure_message {
         __typename
         rich_text_text: text
     }
```

### Comparing `lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttempt.py` & `lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttempt.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttemptStatus.py` & `lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttemptStatus.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py` & `lightspark-1.1.0/lightspark/objects/OutgoingPaymentAttemptToHopsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py` & `lightspark-1.1.0/lightspark/objects/OutgoingPaymentToAttemptsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/PageInfo.py` & `lightspark-1.1.0/lightspark/objects/PageInfo.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/PayInvoiceInput.py` & `lightspark-1.1.0/lightspark/objects/PayInvoiceInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/PayInvoiceOutput.py` & `lightspark-1.1.0/lightspark/objects/PayInvoiceOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/PaymentFailureReason.py` & `lightspark-1.1.0/lightspark/objects/PaymentFailureReason.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/PaymentRequest.py` & `lightspark-1.1.0/lightspark/objects/PaymentRequest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 currency_amount_original_unit: original_unit
                 currency_amount_preferred_currency_unit: preferred_currency_unit
                 currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                 currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
             }
             invoice_data_created_at: created_at
             invoice_data_expires_at: expires_at
+            invoice_data_memo: memo
             invoice_data_destination: destination {
                 __typename
                 ... on GraphNode {
                     __typename
                     graph_node_id: id
                     graph_node_created_at: created_at
                     graph_node_updated_at: updated_at
@@ -176,15 +177,14 @@
                         currency_amount_preferred_currency_unit: preferred_currency_unit
                         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                     }
                     lightspark_node_status: status
                 }
             }
-            invoice_data_memo: memo
         }
         invoice_status: status
         invoice_amount_paid: amount_paid {
             __typename
             currency_amount_original_value: original_value
             currency_amount_original_unit: original_unit
             currency_amount_preferred_currency_unit: preferred_currency_unit
```

### Comparing `lightspark-1.0.0/lightspark/objects/PaymentRequestData.py` & `lightspark-1.1.0/lightspark/objects/InvoiceData.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,196 +1,202 @@
 # Copyright ©, 2022-present, Lightspark Group, Inc. - All Rights Reserved
 
 from dataclasses import dataclass
-from typing import Any, Mapping
+from datetime import datetime
+from typing import Any, Mapping, Optional
 
-from lightspark.exceptions import LightsparkException
 from lightspark.objects.BitcoinNetwork import BitcoinNetwork
 from lightspark.requests.requester import Requester
 from lightspark.utils.enums import parse_enum
 
 from .BitcoinNetwork import BitcoinNetwork
+from .CurrencyAmount import CurrencyAmount
 from .CurrencyAmount import from_json as CurrencyAmount_from_json
+from .Node import Node
 from .Node import from_json as Node_from_json
+from .PaymentRequestData import PaymentRequestData
 
 
 @dataclass
-class PaymentRequestData:
-    """The interface of a payment request on the Lightning Network (a.k.a. Lightning Invoice)."""
+class InvoiceData(PaymentRequestData):
+    """This object represents the BOLT #11 invoice protocol for Lightning Payments. See https://github.com/lightning/bolts/blob/master/11-payment-encoding.md."""
 
     requester: Requester
 
     encoded_payment_request: str
 
     bitcoin_network: BitcoinNetwork
 
+    payment_hash: str
+    """The payment hash of this invoice."""
+
+    amount: CurrencyAmount
+    """The requested amount in this invoice. If it is equal to 0, the sender should choose the amount to send."""
+
+    created_at: datetime
+    """The date and time when this invoice was created."""
+
+    expires_at: datetime
+    """The date and time when this invoice will expire."""
+
+    memo: Optional[str]
+    """A short, UTF-8 encoded, description of the purpose of this invoice."""
+
+    destination: Node
+    """The lightning node that will be paid when fulfilling this invoice."""
     typename: str
 
 
 FRAGMENT = """
-fragment PaymentRequestDataFragment on PaymentRequestData {
+fragment InvoiceDataFragment on InvoiceData {
     __typename
-    ... on InvoiceData {
+    invoice_data_encoded_payment_request: encoded_payment_request
+    invoice_data_bitcoin_network: bitcoin_network
+    invoice_data_payment_hash: payment_hash
+    invoice_data_amount: amount {
+        __typename
+        currency_amount_original_value: original_value
+        currency_amount_original_unit: original_unit
+        currency_amount_preferred_currency_unit: preferred_currency_unit
+        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+    }
+    invoice_data_created_at: created_at
+    invoice_data_expires_at: expires_at
+    invoice_data_memo: memo
+    invoice_data_destination: destination {
         __typename
-        invoice_data_encoded_payment_request: encoded_payment_request
-        invoice_data_bitcoin_network: bitcoin_network
-        invoice_data_payment_hash: payment_hash
-        invoice_data_amount: amount {
+        ... on GraphNode {
             __typename
-            currency_amount_original_value: original_value
-            currency_amount_original_unit: original_unit
-            currency_amount_preferred_currency_unit: preferred_currency_unit
-            currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-            currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            graph_node_id: id
+            graph_node_created_at: created_at
+            graph_node_updated_at: updated_at
+            graph_node_alias: alias
+            graph_node_bitcoin_network: bitcoin_network
+            graph_node_color: color
+            graph_node_conductivity: conductivity
+            graph_node_display_name: display_name
+            graph_node_public_key: public_key
         }
-        invoice_data_created_at: created_at
-        invoice_data_expires_at: expires_at
-        invoice_data_destination: destination {
+        ... on LightsparkNode {
             __typename
-            ... on GraphNode {
-                __typename
-                graph_node_id: id
-                graph_node_created_at: created_at
-                graph_node_updated_at: updated_at
-                graph_node_alias: alias
-                graph_node_bitcoin_network: bitcoin_network
-                graph_node_color: color
-                graph_node_conductivity: conductivity
-                graph_node_display_name: display_name
-                graph_node_public_key: public_key
+            lightspark_node_id: id
+            lightspark_node_created_at: created_at
+            lightspark_node_updated_at: updated_at
+            lightspark_node_alias: alias
+            lightspark_node_bitcoin_network: bitcoin_network
+            lightspark_node_color: color
+            lightspark_node_conductivity: conductivity
+            lightspark_node_display_name: display_name
+            lightspark_node_public_key: public_key
+            lightspark_node_account: account {
+                id
             }
-            ... on LightsparkNode {
+            lightspark_node_blockchain_balance: blockchain_balance {
                 __typename
-                lightspark_node_id: id
-                lightspark_node_created_at: created_at
-                lightspark_node_updated_at: updated_at
-                lightspark_node_alias: alias
-                lightspark_node_bitcoin_network: bitcoin_network
-                lightspark_node_color: color
-                lightspark_node_conductivity: conductivity
-                lightspark_node_display_name: display_name
-                lightspark_node_public_key: public_key
-                lightspark_node_account: account {
-                    id
-                }
-                lightspark_node_blockchain_balance: blockchain_balance {
+                blockchain_balance_total_balance: total_balance {
                     __typename
-                    blockchain_balance_total_balance: total_balance {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
-                    blockchain_balance_confirmed_balance: confirmed_balance {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
-                    blockchain_balance_unconfirmed_balance: unconfirmed_balance {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
-                    blockchain_balance_locked_balance: locked_balance {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
-                    blockchain_balance_required_reserve: required_reserve {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
-                    blockchain_balance_available_balance: available_balance {
-                        __typename
-                        currency_amount_original_value: original_value
-                        currency_amount_original_unit: original_unit
-                        currency_amount_preferred_currency_unit: preferred_currency_unit
-                        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
-                        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
-                    }
+                    currency_amount_original_value: original_value
+                    currency_amount_original_unit: original_unit
+                    currency_amount_preferred_currency_unit: preferred_currency_unit
+                    currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                    currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_encrypted_signing_private_key: encrypted_signing_private_key {
+                blockchain_balance_confirmed_balance: confirmed_balance {
                     __typename
-                    secret_encrypted_value: encrypted_value
-                    secret_cipher: cipher
+                    currency_amount_original_value: original_value
+                    currency_amount_original_unit: original_unit
+                    currency_amount_preferred_currency_unit: preferred_currency_unit
+                    currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                    currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_total_balance: total_balance {
+                blockchain_balance_unconfirmed_balance: unconfirmed_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_total_local_balance: total_local_balance {
+                blockchain_balance_locked_balance: locked_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_local_balance: local_balance {
+                blockchain_balance_required_reserve: required_reserve {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_purpose: purpose
-                lightspark_node_remote_balance: remote_balance {
+                blockchain_balance_available_balance: available_balance {
                     __typename
                     currency_amount_original_value: original_value
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
-                lightspark_node_status: status
             }
+            lightspark_node_encrypted_signing_private_key: encrypted_signing_private_key {
+                __typename
+                secret_encrypted_value: encrypted_value
+                secret_cipher: cipher
+            }
+            lightspark_node_total_balance: total_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            lightspark_node_total_local_balance: total_local_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            lightspark_node_local_balance: local_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            lightspark_node_purpose: purpose
+            lightspark_node_remote_balance: remote_balance {
+                __typename
+                currency_amount_original_value: original_value
+                currency_amount_original_unit: original_unit
+                currency_amount_preferred_currency_unit: preferred_currency_unit
+                currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+                currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+            }
+            lightspark_node_status: status
         }
-        invoice_data_memo: memo
     }
 }
 """
 
 
-def from_json(requester: Requester, obj: Mapping[str, Any]) -> PaymentRequestData:
-    if obj["__typename"] == "InvoiceData":
-        # pylint: disable=import-outside-toplevel
-        from lightspark.objects.InvoiceData import InvoiceData
-
-        return InvoiceData(
-            requester=requester,
-            typename="InvoiceData",
-            encoded_payment_request=obj["invoice_data_encoded_payment_request"],
-            bitcoin_network=parse_enum(
-                BitcoinNetwork, obj["invoice_data_bitcoin_network"]
-            ),
-            payment_hash=obj["invoice_data_payment_hash"],
-            amount=CurrencyAmount_from_json(requester, obj["invoice_data_amount"]),
-            created_at=obj["invoice_data_created_at"],
-            expires_at=obj["invoice_data_expires_at"],
-            destination=Node_from_json(requester, obj["invoice_data_destination"]),
-            memo=obj["invoice_data_memo"],
-        )
-    graphql_typename = obj["__typename"]
-    raise LightsparkException(
-        "UNKNOWN_INTERFACE",
-        f"Couldn't find a concrete type for interface PaymentRequestData corresponding to the typename={graphql_typename}",
+def from_json(requester: Requester, obj: Mapping[str, Any]) -> InvoiceData:
+    return InvoiceData(
+        requester=requester,
+        typename="InvoiceData",
+        encoded_payment_request=obj["invoice_data_encoded_payment_request"],
+        bitcoin_network=parse_enum(BitcoinNetwork, obj["invoice_data_bitcoin_network"]),
+        payment_hash=obj["invoice_data_payment_hash"],
+        amount=CurrencyAmount_from_json(requester, obj["invoice_data_amount"]),
+        created_at=obj["invoice_data_created_at"],
+        expires_at=obj["invoice_data_expires_at"],
+        memo=obj["invoice_data_memo"],
+        destination=Node_from_json(requester, obj["invoice_data_destination"]),
     )
```

### Comparing `lightspark-1.0.0/lightspark/objects/Permission.py` & `lightspark-1.1.0/lightspark/objects/Permission.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/RequestWithdrawalInput.py` & `lightspark-1.1.0/lightspark/objects/RequestWithdrawalInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/RequestWithdrawalOutput.py` & `lightspark-1.1.0/lightspark/objects/RequestWithdrawalOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/RichText.py` & `lightspark-1.1.0/lightspark/objects/RichText.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/RoutingTransaction.py` & `lightspark-1.1.0/lightspark/objects/RoutingTransaction.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/RoutingTransactionFailureReason.py` & `lightspark-1.1.0/lightspark/objects/RoutingTransactionFailureReason.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Secret.py` & `lightspark-1.1.0/lightspark/objects/Secret.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/SendPaymentInput.py` & `lightspark-1.1.0/lightspark/objects/SendPaymentInput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/SendPaymentOutput.py` & `lightspark-1.1.0/lightspark/objects/SendPaymentOutput.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Transaction.py` & `lightspark-1.1.0/lightspark/objects/Transaction.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,15 @@
                     currency_amount_original_unit: original_unit
                     currency_amount_preferred_currency_unit: preferred_currency_unit
                     currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                     currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                 }
                 invoice_data_created_at: created_at
                 invoice_data_expires_at: expires_at
+                invoice_data_memo: memo
                 invoice_data_destination: destination {
                     __typename
                     ... on GraphNode {
                         __typename
                         graph_node_id: id
                         graph_node_created_at: created_at
                         graph_node_updated_at: updated_at
@@ -336,15 +337,14 @@
                             currency_amount_preferred_currency_unit: preferred_currency_unit
                             currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
                             currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
                         }
                         lightspark_node_status: status
                     }
                 }
-                invoice_data_memo: memo
             }
         }
         outgoing_payment_failure_reason: failure_reason
         outgoing_payment_failure_message: failure_message {
             __typename
             rich_text_text: text
         }
```

### Comparing `lightspark-1.0.0/lightspark/objects/TransactionFailures.py` & `lightspark-1.1.0/lightspark/objects/TransactionFailures.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/TransactionStatus.py` & `lightspark-1.1.0/lightspark/objects/TransactionStatus.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/TransactionType.py` & `lightspark-1.1.0/lightspark/objects/TransactionType.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/Withdrawal.py` & `lightspark-1.1.0/lightspark/objects/Withdrawal.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/WithdrawalRequest.py` & `lightspark-1.1.0/lightspark/objects/WithdrawalRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     updated_at: datetime
     """The date and time when the entity was last updated."""
 
     amount: CurrencyAmount
     """The amount of money that should be withdrawn in this request."""
 
+    estimated_amount: Optional[CurrencyAmount]
+    """If the requested amount is `-1` (i.e. everything), this field may contain an estimate of the amount for the withdrawal."""
+
     bitcoin_address: str
     """The bitcoin address where the funds should be sent."""
 
     withdrawal_mode: WithdrawalMode
     """The strategy that should be used to withdraw the funds from the account."""
 
     status: WithdrawalRequestStatus
@@ -195,14 +198,22 @@
         __typename
         currency_amount_original_value: original_value
         currency_amount_original_unit: original_unit
         currency_amount_preferred_currency_unit: preferred_currency_unit
         currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
         currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
     }
+    withdrawal_request_estimated_amount: estimated_amount {
+        __typename
+        currency_amount_original_value: original_value
+        currency_amount_original_unit: original_unit
+        currency_amount_preferred_currency_unit: preferred_currency_unit
+        currency_amount_preferred_currency_value_rounded: preferred_currency_value_rounded
+        currency_amount_preferred_currency_value_approx: preferred_currency_value_approx
+    }
     withdrawal_request_bitcoin_address: bitcoin_address
     withdrawal_request_withdrawal_mode: withdrawal_mode
     withdrawal_request_status: status
     withdrawal_request_completed_at: completed_at
     withdrawal_request_withdrawal: withdrawal {
         id
     }
@@ -214,14 +225,19 @@
     return WithdrawalRequest(
         requester=requester,
         typename="WithdrawalRequest",
         id=obj["withdrawal_request_id"],
         created_at=obj["withdrawal_request_created_at"],
         updated_at=obj["withdrawal_request_updated_at"],
         amount=CurrencyAmount_from_json(requester, obj["withdrawal_request_amount"]),
+        estimated_amount=CurrencyAmount_from_json(
+            requester, obj["withdrawal_request_estimated_amount"]
+        )
+        if obj["withdrawal_request_estimated_amount"]
+        else None,
         bitcoin_address=obj["withdrawal_request_bitcoin_address"],
         withdrawal_mode=parse_enum(
             WithdrawalMode, obj["withdrawal_request_withdrawal_mode"]
         ),
         status=parse_enum(WithdrawalRequestStatus, obj["withdrawal_request_status"]),
         completed_at=obj["withdrawal_request_completed_at"],
         withdrawal_id=obj["withdrawal_request_withdrawal"]["id"]
```

### Comparing `lightspark-1.0.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py` & `lightspark-1.1.0/lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py` & `lightspark-1.1.0/lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/objects/all_entities.py` & `lightspark-1.1.0/lightspark/objects/all_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 from lightspark.objects.RoutingTransaction import RoutingTransaction
 from lightspark.objects.RoutingTransaction import (
     from_json as RoutingTransaction_from_json,
 )
 from lightspark.objects.Transaction import FRAGMENT as TransactionFragment
 from lightspark.objects.Transaction import Transaction
 from lightspark.objects.Transaction import from_json as Transaction_from_json
+from lightspark.objects.Wallet import FRAGMENT as WalletFragment
+from lightspark.objects.Wallet import Wallet
+from lightspark.objects.Wallet import from_json as Wallet_from_json
 from lightspark.objects.Withdrawal import FRAGMENT as WithdrawalFragment
 from lightspark.objects.Withdrawal import Withdrawal
 from lightspark.objects.Withdrawal import from_json as Withdrawal_from_json
 from lightspark.objects.WithdrawalRequest import FRAGMENT as WithdrawalRequestFragment
 from lightspark.objects.WithdrawalRequest import WithdrawalRequest
 from lightspark.objects.WithdrawalRequest import (
     from_json as WithdrawalRequest_from_json,
@@ -181,14 +184,18 @@
             ...RoutingTransactionFragment
         }
 """,
     Transaction: """        ... on Transaction {
             ...TransactionFragment
         }
 """,
+    Wallet: """        ... on Wallet {
+            ...WalletFragment
+        }
+""",
     Withdrawal: """        ... on Withdrawal {
             ...WithdrawalFragment
         }
 """,
     WithdrawalRequest: """        ... on WithdrawalRequest {
             ...WithdrawalRequestFragment
         }
@@ -212,14 +219,15 @@
     Node: NodeFragment,
     OnChainTransaction: OnChainTransactionFragment,
     OutgoingPayment: OutgoingPaymentFragment,
     OutgoingPaymentAttempt: OutgoingPaymentAttemptFragment,
     PaymentRequest: PaymentRequestFragment,
     RoutingTransaction: RoutingTransactionFragment,
     Transaction: TransactionFragment,
+    Wallet: WalletFragment,
     Withdrawal: WithdrawalFragment,
     WithdrawalRequest: WithdrawalRequestFragment,
 }
 ALL_JSON_LOADERS: Mapping[Type, Callable] = {
     Account: Account_from_json,
     ApiToken: ApiToken_from_json,
     Channel: Channel_from_json,
@@ -236,14 +244,15 @@
     Node: Node_from_json,
     OnChainTransaction: OnChainTransaction_from_json,
     OutgoingPayment: OutgoingPayment_from_json,
     OutgoingPaymentAttempt: OutgoingPaymentAttempt_from_json,
     PaymentRequest: PaymentRequest_from_json,
     RoutingTransaction: RoutingTransaction_from_json,
     Transaction: Transaction_from_json,
+    Wallet: Wallet_from_json,
     Withdrawal: Withdrawal_from_json,
     WithdrawalRequest: WithdrawalRequest_from_json,
 }
 
 
 def get_entity(
     requester: Requester, entity_id: str, entity_class: Type[ENTITY]
```

### Comparing `lightspark-1.0.0/lightspark/requests/requester.py` & `lightspark-1.1.0/lightspark/requests/requester.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from requests.utils import default_user_agent
 
 from lightspark.exceptions import LightsparkException
 from lightspark.requests.encoder import Encoder
 from lightspark.utils.crypto import sign_payload
 from lightspark.version import __version__
 
-DEFAULT_BASE_URL = "https://api.lightspark.com/graphql/2023-04-04"
+DEFAULT_BASE_URL = "https://api.lightspark.com/graphql/server/2023-04-04"
 
 logger = logging.getLogger("lightspark")
 
 
 class Requester:
     def __init__(
         self,
```

### Comparing `lightspark-1.0.0/lightspark/utils/crypto.py` & `lightspark-1.1.0/lightspark/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/utils/enums.py` & `lightspark-1.1.0/lightspark/utils/enums.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark/webhooks.py` & `lightspark-1.1.0/lightspark/webhooks.py`

 * *Files identical despite different names*

### Comparing `lightspark-1.0.0/lightspark.egg-info/SOURCES.txt` & `lightspark-1.1.0/lightspark.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 lightspark.egg-info/top_level.txt
 lightspark/objects/Account.py
 lightspark/objects/AccountToApiTokensConnection.py
 lightspark/objects/AccountToChannelsConnection.py
 lightspark/objects/AccountToNodesConnection.py
 lightspark/objects/AccountToPaymentRequestsConnection.py
 lightspark/objects/AccountToTransactionsConnection.py
+lightspark/objects/AccountToWalletsConnection.py
 lightspark/objects/ApiToken.py
+lightspark/objects/Balances.py
 lightspark/objects/BitcoinNetwork.py
 lightspark/objects/BlockchainBalance.py
 lightspark/objects/Channel.py
 lightspark/objects/ChannelClosingTransaction.py
 lightspark/objects/ChannelFees.py
 lightspark/objects/ChannelOpeningTransaction.py
 lightspark/objects/ChannelStatus.py
@@ -86,14 +88,15 @@
 lightspark/objects/Secret.py
 lightspark/objects/SendPaymentInput.py
 lightspark/objects/SendPaymentOutput.py
 lightspark/objects/Transaction.py
 lightspark/objects/TransactionFailures.py
 lightspark/objects/TransactionStatus.py
 lightspark/objects/TransactionType.py
+lightspark/objects/Wallet.py
 lightspark/objects/WebhookEventType.py
 lightspark/objects/Withdrawal.py
 lightspark/objects/WithdrawalMode.py
 lightspark/objects/WithdrawalRequest.py
 lightspark/objects/WithdrawalRequestStatus.py
 lightspark/objects/WithdrawalRequestToChannelClosingTransactionsConnection.py
 lightspark/objects/WithdrawalRequestToChannelOpeningTransactionsConnection.py
```

### Comparing `lightspark-1.0.0/setup.cfg` & `lightspark-1.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [metadata]
 name = lightspark
 url = https://www.lightspark.com/
 version = attr: lightspark.version.__version__
 description = Python SDK for the Lightspark API
 long_description = file: README.rst
+long_description_content_type = text/markdown
 author = Lightspark Group, Inc.
 author_email = info@lightspark.com
 license = Apache-2.0
 license_files = LICENSE.rst
 project_urls = 
 	Documentation = https://app.lightspark.com/docs/api
 	Source Code = https://github.com/lightsparkdev/python-sdk
 
 [options]
 packages = find:
 install_requires = 
 	cryptography
+	pyjwt
 	requests
 
 [options.packages.find]
 include = lightspark*
 
 [egg_info]
 tag_build =
```

