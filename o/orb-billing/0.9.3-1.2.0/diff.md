# Comparing `tmp/orb-billing-0.9.3.tar.gz` & `tmp/orb-billing-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orb-billing-0.9.3.tar", last modified: Wed May 10 08:35:22 2023, max compression
+gzip compressed data, was "orb-billing-1.2.0.tar", last modified: Thu Apr  6 00:29:12 2023, max compression
```

## Comparing `orb-billing-0.9.3.tar` & `orb-billing-1.2.0.tar`

### file list

```diff
@@ -1,80 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.724232 orb-billing-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 08:35:12.000000 orb-billing-0.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-10 08:35:22.724232 orb-billing-0.9.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     5908 2023-05-10 08:35:12.000000 orb-billing-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:35:22.724232 orb-billing-0.9.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-05-10 08:35:12.000000 orb-billing-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.716232 orb-billing-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.720232 orb-billing-0.9.3/src/orb/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/availability.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13362 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/credits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32036 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22316 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4837 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.720232 orb-billing-0.9.3/src/orb/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.720232 orb-billing-0.9.3/src/orb/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11367 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13268 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customer_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_balance_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3016 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_credits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_credits_ledger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_customers_external_customer_id_external_customer_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13360 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_external_customer_costs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      775 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_invoice_invoice_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_invoices_upcoming.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_plans_external_plan_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      744 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_plans_plan_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13062 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_cost.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3119 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_usage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/list_customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/list_invoices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/list_plans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1667 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/list_subscriptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5162 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/patch_customers_customer_id_usage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5294 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/patch_external_customers_customer_id_usage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      577 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_customers_customer_id_credits_ledger_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_events_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7648 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_ingest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18901 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_subscriptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1339 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_cancel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17056 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_schedule_plan_change.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_plan_changes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6800 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/put_customers_customer_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6889 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/put_customers_external_customer_id_external_customer_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/put_deprecate_events_event_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4286 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/operations/put_events_event_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.724232 orb-billing-0.9.3/src/orb/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1595 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/billingaddress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4842 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/credit_ledger_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5131 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2849 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/customer_balance_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1868 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12401 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/invoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4494 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2270 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/plan_phase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18591 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/price.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1627 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/shippingaddress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5526 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/subscription.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8644 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/models/shared/upcominginvoice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5972 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/plan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5143 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    41533 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.724232 orb-billing-0.9.3/src/orb/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25963 2023-05-10 08:35:12.000000 orb-billing-0.9.3/src/orb/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:35:22.724232 orb-billing-0.9.3/src/orb_billing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-10 08:35:22.000000 orb-billing-0.9.3/src/orb_billing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 08:35:22.000000 orb-billing-0.9.3/src/orb_billing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:35:22.000000 orb-billing-0.9.3/src/orb_billing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-10 08:35:22.000000 orb-billing-0.9.3/src/orb_billing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 08:35:22.000000 orb-billing-0.9.3/src/orb_billing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.207509 orb-billing-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-06 00:29:01.000000 orb-billing-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-06 00:29:12.207509 orb-billing-1.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-04-06 00:29:01.000000 orb-billing-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 00:29:12.207509 orb-billing-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-06 00:29:01.000000 orb-billing-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.199509 orb-billing-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.203509 orb-billing-1.2.0/src/orb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2375 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/availability.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9009 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/coupon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14832 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/credits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39167 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23283 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9366 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.203509 orb-billing-1.2.0/src/orb/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.207509 orb-billing-1.2.0/src/orb/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13451 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4256 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/amend_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/delete_customers_customer_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2489 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/deprecate_event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1777 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_coupons.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_coupons_coupon_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13318 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customer_costs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13569 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customer_costs_by_external_customer_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1669 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_balance_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_credits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3175 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_credits_ledger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      868 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_customers_external_customer_id_external_customer_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_invoice_invoice_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2009 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_invoices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_invoices_upcoming.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_plans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_plans_external_plan_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      754 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_plans_plan_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13091 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscription_id_usage_by_customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1678 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscriptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_by_coupon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_id_usage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      842 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_subscription_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3143 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_subscription_id_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5204 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/patch_customers_customer_id_usage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5336 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/patch_customers_external_customer_id_usage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      430 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_coupons.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_coupons_coupon_id_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15945 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2046 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_customers_customer_id_balance_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5763 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_customers_customer_id_credits_ledger_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2306 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_events_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7700 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_ingest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_invoice_line_items.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_invoices_invoice_id_void.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21288 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_raw.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2339 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_cancel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17602 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_schedule_plan_change.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_cancellation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_plan_changes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2187 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_update_fixed_fee_quantity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15427 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/put_customers_customer_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6895 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/operations/put_customers_external_customer_id_external_customer_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.207509 orb-billing-1.2.0/src/orb/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2161 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5055 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/coupon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5646 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/credit_ledger_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16323 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/customer_balance_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9239 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/customer_tax_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20493 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/invoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14356 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/invoice_line_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2284 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/plan_phase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18683 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/price.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10297 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/subscription.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8889 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/models/shared/upcominginvoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6869 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5140 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65971 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.207509 orb-billing-1.2.0/src/orb/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-06 00:29:01.000000 orb-billing-1.2.0/src/orb/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 00:29:12.207509 orb-billing-1.2.0/src/orb_billing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-06 00:29:12.000000 orb-billing-1.2.0/src/orb_billing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-06 00:29:12.000000 orb-billing-1.2.0/src/orb_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 00:29:12.000000 orb-billing-1.2.0/src/orb_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-06 00:29:12.000000 orb-billing-1.2.0/src/orb_billing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-06 00:29:12.000000 orb-billing-1.2.0/src/orb_billing.egg-info/top_level.txt
```

### Comparing `orb-billing-0.9.3/LICENSE.md` & `orb-billing-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orb-billing-0.9.3/setup.py` & `orb-billing-1.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="orb-billing",
-    version="0.9.3",
-    author="Orb-Speakeasy",
-    description="Python Client SDK Generated by Speakeasy",
+    version="1.2.0",
+    author="speakeasy-sdks",
+    description="Python Client for Orb API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi==2022.12.7",
+        "certifi==2022.12.07",
         "charset-normalizer==2.1.1",
         "dataclasses-json-speakeasy==0.5.8",
         "idna==3.3",
         "marshmallow==3.17.1",
         "marshmallow-enum==1.5.1",
         "mypy-extensions==0.4.3",
         "packaging==21.3",
```

### Comparing `orb-billing-0.9.3/src/orb/availability.py` & `orb-billing-1.2.0/src/orb/availability.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import requests as requests_http
 from . import utils
 from orb.models import operations
 from typing import Optional
 
 class Availability:
-    r"""Actions related to API availability."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,29 +17,39 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def ping(self) -> operations.GetPingResponse:
+    def get_ping(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetPingResponse:
         r"""Check availability
         This endpoint allows you to test your connection to the Orb API and check the validity of your API key, passed in the `Authorization` header. This is particularly useful for checking that your environment is set up properly, and is a great choice for connectors and integrations.
         
         This API does not have any side-effects or return any Orb resources.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/ping'
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPingResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetPing200ApplicationJSON])
```

### Comparing `orb-billing-0.9.3/src/orb/credits.py` & `orb-billing-1.2.0/src/orb/credits.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import requests as requests_http
 from . import utils
 from orb.models import operations, shared
 from typing import Optional
 
 class Credits:
-    r"""Actions related to credit management."""
+    r"""Create and query credits"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,23 +18,125 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def get(self, customer_id: str, request_body: Optional[operations.PostCustomersCustomerIDCreditsLedgerEntryRequestBody] = None) -> operations.PostCustomersCustomerIDCreditsLedgerEntryResponse:
+    def get_customers_customer_id_credits(self, request: operations.GetCustomersCustomerIDCreditsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersCustomerIDCreditsResponse:
+        r"""Retrieve credit balance
+        This [paginated endpoint](../docs/Pagination.md) can be used to fetch the current state of credit balance for the specified `customer_id`.
+        
+        Orb keeps track of credit balances in _credit blocks_, where each block is optionally associated with an `expiry_date`. Each time credits are added, a new credit block is created. Credits which do not expire have an `expiry_date` of `null`. To aid in revenue recognition, credit blocks can optionally have a `per_unit_cost_basis`, to indicate how much in USD a customer paid for a single credit in a block.
+        
+        Orb only returns _unexpired_ credit blocks in this response. For credits that have already expired, you can view this deduction from the customer's balance in the [Credit Ledger](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger/get) response.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetCustomersCustomerIDCreditsRequest, base_url, '/customers/{customer_id}/credits', request)
+        
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetCustomersCustomerIDCreditsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDCredits200ApplicationJSON])
+                res.get_customers_customer_id_credits_200_application_json_object = out
+
+        return res
+
+    def get_customers_customer_id_credits_ledger(self, request: operations.GetCustomersCustomerIDCreditsLedgerRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersCustomerIDCreditsLedgerResponse:
+        r"""View credits ledger
+        The credits ledger provides _auditing_ functionality over Orb's credits system with a list of actions that have taken place to modify a customer's credit balance. This [paginated endpoint](../docs/Pagination.md) lists these entries, starting from the most recent ledger entry.
+        
+        More details on using Orb's real-time credit feature are [here](../docs/Pre-paid-plans.md).
+        
+        There are four major types of modifications to credit balance, detailed below.
+        
+        ## Increment
+        Credits (which optionally expire on a future date) can be added via the API ([Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)). The ledger entry for such an action will always contain the total eligible starting and ending balance for the customer at the time the entry was added to the ledger. 
+        
+        ## Decrement
+        
+        Deductions can occur as a result of an API call to create a ledger entry (see [Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)), or automatically as a result of incurring usage. Both ledger entries present the `decrement` entry type.
+        
+        As usage for a customer is reported into Orb, credits may be deducted according to the customer's plan configuration. An automated deduction of this type will result in a ledger entry, also with a starting and ending balance. In order to provide better tracing capabilities for automatic deductions, Orb always associates each automatic deduction with the `event_id` at the time of ingestion, used to pinpoint _why_ credit deduction took place and to ensure that credits are never deducted without an associated usage event. 
+        
+        By default, Orb uses an algorithm that automatically deducts from the *soonest expiring credit block* first in order to ensure that all credits are utilized appropriately. As an example, if trial credits with an expiration date of 2 weeks from now are present for a customer, they will be used before any deductions take place from a non-expiring credit block. 
+        
+        If there are multiple blocks with the same expiration date, Orb will deduct from the block with the *lower cost basis* first (ex. trial credits with a $0 cost basis before paid credits with a $5.00 cost basis). 
+        
+        It's also possible for a single usage event's deduction to _span_ credit blocks. In this case, Orb will deduct from the next block, ending at the credit block which consists of unexpiring credits. Each of these deductions will lead to a _separate_ ledger entry, one per credit block that is deducted from. By default, the customer's total credit balance in Orb can be negative as a result of a decrement. 
+        
+        ## Expiration change
+        
+        The expiry of credits can be changed as a result of the API (See [Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)). This will create a ledger entry that specifies the balance as well as the initial and target expiry dates. 
+        
+        Note that for this entry type, `starting_balance` will equal `ending_balance`, and the `amount` represents the balance transferred. The credit block linked to the ledger entry is the source credit block from which there was an expiration change.
+        
+        
+        ## Credits expiry
+        
+        When a set of credits expire on pre-set expiration date, the customer's balance automatically reflects this change and adds an entry to the ledger indicating this event. Note that credit expiry should always happen close to a date boundary in the customer's timezone.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetCustomersCustomerIDCreditsLedgerRequest, base_url, '/customers/{customer_id}/credits/ledger', request)
+        
+        query_params = utils.get_query_params(operations.GetCustomersCustomerIDCreditsLedgerRequest, request)
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetCustomersCustomerIDCreditsLedgerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDCreditsLedger200ApplicationJSON])
+                res.get_customers_customer_id_credits_ledger_200_application_json_object = out
+
+        return res
+
+    def post_customers_customer_id_credits_ledger_entry(self, request: operations.PostCustomersCustomerIDCreditsLedgerEntryRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostCustomersCustomerIDCreditsLedgerEntryResponse:
         r"""Add credit ledger entry
         This endpoint allows you to create a new ledger entry for a specified customer's balance. This can be used to increment balance, deduct credits, and change the expiry date of existing credits.
         
         ## Effects of adding a ledger entry
         1. After calling this endpoint, [Fetch Credit Balance](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits/get) will return a credit block that represents the changes (i.e. balance changes or transfers).
         2. A ledger entry will be added to the credits ledger for this customer, and therefore returned in the [View Credits Ledger](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger/get) response as well as serialized in the response to this request. In the case of deductions without a specified block, multiple ledger entries may be created if the deduction spans credit blocks.
-        
+        3. If `invoice_settings` is specified, an invoice will be created that reflects the cost of the credits (based on `amount` and `per_unit_cost_basis`).
         
         ## Adding credits
         Adding credits is done by creating an entry of type `increment`. This requires the caller to specify a number of credits as well as an optional expiry date in `YYYY-MM-DD` format. Orb also recommends specifying a description to assist with auditing. When adding credits, the caller can also specify a cost basis per-credit, to indicate how much in USD a customer paid for a single credit in a block. This can later be used for revenue recognition.
         
         The following snippet illustrates a sample request body to increment credits which will expire in January of 2022.
         
         ```json
@@ -45,16 +147,19 @@
           \"per_unit_cost_basis\": \"0.20\",
           \"description\": \"Purchased 100 credits\"
         }
         ```
         
         Note that by default, Orb will always first increment any _negative_ balance in existing blocks before adding the remaining amount to the desired credit block.
         
+        ### Invoicing for credits
+        By default, Orb manipulates the credit ledger but does not charge for credits. However, if you pass `invoice_settings` in the body of this request, Orb will also generate a one-off invoice for the customer for the credits pre-purchase. Note that you _must_ provide the `per_unit_cost_basis`, since the total charges on the invoice are calculated by multiplying the cost basis with the number of credit units added.
+        
         ## Deducting Credits
-        Orb allows you to deduct credits from a customer by creating an entry of type `decrement`. Orb matches the algorithm for [Automatic Deductions](Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger/get) for determining which credit blocks to decrement from. In the case that the deduction leads to multiple ledger entries, the response from this endpoint will be the final deduction. Orb also optionally allows specifying a description to assist with auditing.
+        Orb allows you to deduct credits from a customer by creating an entry of type `decrement`. Orb matches the algorithm for [Automatic Deductions](Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger/get#decrement) for determining which credit blocks to decrement from. In the case that the deduction leads to multiple ledger entries, the response from this endpoint will be the final deduction. Orb also optionally allows specifying a description to assist with auditing.
         
         The following snippet illustrates a sample request body to decrement credits.
         
         ```json
         {
           \"entry_type\": \"decrement\",
           \"amount\": 20,
@@ -76,128 +181,42 @@
           \"expiry_date\": \"2022-12-28\",
           \"block_id\": \"UiUhFWeLHPrBY4Ad\",
           \"target_expiry_date\": \"2023-12-28\",
           \"description\": \"Extending credit validity\"
         }
         ```
         """
-        request = operations.PostCustomersCustomerIDCreditsLedgerEntryRequest(
-            customer_id=customer_id,
-            request_body=request_body,
-        )
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PostCustomersCustomerIDCreditsLedgerEntryRequest, base_url, '/customers/{customer_id}/credits/ledger_entry', request)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostCustomersCustomerIDCreditsLedgerEntryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreditLedgerEntry])
                 res.credit_ledger_entry = out
 
         return res
 
-    
-    def get_credits(self, customer_id: str) -> operations.GetCustomersCustomerIDCreditsResponse:
-        r"""Retrieve credit balance
-        This [paginated endpoint](docs/Pagination.md) can be used to fetch the current state of credit balance for the specified `customer_id`.
-        
-        Orb keeps track of credit balances in _credit blocks_, where each block is optionally associated with an `expiry_date`. Each time credits are added, a new credit block is created. Credits which do not expire have an `expiry_date` of `null`. To aid in revenue recognition, credit blocks can optionally have a `per_unit_cost_basis`, to indicate how much in USD a customer paid for a single credit in a block.
-        
-        Orb only returns _unexpired_ credit blocks in this response. For credits that have already expired, you can view this deduction from the customer's balance in the [Credit Ledger](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger/get) response.
-        """
-        request = operations.GetCustomersCustomerIDCreditsRequest(
-            customer_id=customer_id,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCustomersCustomerIDCreditsRequest, base_url, '/customers/{customer_id}/credits', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCustomersCustomerIDCreditsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDCredits200ApplicationJSON])
-                res.get_customers_customer_id_credits_200_application_json_object = out
-
-        return res
-
-    
-    def get_credits_ledger(self, customer_id: str, entry_status: Optional[operations.GetCustomersCustomerIDCreditsLedgerEntryStatusEnum] = None, entry_type: Optional[operations.GetCustomersCustomerIDCreditsLedgerEntryTypeEnum] = None, minimum_amount: Optional[float] = None) -> operations.GetCustomersCustomerIDCreditsLedgerResponse:
-        r"""View credits ledger
-        The credits ledger provides _auditing_ functionality over Orb's credits system with a list of actions that have taken place to modify a customer's credit balance. This [paginated endpoint](../docs/Pagination.md) lists these entries, starting from the most recent ledger entry.
-        
-        More details on using Orb's real-time credit feature are [here](../docs/Credits.md).
-        
-        There are four major types of modifications to credit balance, detailed below.
-        
-        ## Increment
-        Credits (which optionally expire on a future date) can be added via the API ([Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)). The ledger entry for such an action will always contain the total eligible starting and ending balance for the customer at the time the entry was added to the ledger. 
-        
-        ## Decrement
-        
-        Deductions can occur as a result of an API call to create a ledger entry (see [Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)), or automatically as a result of incurring usage. Both ledger entries present the `decrement` entry type.
-        
-        As usage for a customer is reported into Orb, credits may be deducted according to the customer's plan configuration. An automated deduction of this type will result in a ledger entry, also with a starting and ending balance. In order to provide better tracing capabilities for automatic deductions, Orb always associates each automatic deduction with the `event_id` at the time of ingestion, used to pinpoint _why_ credit deduction took place and to ensure that credits are never deducted without an associated usage event. 
-        
-        By default, Orb uses an algorithm that automatically deducts from the *soonest expiring credit block* first in order to ensure that all credits are utilized appropriately. As an example, if trial credits are present for a customer, they will be used before any deduction take place from non-expiring credits. 
-        
-        It's also possible for a single usage event's deduction to _span_ credit blocks. In this case, Orb will deduct from the next block, ending at the credit block which consists of unexpiring credits. Each of these deductions will lead to a _separate_ ledger entry, one per credit block that is deducted from. By default, the customer's total credit balance in Orb can be negative as a result of a decrement. 
-        
-        ## Expiration change
-        
-        The expiry of credits can be changed as a result of the API (See [Add Ledger Entry](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1credits~1ledger_entry/post)). This will create a ledger entry that specifies the balance as well as the initial and target expiry dates. 
-        
-        Note that for this entry type, `starting_balance` will equal `ending_balance`, and the `amount` represents the balance transferred. The credit block linked to the ledger entry is the source credit block from which there was an expiration change.
-        
-        
-        ## Credits expiry
-        
-        When a set of credits expire on pre-set expiration date, the customer's balance automatically reflects this change and adds an entry to the ledger indicating this event. Note that credit expiry should always happen close to a date boundary in the customer's timezone.
-        """
-        request = operations.GetCustomersCustomerIDCreditsLedgerRequest(
-            customer_id=customer_id,
-            entry_status=entry_status,
-            entry_type=entry_type,
-            minimum_amount=minimum_amount,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCustomersCustomerIDCreditsLedgerRequest, base_url, '/customers/{customer_id}/credits/ledger', request)
-        
-        query_params = utils.get_query_params(operations.GetCustomersCustomerIDCreditsLedgerRequest, request)
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url, params=query_params)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCustomersCustomerIDCreditsLedgerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDCreditsLedger200ApplicationJSON])
-                res.get_customers_customer_id_credits_ledger_200_application_json_object = out
-
-        return res
-
```

### Comparing `orb-billing-0.9.3/src/orb/customer.py` & `orb-billing-1.2.0/src/orb/customer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from datetime import datetime
 from orb.models import operations, shared
 from typing import Optional
 
 class Customer:
-    r"""Actions related to customer management."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,149 +17,47 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def create(self, request: shared.Customer) -> operations.PostCustomersResponse:
-        r"""Create customer
-        This operation is used to create an Orb customer, who is party to the core billing relationship. See [Customer](../reference/Orb-API.json/components/schemas/Customer) for an overview of the customer resource.
+    def delete_customers_customer_id(self, request: operations.DeleteCustomersCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeleteCustomersCustomerIDResponse:
+        r"""Delete a customer
+        This performs a deletion of this customer, its subscriptions, and its invoices. This operation is irreversible. Note that this is a _soft_ deletion, but the data will be inaccessible through the API and Orb dashboard. For hard-deletion, please reach out to the Orb team directly.
         
-        This endpoint is critical in the following Orb functionality:
-        * Automated charges can be configured by setting `payment_provider` and `payment_provider_id` to automatically issue invoices
-        * [Customer ID Aliases](../docs/Customer-ID-Aliases.md) can be configured by setting `external_customer_id`
-        * [Timezone localization](../docs/Timezone-localization.md) can be configured on a per-customer basis by setting the `timezone` parameter
+        **Note**: This operation happens asynchronously and can be expected to take a few minutes to propagate to related resources. However, querying for the customer on subsequent GET requests while deletion is in process will reflect its deletion with a `deleted: true` property. Once the customer deletion has been fully processed, the customer will not be returned in the API.
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/customers'
+        url = utils.generate_url(operations.DeleteCustomersCustomerIDRequest, base_url, '/customers/{customer_id}', request)
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PostCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 201:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
-                res.customer = out
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
 
-        return res
-
-    
-    def get(self, customer_id: str) -> operations.GetCustomersCustomerIDResponse:
-        r"""Retrieve a customer
-        This endpoint is used to fetch customer details given an identifier.
+        def do_request():
+            return client.request('DELETE', url)
         
-        See the [Customer resource](Orb-API.json/components/schemas/Customer) for a full discussion of the Customer model.
-        """
-        request = operations.GetCustomersCustomerIDRequest(
-            customer_id=customer_id,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCustomersCustomerIDRequest, base_url, '/customers/{customer_id}', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCustomersCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeleteCustomersCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 201:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
-                res.customer = out
 
         return res
 
-    
-    def get_balance(self, customer_id: str) -> operations.GetCustomersCustomerIDBalanceTransactionsResponse:
-        r"""Get customer balance transactions
-        # The customer balance
-        
-        The customer balance is an amount in the customer's currency, which Orb automatically applies to subsequent invoices. This balance can be adjusted manually via Orb's webapp on the customer details page. You can use this balance to provide a fixed mid-period credit to the customer. Commonly, this is done due to system downtime/SLA violation, or an adhoc adjustment discussed with the customer.
-        
-        If the balance is a positive value at the time of invoicing, it represents that the customer has credit that should be used to offset the amount due on the next issued invoice. In this case, Orb will automatically reduce the next invoice by the balance amount, and roll over any remaining balance if the invoice is fully discounted.
-        
-        If the balance is a negative value at the time of invoicing, Orb will increase the invoice's amount due with a positive adjustment, and reset the balance to 0.
-        
-        This endpoint retrieves all customer balance transactions in reverse chronological order for a single customer, providing a complete audit trail of all adjustments and invoice applications.
-        
-        ## Eligibility
-        
-        The customer balance can only be applied to invoices or adjusted manually if invoices are not synced to a separate invoicing provider. If a payment gateway such as Stripe is used, the balance will be applied to the invoice before forwarding payment to the gateway.
-        """
-        request = operations.GetCustomersCustomerIDBalanceTransactionsRequest(
-            customer_id=customer_id,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCustomersCustomerIDBalanceTransactionsRequest, base_url, '/customers/{customer_id}/balance_transactions', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCustomersCustomerIDBalanceTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDBalanceTransactions200ApplicationJSON])
-                res.get_customers_customer_id_balance_transactions_200_application_json_object = out
-
-        return res
-
-    
-    def get_by_external_id(self, external_customer_id: str) -> operations.GetCustomersExternalCustomerIDExternalCustomerIDResponse:
-        r"""Retrieve a customer by external ID
-        This endpoint is used to fetch customer details given an `external_customer_id` (see [Customer ID Aliases](../docs/Customer-ID-Aliases.md)).
-        
-        Note that the resource and semantics of this endpoint exactly mirror [Get Customer](Orb-API.json/paths/~1customers/get).
-        """
-        request = operations.GetCustomersExternalCustomerIDExternalCustomerIDRequest(
-            external_customer_id=external_customer_id,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetCustomersExternalCustomerIDExternalCustomerIDRequest, base_url, '/customers/external_customer_id/{external_customer_id}', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetCustomersExternalCustomerIDExternalCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
-                res.customer = out
-
-        return res
-
-    
-    def get_costs(self, request: operations.GetCustomerCostsRequest) -> operations.GetCustomerCostsResponse:
+    def get_customer_costs(self, request: operations.GetCustomerCostsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomerCostsResponse:
         r"""View customer costs
         This endpoint is used to fetch a day-by-day snapshot of a customer's costs in Orb, calculated by applying pricing information to the underlying usage (see the [subscription usage endpoint](../reference/Orb-API.json/paths/~1subscriptions~1{subscription_id}~1usage/get) to fetch usage per metric, in usage units rather than a currency). 
         
         This endpoint can be leveraged for internal tooling and to provide a more transparent billing experience for your end users:
         
         1. Understand the cost breakdown per line item historically and in real-time for the current billing period. 
         2. Provide customer visibility into how different services are contributing to the overall invoice with a per-day timeseries (as compared to the [upcoming invoice](../reference/Orb-API.json/paths/~1invoices~1upcoming/get) resource, which represents a snapshot for the current period).
@@ -230,149 +126,227 @@
         
         url = utils.generate_url(operations.GetCustomerCostsRequest, base_url, '/customers/{customer_id}/costs', request)
         
         query_params = utils.get_query_params(operations.GetCustomerCostsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCustomerCostsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomerCosts200ApplicationJSON])
                 res.get_customer_costs_200_application_json_object = out
 
         return res
 
-    
-    def get_costs_by_external_id(self, request: operations.GetExternalCustomerCostsRequest) -> operations.GetExternalCustomerCostsResponse:
+    def get_customer_costs_by_external_customer_id(self, request: operations.GetCustomerCostsByExternalCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomerCostsByExternalCustomerIDResponse:
         r"""View customer costs by external customer ID
         This endpoint's resource and semantics exactly mirror [View customer costs](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1costs/get) but operates on an [external customer ID](../docs/Customer-ID-Aliases.md) rather than an Orb issued identifier.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetExternalCustomerCostsRequest, base_url, '/customers/external_customer_id/{external_customer_id}/costs', request)
+        url = utils.generate_url(operations.GetCustomerCostsByExternalCustomerIDRequest, base_url, '/customers/external_customer_id/{external_customer_id}/costs', request)
         
-        query_params = utils.get_query_params(operations.GetExternalCustomerCostsRequest, request)
+        query_params = utils.get_query_params(operations.GetCustomerCostsByExternalCustomerIDRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetExternalCustomerCostsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCustomerCostsByExternalCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetExternalCustomerCosts200ApplicationJSON])
-                res.get_external_customer_costs_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomerCostsByExternalCustomerID200ApplicationJSON])
+                res.get_customer_costs_by_external_customer_id_200_application_json_object = out
 
         return res
 
-    
-    def list(self) -> operations.ListCustomersResponse:
+    def get_customers(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersResponse:
         r"""List customers
         This endpoint returns a list of all customers for an account. The list of customers is ordered starting from the most recently created customer. This endpoint follows Orb's [standardized pagination format](../docs/Pagination.md).
         
         See [Customer](../reference/Orb-API.json/components/schemas/Customer) for an overview of the customer model.
         """
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/customers'
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCustomers200ApplicationJSON])
-                res.list_customers_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomers200ApplicationJSON])
+                res.get_customers_200_application_json_object = out
 
         return res
 
-    
-    def update(self, customer_id: str, request_body: Optional[operations.PutCustomersCustomerIDRequestBody] = None) -> operations.PutCustomersCustomerIDResponse:
-        r"""Update customer
-        This endpoint can be used to update the `payment_provider`, `payment_provider_id`, `name`, `email`, `shipping_address`, and `billing_address` of an existing customer.
+    def get_customers_customer_id(self, request: operations.GetCustomersCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersCustomerIDResponse:
+        r"""Retrieve a customer
+        This endpoint is used to fetch customer details given an identifier. If the `Customer` is in the process of being deleted, only the properties `id` and `deleted: true` will be returned.
         
-        Other fields on a customer are currently immutable.
+        See the [Customer resource](Orb-API.json/components/schemas/Customer) for a full discussion of the Customer model.
         """
-        request = operations.PutCustomersCustomerIDRequest(
-            customer_id=customer_id,
-            request_body=request_body,
-        )
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PutCustomersCustomerIDRequest, base_url, '/customers/{customer_id}', request)
+        url = utils.generate_url(operations.GetCustomersCustomerIDRequest, base_url, '/customers/{customer_id}', request)
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCustomersCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCustomersCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 201:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
                 res.customer = out
 
         return res
 
-    
-    def update_by_external_id(self, external_customer_id: str, request_body: Optional[operations.PutCustomersExternalCustomerIDExternalCustomerIDRequestBody] = None) -> operations.PutCustomersExternalCustomerIDExternalCustomerIDResponse:
-        r"""Update a customer by external ID
-        This endpoint is used to update customer details given an `external_customer_id` (see [Customer ID Aliases](../docs/Customer-ID-Aliases.md)).
+    def get_customers_customer_id_balance_transactions(self, request: operations.GetCustomersCustomerIDBalanceTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersCustomerIDBalanceTransactionsResponse:
+        r"""Get customer balance transactions
+        # The customer balance
         
-        Note that the resource and semantics of this endpoint exactly mirror [Update Customer](Orb-API.json/paths/~1customers~1{customer_id}/put).
+        The customer balance is an amount in the customer's currency, which Orb automatically applies to subsequent invoices. This balance can be adjusted manually via Orb's webapp on the customer details page. You can use this balance to provide a fixed mid-period credit to the customer. Commonly, this is done due to system downtime/SLA violation, or an adhoc adjustment discussed with the customer.
+        
+        If the balance is a positive value at the time of invoicing, it represents that the customer has credit that should be used to offset the amount due on the next issued invoice. In this case, Orb will automatically reduce the next invoice by the balance amount, and roll over any remaining balance if the invoice is fully discounted.
+        
+        If the balance is a negative value at the time of invoicing, Orb will increase the invoice's amount due with a positive adjustment, and reset the balance to 0.
+        
+        This endpoint retrieves all customer balance transactions in reverse chronological order for a single customer, providing a complete audit trail of all adjustments and invoice applications.
+        
+        ## Eligibility
+        
+        The customer balance can only be applied to invoices or adjusted manually if invoices are not synced to a separate invoicing provider. If a payment gateway such as Stripe is used, the balance will be applied to the invoice before forwarding payment to the gateway.
         """
-        request = operations.PutCustomersExternalCustomerIDExternalCustomerIDRequest(
-            external_customer_id=external_customer_id,
-            request_body=request_body,
-        )
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetCustomersCustomerIDBalanceTransactionsRequest, base_url, '/customers/{customer_id}/balance_transactions', request)
+        
         
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetCustomersCustomerIDBalanceTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCustomersCustomerIDBalanceTransactions200ApplicationJSON])
+                res.get_customers_customer_id_balance_transactions_200_application_json_object = out
+
+        return res
+
+    def get_customers_external_customer_id_external_customer_id(self, request: operations.GetCustomersExternalCustomerIDExternalCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCustomersExternalCustomerIDExternalCustomerIDResponse:
+        r"""Retrieve a customer by external ID
+        This endpoint is used to fetch customer details given an `external_customer_id` (see [Customer ID Aliases](../docs/Customer-ID-Aliases.md)).
+        
+        Note that the resource and semantics of this endpoint exactly mirror [Get Customer](Orb-API.json/paths/~1customers/get).
+        """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PutCustomersExternalCustomerIDExternalCustomerIDRequest, base_url, '/customers/external_customer_id/{external_customer_id}', request)
+        url = utils.generate_url(operations.GetCustomersExternalCustomerIDExternalCustomerIDRequest, base_url, '/customers/external_customer_id/{external_customer_id}', request)
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutCustomersExternalCustomerIDExternalCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCustomersExternalCustomerIDExternalCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
                 res.customer = out
 
         return res
 
-    
-    def update_usage(self, customer_id: str, timeframe_end: datetime, timeframe_start: datetime, request_body: Optional[operations.PatchCustomersCustomerIDUsageRequestBody] = None) -> operations.PatchCustomersCustomerIDUsageResponse:
+    def patch_customers_customer_id_usage(self, request: operations.PatchCustomersCustomerIDUsageRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PatchCustomersCustomerIDUsageResponse:
         r"""Amend customer usage
         This endpoint is used to amend usage within a timeframe for a customer that has an active subscription.
         
         This endpoint will mark _all_ existing events within `[timeframe_start, timeframe_end)` as _ignored_  for billing  purposes, and Orb will only use the _new_ events passed in the body of this request as the source of truth for that timeframe moving forwards. Note that a given time period can be amended any number of times, so events can be overwritten in subsequent calls to this endpoint.
         
         This is a powerful and audit-safe mechanism to retroactively change usage data in cases where you need to:
         - decrease historical usage consumption because of degraded service availability in your systems
@@ -421,34 +395,38 @@
         
         
         ## API Limits
         Note that Orb does not currently enforce a hard rate-limit for API usage or a maximum request payload size. Similar to the event ingestion API, this API is architected for high-throughput ingestion. It is also safe to _programmatically_ call this endpoint if your system can automatically detect a need for historical amendment.
         
         In order to overwrite timeframes with a very large number of events, we suggest using multiple calls with small adjacent (e.g. every hour) timeframes.
         """
-        request = operations.PatchCustomersCustomerIDUsageRequest(
-            customer_id=customer_id,
-            timeframe_end=timeframe_end,
-            timeframe_start=timeframe_start,
-            request_body=request_body,
-        )
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PatchCustomersCustomerIDUsageRequest, base_url, '/customers/{customer_id}/usage', request)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.PatchCustomersCustomerIDUsageRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('PATCH', url, params=query_params, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PATCH', url, params=query_params, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PatchCustomersCustomerIDUsageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PatchCustomersCustomerIDUsage200ApplicationJSON])
@@ -456,48 +434,212 @@
         elif http_res.status_code == 400:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PatchCustomersCustomerIDUsage400ApplicationJSON])
                 res.patch_customers_customer_id_usage_400_application_json_object = out
 
         return res
 
-    
-    def update_usage_by_external_id(self, external_customer_id: str, timeframe_end: datetime, timeframe_start: datetime, request_body: Optional[operations.PatchExternalCustomersCustomerIDUsageRequestBody] = None) -> operations.PatchExternalCustomersCustomerIDUsageResponse:
+    def patch_customers_external_customer_id_usage(self, request: operations.PatchCustomersExternalCustomerIDUsageRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PatchCustomersExternalCustomerIDUsageResponse:
         r"""Amend customer usage by external ID
-        This endpoint's resource and semantics exactly mirror [Amend customer usage](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1usage/patch) but operates on an [external customer ID](see (../docs/Customer-ID-Aliases.md)) rather than an Orb issued identifier.
+        This endpoint's resource and semantics exactly mirror [Amend customer usage](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1usage/patch) but operates on an [external customer ID](../docs/Customer-ID-Aliases.md) rather than an Orb issued identifier.
         """
-        request = operations.PatchExternalCustomersCustomerIDUsageRequest(
-            external_customer_id=external_customer_id,
-            timeframe_end=timeframe_end,
-            timeframe_start=timeframe_start,
-            request_body=request_body,
-        )
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PatchExternalCustomersCustomerIDUsageRequest, base_url, '/customers/external_customer_id/{external_customer_id}/usage', request)
+        url = utils.generate_url(operations.PatchCustomersExternalCustomerIDUsageRequest, base_url, '/customers/external_customer_id/{external_customer_id}/usage', request)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.PatchExternalCustomersCustomerIDUsageRequest, request)
+        query_params = utils.get_query_params(operations.PatchCustomersExternalCustomerIDUsageRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('PATCH', url, params=query_params, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PATCH', url, params=query_params, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PatchExternalCustomersCustomerIDUsageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PatchCustomersExternalCustomerIDUsageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PatchExternalCustomersCustomerIDUsage200ApplicationJSON])
-                res.patch_external_customers_customer_id_usage_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PatchCustomersExternalCustomerIDUsage200ApplicationJSON])
+                res.patch_customers_external_customer_id_usage_200_application_json_object = out
         elif http_res.status_code == 400:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PatchExternalCustomersCustomerIDUsage400ApplicationJSON])
-                res.patch_external_customers_customer_id_usage_400_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PatchCustomersExternalCustomerIDUsage400ApplicationJSON])
+                res.patch_customers_external_customer_id_usage_400_application_json_object = out
+
+        return res
+
+    def post_customers(self, request: operations.PostCustomersRequestBody, retries: Optional[utils.RetryConfig] = None) -> operations.PostCustomersResponse:
+        r"""Create customer
+        This operation is used to create an Orb customer, who is party to the core billing relationship. See [Customer](../reference/Orb-API.json/components/schemas/Customer) for an overview of the customer resource.
+        
+        This endpoint is critical in the following Orb functionality:
+        * Automated charges can be configured by setting `payment_provider` and `payment_provider_id` to automatically issue invoices
+        * [Customer ID Aliases](../docs/Customer-ID-Aliases.md) can be configured by setting `external_customer_id`
+        * [Timezone localization](../docs/Timezone-localization.md) can be configured on a per-customer basis by setting the `timezone` parameter
+        """
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/customers'
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 201:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
+                res.customer = out
+
+        return res
+
+    def post_customers_customer_id_balance_transactions(self, request: operations.PostCustomersCustomerIDBalanceTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostCustomersCustomerIDBalanceTransactionsResponse:
+        r"""Create a customer balance transaction
+        Creates an immutable balance transaction that updates the customer's balance and returns back the newly created [transaction](../reference/Orb-API.json/components/schemas/Customer-balance-transaction).
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PostCustomersCustomerIDBalanceTransactionsRequest, base_url, '/customers/{customer_id}/balance_transactions', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostCustomersCustomerIDBalanceTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CustomerBalanceTransaction])
+                res.customer_balance_transaction = out
+
+        return res
+
+    def put_customers_customer_id(self, request: operations.PutCustomersCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PutCustomersCustomerIDResponse:
+        r"""Update customer
+        This endpoint can be used to update the `payment_provider`, `payment_provider_id`, `name`, `email`, `shipping_address`, and `billing_address` of an existing customer.
+        
+        Other fields on a customer are currently immutable.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PutCustomersCustomerIDRequest, base_url, '/customers/{customer_id}', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PutCustomersCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
+                res.customer = out
+
+        return res
+
+    def put_customers_external_customer_id_external_customer_id(self, request: operations.PutCustomersExternalCustomerIDExternalCustomerIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PutCustomersExternalCustomerIDExternalCustomerIDResponse:
+        r"""Update a customer by external ID
+        This endpoint is used to update customer details given an `external_customer_id` (see [Customer ID Aliases](../docs/Customer-ID-Aliases.md)).
+        
+        Note that the resource and semantics of this endpoint exactly mirror [Update Customer](Orb-API.json/paths/~1customers~1{customer_id}/put).
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PutCustomersExternalCustomerIDExternalCustomerIDRequest, base_url, '/customers/external_customer_id/{external_customer_id}', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PutCustomersExternalCustomerIDExternalCustomerIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customer])
+                res.customer = out
 
         return res
```

### Comparing `orb-billing-0.9.3/src/orb/event.py` & `orb-billing-1.2.0/src/orb/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import requests as requests_http
 from . import utils
 from orb.models import operations
 from typing import Optional
 
 class Event:
-    r"""Actions related to event management."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,16 +17,71 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def deprecate(self, event_id: str) -> operations.PutDeprecateEventsEventIDResponse:
+    def amend_event(self, request: operations.AmendEventRequest, retries: Optional[utils.RetryConfig] = None) -> operations.AmendEventResponse:
+        r"""Amend single event
+        This endpoint is used to amend a single usage event with a given `event_id`. `event_id` refers to the `idempotency_key` passed in during ingestion. The event will maintain its existing `event_id` after the amendment.
+        
+        This endpoint will mark the existing event as ignored, and Orb will only use the new event passed in the body of this request as the source of truth for that `event_id`. Note that a single event can be amended any number of times, so the same event can be overwritten in subsequent calls to this endpoint, or overwritten using the [Amend customer usage](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1usage/patch) endpoint. Only a single event with a given `event_id` will be considered the source of truth at any given time.
+        
+        This is a powerful and audit-safe mechanism to retroactively update a single event in cases where you need to:
+        * update an event with new metadata as you iterate on your pricing model
+        * update an event based on the result of an external API call (ex. call to a payment gateway succeeded or failed)
+        
+        This amendment API is always audit-safe. The process will still retain the original event, though it will be ignored for billing calculations. For auditing and data fidelity purposes, Orb never overwrites or permanently deletes ingested usage data.
+        
+        ## Request validation
+        * The `timestamp` of the new event must match the `timestamp` of the existing event already ingested. As with ingestion, all timestamps must be sent in ISO8601 format with UTC timezone offset.
+        * The `customer_id` or `external_customer_id` of the new event must match the `customer_id` or `external_customer_id` of the existing event already ingested. Exactly one of `customer_id` and `external_customer_id` should be specified, and similar to ingestion, the ID must identify a Customer resource within Orb. Unlike ingestion, for event amendment, we strictly enforce that the Customer must be in the Orb system, even during the initial integration period. We do not allow updating the `Customer` an event is associated with.
+        * Orb does not accept an `idempotency_key` with the event in this endpoint, since this request is by design idempotent. On retryable errors, you should retry the request and assume the amendment operation has not succeeded until receipt of a 2xx. 
+        * The event's `timestamp` must fall within the customer's current subscription's billing period, or within the grace period of the customer's current subscription's previous billing period.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.AmendEventRequest, base_url, '/events/{event_id}', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.AmendEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.AmendEvent200ApplicationJSON])
+                res.amend_event_200_application_json_object = out
+        elif http_res.status_code == 400:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.AmendEvent400ApplicationJSON])
+                res.amend_event_400_application_json_object = out
+
+        return res
+
+    def deprecate_event(self, request: operations.DeprecateEventRequest, retries: Optional[utils.RetryConfig] = None) -> operations.DeprecateEventResponse:
         r"""Deprecate single event
         This endpoint is used to deprecate a single usage event with a given `event_id`. `event_id` refers to the `idempotency_key` passed in during ingestion. 
         
         This endpoint will mark the existing event as ignored. Note that if you attempt to re-ingest an event with the same `event_id` as a deprecated event, Orb will return an error.
         
         This is a powerful and audit-safe mechanism to retroactively deprecate a single event in cases where you need to:
         * no longer bill for an event that was improperly reported
@@ -38,43 +92,97 @@
         This API is always audit-safe. The process will still retain the deprecated event, though it will be ignored for billing calculations. For auditing and data fidelity purposes, Orb never overwrites or permanently deletes ingested usage data.
         
         ## Request validation
         * Orb does not accept an `idempotency_key` with the event in this endpoint, since this request is by design idempotent. On retryable errors, you should retry the request and assume the deprecation operation has not succeeded until receipt of a 2xx. 
         * The event's `timestamp` must fall within the customer's current subscription's billing period, or within the grace period of the customer's current subscription's previous billing period. Orb does not allow deprecating events for billing periods that have already invoiced customers.
         * The `customer_id` or the `external_customer_id` of the original event ingestion request must identify a Customer resource within Orb, even if this event was ingested during the initial integration period. We do not allow deprecating events for customers not in the Orb system.
         """
-        request = operations.PutDeprecateEventsEventIDRequest(
-            event_id=event_id,
-        )
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PutDeprecateEventsEventIDRequest, base_url, '/events/{event_id}/deprecate', request)
+        url = utils.generate_url(operations.DeprecateEventRequest, base_url, '/events/{event_id}/deprecate', request)
         
         
         client = self._security_client
         
-        http_res = client.request('PUT', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('PUT', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PutDeprecateEventsEventIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DeprecateEventResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutDeprecateEventsEventID200ApplicationJSON])
-                res.put_deprecate_events_event_id_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.DeprecateEvent200ApplicationJSON])
+                res.deprecate_event_200_application_json_object = out
         elif http_res.status_code == 400:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutDeprecateEventsEventID400ApplicationJSON])
-                res.put_deprecate_events_event_id_400_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.DeprecateEvent400ApplicationJSON])
+                res.deprecate_event_400_application_json_object = out
 
         return res
 
-    
-    def ingest(self, request_body: Optional[operations.PostIngestRequestBody] = None, debug: Optional[operations.PostIngestDebugEnum] = None) -> operations.PostIngestResponse:
+    def post_events_search(self, request: operations.PostEventsSearchRequestBody, retries: Optional[utils.RetryConfig] = None) -> operations.PostEventsSearchResponse:
+        r"""Search events
+        This endpoint returns a filtered set of events for an account in a paginated list format. 
+        
+        Note that this is a `POST` endpoint rather than a `GET` endpoint because it employs a JSON body for search criteria rather than query parameters, allowing for a more flexible search syntax.
+        
+        Note that a search criteria _must_ be specified. Currently, Orb supports the following criteria:
+        - `event_ids`: This is an explicit array of IDs to filter by. Note that an event's ID is the `idempotency_key` that was originally used for ingestion.
+        - `invoice_id`: This is an issued Orb invoice ID (see also [List Invoices](../reference/Orb-API.json/paths/~1invoices/get)). Orb will fetch all events that were used to calculate the invoice. In the common case, this will be a list of events whose `timestamp` property falls within the billing period specified by the invoice.
+        
+        By default, Orb does not return _deprecated_ events in this endpoint.
+        
+        By default, Orb will not throw a `404` if no events matched, Orb will return an empty array for `data` instead.
+        """
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/events/search'
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostEventsSearchResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.PostEventsSearch200ApplicationJSON])
+                res.post_events_search_200_application_json_object = out
+
+        return res
+
+    def post_ingest(self, request: operations.PostIngestRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostIngestResponse:
         r"""Ingest events
         Orb's event ingestion model and API is designed around two core principles:
         
         1. **Data fidelity**: The accuracy of your billing model depends on a robust foundation of events. Orb's API protocol encourages usage patterns that ensure that your data is consistently complete and correct.
         2. **Fast integration**: Sending events into Orb requires no tedious setup steps or explicit field schema for your event shape, making it instant to start streaming in usage in real-time.
         
         
@@ -206,32 +314,38 @@
         
         ```json
         {
           \"validation_failed\": []
         }
         ```
         """
-        request = operations.PostIngestRequest(
-            request_body=request_body,
-            debug=debug,
-        )
-        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/ingest'
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         query_params = utils.get_query_params(operations.PostIngestRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostIngestResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostIngest200ApplicationJSON])
@@ -239,97 +353,8 @@
         elif http_res.status_code == 400:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PostIngest400ApplicationJSON])
                 res.post_ingest_400_application_json_object = out
 
         return res
 
-    
-    def search(self, request: operations.PostEventsSearchRequestBody) -> operations.PostEventsSearchResponse:
-        r"""Search events
-        This endpoint returns a filtered set of events for an account in a paginated list format. 
-        
-        Note that this is a `POST` endpoint rather than a `GET` endpoint because it employs a JSON body for search criteria rather than query parameters, allowing for a more flexible search syntax.
-        
-        Note that a search criteria _must_ be specified. Currently, Orb supports the following criteria:
-        - `event_ids`: This is an explicit array of IDs to filter by. Note that an event's ID is the `idempotency_key` that was originally used for ingestion.
-        - `invoice_id`: This is an issued Orb invoice ID (see also [List Invoices](../reference/Orb-API.json/paths/~1invoices/get)). Orb will fetch all events that were used to calculate the invoice. In the common case, this will be a list of events whose `timestamp` property falls within the billing period specified by the invoice.
-        
-        By default, Orb does not return _deprecated_ events in this endpoint.
-        
-        By default, Orb will not throw a `404` if no events matched, Orb will return an empty array for `data` instead.
-        """
-        base_url = self._server_url
-        
-        url = base_url.removesuffix('/') + '/events/search'
-        
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        
-        client = self._security_client
-        
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PostEventsSearchResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostEventsSearch200ApplicationJSON])
-                res.post_events_search_200_application_json_object = out
-
-        return res
-
-    
-    def update(self, event_id: str, request_body: Optional[operations.PutEventsEventIDRequestBody] = None) -> operations.PutEventsEventIDResponse:
-        r"""Amend single event
-        This endpoint is used to amend a single usage event with a given `event_id`. `event_id` refers to the `idempotency_key` passed in during ingestion. The event will maintain its existing `event_id` after the amendment.
-        
-        This endpoint will mark the existing event as ignored, and Orb will only use the new event passed in the body of this request as the source of truth for that `event_id`. Note that a single event can be amended any number of times, so the same event can be overwritten in subsequent calls to this endpoint, or overwritten using the [Amend customer usage](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1usage/patch) endpoint. Only a single event with a given `event_id` will be considered the source of truth at any given time.
-        
-        This is a powerful and audit-safe mechanism to retroactively update a single event in cases where you need to:
-        * update an event with new metadata as you iterate on your pricing model
-        * update an event based on the result of an external API call (ex. call to a payment gateway succeeded or failed)
-        
-        This amendment API is always audit-safe. The process will still retain the original event, though it will be ignored for billing calculations. For auditing and data fidelity purposes, Orb never overwrites or permanently deletes ingested usage data.
-        
-        ## Request validation
-        * The `timestamp` of the new event must match the `timestamp` of the existing event already ingested. As with ingestion, all timestamps must be sent in ISO8601 format with UTC timezone offset.
-        * The `customer_id` or `external_customer_id` of the new event must match the `customer_id` or `external_customer_id` of the existing event already ingested. Exactly one of `customer_id` and `external_customer_id` should be specified, and similar to ingestion, the ID must identify a Customer resource within Orb. Unlike ingestion, for event amendment, we strictly enforce that the Customer must be in the Orb system, even during the initial integration period. We do not allow updating the `Customer` an event is associated with.
-        * Orb does not accept an `idempotency_key` with the event in this endpoint, since this request is by design idempotent. On retryable errors, you should retry the request and assume the amendment operation has not succeeded until receipt of a 2xx. 
-        * The event's `timestamp` must fall within the customer's current subscription's billing period, or within the grace period of the customer's current subscription's previous billing period.
-        """
-        request = operations.PutEventsEventIDRequest(
-            event_id=event_id,
-            request_body=request_body,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.PutEventsEventIDRequest, base_url, '/events/{event_id}', request)
-        
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        
-        client = self._security_client
-        
-        http_res = client.request('PUT', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PutEventsEventIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutEventsEventID200ApplicationJSON])
-                res.put_events_event_id_200_application_json_object = out
-        elif http_res.status_code == 400:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PutEventsEventID400ApplicationJSON])
-                res.put_events_event_id_400_application_json_object = out
-
-        return res
-
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customer_costs.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customer_costs.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,46 +18,46 @@
     CUMULATIVE = 'cumulative'
 
 
 @dataclasses.dataclass
 class GetCustomerCostsRequest:
     
     customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
-    r"""The Orb Customer ID"""
+    r"""The Orb Customer ID"""  
     group_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'group_by', 'style': 'form', 'explode': True }})
-    r"""Groups per-price costs by the key provided."""
+    r"""Groups per-price costs by the key provided."""  
     timeframe_end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""Costs returned are exclusive of `timeframe_end`."""
+    r"""Costs returned are exclusive of `timeframe_end`."""  
     timeframe_start: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""Costs returned are inclusive of `timeframe_start`."""
+    r"""Costs returned are inclusive of `timeframe_start`."""  
     view_mode: Optional[GetCustomerCostsViewModeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'view_mode', 'style': 'form', 'explode': True }})
-    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""
+    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomerCosts200ApplicationJSONDataPerPriceCostsPriceGroups:
     
     grouping_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_key') }})
-    r"""Grouping key to break down a single price's costs"""
-    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})
+    r"""Grouping key to break down a single price's costs"""  
+    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""
+    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""  
     secondary_grouping_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_key'), 'exclude': lambda f: f is None }})
-    r"""If the price is a matrix price, this is the second dimension key"""
-    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})
+    r"""If the price is a matrix price, this is the second dimension key"""  
+    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomerCosts200ApplicationJSONDataPerPriceCosts:
     r"""Price's contributions for the timeframe, excluding any transforms (minimums and discounts)."""
     
     price_groups: list[GetCustomerCosts200ApplicationJSONDataPerPriceCostsPriceGroups] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_groups') }})
-    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""
+    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""  
     price: Optional[shared_price.Price] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price'), 'exclude': lambda f: f is None }})
     r"""Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given Price object. The model_type field determines the key for the configuration object that is present.
     
     ## Unit pricing
     With unit pricing, each unit costs a fixed amount.
     ```json
     {
@@ -227,45 +227,45 @@
         \"unit_config\": {
            \"unit_amount\": \"2.00\"
         },
         \"fixed_price_quantity\": 3.0
         ...
     }
     ```
-    """
+    """  
     subtotal: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""
+    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""  
     total: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, including any minimums and discounts."""
+    r"""Price's contributions for the timeframe, including any minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomerCosts200ApplicationJSONData:
     
-    per_price_costs: list[GetCustomerCosts200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})
+    per_price_costs: list[GetCustomerCosts200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})  
     subtotal: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal') }})
-    r"""Total costs for the timeframe, excluding minimums and discounts."""
-    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""Total costs for the timeframe, excluding minimums and discounts."""  
+    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for the timeframe, including minimums and discounts."""
+    r"""Total costs for the timeframe, including minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomerCosts200ApplicationJSON:
     r"""OK"""
     
-    data: list[GetCustomerCosts200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[GetCustomerCosts200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
 class GetCustomerCostsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_customer_costs_200_application_json_object: Optional[GetCustomerCosts200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDRequest:
     
     customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
-    r"""Orb customer ID"""
+    r"""Orb customer ID"""  
     
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     customer: Optional[shared_customer.Customer] = dataclasses.field(default=None)
-    r"""Created"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Created"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_balance_transactions.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_balance_transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDBalanceTransactionsRequest:
     
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDBalanceTransactions200ApplicationJSON:
     r"""OK"""
     
-    data: Optional[list[shared_customer_balance_transaction.CustomerBalanceTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[shared_customer_balance_transaction.CustomerBalanceTransaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDBalanceTransactionsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_customers_customer_id_balance_transactions_200_application_json_object: Optional[GetCustomersCustomerIDBalanceTransactions200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_credits.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_credits.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,49 +11,49 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsRequest:
     
     customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
-    r"""The Orb Customer ID"""
+    r"""The Orb Customer ID"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDCredits200ApplicationJSONData:
     
     balance: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance') }})
-    r"""Remaining credits in this block"""
+    r"""Remaining credits in this block"""  
     expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""An ISO 8601 format date with a timezone offset that represents when this block of credits is no longer usable."""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""An ISO 8601 format date with a timezone offset that represents when this block of credits is no longer usable."""  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     per_unit_cost_basis: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_cost_basis') }})
-    r"""How much, in USD, a customer paid for a single credit in this block"""
+    r"""How much, in USD, a customer paid for a single credit in this block"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDCredits200ApplicationJSONPaginationMetadata:
     
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})
-    next_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor'), 'exclude': lambda f: f is None }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})  
+    next_cursor: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDCredits200ApplicationJSON:
     r"""OK"""
     
-    data: list[GetCustomersCustomerIDCredits200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: GetCustomersCustomerIDCredits200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[GetCustomersCustomerIDCredits200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: GetCustomersCustomerIDCredits200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_customers_customer_id_credits_200_application_json_object: Optional[GetCustomersCustomerIDCredits200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customers_customer_id_credits_ledger.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers_customer_id_credits_ledger.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,42 +21,42 @@
     EXPIRATION_CHANGE = 'expiration_change'
     CREDIT_BLOCK_EXPIRY = 'credit_block_expiry'
 
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsLedgerRequest:
     
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})  
     entry_status: Optional[GetCustomersCustomerIDCreditsLedgerEntryStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'entry_status', 'style': 'form', 'explode': True }})
-    r"""Filters to a single status of ledger entry"""
+    r"""Filters to a single status of ledger entry"""  
     entry_type: Optional[GetCustomersCustomerIDCreditsLedgerEntryTypeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'entry_type', 'style': 'form', 'explode': True }})
-    r"""Filter to a single type of ledger entry"""
+    r"""Filter to a single type of ledger entry"""  
     minimum_amount: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'minimum_amount', 'style': 'form', 'explode': True }})
-    r"""Filter to ledger entries that affect at least this amount"""
+    r"""Filter to ledger entries that affect at least this amount"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsLedger200ApplicationJSONPaginationMetadata:
     
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})
-    next_cursor: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})  
+    next_cursor: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsLedger200ApplicationJSON:
     r"""OK"""
     
-    data: list[shared_credit_ledger_entry.CreditLedgerEntry] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: GetCustomersCustomerIDCreditsLedger200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[shared_credit_ledger_entry.CreditLedgerEntry] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: GetCustomersCustomerIDCreditsLedger200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
 class GetCustomersCustomerIDCreditsLedgerResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_customers_customer_id_credits_ledger_200_application_json_object: Optional[GetCustomersCustomerIDCreditsLedger200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_customers_external_customer_id_external_customer_id.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers_external_customer_id_external_customer_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ..shared import customer as shared_customer
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetCustomersExternalCustomerIDExternalCustomerIDRequest:
     
-    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})
+    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetCustomersExternalCustomerIDExternalCustomerIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     customer: Optional[shared_customer.Customer] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_external_customer_costs.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customer_costs_by_external_customer_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,55 +8,55 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from orb import utils
 from typing import Any, Optional
 
-class GetExternalCustomerCostsViewModeEnum(str, Enum):
+class GetCustomerCostsByExternalCustomerIDViewModeEnum(str, Enum):
     r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""
     PERIODIC = 'periodic'
     CUMULATIVE = 'cumulative'
 
 
 @dataclasses.dataclass
-class GetExternalCustomerCostsRequest:
+class GetCustomerCostsByExternalCustomerIDRequest:
     
-    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})
+    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})  
     group_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'group_by', 'style': 'form', 'explode': True }})
-    r"""Groups per-price costs by the key provided."""
+    r"""Groups per-price costs by the key provided."""  
     timeframe_end: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""Costs returned are exclusive of `timeframe_end`."""
+    r"""Costs returned are exclusive of `timeframe_end`."""  
     timeframe_start: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""Costs returned are inclusive of `timeframe_start`."""
-    view_mode: Optional[GetExternalCustomerCostsViewModeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'view_mode', 'style': 'form', 'explode': True }})
-    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""
+    r"""Costs returned are inclusive of `timeframe_start`."""  
+    view_mode: Optional[GetCustomerCostsByExternalCustomerIDViewModeEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'view_mode', 'style': 'form', 'explode': True }})
+    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetExternalCustomerCosts200ApplicationJSONDataPerPriceCostsPriceGroups:
+class GetCustomerCostsByExternalCustomerID200ApplicationJSONDataPerPriceCostsPriceGroups:
     
     grouping_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_key') }})
-    r"""Grouping key to break down a single price's costs"""
-    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})
+    r"""Grouping key to break down a single price's costs"""  
+    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""
+    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""  
     secondary_grouping_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_key'), 'exclude': lambda f: f is None }})
-    r"""If the price is a matrix price, this is the second dimension key"""
-    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})
+    r"""If the price is a matrix price, this is the second dimension key"""  
+    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetExternalCustomerCosts200ApplicationJSONDataPerPriceCosts:
+class GetCustomerCostsByExternalCustomerID200ApplicationJSONDataPerPriceCosts:
     r"""Price's contributions for the timeframe, excluding any transforms (minimums and discounts)."""
     
-    price_groups: list[GetExternalCustomerCosts200ApplicationJSONDataPerPriceCostsPriceGroups] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_groups') }})
-    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""
+    price_groups: list[GetCustomerCostsByExternalCustomerID200ApplicationJSONDataPerPriceCostsPriceGroups] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_groups') }})
+    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""  
     price: Optional[shared_price.Price] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price'), 'exclude': lambda f: f is None }})
     r"""Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given Price object. The model_type field determines the key for the configuration object that is present.
     
     ## Unit pricing
     With unit pricing, each unit costs a fixed amount.
     ```json
     {
@@ -226,45 +226,45 @@
         \"unit_config\": {
            \"unit_amount\": \"2.00\"
         },
         \"fixed_price_quantity\": 3.0
         ...
     }
     ```
-    """
+    """  
     subtotal: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""
+    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""  
     total: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, including any minimums and discounts."""
+    r"""Price's contributions for the timeframe, including any minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetExternalCustomerCosts200ApplicationJSONData:
+class GetCustomerCostsByExternalCustomerID200ApplicationJSONData:
     
-    per_price_costs: list[GetExternalCustomerCosts200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})
+    per_price_costs: list[GetCustomerCostsByExternalCustomerID200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})  
     subtotal: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal') }})
-    r"""Total costs for the timeframe, excluding minimums and discounts."""
-    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""Total costs for the timeframe, excluding minimums and discounts."""  
+    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for the timeframe, including minimums and discounts."""
+    r"""Total costs for the timeframe, including minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetExternalCustomerCosts200ApplicationJSON:
+class GetCustomerCostsByExternalCustomerID200ApplicationJSON:
     r"""OK"""
     
-    data: list[GetExternalCustomerCosts200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[GetCustomerCostsByExternalCustomerID200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
-class GetExternalCustomerCostsResponse:
+class GetCustomerCostsByExternalCustomerIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_external_customer_costs_200_application_json_object: Optional[GetExternalCustomerCosts200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_customer_costs_by_external_customer_id_200_application_json_object: Optional[GetCustomerCostsByExternalCustomerID200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_invoice_invoice_id.py` & `orb-billing-1.2.0/src/orb/models/operations/post_invoices_invoice_id_void.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import dataclasses
 import requests as requests_http
 from ..shared import invoice as shared_invoice
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetInvoiceInvoiceIDRequest:
+class PostInvoicesInvoiceIDVoidRequest:
     
-    invoice_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'invoice_id', 'style': 'simple', 'explode': False }})
+    invoice_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'invoice_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetInvoiceInvoiceIDResponse:
+class PostInvoicesInvoiceIDVoidResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     invoice: Optional[shared_invoice.Invoice] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Created"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_invoices_upcoming.py` & `orb-billing-1.2.0/src/orb/models/operations/get_invoices_upcoming.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ..shared import upcominginvoice as shared_upcominginvoice
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetInvoicesUpcomingRequest:
     
-    subscription_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'subscription_id', 'style': 'form', 'explode': True }})
+    subscription_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'subscription_id', 'style': 'form', 'explode': True }})  
     
 
 @dataclasses.dataclass
 class GetInvoicesUpcomingResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     upcoming_invoice: Optional[shared_upcominginvoice.UpcomingInvoice] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_ping.py` & `orb-billing-1.2.0/src/orb/models/operations/get_ping.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetPing200ApplicationJSON:
     r"""OK"""
     
-    response: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('response') }})
+    response: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('response') }})  
     
 
 @dataclasses.dataclass
 class GetPingResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_ping_200_application_json_object: Optional[GetPing200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_plans_external_plan_id.py` & `orb-billing-1.2.0/src/orb/models/operations/get_plans_external_plan_id.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ..shared import plan as shared_plan
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetPlansExternalPlanIDRequest:
     
-    external_plan_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_plan_id', 'style': 'simple', 'explode': False }})
-    plan: Optional[shared_plan.Plan] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    external_plan_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_plan_id', 'style': 'simple', 'explode': False }})  
+    plan: Optional[shared_plan.Plan] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
 class GetPlansExternalPlanIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_plans_plan_id.py` & `orb-billing-1.2.0/src/orb/models/operations/get_plans_plan_id.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from ..shared import plan as shared_plan
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetPlansPlanIDRequest:
     
-    plan_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'plan_id', 'style': 'simple', 'explode': False }})
+    plan_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'plan_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
 class GetPlansPlanIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     plan: Optional[shared_plan.Plan] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id.py` & `orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_plan_changes.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import dataclasses
 import requests as requests_http
 from ..shared import subscription as shared_subscription
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDRequest:
+class PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest:
     
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDResponse:
+class PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     subscription: Optional[shared_subscription.Subscription] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_cost.py` & `orb-billing-1.2.0/src/orb/models/operations/get_subscription_id_usage_by_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 from datetime import datetime
 from marshmallow import fields
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCostRequest:
+class GetSubscriptionIDUsageByCustomerRequest:
     
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
     group_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'group_by', 'style': 'form', 'explode': True }})
-    r"""Groups per-price costs by the key provided."""
+    r"""Groups per-price costs by the key provided."""  
     timeframe_end: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""Revenue returned is _exclusive_ of `timeframe_end`"""
+    r"""Revenue returned is _exclusive_ of `timeframe_end`"""  
     timeframe_start: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""Revenue returned is _inclusive_ of `timeframe_start`"""
+    r"""Revenue returned is _inclusive_ of `timeframe_start`"""  
     view_mode: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'view_mode', 'style': 'form', 'explode': True }})
-    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""
+    r"""Controls whether Orb returns cumulative costs since the start of the billing period, or incremental day-by-day costs. If your customer has minimums or discounts, it's strongly recommended that you use the default cumulative behavior."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCost200ApplicationJSONDataPerPriceCostsPriceGroups:
+class GetSubscriptionIDUsageByCustomer200ApplicationJSONDataPerPriceCostsPriceGroups:
     
     grouping_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_key') }})
-    r"""Grouping key to break down a single price's costs"""
-    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})
+    r"""Grouping key to break down a single price's costs"""  
+    grouping_value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping_value') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""
+    r"""Total costs for this group for the timeframe. Note that this does not account for any minimums or discounts."""  
     secondary_grouping_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_key'), 'exclude': lambda f: f is None }})
-    r"""If the price is a matrix price, this is the second dimension key"""
-    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})
+    r"""If the price is a matrix price, this is the second dimension key"""  
+    secondary_grouping_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secondary_grouping_value'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCost200ApplicationJSONDataPerPriceCosts:
+class GetSubscriptionIDUsageByCustomer200ApplicationJSONDataPerPriceCosts:
     r"""Price's contributions for the timeframe, excluding any transforms (minimums and discounts)."""
     
-    price_groups: list[GetSubscriptionsSubscriptionIDCost200ApplicationJSONDataPerPriceCostsPriceGroups] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_groups') }})
-    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""
+    price_groups: list[GetSubscriptionIDUsageByCustomer200ApplicationJSONDataPerPriceCostsPriceGroups] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_groups') }})
+    r"""If a `group_by` attribute is passed in, array of costs per `grouping_key`, `grouping_value` or `secondary_grouping_key`, `secondary_grouping_value`."""  
     price: Optional[shared_price.Price] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price'), 'exclude': lambda f: f is None }})
     r"""Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given Price object. The model_type field determines the key for the configuration object that is present.
     
     ## Unit pricing
     With unit pricing, each unit costs a fixed amount.
     ```json
     {
@@ -220,45 +220,45 @@
         \"unit_config\": {
            \"unit_amount\": \"2.00\"
         },
         \"fixed_price_quantity\": 3.0
         ...
     }
     ```
-    """
+    """  
     subtotal: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""
+    r"""Price's contributions for the timeframe, excluding any minimums and discounts."""  
     total: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total'), 'exclude': lambda f: f is None }})
-    r"""Price's contributions for the timeframe, including minimums and discounts."""
+    r"""Price's contributions for the timeframe, including minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCost200ApplicationJSONData:
+class GetSubscriptionIDUsageByCustomer200ApplicationJSONData:
     
-    per_price_costs: list[GetSubscriptionsSubscriptionIDCost200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})
+    per_price_costs: list[GetSubscriptionIDUsageByCustomer200ApplicationJSONDataPerPriceCosts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_price_costs') }})  
     subtotal: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal') }})
-    r"""Total costs for the timeframe, excluding any minimums and discounts."""
-    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""Total costs for the timeframe, excluding any minimums and discounts."""  
+    timeframe_end: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_end'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    timeframe_start: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timeframe_start'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
     total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""Total costs for the timeframe, including any minimums and discounts."""
+    r"""Total costs for the timeframe, including any minimums and discounts."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCost200ApplicationJSON:
+class GetSubscriptionIDUsageByCustomer200ApplicationJSON:
     r"""OK"""
     
-    data: list[GetSubscriptionsSubscriptionIDCost200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[GetSubscriptionIDUsageByCustomer200ApplicationJSONData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDCostResponse:
+class GetSubscriptionIDUsageByCustomerResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_subscriptions_subscription_id_cost_200_application_json_object: Optional[GetSubscriptionsSubscriptionIDCost200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_subscription_id_usage_by_customer_200_application_json_object: Optional[GetSubscriptionIDUsageByCustomer200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_schedule.py` & `orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_subscription_id_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
 class GetSubscriptionsSubscriptionIDScheduleRequest:
     
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONDataPlan:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONData:
     
-    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    plan: Optional[GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONDataPlan] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan'), 'exclude': lambda f: f is None }})
-    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})  
+    plan: Optional[GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONDataPlan] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan'), 'exclude': lambda f: f is None }})  
+    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetSubscriptionsSubscriptionIDSchedule200ApplicationJSON:
     r"""OK"""
     
-    data: Optional[list[GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONData]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[GetSubscriptionsSubscriptionIDSchedule200ApplicationJSONData]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
 class GetSubscriptionsSubscriptionIDScheduleResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     get_subscriptions_subscription_id_schedule_200_application_json_object: Optional[GetSubscriptionsSubscriptionIDSchedule200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/get_subscriptions_subscription_id_usage.py` & `orb-billing-1.2.0/src/orb/models/operations/get_invoices.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from datetime import datetime
-from enum import Enum
-from typing import Optional
+from ..shared import invoice as shared_invoice
+from dataclasses_json import Undefined, dataclass_json
+from orb import utils
+from typing import Any, Optional
 
-class GetSubscriptionsSubscriptionIDUsageGranularityEnum(str, Enum):
-    r"""This determines the windowing of usage reporting."""
-    DAY = 'day'
 
+@dataclasses.dataclass
+class GetInvoicesRequest:
+    
+    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'customer_id', 'style': 'form', 'explode': True }})
+    r"""Filter by a specific customer (cannot be used with `external_customer_id`)"""  
+    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'external_customer_id', 'style': 'form', 'explode': True }})
+    r"""Filter by a specific customer (cannot be used with `customer_id`)"""  
+    subscription_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'subscription_id', 'style': 'form', 'explode': True }})
+    r"""Filter by a specific subscription"""  
+    
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDUsageRequest:
+class GetInvoices200ApplicationJSON:
+    r"""OK"""
     
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
-    billable_metric_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'billable_metric_id', 'style': 'form', 'explode': True }})
-    r"""When specified in conjunction with `group_by`, this parameter filters usage to a single billable metric. Note that both `group_by` and `billable_metric_id` must be specific together."""
-    granularity: Optional[GetSubscriptionsSubscriptionIDUsageGranularityEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'granularity', 'style': 'form', 'explode': True }})
-    r"""This determines the windowing of usage reporting."""
-    group_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'group_by', 'style': 'form', 'explode': True }})
-    r"""When specified in conjunction with `billable_metric_id`, this parameter groups by the key provided. Note that both `group_by` and `billable_metric_id` must be specific together."""
-    timeframe_end: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""Usage returned is _exclusive_ of `timeframe_end`"""
-    timeframe_start: Optional[datetime] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""Usage returned is _inclusive_ of `timeframe_start`"""
+    data: Optional[list[shared_invoice.Invoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
-class GetSubscriptionsSubscriptionIDUsageResponse:
+class GetInvoicesResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_invoices_200_application_json_object: Optional[GetInvoices200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/list_customers.py` & `orb-billing-1.2.0/src/orb/models/operations/get_customers.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListCustomers200ApplicationJSONPaginationMetadata:
+class GetCustomers200ApplicationJSONPaginationMetadata:
     
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})
-    next_cursor: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('has_more') }})  
+    next_cursor: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next_cursor') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListCustomers200ApplicationJSON:
+class GetCustomers200ApplicationJSON:
     r"""OK"""
     
-    data: list[shared_customer.Customer] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    pagination_metadata: ListCustomers200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})
+    data: list[shared_customer.Customer] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})  
+    pagination_metadata: GetCustomers200ApplicationJSONPaginationMetadata = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata') }})  
     
 
 @dataclasses.dataclass
-class ListCustomersResponse:
+class GetCustomersResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    list_customers_200_application_json_object: Optional[ListCustomers200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_customers_200_application_json_object: Optional[GetCustomers200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/list_invoices.py` & `orb-billing-1.2.0/src/orb/models/operations/get_subscriptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import invoice as shared_invoice
+from ..shared import subscription as shared_subscription
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
-class ListInvoicesRequest:
+class GetSubscriptionsRequest:
     
-    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'customer_id', 'style': 'form', 'explode': True }})
-    r"""Filter by a specific customer (cannot be used with `external_customer_id`)"""
-    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'external_customer_id', 'style': 'form', 'explode': True }})
-    r"""Filter by a specific customer (cannot be used with `customer_id`)"""
-    subscription_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'subscription_id', 'style': 'form', 'explode': True }})
-    r"""Filter by a specific subscription"""
+    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'customer_id', 'style': 'form', 'explode': True }})  
+    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'external_customer_id', 'style': 'form', 'explode': True }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListInvoices200ApplicationJSON:
+class GetSubscriptions200ApplicationJSON:
     r"""OK"""
     
-    data: Optional[list[shared_invoice.Invoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[shared_subscription.Subscription]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
-class ListInvoicesResponse:
+class GetSubscriptionsResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    list_invoices_200_application_json_object: Optional[ListInvoices200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_subscriptions_200_application_json_object: Optional[GetSubscriptions200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/list_plans.py` & `orb-billing-1.2.0/src/orb/models/operations/get_plans.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListPlansRequestBody:
+class GetPlans200ApplicationJSON:
+    r"""OK"""
     
-    data: Optional[list[shared_plan.Plan]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[shared_plan.Plan]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
-class ListPlansResponse:
+class GetPlansResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_plans_200_application_json_object: Optional[GetPlans200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/list_subscriptions.py` & `orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_by_coupon.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,30 @@
 from ..shared import subscription as shared_subscription
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclasses.dataclass
-class ListSubscriptionsRequest:
+class GetSubscriptionsByCouponRequest:
     
-    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'customer_id', 'style': 'form', 'explode': True }})
-    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'external_customer_id', 'style': 'form', 'explode': True }})
+    coupon_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'coupon_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListSubscriptions200ApplicationJSON:
+class GetSubscriptionsByCoupon200ApplicationJSON:
     r"""OK"""
     
-    data: Optional[list[shared_subscription.Subscription]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[shared_subscription.Subscription]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
-class ListSubscriptionsResponse:
+class GetSubscriptionsByCouponResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    list_subscriptions_200_application_json_object: Optional[ListSubscriptions200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    get_subscriptions_by_coupon_200_application_json_object: Optional[GetSubscriptionsByCoupon200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/patch_customers_customer_id_usage.py` & `orb-billing-1.2.0/src/orb/models/operations/patch_customers_customer_id_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,77 +10,77 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsageRequestBodyEvents:
     
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
-    r"""A name to meaningfully identify the action or event type."""
+    r"""A name to meaningfully identify the action or event type."""  
     properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
-    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""
+    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""  
     timestamp: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
-    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""
+    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsageRequestBody:
     
-    events: list[PatchCustomersCustomerIDUsageRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})
+    events: list[PatchCustomersCustomerIDUsageRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})  
     
 
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsageRequest:
     
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})  
     timeframe_end: datetime = dataclasses.field(metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""This bound is exclusive (i.e. events before this timestamp will be updated)"""
+    r"""This bound is exclusive (i.e. events before this timestamp will be updated)"""  
     timeframe_start: datetime = dataclasses.field(metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""This bound is inclusive (i.e. events with this timestamp onward, inclusive will be updated)"""
-    request_body: Optional[PatchCustomersCustomerIDUsageRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""This bound is inclusive (i.e. events with this timestamp onward, inclusive will be updated)"""  
+    request_body: Optional[PatchCustomersCustomerIDUsageRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsage400ApplicationJSONValidationErrors:
     
-    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})
+    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})  
     validation_errors: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
-    r"""An array of strings corresponding to each validation failure"""
+    r"""An array of strings corresponding to each validation failure"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsage400ApplicationJSON:
     r"""Bad Request"""
     
     status: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""HTTP Code"""
+    r"""HTTP Code"""  
     title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
-    r"""Error message"""
-    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""Error message"""  
+    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
     validation_errors: list[PatchCustomersCustomerIDUsage400ApplicationJSONValidationErrors] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors') }})
-    r"""Contains all failing validation events."""
+    r"""Contains all failing validation events."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsage200ApplicationJSON:
     r"""OK"""
     
     duplicate: Optional[list[dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})
-    r"""An array of strings, corresponding to idempotency_key's marked as duplicates (previously ingested)"""
+    r"""An array of strings, corresponding to idempotency_key's marked as duplicates (previously ingested)"""  
     ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})
-    r"""An array of strings, corresponding to idempotency_key's which were successfully ingested."""
+    r"""An array of strings, corresponding to idempotency_key's which were successfully ingested."""  
     
 
 @dataclasses.dataclass
 class PatchCustomersCustomerIDUsageResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     patch_customers_customer_id_usage_200_application_json_object: Optional[PatchCustomersCustomerIDUsage200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""  
     patch_customers_customer_id_usage_400_application_json_object: Optional[PatchCustomersCustomerIDUsage400ApplicationJSON] = dataclasses.field(default=None)
-    r"""Bad Request"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/patch_external_customers_customer_id_usage.py` & `orb-billing-1.2.0/src/orb/models/operations/patch_customers_external_customer_id_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,80 +7,80 @@
 from datetime import datetime
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsageRequestBodyEvents:
+class PatchCustomersExternalCustomerIDUsageRequestBodyEvents:
     
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
-    r"""A name to meaningfully identify the action or event type."""
+    r"""A name to meaningfully identify the action or event type."""  
     properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
-    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""
+    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""  
     timestamp: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
-    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""
+    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsageRequestBody:
+class PatchCustomersExternalCustomerIDUsageRequestBody:
     
-    events: list[PatchExternalCustomersCustomerIDUsageRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})
+    events: list[PatchCustomersExternalCustomerIDUsageRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})  
     
 
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsageRequest:
+class PatchCustomersExternalCustomerIDUsageRequest:
     
-    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})
+    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})  
     timeframe_end: datetime = dataclasses.field(metadata={'query_param': { 'field_name': 'timeframe_end', 'style': 'form', 'explode': True }})
-    r"""This bound is exclusive (i.e. events before this timestamp will be updated)"""
+    r"""This bound is exclusive (i.e. events before this timestamp will be updated)"""  
     timeframe_start: datetime = dataclasses.field(metadata={'query_param': { 'field_name': 'timeframe_start', 'style': 'form', 'explode': True }})
-    r"""This bound is inclusive (i.e. events with this timestamp onward, inclusive will be updated)"""
-    request_body: Optional[PatchExternalCustomersCustomerIDUsageRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""This bound is inclusive (i.e. events with this timestamp onward, inclusive will be updated)"""  
+    request_body: Optional[PatchCustomersExternalCustomerIDUsageRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsage400ApplicationJSONValidationErrors:
+class PatchCustomersExternalCustomerIDUsage400ApplicationJSONValidationErrors:
     
-    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})
+    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})  
     validation_errors: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
-    r"""An array of strings corresponding to each validation failure"""
+    r"""An array of strings corresponding to each validation failure"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsage400ApplicationJSON:
+class PatchCustomersExternalCustomerIDUsage400ApplicationJSON:
     r"""Bad Request"""
     
     status: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-    r"""HTTP Code"""
+    r"""HTTP Code"""  
     title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})
-    r"""Error message"""
-    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    validation_errors: list[PatchExternalCustomersCustomerIDUsage400ApplicationJSONValidationErrors] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors') }})
-    r"""Contains all failing validation events."""
+    r"""Error message"""  
+    type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    validation_errors: list[PatchCustomersExternalCustomerIDUsage400ApplicationJSONValidationErrors] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors') }})
+    r"""Contains all failing validation events."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsage200ApplicationJSON:
+class PatchCustomersExternalCustomerIDUsage200ApplicationJSON:
     r"""OK"""
     
     duplicate: Optional[list[dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})
-    r"""An array of strings, corresponding to idempotency_key's marked as duplicates (previously ingested)"""
+    r"""An array of strings, corresponding to idempotency_key's marked as duplicates (previously ingested)"""  
     ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})
-    r"""An array of strings, corresponding to idempotency_key's which were successfully ingested."""
+    r"""An array of strings, corresponding to idempotency_key's which were successfully ingested."""  
     
 
 @dataclasses.dataclass
-class PatchExternalCustomersCustomerIDUsageResponse:
+class PatchCustomersExternalCustomerIDUsageResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    patch_external_customers_customer_id_usage_200_application_json_object: Optional[PatchExternalCustomersCustomerIDUsage200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    patch_external_customers_customer_id_usage_400_application_json_object: Optional[PatchExternalCustomersCustomerIDUsage400ApplicationJSON] = dataclasses.field(default=None)
-    r"""Bad Request"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    patch_customers_external_customer_id_usage_200_application_json_object: Optional[PatchCustomersExternalCustomerIDUsage200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    patch_customers_external_customer_id_usage_400_application_json_object: Optional[PatchCustomersExternalCustomerIDUsage400ApplicationJSON] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_customers.py` & `orb-billing-1.2.0/src/orb/models/operations/delete_customers_customer_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import customer as shared_customer
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PostCustomersResponse:
+class DeleteCustomersCustomerIDRequest:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    customer: Optional[shared_customer.Customer] = dataclasses.field(default=None)
-    r"""Created"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
+    r"""Orb customer ID"""  
+    
+
+@dataclasses.dataclass
+class DeleteCustomersCustomerIDResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_customers_customer_id_credits_ledger_entry.py` & `orb-billing-1.2.0/src/orb/models/operations/amend_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,71 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 import requests as requests_http
-from ..shared import credit_ledger_entry as shared_credit_ledger_entry
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
-from enum import Enum
+from datetime import datetime
 from marshmallow import fields
 from orb import utils
-from typing import Optional
-
-class PostCustomersCustomerIDCreditsLedgerEntryRequestBodyEntryTypeEnum(str, Enum):
-    INCREMENT = 'increment'
-    DECREMENT = 'decrement'
-    EXPIRATION_CHANGE = 'expiration_change'
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCustomersCustomerIDCreditsLedgerEntryRequestBody:
+class AmendEventRequestBody:
     
-    amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    entry_type: PostCustomersCustomerIDCreditsLedgerEntryRequestBodyEntryTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('entry_type') }})
-    block_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_id'), 'exclude': lambda f: f is None }})
-    r"""The ID of the block affected by an `expiration_change`"""
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    r"""Optional metadata that can be specified when adding ledger results via the API. For example, this can be used to note an increment refers to trial credits, or for noting corrections as a result of an incident, etc."""
-    expiry_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiry_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""A future date (specified in YYYY-MM-DD format) that denotes when this credit balance should expire."""
-    per_unit_cost_basis: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_cost_basis'), 'exclude': lambda f: f is None }})
-    r"""Can only be specified when `entry_type=increment`. How much, in USD, a customer paid for a single credit in this block"""
-    target_expiry_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target_expiry_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""A future date (specified in YYYY-MM-DD) used for `expiration_change`"""
+    event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
+    r"""A name to meaningfully identify the action or event type."""  
+    properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
+    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""  
+    timestamp: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""  
+    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id'), 'exclude': lambda f: f is None }})
+    r"""The Orb Customer identifier"""  
+    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
+    r"""An alias for the Orb customer, whose mapping is specified when creating the customer"""  
     
 
 @dataclasses.dataclass
-class PostCustomersCustomerIDCreditsLedgerEntryRequest:
+class AmendEventRequest:
     
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
-    request_body: Optional[PostCustomersCustomerIDCreditsLedgerEntryRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    event_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'event_id', 'style': 'simple', 'explode': False }})
+    r"""Identical to the `idempotency_key` provided on event ingestion. Uniquely identifies an event in the system."""  
+    request_body: Optional[AmendEventRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostCustomersCustomerIDCreditsLedgerEntryResponse:
+class AmendEvent400ApplicationJSON:
+    r"""Bad Request"""
+    
+    status: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    r"""HTTP Code"""  
+    title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
+    r"""Error message"""  
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})  
+    validation_errors: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
+    r"""An array of strings corresponding to the validation failures"""  
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    credit_ledger_entry: Optional[shared_credit_ledger_entry.CreditLedgerEntry] = dataclasses.field(default=None)
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class AmendEvent200ApplicationJSON:
     r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    
+    amended: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amended'), 'exclude': lambda f: f is None }})
+    r"""event_id of the amended event, if successfully ingested"""  
+    
+
+@dataclasses.dataclass
+class AmendEventResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    amend_event_200_application_json_object: Optional[AmendEvent200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    amend_event_400_application_json_object: Optional[AmendEvent400ApplicationJSON] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_events_search.py` & `orb-billing-1.2.0/src/orb/models/operations/post_events_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostEventsSearchRequestBody:
     
     event_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_ids'), 'exclude': lambda f: f is None }})
-    r"""This is an explicit array of IDs to filter by. Note that an event's ID is the idempotency_key that was originally used for ingestion. Values in this array will be treated case sensitively."""
+    r"""This is an explicit array of IDs to filter by. Note that an event's ID is the idempotency_key that was originally used for ingestion. Values in this array will be treated case sensitively."""  
     invoice_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_id'), 'exclude': lambda f: f is None }})
-    r"""This is an issued Orb invoice ID (see also List Invoices). Orb will fetch all events that were used to calculate the invoice. In the common case, this will be a list of events whose timestamp property falls within the billing period specified by the invoice."""
+    r"""This is an issued Orb invoice ID (see also List Invoices). Orb will fetch all events that were used to calculate the invoice. In the common case, this will be a list of events whose timestamp property falls within the billing period specified by the invoice."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostEventsSearch200ApplicationJSON:
     r"""An array of events matching the specified search_criteria. If no events match, this array will be empty."""
     
-    data: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})
+    data: Optional[list[shared_event.Event]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    pagination_metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination_metadata'), 'exclude': lambda f: f is None }})  
     
 
 @dataclasses.dataclass
 class PostEventsSearchResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     post_events_search_200_application_json_object: Optional[PostEventsSearch200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_ingest.py` & `orb-billing-1.2.0/src/orb/models/operations/post_ingest.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,110 +10,110 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngestRequestBodyEvents:
     
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
-    r"""A name to meaningfully identify the action or event type."""
+    r"""A name to meaningfully identify the action or event type."""  
     idempotency_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key') }})
-    r"""A unique value, generated by the client, that is used to de-duplicate events. Exactly one event with a given idempotency key will be ingested, which allows for safe request retries."""
+    r"""A unique value, generated by the client, that is used to de-duplicate events. Exactly one event with a given idempotency key will be ingested, which allows for safe request retries."""  
     properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
-    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""
+    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""  
     timestamp: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
-    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""
+    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""  
     customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id'), 'exclude': lambda f: f is None }})
-    r"""The Orb Customer identifier"""
+    r"""The Orb Customer identifier"""  
     external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
-    r"""An alias for the Orb customer, whose mapping is specified when creating the customer"""
+    r"""An alias for the Orb customer, whose mapping is specified when creating the customer"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngestRequestBody:
     
-    events: list[PostIngestRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})
+    events: list[PostIngestRequestBodyEvents] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('events') }})  
     
 class PostIngestDebugEnum(str, Enum):
     r"""Flag to enable additional debug information in the endpoint response"""
     TRUE = 'true'
     FALSE = 'false'
 
 
 @dataclasses.dataclass
 class PostIngestRequest:
     
     debug: Optional[PostIngestDebugEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'debug', 'style': 'form', 'explode': True }})
-    r"""Flag to enable additional debug information in the endpoint response"""
-    request_body: Optional[PostIngestRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Flag to enable additional debug information in the endpoint response"""  
+    request_body: Optional[PostIngestRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest400ApplicationJSONDebug:
     r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""
     
-    duplicate: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})
-    ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})
+    duplicate: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})  
+    ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest400ApplicationJSONValidationFailed:
     
-    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})
+    idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})  
     validation_errors: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
-    r"""An array of objects corresponding to validation failures for each idempotency_key."""
+    r"""An array of objects corresponding to validation failures for each idempotency_key."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest400ApplicationJSON:
     r"""Bad Request"""
     
     validation_failed: list[PostIngest400ApplicationJSONValidationFailed] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_failed') }})
-    r"""Contains all failing validation events. In the case of a 400, there will be at least one entry in this array."""
+    r"""Contains all failing validation events. In the case of a 400, there will be at least one entry in this array."""  
     debug: Optional[PostIngest400ApplicationJSONDebug] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('debug'), 'exclude': lambda f: f is None }})
-    r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""
+    r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest200ApplicationJSONDebug:
     r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""
     
-    duplicate: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})
-    ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})
+    duplicate: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duplicate'), 'exclude': lambda f: f is None }})  
+    ingested: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ingested'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest200ApplicationJSONValidationFailed:
     
     idempotency_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('idempotency_key'), 'exclude': lambda f: f is None }})
-    r"""The passed idempotency_key corresponding to the validation_errors"""
+    r"""The passed idempotency_key corresponding to the validation_errors"""  
     validation_errors: Optional[list[dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
-    r"""An array of objects corresponding to validation failures for each idempotency_key."""
+    r"""An array of objects corresponding to validation failures for each idempotency_key."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostIngest200ApplicationJSON:
     r"""OK"""
     
     validation_failed: list[PostIngest200ApplicationJSONValidationFailed] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_failed') }})
-    r"""Contains all failing validation events. In the case of a 200, this array will always be empty. This field will always be present."""
+    r"""Contains all failing validation events. In the case of a 200, this array will always be empty. This field will always be present."""  
     debug: Optional[PostIngest200ApplicationJSONDebug] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('debug'), 'exclude': lambda f: f is None }})
-    r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""
+    r"""Optional debug information (only present when debug=true is passed to the endpoint). Contains ingested and duplicate event idempotency keys."""  
     
 
 @dataclasses.dataclass
 class PostIngestResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     post_ingest_200_application_json_object: Optional[PostIngest200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""  
     post_ingest_400_application_json_object: Optional[PostIngest400ApplicationJSON] = dataclasses.field(default=None)
-    r"""Bad Request"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_subscriptions.py` & `orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_schedule_plan_change.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,269 +1,252 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 import requests as requests_http
 from ..shared import subscription as shared_subscription
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
+from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from orb import utils
 from typing import Any, Optional
 
-class PostSubscriptionsRequestBodyExternalMarketplaceEnum(str, Enum):
-    r"""Optionally provide the name of the external marketplace that the subscription is attached to."""
-    GOOGLE = 'google'
-    AWS = 'aws'
-    AZURE = 'azure'
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyChangeOptionEnum(str, Enum):
+    r"""Determines the timing of the plan change"""
+    REQUESTED_DATE = 'requested_date'
+    END_OF_SUBSCRIPTION_TERM = 'end_of_subscription_term'
+    IMMEDIATE = 'immediate'
 
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PostSubscriptionsRequestBodyPhaseOverrides:
-    
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
-    minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The new minimum amount for the phase. Providing `null` will clear the existing minimum, if it exists."""
-    order: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order'), 'exclude': lambda f: f is None }})
-    r"""The phase order that is being modified."""
-    
-class PostSubscriptionsRequestBodyPriceOverrides7ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7ModelTypeEnum(str, Enum):
     TIERED_BPS = 'tiered_bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides7TieredBpsConfigTiers:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfigTiers:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})
-    minimum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})  
+    minimum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides7TieredBpsConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfig:
     
-    tiers: list[PostSubscriptionsRequestBodyPriceOverrides7TieredBpsConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})
+    tiers: list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides7:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7:
     r"""Tiered BPS price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides7ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    tiered_bps_config: PostSubscriptionsRequestBodyPriceOverrides7TieredBpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_bps_config') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    tiered_bps_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_bps_config') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides6BulkBpsConfigTiers:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfigTiers:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides6BulkBpsConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfig:
     
-    tiers: Optional[list[PostSubscriptionsRequestBodyPriceOverrides6BulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
-class PostSubscriptionsRequestBodyPriceOverrides6ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6ModelTypeEnum(str, Enum):
     BULK_BPS = 'bulk_bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides6:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6:
     r"""Bulk BPS price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides6ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    bulk_bps_config: Optional[PostSubscriptionsRequestBodyPriceOverrides6BulkBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_bps_config'), 'exclude': lambda f: f is None }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    bulk_bps_config: Optional[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_bps_config'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides5BpsConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5BpsConfig:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
-class PostSubscriptionsRequestBodyPriceOverrides5ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5ModelTypeEnum(str, Enum):
     BPS = 'bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides5:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5:
     r"""BPS price override"""
     
-    bps_config: PostSubscriptionsRequestBodyPriceOverrides5BpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps_config') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides5ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    bps_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5BpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps_config') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsRequestBodyPriceOverrides4ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4ModelTypeEnum(str, Enum):
     PACKAGE = 'package'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides4PackageConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4PackageConfig:
     
-    package_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_amount') }})
-    package_size: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_size') }})
+    num_units: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_units') }})  
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides4:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4:
     r"""Package price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides4ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    package_config: PostSubscriptionsRequestBodyPriceOverrides4PackageConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_config') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    package_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4PackageConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_config') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides3BulkConfigTiers:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfigTiers:
     
-    maximum_units: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units') }})
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    maximum_units: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units') }})  
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides3BulkConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfig:
     
-    tiers: list[PostSubscriptionsRequestBodyPriceOverrides3BulkConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})
+    tiers: list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})  
     
-class PostSubscriptionsRequestBodyPriceOverrides3ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3ModelTypeEnum(str, Enum):
     BULK = 'bulk'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides3:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3:
     r"""Bulk price override"""
     
-    bulk_config: PostSubscriptionsRequestBodyPriceOverrides3BulkConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_config') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides3ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    bulk_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_config') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsRequestBodyPriceOverrides2ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2ModelTypeEnum(str, Enum):
     UNIT = 'unit'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides2UnitConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2UnitConfig:
     
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides2:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2:
     r"""Unit price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsRequestBodyPriceOverrides2ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    unit_config: PostSubscriptionsRequestBodyPriceOverrides2UnitConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_config') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
-    fixed_price_quantity: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixed_price_quantity'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    unit_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2UnitConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_config') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsRequestBodyPriceOverrides1ModelTypeEnum(str, Enum):
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1ModelTypeEnum(str, Enum):
     TIERED = 'tiered'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides1TieredConfigTiers:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfigTiers:
     
-    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})
-    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})  
+    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})  
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides1TieredConfig:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfig:
     
-    tiers: Optional[list[PostSubscriptionsRequestBodyPriceOverrides1TieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBodyPriceOverrides1:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1:
     r"""Tiered price override"""
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""price_id"""
-    model_type: PostSubscriptionsRequestBodyPriceOverrides1ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    tiered_config: PostSubscriptionsRequestBodyPriceOverrides1TieredConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_config') }})
-    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})
+    r"""price_id"""  
+    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    tiered_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_config') }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsRequestBody:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBody:
     
-    align_billing_with_subscription_start_date: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('align_billing_with_subscription_start_date'), 'exclude': lambda f: f is None }})
-    r"""Align billing periods with the subscription's start_date. If this is not provided, this defaults to aligning billing periods with the start of the month."""
-    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id'), 'exclude': lambda f: f is None }})
-    r"""The ID of the customer to subscribe."""
-    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
-    r"""The external ID of the customer to subscribe, as an alternate to passing the `customer_id`."""
-    external_marketplace: Optional[PostSubscriptionsRequestBodyExternalMarketplaceEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_marketplace'), 'exclude': lambda f: f is None }})
-    r"""Optionally provide the name of the external marketplace that the subscription is attached to."""
-    external_marketplace_reporting_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_marketplace_reporting_id'), 'exclude': lambda f: f is None }})
-    r"""The reporting ID to associate this subscription with the external marketplace. Required if external_marketplace is specified."""
+    change_option: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyChangeOptionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('change_option') }})
+    r"""Determines the timing of the plan change"""  
+    align_billing_with_plan_change_date: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('align_billing_with_plan_change_date'), 'exclude': lambda f: f is None }})
+    r"""Reset billing periods to be aligned with the plan change’s effective date."""  
+    change_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('change_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The date that the plan change should take effect. This parameter can only be passed if the `change_option` is `requested_date`."""  
+    coupon_redemption_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('coupon_redemption_code'), 'exclude': lambda f: f is None }})
+    r"""Redemption code to be used for this subscription. If the coupon cannot be found by its redemption code, or cannot be redeemed, an error response will be returned and the plan change will not be scheduled."""  
     external_plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_plan_id'), 'exclude': lambda f: f is None }})
-    r"""The external ID of the plan, which can be used in place of the `plan_id`."""
+    r"""The external_plan_id of the plan that the given subscription should be switched to. Note that either this property or `plan_id` must be specified."""  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for the plan."""
-    phase_overrides: Optional[list[PostSubscriptionsRequestBodyPhaseOverrides]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phase_overrides'), 'exclude': lambda f: f is None }})
-    r"""Optionally provide a list of minimum amount or discount overrides for phases on the plan."""
+    r"""The subscription's override minimum amount for the plan."""  
     plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_id'), 'exclude': lambda f: f is None }})
-    r"""The plan that the given customer should be subscribed to. The plan determines the pricing and cadence of the subscription."""
+    r"""The plan that the given subscription should be switched to. Note that either this property or `external_plan_id` must be specified."""  
     price_overrides: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_overrides'), 'exclude': lambda f: f is None }})
-    r"""Optionally provide a list of overrides for prices on the plan"""
-    start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date that Orb should start billing for the subscription, localized to the customer's timezone. If this is not provided, this defaults to the current date in the customer's timezone."""
+    r"""Optionally provide a list of overrides for prices on the plan"""  
+    
+
+@dataclasses.dataclass
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequest:
+    
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
-class PostSubscriptionsResponse:
+class PostSubscriptionsSubscriptionIDSchedulePlanChangeResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     subscription: Optional[shared_subscription.Subscription] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_cancel.py` & `orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_cancellation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import subscription as shared_subscription
-from enum import Enum
 from typing import Optional
 
-class PostSubscriptionsSubscriptionIDCancelCancelOptionEnum(str, Enum):
-    r"""Determines the timing of subscription cancellation"""
-    END_OF_SUBSCRIPTION_TERM = 'end_of_subscription_term'
-    IMMEDIATE = 'immediate'
-
 
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDCancelRequest:
+class PostSubscriptionsSubscriptionIDUnschedulePendingCancellationRequest:
     
-    cancel_option: PostSubscriptionsSubscriptionIDCancelCancelOptionEnum = dataclasses.field(metadata={'query_param': { 'field_name': 'cancel_option', 'style': 'form', 'explode': True }})
-    r"""Determines the timing of subscription cancellation"""
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDCancelResponse:
+class PostSubscriptionsSubscriptionIDUnschedulePendingCancellationResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     subscription: Optional[shared_subscription.Subscription] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_schedule_plan_change.py` & `orb-billing-1.2.0/src/orb/models/operations/post_subscriptions_json.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,243 +7,273 @@
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
 from orb import utils
 from typing import Any, Optional
 
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyChangeOptionEnum(str, Enum):
-    r"""Determines the timing of the plan change"""
-    REQUESTED_DATE = 'requested_date'
-    END_OF_SUBSCRIPTION_TERM = 'end_of_subscription_term'
-    IMMEDIATE = 'immediate'
+class PostSubscriptionsApplicationJSONExternalMarketplaceEnum(str, Enum):
+    r"""Optionally provide the name of the external marketplace that the subscription is attached to."""
+    GOOGLE = 'google'
+    AWS = 'aws'
+    AZURE = 'azure'
 
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7ModelTypeEnum(str, Enum):
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class PostSubscriptionsApplicationJSONPhaseOverrides:
+    
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
+    minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
+    r"""The new minimum amount for the phase. Providing `null` will clear the existing minimum, if it exists."""  
+    order: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order'), 'exclude': lambda f: f is None }})
+    r"""The phase order that is being modified."""  
+    
+class PostSubscriptionsApplicationJSONPriceOverrides7ModelTypeEnum(str, Enum):
     TIERED_BPS = 'tiered_bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfigTiers:
+class PostSubscriptionsApplicationJSONPriceOverrides7TieredBpsConfigTiers:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})
-    minimum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})  
+    minimum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides7TieredBpsConfig:
     
-    tiers: list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})
+    tiers: list[PostSubscriptionsApplicationJSONPriceOverrides7TieredBpsConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7:
+class PostSubscriptionsApplicationJSONPriceOverrides7:
     r"""Tiered BPS price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    tiered_bps_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides7TieredBpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_bps_config') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides7ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    tiered_bps_config: PostSubscriptionsApplicationJSONPriceOverrides7TieredBpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_bps_config') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfigTiers:
+class PostSubscriptionsApplicationJSONPriceOverrides6BulkBpsConfigTiers:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    maximum_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides6BulkBpsConfig:
     
-    tiers: Optional[list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PostSubscriptionsApplicationJSONPriceOverrides6BulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides6ModelTypeEnum(str, Enum):
     BULK_BPS = 'bulk_bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6:
+class PostSubscriptionsApplicationJSONPriceOverrides6:
     r"""Bulk BPS price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    bulk_bps_config: Optional[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides6BulkBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_bps_config'), 'exclude': lambda f: f is None }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides6ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    bulk_bps_config: Optional[PostSubscriptionsApplicationJSONPriceOverrides6BulkBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_bps_config'), 'exclude': lambda f: f is None }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5BpsConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides5BpsConfig:
     
-    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})
-    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})
+    bps: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps') }})  
+    per_unit_maximum: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum') }})  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides5ModelTypeEnum(str, Enum):
     BPS = 'bps'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5:
+class PostSubscriptionsApplicationJSONPriceOverrides5:
     r"""BPS price override"""
     
-    bps_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5BpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps_config') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides5ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
+    bps_config: PostSubscriptionsApplicationJSONPriceOverrides5BpsConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps_config') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides5ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides4ModelTypeEnum(str, Enum):
     PACKAGE = 'package'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4PackageConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides4PackageConfig:
     
-    num_units: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_units') }})
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    package_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_amount') }})  
+    package_size: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_size') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4:
+class PostSubscriptionsApplicationJSONPriceOverrides4:
     r"""Package price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    package_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides4PackageConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_config') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides4ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    package_config: PostSubscriptionsApplicationJSONPriceOverrides4PackageConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_config') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfigTiers:
+class PostSubscriptionsApplicationJSONPriceOverrides3BulkConfigTiers:
     
-    maximum_units: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units') }})
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    maximum_units: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units') }})  
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides3BulkConfig:
     
-    tiers: list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})
+    tiers: list[PostSubscriptionsApplicationJSONPriceOverrides3BulkConfigTiers] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers') }})  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides3ModelTypeEnum(str, Enum):
     BULK = 'bulk'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3:
+class PostSubscriptionsApplicationJSONPriceOverrides3:
     r"""Bulk price override"""
     
-    bulk_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3BulkConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_config') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides3ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
+    bulk_config: PostSubscriptionsApplicationJSONPriceOverrides3BulkConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_config') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides3ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides2ModelTypeEnum(str, Enum):
     UNIT = 'unit'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2UnitConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides2UnitConfig:
     
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2:
+class PostSubscriptionsApplicationJSONPriceOverrides2:
     r"""Unit price override"""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    unit_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides2UnitConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_config') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides2ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    unit_config: PostSubscriptionsApplicationJSONPriceOverrides2UnitConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_config') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
+    fixed_price_quantity: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixed_price_quantity'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1ModelTypeEnum(str, Enum):
+class PostSubscriptionsApplicationJSONPriceOverrides1ModelTypeEnum(str, Enum):
     TIERED = 'tiered'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfigTiers:
+class PostSubscriptionsApplicationJSONPriceOverrides1TieredConfigTiers:
     
-    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})
-    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})  
+    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})  
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfig:
+class PostSubscriptionsApplicationJSONPriceOverrides1TieredConfig:
     
-    tiers: Optional[list[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PostSubscriptionsApplicationJSONPriceOverrides1TieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1:
+class PostSubscriptionsApplicationJSONPriceOverrides1:
     r"""Tiered price override"""
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""price_id"""
-    model_type: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})
-    tiered_config: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyPriceOverrides1TieredConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_config') }})
+    r"""price_id"""  
+    model_type: PostSubscriptionsApplicationJSONPriceOverrides1ModelTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type') }})  
+    tiered_config: PostSubscriptionsApplicationJSONPriceOverrides1TieredConfig = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_config') }})  
+    discount: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount'), 'exclude': lambda f: f is None }})  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for this price."""
+    r"""The subscription's override minimum amount for this price."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBody:
+class PostSubscriptionsApplicationJSON:
     
-    change_option: PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBodyChangeOptionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('change_option') }})
-    r"""Determines the timing of the plan change"""
-    align_billing_with_plan_change_date: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('align_billing_with_plan_change_date'), 'exclude': lambda f: f is None }})
-    r"""Reset billing periods to be aligned with the plan change’s effective date."""
-    change_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('change_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date that the plan change should take effect, localized to the customer's timezone. This parameter can only be passed if the `change_option` is `requested_date`."""
+    align_billing_with_subscription_start_date: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('align_billing_with_subscription_start_date'), 'exclude': lambda f: f is None }})
+    r"""Align billing periods with the subscription's start_date. If this is not provided, this defaults to aligning billing periods with the start of the month."""  
+    auto_collection: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auto_collection'), 'exclude': lambda f: f is None }})
+    r"""Used to determine whether Orb will attempt to automatically charge the payment method on file for the customer corresponding to this subscription. If not provided, the property on the corresponding customer will be honored."""  
+    coupon_redemption_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('coupon_redemption_code'), 'exclude': lambda f: f is None }})
+    r"""Redemption code to be used for this subscription. If the coupon cannot be found by its redemption code, or cannot be redeemed, an error response will be returned and the plan change will not be scheduled."""  
+    customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id'), 'exclude': lambda f: f is None }})
+    r"""The ID of the customer to subscribe."""  
+    default_invoice_memo: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default_invoice_memo'), 'exclude': lambda f: f is None }})
+    r"""Invoices for this subscription will populate with this memo. When not set, the plan-level setting for memo will be used."""  
+    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
+    r"""The external ID of the customer to subscribe, as an alternate to passing the `customer_id`."""  
+    external_marketplace: Optional[PostSubscriptionsApplicationJSONExternalMarketplaceEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_marketplace'), 'exclude': lambda f: f is None }})
+    r"""Optionally provide the name of the external marketplace that the subscription is attached to."""  
+    external_marketplace_reporting_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_marketplace_reporting_id'), 'exclude': lambda f: f is None }})
+    r"""The reporting ID to associate this subscription with the external marketplace. Required if external_marketplace is specified."""  
     external_plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_plan_id'), 'exclude': lambda f: f is None }})
-    r"""The external_plan_id of the plan that the given subscription should be switched to. Note that either this property or `plan_id` must be specified."""
+    r"""The external ID of the plan, which can be used in place of the `plan_id`."""  
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    r"""User-specified key value pairs, often useful for referencing internal resources or IDs. Returned as-is in the subscription resource."""  
     minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    r"""The subscription's override minimum amount for the plan."""
+    r"""The subscription's override minimum amount for the plan."""  
+    net_terms: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_terms'), 'exclude': lambda f: f is None }})
+    r"""The net terms of a subscription determine when a subscription's invoice is due relative to its issue date. Whereas a net terms of 0 signifies \\"due on issue\\", a net terms of 30 can be used to provide the customer one month to pay the invoice. By default, the subscription defaults to the plan's net terms configuration."""  
+    phase_overrides: Optional[list[PostSubscriptionsApplicationJSONPhaseOverrides]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('phase_overrides'), 'exclude': lambda f: f is None }})
+    r"""Optionally provide a list of minimum amount or discount overrides for phases on the plan."""  
     plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_id'), 'exclude': lambda f: f is None }})
-    r"""The plan that the given subscription should be switched to. Note that either this property or `external_plan_id` must be specified."""
+    r"""The plan that the given customer should be subscribed to. The plan determines the pricing and cadence of the subscription."""  
     price_overrides: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_overrides'), 'exclude': lambda f: f is None }})
-    r"""Optionally provide a list of overrides for prices on the plan"""
-    
-
-@dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeRequest:
-    
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
-    request_body: Optional[PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Optionally provide a list of overrides for prices on the plan"""  
+    start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The date that Orb should start billing for the subscription, localized to the customer's timezone. If this is not provided, this defaults to the current date in the customer's timezone."""  
     
 
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDSchedulePlanChangeResponse:
+class PostSubscriptionsJSONResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     subscription: Optional[shared_subscription.Subscription] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_plan_changes.py` & `orb-billing-1.2.0/src/orb/models/operations/get_subscriptions_subscription_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 import dataclasses
 import requests as requests_http
 from ..shared import subscription as shared_subscription
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest:
+class GetSubscriptionsSubscriptionIDRequest:
     
-    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})
+    subscription_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'subscription_id', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse:
+class GetSubscriptionsSubscriptionIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
     subscription: Optional[shared_subscription.Subscription] = dataclasses.field(default=None)
-    r"""OK"""
+    r"""OK"""
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/put_customers_customer_id.py` & `orb-billing-1.2.0/src/orb/models/operations/put_customers_external_customer_id_external_customer_id.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,84 +8,80 @@
 from enum import Enum
 from orb import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCustomersCustomerIDRequestBodyBillingAddress:
+class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyBillingAddress:
     r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""
     
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})  
     country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""Two-letter country code (ISO 3166-1 alpha-2)."""
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
+    r"""Two-letter country code (ISO 3166-1 alpha-2)."""  
+    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})  
+    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})  
     postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postal_code'), 'exclude': lambda f: f is None }})
-    r"""ZIP or postal code"""
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    r"""ZIP or postal code"""  
+    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})  
     
-class PutCustomersCustomerIDRequestBodyPaymentProviderEnum(str, Enum):
+class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyPaymentProviderEnum(str, Enum):
     r"""This is used for creating charges or invoices in an external system via Orb. When not in test mode:
     - the connection must first be configured in the Orb webapp. 
     - if the provider is an invoicing provider (`stripe_invoice`, `quickbooks`, `bill.com`), any product mappings must first be configured with the Orb team.
     """
-    STRIPE_INVOICE = 'stripe_invoice'
     QUICKBOOKS = 'quickbooks'
-    BILL_COM = 'bill.com'
     STRIPE_CHARGE = 'stripe_charge'
-    LESS_THAN_NIL_GREATER_THAN_ = '<nil>'
+    STRIPE_INVOICE = 'stripe_invoice'
+    BILL_COM = 'bill.com'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCustomersCustomerIDRequestBodyShippingAddress:
+class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyShippingAddress:
     r"""The customer's shipping address; all fields in the address are optional. Note that downstream tax calculations are based on the shipping address."""
     
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})  
     country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""Two-letter country code (ISO 3166-1 alpha-2)."""
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
+    r"""Two-letter country code (ISO 3166-1 alpha-2)."""  
+    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})  
+    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})  
     postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postal_code'), 'exclude': lambda f: f is None }})
-    r"""ZIP or postal code"""
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    r"""ZIP or postal code"""  
+    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCustomersCustomerIDRequestBody:
-    r"""The external payments or invoicing solution connected to this customer."""
+class PutCustomersExternalCustomerIDExternalCustomerIDRequestBody:
     
-    billing_address: Optional[PutCustomersCustomerIDRequestBodyBillingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billing_address'), 'exclude': lambda f: f is None }})
-    r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    r"""A valid customer email, to be used for invoicing and notifications."""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    payment_provider: Optional[PutCustomersCustomerIDRequestBodyPaymentProviderEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment_provider'), 'exclude': lambda f: f is None }})
+    billing_address: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyBillingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billing_address'), 'exclude': lambda f: f is None }})
+    r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""  
+    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})  
+    payment_provider: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyPaymentProviderEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment_provider'), 'exclude': lambda f: f is None }})
     r"""This is used for creating charges or invoices in an external system via Orb. When not in test mode:
     - the connection must first be configured in the Orb webapp. 
     - if the provider is an invoicing provider (`stripe_invoice`, `quickbooks`, `bill.com`), any product mappings must first be configured with the Orb team.
-    """
+    """  
     payment_provider_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment_provider_id'), 'exclude': lambda f: f is None }})
-    r"""The ID of this customer in an external payments solution, such as Stripe. This is used for creating charges or invoices in the external system via Orb."""
-    shipping_address: Optional[PutCustomersCustomerIDRequestBodyShippingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_address'), 'exclude': lambda f: f is None }})
-    r"""The customer's shipping address; all fields in the address are optional. Note that downstream tax calculations are based on the shipping address."""
+    r"""The ID of this customer in an external payments solution, such as Stripe. This is used for creating charges or invoices in the external system via Orb."""  
+    shipping_address: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyShippingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_address'), 'exclude': lambda f: f is None }})
+    r"""The customer's shipping address; all fields in the address are optional. Note that downstream tax calculations are based on the shipping address."""  
     
 
 @dataclasses.dataclass
-class PutCustomersCustomerIDRequest:
+class PutCustomersExternalCustomerIDExternalCustomerIDRequest:
     
-    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})
-    r"""Orb customer ID"""
-    request_body: Optional[PutCustomersCustomerIDRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
-class PutCustomersCustomerIDResponse:
+class PutCustomersExternalCustomerIDExternalCustomerIDResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
     customer: Optional[shared_customer.Customer] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/put_customers_external_customer_id_external_customer_id.py` & `orb-billing-1.2.0/src/orb/models/operations/post_customers_customer_id_credits_ledger_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,71 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import customer as shared_customer
+from ..shared import credit_ledger_entry as shared_credit_ledger_entry
 from dataclasses_json import Undefined, dataclass_json
+from datetime import date
 from enum import Enum
+from marshmallow import fields
 from orb import utils
-from typing import Optional
+from typing import Any, Optional
 
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyBillingAddress:
-    r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""
-    
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""Two-letter country code (ISO 3166-1 alpha-2)."""
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postal_code'), 'exclude': lambda f: f is None }})
-    r"""ZIP or postal code"""
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
-    
-class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyPaymentProviderEnum(str, Enum):
-    r"""This is used for creating charges or invoices in an external system via Orb. When not in test mode:
-    - the connection must first be configured in the Orb webapp. 
-    - if the provider is an invoicing provider (`stripe_invoice`, `quickbooks`, `bill.com`), any product mappings must first be configured with the Orb team.
-    """
-    QUICKBOOKS = 'quickbooks'
-    STRIPE_CHARGE = 'stripe_charge'
-    STRIPE_INVOICE = 'stripe_invoice'
-    BILL_COM = 'bill.com'
-    LESS_THAN_NIL_GREATER_THAN_ = '<nil>'
+class PostCustomersCustomerIDCreditsLedgerEntryRequestBodyEntryTypeEnum(str, Enum):
+    INCREMENT = 'increment'
+    DECREMENT = 'decrement'
+    EXPIRATION_CHANGE = 'expiration_change'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyShippingAddress:
-    r"""The customer's shipping address; all fields in the address are optional. Note that downstream tax calculations are based on the shipping address."""
+class PostCustomersCustomerIDCreditsLedgerEntryRequestBodyInvoiceSettings:
+    r"""Passing `invoice_settings` automatically generates an invoice for the newly added credits. If `invoice_settings` is passed, you must specify `per_unit_cost_basis`, as the calculation of the invoice total is done on that basis."""
     
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""Two-letter country code (ISO 3166-1 alpha-2)."""
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postal_code'), 'exclude': lambda f: f is None }})
-    r"""ZIP or postal code"""
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    auto_collection: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auto_collection') }})
+    r"""Whether the credits purchase invoice should auto collect with the customer's saved payment method."""  
+    net_terms: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_terms') }})
+    r"""The net terms determines the difference between the invoice date and the issue date for the invoice. If you intend the invoice to be due on issue, set this to 0."""  
+    memo: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('memo'), 'exclude': lambda f: f is None }})
+    r"""An optional memo to display on the invoice."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutCustomersExternalCustomerIDExternalCustomerIDRequestBody:
+class PostCustomersCustomerIDCreditsLedgerEntryRequestBody:
     
-    billing_address: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyBillingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billing_address'), 'exclude': lambda f: f is None }})
-    r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""
-    email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    payment_provider: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyPaymentProviderEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment_provider'), 'exclude': lambda f: f is None }})
-    r"""This is used for creating charges or invoices in an external system via Orb. When not in test mode:
-    - the connection must first be configured in the Orb webapp. 
-    - if the provider is an invoicing provider (`stripe_invoice`, `quickbooks`, `bill.com`), any product mappings must first be configured with the Orb team.
-    """
-    payment_provider_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('payment_provider_id'), 'exclude': lambda f: f is None }})
-    r"""The ID of this customer in an external payments solution, such as Stripe. This is used for creating charges or invoices in the external system via Orb."""
-    shipping_address: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBodyShippingAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipping_address'), 'exclude': lambda f: f is None }})
-    r"""The customer's shipping address; all fields in the address are optional. Note that downstream tax calculations are based on the shipping address."""
+    entry_type: PostCustomersCustomerIDCreditsLedgerEntryRequestBodyEntryTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('entry_type') }})  
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    r"""The number of credits to effect. Note that this is required for increment or decrement operations."""  
+    block_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_id'), 'exclude': lambda f: f is None }})
+    r"""The ID of the block affected by an `expiration_change`"""  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Optional metadata that can be specified when adding ledger results via the API. For example, this can be used to note an increment refers to trial credits, or for noting corrections as a result of an incident, etc."""  
+    expiry_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiry_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""A future date (specified in YYYY-MM-DD format) that denotes when this credit balance should expire."""  
+    invoice_settings: Optional[PostCustomersCustomerIDCreditsLedgerEntryRequestBodyInvoiceSettings] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_settings'), 'exclude': lambda f: f is None }})
+    r"""Passing `invoice_settings` automatically generates an invoice for the newly added credits. If `invoice_settings` is passed, you must specify `per_unit_cost_basis`, as the calculation of the invoice total is done on that basis."""  
+    metadata: Optional[dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    r"""User-specified key/value pairs for the ledger entry resource."""  
+    per_unit_cost_basis: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_cost_basis'), 'exclude': lambda f: f is None }})
+    r"""Can only be specified when `entry_type=increment`. How much, in USD, a customer paid for a single credit in this block"""  
+    target_expiry_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target_expiry_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""A future date (specified in YYYY-MM-DD) used for `expiration_change`"""  
     
 
 @dataclasses.dataclass
-class PutCustomersExternalCustomerIDExternalCustomerIDRequest:
+class PostCustomersCustomerIDCreditsLedgerEntryRequest:
     
-    external_customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'external_customer_id', 'style': 'simple', 'explode': False }})
-    request_body: Optional[PutCustomersExternalCustomerIDExternalCustomerIDRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    customer_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'customer_id', 'style': 'simple', 'explode': False }})  
+    request_body: Optional[PostCustomersCustomerIDCreditsLedgerEntryRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})  
     
 
 @dataclasses.dataclass
-class PutCustomersExternalCustomerIDExternalCustomerIDResponse:
+class PostCustomersCustomerIDCreditsLedgerEntryResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    customer: Optional[shared_customer.Customer] = dataclasses.field(default=None)
-    r"""OK"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    credit_ledger_entry: Optional[shared_credit_ledger_entry.CreditLedgerEntry] = dataclasses.field(default=None)
+    r"""OK"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/operations/put_deprecate_events_event_id.py` & `orb-billing-1.2.0/src/orb/models/operations/deprecate_event.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 import requests as requests_http
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
-class PutDeprecateEventsEventIDRequest:
+class DeprecateEventRequest:
     
     event_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'event_id', 'style': 'simple', 'explode': False }})
-    r"""Identical to the `idempotency_key` provided on event ingestion. Uniquely identifies an event in the system."""
+    r"""Identical to the `idempotency_key` provided on event ingestion. Uniquely identifies an event in the system."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutDeprecateEventsEventID400ApplicationJSON:
+class DeprecateEvent400ApplicationJSON:
     r"""Bad Request"""
     
     status: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""HTTP Code"""
+    r"""HTTP Code"""  
     title: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title'), 'exclude': lambda f: f is None }})
-    r"""Error message"""
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    r"""Error message"""  
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})  
     validation_errors: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation_errors'), 'exclude': lambda f: f is None }})
-    r"""An array of strings corresponding to the validation failures"""
+    r"""An array of strings corresponding to the validation failures"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PutDeprecateEventsEventID200ApplicationJSON:
+class DeprecateEvent200ApplicationJSON:
     r"""OK"""
     
     deprecated: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deprecated'), 'exclude': lambda f: f is None }})
-    r"""event_id of the deprecated event, if successfully updated"""
+    r"""event_id of the deprecated event, if successfully updated"""  
     
 
 @dataclasses.dataclass
-class PutDeprecateEventsEventIDResponse:
+class DeprecateEventResponse:
     
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    put_deprecate_events_event_id_200_application_json_object: Optional[PutDeprecateEventsEventID200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""
-    put_deprecate_events_event_id_400_application_json_object: Optional[PutDeprecateEventsEventID400ApplicationJSON] = dataclasses.field(default=None)
-    r"""Bad Request"""
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    deprecate_event_200_application_json_object: Optional[DeprecateEvent200ApplicationJSON] = dataclasses.field(default=None)
+    r"""OK"""  
+    deprecate_event_400_application_json_object: Optional[DeprecateEvent400ApplicationJSON] = dataclasses.field(default=None)
+    r"""Bad Request"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/__init__.py` & `orb-billing-1.2.0/src/orb/models/shared/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-from .billingaddress import *
+from .coupon import *
 from .credit_ledger_entry import *
 from .customer import *
 from .customer_balance_transaction import *
+from .customer_tax_id import *
 from .event import *
 from .invoice import *
+from .invoice_line_item import *
 from .plan import *
 from .plan_phase import *
 from .price import *
 from .security import *
-from .shippingaddress import *
 from .subscription import *
 from .upcominginvoice import *
 
-__all__ = ["BillingAddress","CreditLedgerEntry","CreditLedgerEntryCreditBlock","CreditLedgerEntryCustomer","CreditLedgerEntryEntryStatusEnum","CreditLedgerEntryEntryTypeEnum","Customer","CustomerBalanceTransaction","CustomerBalanceTransactionActionEnum","CustomerBalanceTransactionInvoice","CustomerPaymentProviderEnum","Event","Invoice","InvoiceCustomer","InvoiceLineItems","InvoiceLineItemsGrouping","InvoiceLineItemsSubLineItems","InvoiceLineItemsSubLineItemsMatrixConfig","InvoiceLineItemsSubLineItemsTierConfig","InvoiceLineItemsSubLineItemsTypeEnum","InvoiceLineItemsTaxAmounts","InvoiceStatusEnum","InvoiceSubscription","Plan","PlanPhase","PlanPhaseDurationUnitEnum","PlanProduct","PlanTrialConfig","PlanTrialConfigTrialPeriodUnitEnum","Price","PriceBillableMetric","PriceBpsConfig","PriceBulkBpsConfig","PriceBulkBpsConfigTiers","PriceBulkConfig","PriceBulkConfigTiers","PriceCadenceEnum","PriceMatrixConfig","PriceMatrixConfigMatrixValues","PriceModelTypeEnum","PricePackageConfig","PriceTieredBpsConfig","PriceTieredBpsConfigTiers","PriceTieredConfig","PriceTieredConfigTiers","PriceUnitConfig","Security","ShippingAddress","Subscription","SubscriptionStatusEnum","UpcomingInvoice","UpcomingInvoiceCustomer","UpcomingInvoiceLineItems","UpcomingInvoiceLineItemsGrouping","UpcomingInvoiceLineItemsSubLineItems","UpcomingInvoiceLineItemsSubLineItemsMatrixConfig","UpcomingInvoiceLineItemsSubLineItemsTierConfig","UpcomingInvoiceLineItemsSubLineItemsTypeEnum","UpcomingInvoiceSubscription"]
+__all__ = ["Coupon","CouponInput","CreditLedgerEntry","CreditLedgerEntryCreditBlock","CreditLedgerEntryCustomer","CreditLedgerEntryEntryStatusEnum","CreditLedgerEntryEntryTypeEnum","Customer","CustomerBalanceTransaction","CustomerBalanceTransactionActionEnum","CustomerBalanceTransactionInvoice","CustomerBalanceTransactionTypeEnum","CustomerBillingAddress","CustomerPaymentProviderEnum","CustomerShippingAddress","CustomerTaxID","Event","Invoice","InvoiceAutoCollection","InvoiceCustomer","InvoiceLineItem","InvoiceLineItemSubLineItems","InvoiceLineItemSubLineItemsGrouping","InvoiceLineItemSubLineItemsMatrixConfig","InvoiceLineItemSubLineItemsTierConfig","InvoiceLineItemSubLineItemsTypeEnum","InvoiceLineItemTaxAmounts","InvoiceStatusEnum","InvoiceSubscription","Plan","PlanBasePlan","PlanPhase","PlanPhaseDurationUnitEnum","PlanProduct","PlanTrialConfig","PlanTrialConfigTrialPeriodUnitEnum","Price","PriceBillableMetric","PriceBpsConfig","PriceBulkBpsConfig","PriceBulkBpsConfigTiers","PriceBulkConfig","PriceBulkConfigTiers","PriceCadenceEnum","PriceMatrixConfig","PriceMatrixConfigMatrixValues","PriceModelTypeEnum","PricePackageConfig","PriceTieredBpsConfig","PriceTieredBpsConfigTiers","PriceTieredConfig","PriceTieredConfigTiers","PriceUnitConfig","Security","Subscription","SubscriptionFixedFeeQuantitySchedule","SubscriptionRedeemedCoupon","SubscriptionStatusEnum","UpcomingInvoice","UpcomingInvoiceCustomer","UpcomingInvoiceLineItems","UpcomingInvoiceLineItemsGrouping","UpcomingInvoiceLineItemsSubLineItems","UpcomingInvoiceLineItemsSubLineItemsMatrixConfig","UpcomingInvoiceLineItemsSubLineItemsTierConfig","UpcomingInvoiceLineItemsSubLineItemsTypeEnum","UpcomingInvoiceSubscription"]
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/billingaddress.py` & `orb-billing-1.2.0/src/orb/models/shared/event.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from orb import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class BillingAddress:
-    r"""The customer's billing address; all fields in the address are optional. This address appears on customer invoices."""
+class Event:
     
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""Two-letter country code (ISO 3166-1 alpha-2)."""
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postal_code'), 'exclude': lambda f: f is None }})
-    r"""ZIP or postal code"""
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id') }})
+    r"""The Orb Customer identifier"""  
+    event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
+    r"""A name to meaningfully identify the action or event type."""  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""A unique value, generated by the client, that is used to de-duplicate events. Note that on ingestion, this value is passed in as idempotency_key"""  
+    properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
+    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""  
+    timestamp: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
+    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""  
+    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
+    r"""An alias for the Orb customer, whose mapping is specified when creating the customer"""
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/credit_ledger_entry.py` & `orb-billing-1.2.0/src/orb/models/shared/credit_ledger_entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 import dataclasses
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from orb import utils
-from typing import Optional
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreditLedgerEntryCreditBlock:
     r"""Credit block that the entry affected"""
     
     expiry_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expiry_date') }})
-    r"""Complete timestamp with date and time for when this block expires"""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""Complete timestamp with date and time for when this block expires"""  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     per_unit_cost_basis: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_cost_basis') }})
-    r"""How much, in USD, a customer paid for a single credit in this block"""
+    r"""How much, in USD, a customer paid for a single credit in this block"""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreditLedgerEntryCustomer:
     
-    external_customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    external_customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     
 class CreditLedgerEntryEntryStatusEnum(str, Enum):
     r"""Committed entries are older than the ingestion grace period, and cannot change. Pending entries are newer than the grace period and are subject to updates"""
     COMMITTED = 'committed'
     PENDING = 'pending'
 
 class CreditLedgerEntryEntryTypeEnum(str, Enum):
@@ -41,31 +41,35 @@
     EXPIRATION_CHANGE = 'expiration_change'
     CREDIT_BLOCK_EXPIRY = 'credit_block_expiry'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreditLedgerEntry:
-    r"""A credit ledger entry is a single entry in the customer balance ledger. More details about working with real-time balances are [here](../docs/Credits.md).
+    r"""A credit ledger entry is a single entry in the customer balance ledger. More details about working with real-time balances are [here](../docs/Pre-paid-plans.md).
     
     To support late and out-of-order event reporting, ledger entries are marked as either __committed_ or _pending_. Committed entries are finalized and will not change. Pending entries can be updated up until the event reporting grace period.
     """
     
-    amount: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    r"""Number of credits that were impacted"""
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
     credit_block: CreditLedgerEntryCreditBlock = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credit_block') }})
-    r"""Credit block that the entry affected"""
-    customer: CreditLedgerEntryCustomer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
+    r"""Credit block that the entry affected"""  
+    customer: CreditLedgerEntryCustomer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})  
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    r"""Optional metadata that can be specified when adding ledger results via the API"""
-    ending_balance: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ending_balance') }})
+    r"""Optional metadata that can be specified when adding ledger results via the API"""  
+    ending_balance: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ending_balance') }})  
     entry_status: CreditLedgerEntryEntryStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('entry_status') }})
-    r"""Committed entries are older than the ingestion grace period, and cannot change. Pending entries are newer than the grace period and are subject to updates"""
-    entry_type: CreditLedgerEntryEntryTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('entry_type') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""Committed entries are older than the ingestion grace period, and cannot change. Pending entries are newer than the grace period and are subject to updates"""  
+    entry_type: CreditLedgerEntryEntryTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('entry_type') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     ledger_sequence_number: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger_sequence_number') }})
-    r"""The position in which this entry appears in the ledger, starting at 0"""
-    starting_balance: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('starting_balance') }})
-    event_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_id'), 'exclude': lambda f: f is None }})
-    price_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_id'), 'exclude': lambda f: f is None }})
+    r"""The position in which this entry appears in the ledger, starting at 0"""  
+    metadata: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    r"""User-specified metadata dictionary that's specified when adding a ledger entry. This contains key/value pairs if metadata is specified, but otherwise is an empty dictionary."""  
+    starting_balance: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('starting_balance') }})  
+    amount: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount'), 'exclude': lambda f: f is None }})
+    r"""Number of credits that were impacted. Required on creation for increment and decrement entries."""  
+    event_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_id'), 'exclude': lambda f: f is None }})  
+    new_block_expiry_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('new_block_expiry_date'), 'exclude': lambda f: f is None }})
+    r"""In the case of an expiration change ledger entry, this represents the expiration time of the new block."""  
+    price_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('price_id'), 'exclude': lambda f: f is None }})
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/customer_balance_transaction.py` & `orb-billing-1.2.0/src/orb/models/shared/customer_balance_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,32 +18,37 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomerBalanceTransactionInvoice:
     r"""The Invoice associated with this transaction"""
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""The Invoice id"""
+    r"""The Invoice id"""  
     
+class CustomerBalanceTransactionTypeEnum(str, Enum):
+    INCREMENT = 'increment'
+    DECREMENT = 'decrement'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomerBalanceTransaction:
     r"""A single change to the customer balance. All amounts are in the customer's currency."""
     
     action: CustomerBalanceTransactionActionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action') }})
-    r"""Describes the reason that this transaction took place."""
+    r"""Describes the reason that this transaction took place."""  
     amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    r"""The value of the amount changed in the transaction."""
+    r"""The value of the amount changed in the transaction."""  
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The creation time of this transaction."""
+    r"""The creation time of this transaction."""  
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    r"""An optional description provided for manual customer balance adjustments."""
+    r"""An optional description provided for manual customer balance adjustments."""  
     ending_balance: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ending_balance') }})
-    r"""The new value of the customer's balance prior to the transaction, in the customer's currency."""
+    r"""The new value of the customer's balance prior to the transaction, in the customer's currency."""  
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""A unique id for this transaction."""
+    r"""A unique id for this transaction."""  
     invoice: CustomerBalanceTransactionInvoice = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice') }})
-    r"""The Invoice associated with this transaction"""
+    r"""The Invoice associated with this transaction"""  
     starting_balance: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('starting_balance') }})
-    r"""The original value of the customer's balance prior to the transaction, in the customer's currency."""
+    r"""The original value of the customer's balance prior to the transaction, in the customer's currency."""  
+    type: CustomerBalanceTransactionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/event.py` & `orb-billing-1.2.0/src/orb/models/shared/plan_phase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
 from orb import utils
 from typing import Any, Optional
 
+class PlanPhaseDurationUnitEnum(str, Enum):
+    r"""Term for this plan, which is the maximum cadence among all component prices"""
+    MONTHLY = 'monthly'
+    QUARTERLY = 'quarterly'
+    ANNUAL = 'annual'
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Event:
+class PlanPhase:
+    r"""A plan can optionally consist of plan phases, which represents a pricing configuration that's only active for the length of time specified by `duration` and `duration_unit`. All plans must have an evergreen phase, which is the last phase and active indefinitely."""
     
-    customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id') }})
-    r"""The Orb Customer identifier"""
-    event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('event_name') }})
-    r"""A name to meaningfully identify the action or event type."""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""A unique value, generated by the client, that is used to de-duplicate events. Note that on ingestion, this value is passed in as idempotency_key"""
-    properties: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties') }})
-    r"""A dictionary of custom properties. Values in this dictionary must be numeric, boolean, or strings. Nested dictionaries are disallowed."""
-    timestamp: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp') }})
-    r"""An ISO 8601 format date with no timezone offset (i.e. UTC). This should represent the time that usage was recorded, and is particularly important to attribute usage to a given billing period."""
-    external_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id'), 'exclude': lambda f: f is None }})
-    r"""An alias for the Orb customer, whose mapping is specified when creating the customer"""
+    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})  
+    duration_unit: PlanPhaseDurationUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration_unit') }})
+    r"""Term for this plan, which is the maximum cadence among all component prices"""  
+    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})  
+    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
+    r"""How many terms of length `duration_unit` this phase is active for. If null, this phase is evergreen and active indefinitely"""  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})  
+    order: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order'), 'exclude': lambda f: f is None }})
+    r"""Determines the ordering of the phase in a plan's lifecycle. 1 = first phase."""
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/invoice.py` & `orb-billing-1.2.0/src/orb/models/shared/upcominginvoice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,158 +1,127 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from ..shared import customer_balance_transaction as shared_customer_balance_transaction
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
+from datetime import date, datetime
 from enum import Enum
 from marshmallow import fields
 from orb import utils
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceCustomer:
+class UpcomingInvoiceCustomer:
     r"""The customer receiving this invoice."""
     
-    external_customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    external_customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_customer_id') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineItemsGrouping:
+class UpcomingInvoiceLineItemsGrouping:
     r"""For configured prices that are split by a grouping key, this will be populated with the key and a value. The `amount` and `subtotal` will be the values for this particular grouping."""
     
-    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
+    key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})  
+    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineItemsSubLineItemsMatrixConfig:
+class UpcomingInvoiceLineItemsSubLineItemsMatrixConfig:
     r"""Only available if `type` is `matrix`. Contains the values of the matrix that this `sub_line_item` represents."""
     
     dimension_values: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimension_values') }})
-    r"""The ordered dimension values for this line item."""
+    r"""The ordered dimension values for this line item."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineItemsSubLineItemsTierConfig:
+class UpcomingInvoiceLineItemsSubLineItemsTierConfig:
     r"""Only available if `type` is `tier`. Contains the range of units in this tier and the unit amount."""
     
-    first_unit: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit') }})
-    last_unit: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit') }})
-    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})
+    first_unit: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit') }})  
+    last_unit: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit') }})  
+    unit_amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount') }})  
     
-class InvoiceLineItemsSubLineItemsTypeEnum(str, Enum):
+class UpcomingInvoiceLineItemsSubLineItemsTypeEnum(str, Enum):
     r"""An identifier for a sub line item that is specific to a pricing model."""
     MATRIX = 'matrix'
     TIER = 'tier'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineItemsSubLineItems:
+class UpcomingInvoiceLineItemsSubLineItems:
     
     amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    r"""The total amount for this sub line item."""
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
-    type: InvoiceLineItemsSubLineItemsTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""An identifier for a sub line item that is specific to a pricing model."""
-    matrix_config: Optional[InvoiceLineItemsSubLineItemsMatrixConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('matrix_config'), 'exclude': lambda f: f is None }})
-    r"""Only available if `type` is `matrix`. Contains the values of the matrix that this `sub_line_item` represents."""
-    tier_config: Optional[InvoiceLineItemsSubLineItemsTierConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tier_config'), 'exclude': lambda f: f is None }})
-    r"""Only available if `type` is `tier`. Contains the range of units in this tier and the unit amount."""
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class InvoiceLineItemsTaxAmounts:
-    
-    amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    r"""The amount of additional tax incurred by this tax rate."""
-    tax_rate_description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tax_rate_description') }})
-    r"""The human-readable description of the applied tax rate."""
-    tax_rate_percentage: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tax_rate_percentage') }})
-    r"""The tax rate percentage, out of 100."""
+    r"""The total amount for this sub line item."""  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})  
+    type: UpcomingInvoiceLineItemsSubLineItemsTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""An identifier for a sub line item that is specific to a pricing model."""  
+    matrix_config: Optional[UpcomingInvoiceLineItemsSubLineItemsMatrixConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('matrix_config'), 'exclude': lambda f: f is None }})
+    r"""Only available if `type` is `matrix`. Contains the values of the matrix that this `sub_line_item` represents."""  
+    tier_config: Optional[UpcomingInvoiceLineItemsSubLineItemsTierConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tier_config'), 'exclude': lambda f: f is None }})
+    r"""Only available if `type` is `tier`. Contains the range of units in this tier and the unit amount."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceLineItems:
+class UpcomingInvoiceLineItems:
     
     amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
-    r"""The final amount after any discounts or minimums."""
-    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})
+    r"""The final amount after any discounts or minimums."""  
     end_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The end date of the range of time applied for this line item's price."""
-    grouping: InvoiceLineItemsGrouping = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping') }})
-    r"""For configured prices that are split by a grouping key, this will be populated with the key and a value. The `amount` and `subtotal` will be the values for this particular grouping."""
-    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})
+    r"""The end date of the range of time applied for this line item's price."""  
+    grouping: UpcomingInvoiceLineItemsGrouping = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grouping') }})
+    r"""For configured prices that are split by a grouping key, this will be populated with the key and a value. The `amount` and `subtotal` will be the values for this particular grouping."""  
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""The name of the price associated with this line item."""
-    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
+    r"""The name of the price associated with this line item."""  
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})  
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The start date of the range of time applied for this line item's price."""
-    sub_line_items: list[InvoiceLineItemsSubLineItems] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sub_line_items') }})
-    r"""For complex pricing structures, the line item can be broken down further in `sub_line_items`."""
+    r"""The start date of the range of time applied for this line item's price."""  
+    sub_line_items: list[UpcomingInvoiceLineItemsSubLineItems] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sub_line_items') }})
+    r"""For complex pricing structures, the line item can be broken down further in `sub_line_items`."""  
     subtotal: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal') }})
-    r"""The line amount before any line item-specific discounts or minimums."""
-    tax_amounts: list[InvoiceLineItemsTaxAmounts] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tax_amounts') }})
-    r"""An array of tax rates and their incurred tax amounts. Empty if no tax integration is configured."""
+    r"""The line amount before any line item-specific discounts or minimums."""  
     
-class InvoiceStatusEnum(str, Enum):
-    r"""The status of this invoice as known to Orb. Invoices that have been issued for past billing periods are marked `\\"issued\\"`. Invoices will be marked `\\"paid\\"` upon confirmation of successful automatic payment collection by Orb. Invoices synced to an external billing provider (such as Bill.com, QuickBooks, or Stripe Invoicing) will be marked as `\\"synced\\"`."""
-    ISSUED = 'issued'
-    PAID = 'paid'
-    SYNCED = 'synced'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InvoiceSubscription:
+class UpcomingInvoiceSubscription:
     r"""The associated subscription for this invoice."""
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Invoice:
-    r"""An [`Invoice`](../reference/Orb-API.json/components/schemas/Invoice) is a fundamental billing entity, representing the request for payment for a single subscription. This includes a set of line items, which correspond to prices in the subscription's plan and can represent fixed recurring fees or usage-based fees. They are generated at the end of a billing period, or as the result of an action, such as a cancellation."""
+class UpcomingInvoice:
+    r"""Upcoming invoices contain a line-by-line breakdown of an upcoming amount due for a subscription, including incurred usage in the billing period as well as any recurring fees.
+    
+    Although each line item will be invoiced on the `target_date`, each invoice line item may have distinct date ranges (e.g. for usage billed in arrears, the range may specify the current month whereas an in-advance recurring fees will be for the following month).
+    
+    Since an invoice resource has not been created for this upcoming invoice, this endpoint intentionally does not return an `id` field.
+    """
     
     amount_due: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount_due') }})
-    r"""This is the final amount required to be charged to the customer and reflects the application of the customer balance to the `total` of the invoice."""
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""The creation time of the resource in Orb."""
+    r"""The final amount to be charged to the customer after all minimums and discounts have been applied. Only populated for non-pre-paid plans."""  
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-    r"""An ISO 4217 currency string or `credits`"""
-    customer: InvoiceCustomer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
-    r"""The customer receiving this invoice."""
-    customer_balance_transactions: list[shared_customer_balance_transaction.CustomerBalanceTransaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_balance_transactions') }})
-    r"""A list of Customer balance transactions that may be associated with this invoice."""
-    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})
-    due_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('due_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""When the invoice payment is due."""
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    invoice_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    r"""Issue date of the invoice"""
-    invoice_pdf: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_pdf') }})
-    r"""The link to download the PDF representation of the `Invoice`."""
-    line_items: list[InvoiceLineItems] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line_items') }})
-    r"""The breakdown of prices in this invoice."""
-    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})
-    subscription: InvoiceSubscription = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscription') }})
-    r"""The associated subscription for this invoice."""
+    r"""An ISO 4217 currency string or `credits`"""  
+    customer: UpcomingInvoiceCustomer = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer') }})
+    r"""The customer receiving this invoice."""  
+    hosted_invoice_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hosted_invoice_url') }})
+    r"""A URL for the invoice portal."""  
+    line_items: list[UpcomingInvoiceLineItems] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line_items') }})
+    r"""The breakdown of prices in this invoice."""  
+    subscription: UpcomingInvoiceSubscription = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscription') }})
+    r"""The associated subscription for this invoice."""  
     subtotal: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtotal') }})
-    r"""The total before any discounts and minimums are applied."""
-    total: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('total') }})
-    r"""The total after any minimums, discounts, and taxes have been applied."""
-    status: Optional[InvoiceStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""The status of this invoice as known to Orb. Invoices that have been issued for past billing periods are marked `\\"issued\\"`. Invoices will be marked `\\"paid\\"` upon confirmation of successful automatic payment collection by Orb. Invoices synced to an external billing provider (such as Bill.com, QuickBooks, or Stripe Invoicing) will be marked as `\\"synced\\"`."""
+    r"""The total before any discounts and minimums are applied."""  
+    target_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+    r"""The expected issue date of the invoice."""
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/plan.py` & `orb-billing-1.2.0/src/orb/models/shared/plan.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,50 +11,66 @@
 from marshmallow import fields
 from orb import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
+class PlanBasePlan:
+    r"""The parent plan if the given plan was created by overriding one or more of the parent's prices"""
+    
+    external_plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_plan_id'), 'exclude': lambda f: f is None }})  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})  
+    
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
 class PlanProduct:
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
     
 class PlanTrialConfigTrialPeriodUnitEnum(str, Enum):
     DAYS = 'days'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PlanTrialConfig:
     
-    trial_period_unit: PlanTrialConfigTrialPeriodUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_period_unit') }})
-    trial_period: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_period'), 'exclude': lambda f: f is None }})
+    trial_period_unit: PlanTrialConfigTrialPeriodUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_period_unit') }})  
+    trial_period: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_period'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Plan:
     r"""OK"""
     
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})  
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-    r"""An ISO 4217 currency string or custom pricing unit (`credits`) for this plan's prices."""
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""An ISO 4217 currency string or custom pricing unit (`credits`) for this plan's prices."""  
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})  
+    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})  
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})  
     invoicing_currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoicing_currency') }})
-    r"""An ISO 4217 currency string for which this plan is billed in. Matches `currency` unless `currency` is a custom pricing unit."""
-    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    r"""An ISO 4217 currency string for which this plan is billed in. Matches `currency` unless `currency` is a custom pricing unit."""  
+    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})  
     prices: list[shared_price.Price] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prices') }})
-    r"""Prices for this plan. If the plan has phases, this includes prices across all phases of the plan."""
-    product: PlanProduct = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('product') }})
+    r"""Prices for this plan. If the plan has phases, this includes prices across all phases of the plan."""  
+    product: PlanProduct = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('product') }})  
+    base_plan: Optional[PlanBasePlan] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_plan'), 'exclude': lambda f: f is None }})
+    r"""The parent plan if the given plan was created by overriding one or more of the parent's prices"""  
     base_plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_plan_id'), 'exclude': lambda f: f is None }})
-    r"""The parent plan id if the given plan was created by overriding one or more of the parent's prices"""
+    r"""The parent plan id if the given plan was created by overriding one or more of the parent's prices"""  
+    default_invoice_memo: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default_invoice_memo'), 'exclude': lambda f: f is None }})
+    r"""The default memo text on the invoices corresponding to subscriptions on this plan. Note that each subscription may configure its own memo."""  
     external_plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('external_plan_id'), 'exclude': lambda f: f is None }})
-    r"""An optional user-defined ID for this plan resource, used throughout the system as an alias for this Plan. Use this field to identify a plan by an existing identifier in your system."""
-    plan_phases: Optional[list[shared_plan_phase.PlanPhase]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_phases'), 'exclude': lambda f: f is None }})
-    trial_config: Optional[PlanTrialConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_config'), 'exclude': lambda f: f is None }})
+    r"""An optional user-defined ID for this plan resource, used throughout the system as an alias for this Plan. Use this field to identify a plan by an existing identifier in your system."""  
+    net_terms: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('net_terms'), 'exclude': lambda f: f is None }})
+    r"""Determines the difference between the invoice issue date and the due date. A value of \\"0\\" here signifies that invoices are due on issue, whereas a value of \\"30\\" means that the customer has a month to pay the invoice before its overdue. Note that individual subscriptions or invoices may set a different net terms configuration."""  
+    plan_phases: Optional[list[shared_plan_phase.PlanPhase]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_phases'), 'exclude': lambda f: f is None }})  
+    trial_config: Optional[PlanTrialConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('trial_config'), 'exclude': lambda f: f is None }})
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/plan_phase.py` & `orb-billing-1.2.0/src/orb/models/operations/post_invoice_line_items.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import requests as requests_http
+from ..shared import invoice_line_item as shared_invoice_line_item
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
+from datetime import date
+from marshmallow import fields
 from orb import utils
-from typing import Any, Optional
-
-class PlanPhaseDurationUnitEnum(str, Enum):
-    r"""Term for this plan, which is the maximum cadence among all component prices"""
-    MONTHLY = 'monthly'
-    QUARTERLY = 'quarterly'
-    ANNUAL = 'annual'
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class PlanPhase:
-    r"""A plan can optionally consist of plan phases, which represents a pricing configuration that's only active for the length of time specified by `duration` and `duration_unit`. All plans must have an evergreen phase, which is the last phase and active indefinitely."""
+class PostInvoiceLineItemsRequestBody:
+    
+    amount: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    r"""The total amount in the invoice's currency to add to the line item."""  
+    end_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+    r"""An date string to specify the line item's end date in the customer's timezone."""  
+    invoice_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_id') }})
+    r"""The id of the `Invoice` to add this line item."""  
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    r"""The item name associated with this line item. If an item with the same name exists in Orb, that item will be associated with the line item."""  
+    quantity: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quantity') }})
+    r"""The number of units on the line item"""  
+    start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+    r"""An date string to specify the line item's start date in the customer's timezone."""  
+    
+
+@dataclasses.dataclass
+class PostInvoiceLineItemsResponse:
     
-    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})
-    duration_unit: PlanPhaseDurationUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration_unit') }})
-    r"""Term for this plan, which is the maximum cadence among all component prices"""
-    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})
-    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    duration: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-    r"""How many terms of length `duration_unit` this phase is active for. If null, this phase is evergreen and active indefinitely"""
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    order: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('order'), 'exclude': lambda f: f is None }})
-    r"""Determines the ordering of the phase in a plan's lifecycle. 1 = first phase."""
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    invoice_line_item: Optional[shared_invoice_line_item.InvoiceLineItem] = dataclasses.field(default=None)
+    r"""Created"""  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
```

### Comparing `orb-billing-0.9.3/src/orb/models/shared/price.py` & `orb-billing-1.2.0/src/orb/models/shared/price.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,80 +11,80 @@
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBillableMetric:
     
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBpsConfig:
     r"""Provided when model_type is `bps`"""
     
-    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})
-    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})
+    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})  
+    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBulkBpsConfigTiers:
     
-    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})
-    maximum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount'), 'exclude': lambda f: f is None }})
-    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})
+    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})  
+    maximum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount'), 'exclude': lambda f: f is None }})  
+    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBulkBpsConfig:
     r"""Provided when model_type is `bulk_bps`"""
     
-    tiers: Optional[list[PriceBulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PriceBulkBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBulkConfigTiers:
     
-    maximum_units: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units'), 'exclude': lambda f: f is None }})
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    maximum_units: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_units'), 'exclude': lambda f: f is None }})  
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceBulkConfig:
     r"""Provided when model_type is `bulk`"""
     
-    tiers: Optional[list[PriceBulkConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PriceBulkConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 class PriceCadenceEnum(str, Enum):
     ANNUAL = 'annual'
     MONTHLY = 'monthly'
     QUARTERLY = 'quarterly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceMatrixConfigMatrixValues:
     
-    dimension_values: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimension_values'), 'exclude': lambda f: f is None }})
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    dimension_values: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimension_values'), 'exclude': lambda f: f is None }})  
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceMatrixConfig:
     r"""Provided when model_type is `matrix`"""
     
-    default_unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default_unit_amount'), 'exclude': lambda f: f is None }})
-    dimensions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimensions'), 'exclude': lambda f: f is None }})
-    matrix_values: Optional[list[PriceMatrixConfigMatrixValues]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('matrix_values'), 'exclude': lambda f: f is None }})
+    default_unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('default_unit_amount'), 'exclude': lambda f: f is None }})  
+    dimensions: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimensions'), 'exclude': lambda f: f is None }})  
+    matrix_values: Optional[list[PriceMatrixConfigMatrixValues]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('matrix_values'), 'exclude': lambda f: f is None }})  
     
 class PriceModelTypeEnum(str, Enum):
     UNIT = 'unit'
     TIERED = 'tiered'
     BULK = 'bulk'
     PACKAGE = 'package'
     BPS = 'bps'
@@ -94,59 +94,59 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PricePackageConfig:
     r"""Provided when model_type is `package`"""
     
-    package_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_amount'), 'exclude': lambda f: f is None }})
-    package_size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_size'), 'exclude': lambda f: f is None }})
+    package_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_amount'), 'exclude': lambda f: f is None }})  
+    package_size: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_size'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceTieredBpsConfigTiers:
     
-    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})
-    maximum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount'), 'exclude': lambda f: f is None }})
-    minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})
-    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})
+    bps: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps'), 'exclude': lambda f: f is None }})  
+    maximum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maximum_amount'), 'exclude': lambda f: f is None }})  
+    minimum_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum_amount'), 'exclude': lambda f: f is None }})  
+    per_unit_maximum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('per_unit_maximum'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceTieredBpsConfig:
     r"""Provided when model_type is `tiered_bps`"""
     
-    tiers: Optional[list[PriceTieredBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PriceTieredBpsConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceTieredConfigTiers:
     
-    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})
-    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    first_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('first_unit'), 'exclude': lambda f: f is None }})  
+    last_unit: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('last_unit'), 'exclude': lambda f: f is None }})  
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceTieredConfig:
     r"""Provided when model_type is`tiered`"""
     
-    tiers: Optional[list[PriceTieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})
+    tiers: Optional[list[PriceTieredConfigTiers]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiers'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PriceUnitConfig:
     r"""Provided when model_type is `unit`"""
     
-    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})
+    unit_amount: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_amount'), 'exclude': lambda f: f is None }})  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Price:
     r"""Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given Price object. The model_type field determines the key for the configuration object that is present.
     
@@ -323,37 +323,37 @@
         \"fixed_price_quantity\": 3.0
         ...
     }
     ```
     """
     
     currency: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency') }})
-    r"""An ISO 4217 currency string for this plan's prices."""
-    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})
-    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})
+    r"""An ISO 4217 currency string for this plan's prices."""  
+    discount: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discount') }})  
+    minimum: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minimum') }})  
     plan_phase_order: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_phase_order') }})
-    r"""The phase order which includes this price, only applicable to a plan with phases."""
-    billable_metric: Optional[PriceBillableMetric] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billable_metric'), 'exclude': lambda f: f is None }})
+    r"""The phase order which includes this price, only applicable to a plan with phases."""  
+    billable_metric: Optional[PriceBillableMetric] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billable_metric'), 'exclude': lambda f: f is None }})  
     bps_config: Optional[PriceBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bps_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `bps`"""
+    r"""Provided when model_type is `bps`"""  
     bulk_bps_config: Optional[PriceBulkBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_bps_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `bulk_bps`"""
+    r"""Provided when model_type is `bulk_bps`"""  
     bulk_config: Optional[PriceBulkConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bulk_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `bulk`"""
-    cadence: Optional[PriceCadenceEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cadence'), 'exclude': lambda f: f is None }})
-    created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Provided when model_type is `bulk`"""  
+    cadence: Optional[PriceCadenceEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cadence'), 'exclude': lambda f: f is None }})  
+    created_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('created_at'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})  
     fixed_price_quantity: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fixed_price_quantity'), 'exclude': lambda f: f is None }})
-    r"""If the Price represents a fixed cost, this represents the quantity of units applied. Mutually exclusive with billable_metric."""
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    r"""If the Price represents a fixed cost, this represents the quantity of units applied. Mutually exclusive with billable_metric."""  
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})  
     matrix_config: Optional[PriceMatrixConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('matrix_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `matrix`"""
-    model_type: Optional[PriceModelTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Provided when model_type is `matrix`"""  
+    model_type: Optional[PriceModelTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_type'), 'exclude': lambda f: f is None }})  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})  
     package_config: Optional[PricePackageConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('package_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `package`"""
+    r"""Provided when model_type is `package`"""  
     tiered_bps_config: Optional[PriceTieredBpsConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_bps_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `tiered_bps`"""
+    r"""Provided when model_type is `tiered_bps`"""  
     tiered_config: Optional[PriceTieredConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiered_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is`tiered`"""
+    r"""Provided when model_type is`tiered`"""  
     unit_config: Optional[PriceUnitConfig] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unit_config'), 'exclude': lambda f: f is None }})
-    r"""Provided when model_type is `unit`"""
+    r"""Provided when model_type is `unit`"""
```

### Comparing `orb-billing-0.9.3/src/orb/plan.py` & `orb-billing-1.2.0/src/orb/plan.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import requests as requests_http
 from . import utils
 from orb.models import operations, shared
 from typing import Optional
 
 class Plan:
-    r"""Actions related to plan management."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,100 +17,120 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def get(self, plan_id: str) -> operations.GetPlansPlanIDResponse:
-        r"""Retrieve a plan
-        This endpoint is used to fetch [plan](../reference/Orb-API.json/components/schemas/Plan) details given a plan identifier. It returns information about the prices included in the plan and their configuration, as well as the product that the plan is attached to.
-        
-        ## Serialized prices
-        Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given [Price](../reference/Orb-API.json/components/schemas/Price) object. The `model_type` field determines the key for the configuration object that is present. A detailed explanation of price types can be found in the [Price schema](../reference/Orb-API.json/components/schemas/Price). 
+    def get_plans(self, retries: Optional[utils.RetryConfig] = None) -> operations.GetPlansResponse:
+        r"""List plans
+        This endpoint returns a list of all [plans](../reference/Orb-API.json/components/schemas/Plan) for an account in a list format. 
         
-        ## Phases
-        Orb supports plan phases, also known as contract ramps. For plans with phases, the serialized prices refer to all prices across all phases.
+        The list of plans is ordered starting from the most recently created plan. The response also includes [`pagination_metadata`](../reference/Orb-API.json/components/schemas/Pagination-metadata), which lets the caller retrieve the next page of results if they exist. More information about pagination can be found in the [Pagination-metadata schema](../reference/Orb-API.json/components/schemas/Pagination-metadata).
         """
-        request = operations.GetPlansPlanIDRequest(
-            plan_id=plan_id,
-        )
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetPlansPlanIDRequest, base_url, '/plans/{plan_id}', request)
+        url = base_url.removesuffix('/') + '/plans'
         
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetPlansPlanIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetPlansResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Plan])
-                res.plan = out
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetPlans200ApplicationJSON])
+                res.get_plans_200_application_json_object = out
 
         return res
 
-    
-    def get_by_external_id(self, external_plan_id: str, plan: Optional[shared.Plan] = None) -> operations.GetPlansExternalPlanIDResponse:
+    def get_plans_external_plan_id(self, request: operations.GetPlansExternalPlanIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPlansExternalPlanIDResponse:
         r"""Retrieve a plan by external plan ID
         This endpoint is used to fetch [plan](../reference/Orb-API.json/components/schemas/Plan) details given an external_plan_id identifier. It returns information about the prices included in the plan and their configuration, as well as the product that the plan is attached to.
         
         ## Serialized prices
         Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given [Price](../reference/Orb-API.json/components/schemas/Price) object. The `model_type` field determines the key for the configuration object that is present. A detailed explanation of price types can be found in the [Price schema](../reference/Orb-API.json/components/schemas/Price).
         """
-        request = operations.GetPlansExternalPlanIDRequest(
-            external_plan_id=external_plan_id,
-            plan=plan,
-        )
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetPlansExternalPlanIDRequest, base_url, '/plans/external_plan_id/{external_plan_id}', request)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "plan", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('GET', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetPlansExternalPlanIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
 
         return res
 
-    
-    def list(self, request: operations.ListPlansRequestBody) -> operations.ListPlansResponse:
-        r"""List plans
-        This endpoint returns a list of all [plans](../reference/Orb-API.json/components/schemas/Plan) for an account in a list format. 
+    def get_plans_plan_id(self, request: operations.GetPlansPlanIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetPlansPlanIDResponse:
+        r"""Retrieve a plan
+        This endpoint is used to fetch [plan](../reference/Orb-API.json/components/schemas/Plan) details given a plan identifier. It returns information about the prices included in the plan and their configuration, as well as the product that the plan is attached to.
         
-        The list of plans is ordered starting from the most recently created plan. The response also includes [`pagination_metadata`](../reference/Orb-API.json/components/schemas/Pagination-metadata), which lets the caller retrieve the next page of results if they exist. More information about pagination can be found in the [Pagination-metadata schema](../reference/Orb-API.json/components/schemas/Pagination-metadata).
+        ## Serialized prices
+        Orb supports a few different pricing models out of the box. Each of these models is serialized differently in a given [Price](../reference/Orb-API.json/components/schemas/Price) object. The `model_type` field determines the key for the configuration object that is present. A detailed explanation of price types can be found in the [Price schema](../reference/Orb-API.json/components/schemas/Price). 
+        
+        ## Phases
+        Orb supports plan phases, also known as contract ramps. For plans with phases, the serialized prices refer to all prices across all phases.
         """
         base_url = self._server_url
         
-        url = base_url.removesuffix('/') + '/plans'
+        url = utils.generate_url(operations.GetPlansPlanIDRequest, base_url, '/plans/{plan_id}', request)
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('GET', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListPlansResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetPlansPlanIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Plan])
+                res.plan = out
 
         return res
```

### Comparing `orb-billing-0.9.3/src/orb/subscription.py` & `orb-billing-1.2.0/src/orb/subscription.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import requests as requests_http
 from . import utils
 from orb.models import operations, shared
 from typing import Optional
 
 class Subscription:
-    r"""Actions related to subscription mangement."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -18,112 +17,535 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    
-    def cancel(self, cancel_option: operations.PostSubscriptionsSubscriptionIDCancelCancelOptionEnum, subscription_id: str) -> operations.PostSubscriptionsSubscriptionIDCancelResponse:
+    def get_subscription_id_usage_by_customer(self, request: operations.GetSubscriptionIDUsageByCustomerRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSubscriptionIDUsageByCustomerResponse:
+        r"""View subscription costs
+        This endpoint is used to fetch a day-by-day snapshot of a subscription's costs in Orb, calculated by applying pricing information to the underlying usage (see the [subscription usage endpoint](../reference/Orb-API.json/paths/~1subscriptions~1{subscription_id}~1usage/get) to fetch usage per metric, in usage units rather than a currency). 
+        
+        
+        The semantics of this endpoint exactly mirror those of [fetching a customer's costs](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1costs/get). Use this endpoint to limit your analysis of costs to a specific subscription for the customer (e.g. to de-aggregate costs when a customer's subscription has started and stopped on the same day).
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetSubscriptionIDUsageByCustomerRequest, base_url, '/subscriptions/{subscription_id}/costs', request)
+        
+        query_params = utils.get_query_params(operations.GetSubscriptionIDUsageByCustomerRequest, request)
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetSubscriptionIDUsageByCustomerResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSubscriptionIDUsageByCustomer200ApplicationJSON])
+                res.get_subscription_id_usage_by_customer_200_application_json_object = out
+
+        return res
+
+    def get_subscriptions(self, request: operations.GetSubscriptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSubscriptionsResponse:
+        r"""List subscriptions
+        This endpoint returns a list of all subscriptions for an account as a [paginated](../docs/Pagination.md) list, ordered starting from the most recently created subscription. For a full discussion of the subscription resource, see [Subscription](../reference/Orb-API.json/components/schemas/Subscription).
+        
+        Subscriptions can be filtered to a single customer by passing in the `customer_id` query parameter or the `external_customer_id` query parameter.
+        """
+        base_url = self._server_url
+        
+        url = base_url.removesuffix('/') + '/subscriptions'
+        
+        query_params = utils.get_query_params(operations.GetSubscriptionsRequest, request)
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetSubscriptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSubscriptions200ApplicationJSON])
+                res.get_subscriptions_200_application_json_object = out
+
+        return res
+
+    def get_subscriptions_id_usage(self, request: operations.GetSubscriptionsIDUsageRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSubscriptionsIDUsageResponse:
+        r"""View subscription usage
+        This endpoint is used to fetch a subscription's usage in Orb. Especially when combined with optional query parameters, this endpoint is a powerful way to build visualizations on top of Orb's event data and metrics.
+        
+        With no query parameters specified, this endpoint returns usage for the subscription's _current billing period_ across each billable metric that participates in the subscription. Usage quantities returned are the result of evaluating the metric definition for the entirety of the customer's billing period.
+        
+        ### Default response shape
+        
+        Orb returns a `data` array with an object corresponding to each billable metric. Nested within this object is a `usage` array which has a `quantity` value and a corresponding `timeframe_start` and `timeframe_end`.  The `quantity` value represents the calculated usage value for the billable metric over the specified timeframe (inclusive of the `timeframe_start` timestamp and exclusive of the `timeframe_end` timestamp).
+        
+        Orb will include _every_ window in the response starting from the beginning of the billing period, even when there were no events (and therefore no usage) in the window. This increases the size of the response but prevents the caller from filling in gaps and handling cumbersome time-based logic.
+        
+        The query parameters in this endpoint serve to override this behavior and provide some key functionality, as listed below. Note that this functionality can also be used _in conjunction_ with each other, e.g. to display grouped usage on a custom timeframe.
+        
+        ## Custom timeframe
+        
+        In order to view usage for a custom timeframe rather than the current billing period, specify a `timeframe_start` and `timeframe_end`. This will calculate quantities for usage incurred between timeframe_start (inclusive) and timeframe_end (exclusive), i.e. `[timeframe_start, timeframe_end)`.
+        
+        Note:
+        - These timestamps must be specified in ISO 8601 format and UTC timezone, e.g. `2022-02-01T05:00:00Z`.
+        - Both parameters must be specified if either is specified.
+        
+        ## Grouping by custom attributes
+        In order to view a single metric grouped by a specific _attribute_ that each event is tagged with (e.g. `cluster`), you must additionally specify a `billable_metric_id` and a `group_by` key. The `group_by` key denotes the event property on which to group. 
+        
+        When returning grouped usage, only usage for `billable_metric_id` is  returned, and a separate object in the `data` array is returned for each value of the `group_by` key present in your events. The `quantity` value is the result of evaluating the billable metric for events filtered to a single value of the `group_by` key.
+        
+        Orb expects that events that match the billable metric will contain values in the `properties` dictionary that correspond to the `group_by` key specified. By default, Orb will not return a `null` group (i.e. events that match the metric but do not have the key set). Currently, it is only possible to view usage grouped by a single attribute at a time.
+        
+        The following example shows usage for an \"API Requests\" billable metric grouped by `region`. Note the extra `metric_group` dictionary in the response, which provides metadata about the group:
+        
+        ```json
+        {
+          \"data\": [
+            {
+              \"usage\": [
+                {
+                  \"quantity\": 0.19291,
+                  \"timeframe_start\": \"2021-10-01T07:00:00Z\",
+                  \"timeframe_end\": \"2021-10-02T07:00:00Z\",
+                },
+                ...
+              ],
+              “metric_group”: {
+                 “property_key”: “region”,
+                 “property_value”: “asia/pacific”
+              },
+              \"billable_metric\": {
+                \"id\": \"Fe9pbpMk86xpwdGB\",
+                \"name\": \"API Requests\"
+               },
+              \"view_mode\": \"periodic\"
+            },
+            ...
+          ]
+        }
+        ```
+        
+        ## Windowed usage
+        The `granularity` parameter can be used to _window_ the usage `quantity` value into periods. When not specified, usage is returned for the entirety of the time range. 
+        
+        When `granularity = day` is specified with a timeframe longer than a day, Orb will return a `quantity` value for each full day between `timeframe_start` and `timeframe_end`. Note that the days are demarcated by the _customer's local midnight_.
+        
+        For example, with `timeframe_start = 2022-02-01T05:00:00Z`, `timeframe_end = 2022-02-04T01:00:00Z` and `granularity=day`, the following windows will be returned for a customer in the `America/Los_Angeles` timezone since local midnight is `08:00` UTC:
+        - `[2022-02-01T05:00:00Z, 2022-02-01T08:00:00Z)`
+        - `[2022-02-01T08:00:00, 2022-02-02T08:00:00Z)`
+        - `[2022-02-02T08:00:00, 2022-02-03T08:00:00Z)`
+        - `[2022-02-03T08:00:00, 2022-02-04T01:00:00Z)`
+        
+        ```json
+        {
+            \"data\": [
+                {
+                    \"billable_metric\": {
+                        \"id\": \"Q8w89wjTtBdejXKsm\",
+                        \"name\": \"API Requests\"
+                    },
+                    \"usage\": [
+                        {
+                            \"quantity\": 0,
+                            \"timeframe_end\": \"2022-02-01T08:00:00+00:00\",
+                            \"timeframe_start\": \"2022-02-01T05:00:00+00:00\"
+                        },
+                        {
+                            \"quantity\": 0,
+                            \"timeframe_end\": \"2022-02-02T08:00:00+00:00\",
+                            \"timeframe_start\": \"2022-02-01T08:00:00+00:00\"
+                        },
+                        {
+                            \"quantity\": 0,
+                            \"timeframe_end\": \"2022-02-03T08:00:00+00:00\",
+                            \"timeframe_start\": \"2022-02-02T08:00:00+00:00\"
+                        },
+                        {
+                            \"quantity\": 0,
+                            \"timeframe_end\": \"2022-02-04T01:00:00+00:00\",
+                            \"timeframe_start\": \"2022-02-03T08:00:00+00:00\"
+                        }
+                    ],
+                    \"view_mode\": \"periodic\"
+                },
+                ...
+            ]
+        }
+        ```
+        
+        ## Decomposable vs. non-decomposable metrics
+        Billable metrics fall into one of two categories: decomposable and non-decomposable. A decomposable billable metric, such as a sum or a count, can be displayed and aggregated across arbitrary timescales. On the other hand, a non-decomposable metric is not meaningful when only a slice of the billing window is considered. 
+        
+        As an example, if we have a billable metric that's defined to count unique users, displaying a graph of unique users for each day is not representative of the billable metric value over the month (days could have an overlapping set of 'unique' users). Instead, what's useful for any given day is the number of unique users in the billing period so far, which are the _cumulative_ unique users.
+        
+        Accordingly, this endpoint returns treats these two types of metrics differently when `group_by` is specified:
+        - Decomposable metrics can be grouped by any event property.
+        - Non-decomposable metrics can only be grouped by the corresponding price's invoice grouping key. If no invoice grouping key is present, the metric does not support `group_by`.
+        
+        ## Matrix prices
+        When a billable metric is attached to a price that uses matrix pricing, it's important to view usage grouped by those matrix dimensions. In this case, use the query parameters `first_dimension_key`, `first_dimension_value` and `second_dimension_key`, `second_dimension_value` while filtering to a specific `billable_metric_id`. 
+        
+        For example, if your compute metric has a separate unit price (i.e. a matrix pricing model) per `region` and `provider`, your request might provide the following parameters:
+        
+        - `first_dimension_key`: `region`
+        - `first_dimension_value`: `us-east-1` 
+        - `second_dimension_key`: `provider`
+        - `second_dimension_value`: `aws`
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetSubscriptionsIDUsageRequest, base_url, '/subscriptions/{subscription_id}/usage', request)
+        
+        query_params = utils.get_query_params(operations.GetSubscriptionsIDUsageRequest, request)
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url, params=query_params)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetSubscriptionsIDUsageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+
+        return res
+
+    def get_subscriptions_subscription_id(self, request: operations.GetSubscriptionsSubscriptionIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSubscriptionsSubscriptionIDResponse:
+        r"""Retrieve a subscription
+        This endpoint is used to fetch a [Subscription](../reference/Orb-API.json/components/schemas/Subscription) given an identifier.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDRequest, base_url, '/subscriptions/{subscription_id}', request)
+        
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetSubscriptionsSubscriptionIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
+                res.subscription = out
+
+        return res
+
+    def get_subscriptions_subscription_id_schedule(self, request: operations.GetSubscriptionsSubscriptionIDScheduleRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSubscriptionsSubscriptionIDScheduleResponse:
+        r"""View subscription schedule
+        This endpoint returns a [paginated](../docs/Pagination.md) list of all plans associated with a subscription along with their start and end dates. This list contains the subscription's initial plan along with past and future plan changes.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDScheduleRequest, base_url, '/subscriptions/{subscription_id}/schedule', request)
+        
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('GET', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetSubscriptionsSubscriptionIDScheduleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSubscriptionsSubscriptionIDSchedule200ApplicationJSON])
+                res.get_subscriptions_subscription_id_schedule_200_application_json_object = out
+
+        return res
+
+    def post_subscriptions_subscription_id_cancel(self, request: operations.PostSubscriptionsSubscriptionIDCancelRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsSubscriptionIDCancelResponse:
         r"""Cancel subscription
         This endpoint can be used to cancel an existing subscription. It returns the serialized subscription object with an `end_date` parameter that signifies when the subscription will transition to an ended state.
         
         The body parameter `cancel_option` determines the cancellation behavior. Orb supports two cancellation options: 
         
         - `end_of_subscription_term`: stops the subscription from auto-renewing. Subscriptions that have been cancelled with this option can still incur charges for the remainder of their term:
             - Issuing this cancellation request for a monthly subscription will keep the subscription active until the start of the subsequent month, and potentially issue an invoice for any usage charges incurred in the intervening period.
             - Issuing this cancellation request for a quarterly subscription will keep the subscription active until the end of the quarter and potentially issue an invoice for any usage charges incurred in the intervening period.
             - Issuing this cancellation request for a yearly subscription will keep the subscription active for the full year. For example, a yearly subscription starting on 2021-11-01 and cancelled on 2021-12-08 will remain active until 2022-11-01 and potentially issue charges in the intervening months for any recurring monthly usage charges in its plan.
             - **Note**: If a subscription's plan contains prices with difference cadences, the end of term date will be determined by the largest cadence value. For example, cancelling end of term for a subscription with a quarterly fixed fee with a monthly usage fee will result in the subscription ending at the end of the quarter.
         
         - `immediate`: ends the subscription immediately, setting the `end_date` to the current time:
           - Subscriptions that have been cancelled with this option will be invoiced immediately. This invoice will include any usage fees incurred in the billing period up to the cancellation, along with any prorated recurring fees for the billing period, if applicable. 
           - **Note**: If the subscription has a recurring fee that was paid in-advance, the prorated amount for the remaining time period will be added to the [customer's balance](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1balance_transactions/get) upon immediate cancellation. However, if the customer is ineligible to use the customer balance, the subscription cannot be cancelled immediately.
+          
+        - `requested_date`: ends the subscription on a specified date, which requires a `cancellation_date` to be passed in. If no timezone is provided, the customer's timezone is used.  For example, a subscription starting on January 1st with a monthly price can be set to be cancelled on the first of any month after January 1st (e.g. March 1st, April 1st, May 1st). A subscription with multiple prices with different cadences defines the \"term\" to be the highest cadence of the prices.
         
         
         Upcoming subscriptions are only eligible for immediate cancellation, which will set the `end_date` equal to the `start_date` upon cancellation.
-        """
-        request = operations.PostSubscriptionsSubscriptionIDCancelRequest(
-            cancel_option=cancel_option,
-            subscription_id=subscription_id,
-        )
         
+        ## Backdated cancellations
+        Orb allows you to cancel a subscription in the past as long as there are no paid invoices between the `requested_date` and the current time. If the cancellation is after the latest issued invoice, Orb will generate a balance refund for the current period. If the cancellation is before the most recently issued invoice, Orb will void the intervening invoice and generate a new one based on the new dates for the subscription. See the section on [cancellation behaviors](../docs/Subscription-management.md#cancellation-behaviors).
+        """
         base_url = self._server_url
         
         url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDCancelRequest, base_url, '/subscriptions/{subscription_id}/cancel', request)
         
-        query_params = utils.get_query_params(operations.PostSubscriptionsSubscriptionIDCancelRequest, request)
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, params=query_params)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostSubscriptionsSubscriptionIDCancelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
                 res.subscription = out
 
         return res
 
-    
-    def change_schedule(self, subscription_id: str, request_body: Optional[operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeRequestBody] = None) -> operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeResponse:
+    def post_subscriptions_subscription_id_schedule_plan_change(self, request: operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeResponse:
         r"""Schedule plan change
         This endpoint can be used to change the plan on an existing subscription. It returns the serialized updated subscription object.
         
         The body parameter `change_option` determines the timing of the plan change. Orb supports three options: 
         
         - `end_of_subscription_term`: changes the plan at the end of the existing plan's term.
             - Issuing this plan change request for a monthly subscription will keep the existing plan active until the start of the subsequent month, and potentially issue an invoice for any usage charges incurred in the intervening period.
             - Issuing this plan change request for a yearly subscription will keep the existing plan active for the full year.
         
         - `immediate`: changes the plan immediately. Subscriptions that have their plan changed with this option will be invoiced immediately. This invoice will include any usage fees incurred in the billing period up to the change, along with any prorated recurring fees for the billing period, if applicable.
         
-        - `requested_date`: changes the plan on the requested date (`change_date`) at midnight in the customer's timezone. The `change_date` body parameter is required if this option is chosen.
+        - `requested_date`: changes the plan on the requested date (`change_date`). If no timezone is provided, the customer's timezone is used. The `change_date` body parameter is required if this option is chosen.
         
         Note that one of `plan_id` or `external_plan_id` is required in the request body for this operation.
         
         ## Price overrides and minimums
         Price overrides are used to update some or all prices in the target plan. Minimums, much like price overrides, can be useful when a new customer has negotiated a new or different minimum than the default for the plan. The request format for price overrides and minimums are the same as those in [subscription creation](Orb-API.json/paths/~1subscriptions/post).
         
         ## Prorations for in-advance fees
         By default, Orb calculates the prorated difference in any fixed fees when making a plan change, adjusting the customer balance as needed. For details on this behavior, [Subscription management](../docs/Subscription-management.md#prorations-for-in-advance-fees).
         """
-        request = operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeRequest(
-            subscription_id=subscription_id,
-            request_body=request_body,
-        )
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeRequest, base_url, '/subscriptions/{subscription_id}/schedule_plan_change', request)
         
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.PostSubscriptionsSubscriptionIDSchedulePlanChangeResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
                 res.subscription = out
 
         return res
 
-    
-    def create(self, request: operations.PostSubscriptionsRequestBody) -> operations.PostSubscriptionsResponse:
+    def post_subscriptions_subscription_id_unschedule_pending_cancellation(self, request: operations.PostSubscriptionsSubscriptionIDUnschedulePendingCancellationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsSubscriptionIDUnschedulePendingCancellationResponse:
+        r"""Unschedule pending cancellation
+        This endpoint can be used to unschedule any pending cancellations for a subscription. 
+        
+        To be eligible, the subscription must currently be active and have a future cancellation (\"Auto-renew turned off\"). This operation will turn on auto-renew, ensuring that the subscription does not end at the currently scheduled cancellation time.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDUnschedulePendingCancellationRequest, base_url, '/subscriptions/{subscription_id}/unschedule_cancellation', request)
+        
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostSubscriptionsSubscriptionIDUnschedulePendingCancellationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
+                res.subscription = out
+
+        return res
+
+    def post_subscriptions_subscription_id_unschedule_pending_plan_changes(self, request: operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse:
+        r"""Unschedule pending plan changes
+        This endpoint can be used to unschedule any pending plan changes on an existing subscription.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest, base_url, '/subscriptions/{subscription_id}/unschedule_pending_plan_changes', request)
+        
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
+                res.subscription = out
+
+        return res
+
+    def post_subscriptions_subscription_id_update_fixed_fee_quantity(self, request: operations.PostSubscriptionsSubscriptionIDUpdateFixedFeeQuantityRequest, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsSubscriptionIDUpdateFixedFeeQuantityResponse:
+        r"""Update fixed fee quantity
+        This endpoint can be used to update the quantity for a fixed fee.
+        
+        To be eligible, the subscription must currently be active and the price specified must be a fixed fee (not usage-based). This operation will immediately update the quantity for the fee, or if a `effective_date` is passed in, will update the quantity on the requested date at midnight in the customer's timezone. 
+        
+        If the fee is an in-advance fixed fee, it will also issue an immediate invoice for the difference for the remainder of the billing period.
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDUpdateFixedFeeQuantityRequest, base_url, '/subscriptions/{subscription_id}/update_fixed_fee_quantity', request)
+        
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        
+        client = self._security_client
+        
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.PostSubscriptionsSubscriptionIDUpdateFixedFeeQuantityResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
+                res.subscription = out
+
+        return res
+
+    def post_subscriptions_json(self, request: operations.PostSubscriptionsApplicationJSON, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsJSONResponse:
         r"""Create subscription
         A subscription represents the purchase of a plan by a customer. The customer is identified by either the `customer_id` or the `external_customer_id`, and exactly one of these fields must be provided.
         
         By default, subscriptions begin on the day that they're created and renew automatically for each billing cycle at the cadence that's configured in the plan definition.
         
         The default configuration for subscriptions in Orb is **In-advance billing** and **Beginning of month alignment** (see [Subscription](../reference/Orb-API.json/components/schemas/Subscription) for more details).
         
@@ -411,15 +833,15 @@
           \"amount_discount\": string, 
           \"percentage_discount\": string,
           \"usage_discount\": string
         }
         ```
         where either `amount_discount`, `percentage_discount`, or `usage_discount` is provided.
         
-        We only support `usage` type discounts on prices.
+        The `usage` type discount can only be created on individual prices and not on the plan.
         
         Price discount example
         ```json
         {
           ...
           \"id\": \"price_id\",
           \"model_type\": \"unit\",
@@ -472,305 +894,409 @@
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url, data=data, files=form, headers=headers)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.PostSubscriptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
-                res.subscription = out
-
-        return res
-
-    
-    def get(self, subscription_id: str) -> operations.GetSubscriptionsSubscriptionIDResponse:
-        r"""Retrieve a subscription
-        This endpoint is used to fetch a [Subscription](../reference/Orb-API.json/components/schemas/Subscription) given an identifier.
-        """
-        request = operations.GetSubscriptionsSubscriptionIDRequest(
-            subscription_id=subscription_id,
-        )
-        
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDRequest, base_url, '/subscriptions/{subscription_id}', request)
-        
-        
-        client = self._security_client
-        
-        http_res = client.request('GET', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetSubscriptionsSubscriptionIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostSubscriptionsJSONResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
                 res.subscription = out
 
         return res
 
-    
-    def get_cost(self, request: operations.GetSubscriptionsSubscriptionIDCostRequest) -> operations.GetSubscriptionsSubscriptionIDCostResponse:
-        r"""View subscription costs
-        This endpoint is used to fetch a day-by-day snapshot of a subscription's costs in Orb, calculated by applying pricing information to the underlying usage (see the [subscription usage endpoint](../reference/Orb-API.json/paths/~1subscriptions~1{subscription_id}~1usage/get) to fetch usage per metric, in usage units rather than a currency). 
-        
-        
-        The semantics of this endpoint exactly mirror those of [fetching a customer's costs](../reference/Orb-API.json/paths/~1customers~1{customer_id}~1costs/get). Use this endpoint to limit your analysis of costs to a specific subscription for the customer (e.g. to de-aggregate costs when a customer's subscription has started and stopped on the same day).
-        """
-        base_url = self._server_url
-        
-        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDCostRequest, base_url, '/subscriptions/{subscription_id}/costs', request)
+    def post_subscriptions_raw(self, request: bytes, retries: Optional[utils.RetryConfig] = None) -> operations.PostSubscriptionsRawResponse:
+        r"""Create subscription
+        A subscription represents the purchase of a plan by a customer. The customer is identified by either the `customer_id` or the `external_customer_id`, and exactly one of these fields must be provided.
         
-        query_params = utils.get_query_params(operations.GetSubscriptionsSubscriptionIDCostRequest, request)
+        By default, subscriptions begin on the day that they're created and renew automatically for each billing cycle at the cadence that's configured in the plan definition.
         
-        client = self._security_client
+        The default configuration for subscriptions in Orb is **In-advance billing** and **Beginning of month alignment** (see [Subscription](../reference/Orb-API.json/components/schemas/Subscription) for more details).
         
-        http_res = client.request('GET', url, params=query_params)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetSubscriptionsSubscriptionIDCostResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        In order to change the alignment behavior, Orb also supports billing subscriptions on the day of the month they are created. If `align_billing_with_subscription_start_date = true` is specified, subscriptions have billing cycles that are aligned with their `start_date`. For example, a subscription that begins on January 15th will have a billing cycle from January 15th to February 15th. Every subsequent billing cycle will continue to start and invoice on the 15th.
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSubscriptionsSubscriptionIDCost200ApplicationJSON])
-                res.get_subscriptions_subscription_id_cost_200_application_json_object = out
-
-        return res
-
-    
-    def get_schedule(self, subscription_id: str) -> operations.GetSubscriptionsSubscriptionIDScheduleResponse:
-        r"""View subscription schedule
-        This endpoint returns a [paginated](../docs/Pagination.md) list of all plans associated with a subscription along with their start and end dates. This list contains the subscription's initial plan along with past and future plan changes.
-        """
-        request = operations.GetSubscriptionsSubscriptionIDScheduleRequest(
-            subscription_id=subscription_id,
-        )
+        If the \"day\" value is greater than the number of days in the month, the next billing cycle will start at the end of the month. For example, if the start_date is January 31st, the next billing cycle will start on February 28th.
         
-        base_url = self._server_url
+        If a customer was created with a currency, Orb only allows subscribing the customer to a plan with a matching `invoicing_currency`. If the customer does not have a currency set, on subscription creation, we set the customer's currency to be the `invoicing_currency` of the plan.
         
-        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDScheduleRequest, base_url, '/subscriptions/{subscription_id}/schedule', request)
+        ## Price overrides
         
+        Price overrides are used to update some or all prices in a plan for the specific subscription being created. This is useful when a new customer has negotiated one or more different prices for a specific plan than the plan's default prices. Any type of price can be overridden, if the correct data is provided. The billable metric, cadence, type, and name of a price can not be overridden.
         
-        client = self._security_client
         
-        http_res = client.request('GET', url)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetSubscriptionsSubscriptionIDScheduleResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        To override prices, provide a list of objects with the key `price_overrides`. The price object in the list of overrides is expected to contain the existing price id, the `model_type` and config value in the format below. The specific numerical values can be updated, but the config value and `model_type` must match the existing price that is being overridden
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetSubscriptionsSubscriptionIDSchedule200ApplicationJSON])
-                res.get_subscriptions_subscription_id_schedule_200_application_json_object = out
-
-        return res
-
-    
-    def get_usage(self, request: operations.GetSubscriptionsSubscriptionIDUsageRequest) -> operations.GetSubscriptionsSubscriptionIDUsageResponse:
-        r"""View subscription usage
-        This endpoint is used to fetch a subscription's usage in Orb. Especially when combined with optional query parameters, this endpoint is a powerful way to build visualizations on top of Orb's event data and metrics.
+        ### Request format for price overrides
         
-        With no query parameters specified, this endpoint returns usage for the subscription's _current billing period_ across each billable metric that participates in the subscription. Usage quantities returned are the result of evaluating the metric definition for the entirety of the customer's billing period.
+        Orb supports a few different pricing models out of the box. The `model_type` field determines the key for the configuration object that is present.
         
-        ### Default response shape
+        ### Unit pricing
         
-        Orb returns a `data` array with an object corresponding to each billable metric. Nested within this object is a `usage` array which has a `quantity` value and a corresponding `timeframe_start` and `timeframe_end`.  The `quantity` value represents the calculated usage value for the billable metric over the specified timeframe (inclusive of the `timeframe_start` timestamp and exclusive of the `timeframe_end` timestamp).
+        With unit pricing, each unit costs a fixed amount.
         
-        Orb will include _every_ window in the response starting from the beginning of the billing period, even when there were no events (and therefore no usage) in the window. This increases the size of the response but prevents the caller from filling in gaps and handling cumbersome time-based logic.
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+               \"unit_amount\": \"0.50\"
+            }
+            ...
+        }
+        ```
         
-        The query parameters in this endpoint serve to override this behavior and provide some key functionality, as listed below. Note that this functionality can also be used _in conjunction_ with each other, e.g. to display grouped usage on a custom timeframe.
+        ### Tiered pricing
         
-        ## Custom timeframe
+        In tiered pricing, the cost of a given unit depends on the tier range that it falls into, where each tier range is defined by an upper and lower bound. For example, the first ten units may cost $0.50 each and all units thereafter may cost $0.10 each. Tiered prices can be overridden with a new number of tiers or new values for `first_unit`, `last_unit`, or `unit_amount`.
         
-        In order to view usage for a custom timeframe rather than the current billing period, specify a `timeframe_start` and `timeframe_end`. This will calculate quantities for usage incurred between timeframe_start (inclusive) and timeframe_end (exclusive), i.e. `[timeframe_start, timeframe_end)`.
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"tiered\",
+            \"tiered_config\": {
+                \"tiers\": [ 
+                   {
+                        \"first_unit\":\"1\",
+                        \"last_unit\": \"10\",
+                        \"unit_amount\": \"0.50\"
+                    },
+                    {
+                        \"first_unit\": \"10\",
+                        \"last_unit\": null,
+                        \"unit_amount\": \"0.10\"
+                    }
+                ]
+            }
+            ...
+        }
+        ```
         
-        Note:
-        - These timestamps must be specified in ISO 8601 format and UTC timezone, e.g. `2022-02-01T05:00:00Z`.
-        - Both parameters must be specified if either is specified.
+        ### Bulk pricing
         
-        ## Grouping by custom attributes
-        In order to view a single metric grouped by a specific _attribute_ that each event is tagged with (e.g. `cluster`), you must additionally specify a `billable_metric_id` and a `group_by` key. The `group_by` key denotes the event property on which to group. 
+        Bulk pricing applies when the number of units determine the cost of _all_ units. For example, if you've bought less than 10 units, they may each be $0.50 for a total of $5.00. Once you've bought more than 10 units, all units may now be priced at $0.40 (i.e. 101 units total would be $40.40). Bulk prices can be overridden with a new number of tiers or new values for `maximum_units`, or `unit_amount`.
         
-        When returning grouped usage, only usage for `billable_metric_id` is  returned, and a separate object in the `data` array is returned for each value of the `group_by` key present in your events. The `quantity` value is the result of evaluating the billable metric for events filtered to a single value of the `group_by` key.
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"bulk\",
+            \"bulk_config\": {
+                \"tiers\": [ 
+                    {
+                        \"maximum_units\": \"10\",
+                        \"unit_amount\": \"0.50\"
+                    },
+                    {
+                        \"maximum_units\": \"1000\",
+                        \"unit_amount\": \"0.40\"
+                    }
+                  ]
+            }
+            ...
+        }
+        ```
+        ### Package pricing
         
-        Orb expects that events that match the billable metric will contain values in the `properties` dictionary that correspond to the `group_by` key specified. By default, Orb will not return a `null` group (i.e. events that match the metric but do not have the key set). Currently, it is only possible to view usage grouped by a single attribute at a time.
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"package\",
+            \"package_config\": {
+               \"package_amount\": \"0.80\",
+               \"package_size\": 10
+            }
+            ...
+         }
+         ```
+        ### BPS pricing
         
-        The following example shows usage for an \"API Requests\" billable metric grouped by `region`. Note the extra `metric_group` dictionary in the response, which provides metadata about the group:
+        BPS pricing specifies a per-event (e.g. per-payment) rate in one hundredth of a percent (the number of basis points to charge), as well as a cap per event to assess. For example, this would allow you to assess a fee of 0.25% on every payment you process, with a maximum charge of $25 per payment.
         
         ```json
         {
-          \"data\": [
-            {
-              \"usage\": [
-                {
-                  \"quantity\": 0.19291,
-                  \"timeframe_start\": \"2021-10-01T07:00:00Z\",
-                  \"timeframe_end\": \"2021-10-02T07:00:00Z\",
-                },
-                ...
-              ],
-              “metric_group”: {
-                 “property_key”: “region”,
-                 “property_value”: “asia/pacific”
-              },
-              \"billable_metric\": {
-                \"id\": \"Fe9pbpMk86xpwdGB\",
-                \"name\": \"API Requests\"
-               },
-              \"view_mode\": \"periodic\"
-            },
             ...
-          ]
-        }
+            \"id\": \"price_id\"
+            \"model_type\": \"bps\",
+            \"bps_config\": {
+               \"bps\": 125,
+               \"per_event_cap\": \"11.00\"
+            }
+            ...
+         }
         ```
+        ### Bulk BPS pricing
         
-        ## Windowed usage
-        The `granularity` parameter can be used to _window_ the usage `quantity` value into periods. When not specified, usage is returned for the entirety of the time range. 
-        
-        When `granularity = day` is specified with a timeframe longer than a day, Orb will return a `quantity` value for each full day between `timeframe_start` and `timeframe_end`. Note that the days are demarcated by the _customer's local midnight_.
+        Bulk BPS pricing specifies BPS parameters in a tiered manner, dependent on the total quantity across all events. Similar to bulk pricing, the BPS parameters of a given event depends on the tier range that the billing period falls into. Each tier range is defined by an upper and lower bound. For example, after $1.5M of payment volume is reached, each individual payment may have a lower cap or a smaller take-rate.
         
-        For example, with `timeframe_start = 2022-02-01T05:00:00Z`, `timeframe_end = 2022-02-04T01:00:00Z` and `granularity=day`, the following windows will be returned for a customer in the `America/Los_Angeles` timezone since local midnight is `08:00` UTC:
-        - `[2022-02-01T05:00:00Z, 2022-02-01T08:00:00Z)`
-        - `[2022-02-01T08:00:00, 2022-02-02T08:00:00Z)`
-        - `[2022-02-02T08:00:00, 2022-02-03T08:00:00Z)`
-        - `[2022-02-03T08:00:00, 2022-02-04T01:00:00Z)`
+        ```json
+        {
+            ...
+            \"id\": \"price_id\"
+            \"model_type\": \"bulk_bps\",
+            \"bulk_bps_config\": {
+                \"tiers\": [ 
+                   {
+                        \"minimum_amount\": \"0.00\",
+                        \"maximum_amount\": \"1000000.00\",
+                        \"bps\": 125,
+                        \"per_event_cap\": \"19.00\"
+                   },
+                  {
+                        \"minimum_amount\":\"1000000.00\",
+                        \"maximum_amount\": null,
+                        \"bps\": 115,
+                        \"per_event_cap\": \"4.00\"
+                    }
+                ]
+            }
+            ...
+         }
+        ```
+        ### Tiered BPS pricing
+        Tiered BPS pricing specifies BPS parameters in a graduated manner, where an event's applicable parameter is a function of its marginal addition to the period total. Similar to tiered pricing, the BPS parameters of a given event depends on the tier range that it falls into, where each tier range is defined by an upper and lower bound. For example, the first few payments may have a 0.8 BPS take-rate and all payments after a specific volume may incur a take-rate of 0.5 BPS each.
         
         ```json
         {
-            \"data\": [
+            ...
+            \"id\": \"price_id\"
+            \"model_type\": \"tiered_bps\",
+            \"tiered_bps_config\": {
+                \"tiers\": [ 
+                   {
+                        \"minimum_amount\": \"0.00\",
+                        \"maximum_amount\": \"1000000.00\",
+                        \"bps\": 125,
+                        \"per_event_cap\": \"19.00\"
+                   },
+                  {
+                        \"minimum_amount\":\"1000000\",
+                        \"maximum_amount\": null,
+                        \"bps\": 115,
+                        \"per_event_cap\": \"4.00\"
+                    }
+                ]
+            }
+            ...
+         }
+        ```
+        ### Matrix pricing
+        Matrix pricing defines a set of unit prices in a one or two-dimensional matrix. `dimensions` defines the two event property values evaluated in this pricing model. In a one-dimensional matrix, the second value is `null`. Every configuration has a list of `matrix_values` which give the unit prices for specified property values. In a one-dimensional matrix, the matrix values will have `dimension_values` where the second value of the pair is null. If an event does not match any of the dimension values in the matrix, it will resort to the `default_unit_amount`.
+        ```json
+        ...
+        \"model_type\": \"matrix\"
+        \"matrix_config\": {
+            \"default_unit_amount\": \"3.00\",
+            \"dimensions\": [
+                \"cluster_name\",
+                \"region\"
+            ],
+            \"matrix_values\": [
                 {
-                    \"billable_metric\": {
-                        \"id\": \"Q8w89wjTtBdejXKsm\",
-                        \"name\": \"API Requests\"
-                    },
-                    \"usage\": [
-                        {
-                            \"quantity\": 0,
-                            \"timeframe_end\": \"2022-02-01T08:00:00+00:00\",
-                            \"timeframe_start\": \"2022-02-01T05:00:00+00:00\"
-                        },
-                        {
-                            \"quantity\": 0,
-                            \"timeframe_end\": \"2022-02-02T08:00:00+00:00\",
-                            \"timeframe_start\": \"2022-02-01T08:00:00+00:00\"
-                        },
-                        {
-                            \"quantity\": 0,
-                            \"timeframe_end\": \"2022-02-03T08:00:00+00:00\",
-                            \"timeframe_start\": \"2022-02-02T08:00:00+00:00\"
-                        },
-                        {
-                            \"quantity\": 0,
-                            \"timeframe_end\": \"2022-02-04T01:00:00+00:00\",
-                            \"timeframe_start\": \"2022-02-03T08:00:00+00:00\"
-                        }
+                    \"dimension_values\": [
+                        \"alpha\",
+                        \"west\"
                     ],
-                    \"view_mode\": \"periodic\"
+                    \"unit_amount\": \"2.00\"
                 },
                 ...
             ]
         }
+        ...
         ```
         
-        ## Decomposable vs. non-decomposable metrics
-        Billable metrics fall into one of two categories: decomposable and non-decomposable. A decomposable billable metric, such as a sum or a count, can be displayed and aggregated across arbitrary timescales. On the other hand, a non-decomposable metric is not meaningful when only a slice of the billing window is considered. 
+        ### Fixed fees
+        Fixed fees follow unit pricing, and also have an additional parameter `fixed_price_quantity` that indicates how many of a fixed fee that should be applied for a subscription. This parameter defaults to 1. 
         
-        As an example, if we have a billable metric that's defined to count unique users, displaying a graph of unique users for each day is not representative of the billable metric value over the month (days could have an overlapping set of 'unique' users). Instead, what's useful for any given day is the number of unique users in the billing period so far, which are the _cumulative_ unique users.
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+               \"unit_amount\": \"2.00\"
+            },
+            \"fixed_price_quantity\": 3.0
+            ...
+        }
+        ```
         
-        Accordingly, this endpoint returns treats these two types of metrics differently and specifies the type in the `view_mode` return field:
-        - Decomposable metrics will return _periodic_ totals, which means that the `quantity` value between `timeframe_start` and `timeframe_end` is the usage incurred only within that timeframe.
-        - Non-decomposable metrics will return _cumulative_ totals. The `quantity` value between `timeframe_start` and `timeframe_end` represents the new _cumulative_ total since the beginning of the billing period.
+        ## Minimums
+        Minimums, much like price overrides, can be useful when a new customer has negotiated a new or different minimum than the default for the plan. Minimums can be added to either a price or a plan. If a minimum exists for a price or plan and null is provided for the minimum override on creation, then there will be no minimum on the new subscription. If no minimum is provided, then the default plan minimum is used.
         
+        To add a minimum for a specific price, add `minimum_amount` to the specific price in the `price_overrides` object. To add a minimum to a plan, add `minimum_amount` to the base object. The value for `minimum_amount` should be a string with the minimum dollar amount in decimal format.
         
-        ## Matrix prices
-        When a billable metric is attached to a price that uses matrix pricing, it's important to view usage grouped by those matrix dimensions. In this case, use the query parameters `first_dimension_key`, `first_dimension_value` and `second_dimension_key`, `second_dimension_value` while filtering to a specific `billable_metric_id`. 
         
-        For example, if your compute metric has a separate unit price (i.e. a matrix pricing model) per `region` and `provider`, your request might provide the following parameters:
+        ### Minimum override example
         
-        - `first_dimension_key`: `region`
-        - `first_dimension_value`: `us-east-1` 
-        - `second_dimension_key`: `provider`
-        - `second_dimension_value`: `aws`
-        """
-        base_url = self._server_url
+        Price minimum override example:
         
-        url = utils.generate_url(operations.GetSubscriptionsSubscriptionIDUsageRequest, base_url, '/subscriptions/{subscription_id}/usage', request)
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+                \"unit_amount\": \"0.50\"
+            },
+            \"minimum_amount\": \"100.00\"
+            ...
+        }
+        ```
         
-        query_params = utils.get_query_params(operations.GetSubscriptionsSubscriptionIDUsageRequest, request)
         
-        client = self._security_client
+        Plan minimum override example:
         
-        http_res = client.request('GET', url, params=query_params)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.GetSubscriptionsSubscriptionIDUsageResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        ```json
+        {
+            \"customer_id\": \"customer_id\",
+            \"plan_id\": \"plan_id\",
+            \"minimum_amount\": \"1000.00\",
+            \"price_overrides\": [ ... ]
+            ...
+        }
+        ```
         
-
-        return res
-
-    
-    def list(self, customer_id: Optional[str] = None, external_customer_id: Optional[str] = None) -> operations.ListSubscriptionsResponse:
-        r"""List subscriptions
-        This endpoint returns a list of all subscriptions for an account as a [paginated](../docs/Pagination.md) list, ordered starting from the most recently created subscription. For a full discussion of the subscription resource, see [Subscription](../reference/Orb-API.json/components/schemas/Subscription).
+        Removing an existing minimum example
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+                \"unit_amount\": \"0.50\"
+            },
+            \"minimum_amount\": null
+            ...
+        }
+        ```
         
-        Subscriptions can be filtered to a single customer by passing in the `customer_id` query parameter or the `external_customer_id` query parameter.
-        """
-        request = operations.ListSubscriptionsRequest(
-            customer_id=customer_id,
-            external_customer_id=external_customer_id,
-        )
+        Using the plan's minimum example
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+                \"unit_amount\": \"0.50\"
+            },
+            ...
+        }
+        ```
         
-        base_url = self._server_url
+        ## Discounts
+        Discounts, like price overrides, can be useful when a new customer has negotiated a new or custom discount than the default for the plan. Discounts can be added to either a price or a plan, and a single plan or price can have at most one discount. If a discount exists for a price or a plan and a null discount is provided on creation, then there will be no discount on the new subscription.
         
-        url = base_url.removesuffix('/') + '/subscriptions'
+        To add a discount for a specific price, add `discount_override` to the price in the `price_overrides` object. To add a discount to a plan, add `discount_override` to the base object. 
+        Discount should be a dictionary of the format:
+        ```json
+        {
+          \"discount_type\": \"amount\" | \"percentage\" | \"usage\", 
+          \"amount_discount\": string, 
+          \"percentage_discount\": string,
+          \"usage_discount\": string
+        }
+        ```
+        where either `amount_discount`, `percentage_discount`, or `usage_discount` is provided.
         
-        query_params = utils.get_query_params(operations.ListSubscriptionsRequest, request)
+        The `usage` type discount can only be created on individual prices and not on the plan.
         
-        client = self._security_client
+        Price discount example
+        ```json
+        {
+          ...
+          \"id\": \"price_id\",
+          \"model_type\": \"unit\",
+          \"unit_config\": {
+              \"unit_amount\": \"0.50\"
+          },
+          \"discount\": {\"discount_type\": \"amount\", \"amount_discount\": \"175\"},
+        }
+        ```
         
-        http_res = client.request('GET', url, params=query_params)
-        content_type = http_res.headers.get('Content-Type')
-
-        res = operations.ListSubscriptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        Plan discount example
+        ```json
+        {
+            \"customer_id\": \"customer_id\",
+            \"plan_id\": \"plan_id\",
+            \"discount\": {\"discount_type\": \"percentage\", \"percentage_discount\": \"12.5\"},
+            \"price_overrides\": [ ... ]
+            ...
+        }
+        ```
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListSubscriptions200ApplicationJSON])
-                res.list_subscriptions_200_application_json_object = out
-
-        return res
-
-    
-    def unschedule(self, subscription_id: str) -> operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse:
-        r"""Unschedule pending plan changes
-        This endpoint can be used to unschedule any pending plan changes on an existing subscription.
-        """
-        request = operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest(
-            subscription_id=subscription_id,
-        )
+        Removing an existing discount example
+        ```json
+        {
+            \"customer_id\": \"customer_id\",
+            \"plan_id\": \"plan_id\",
+            \"discount\": null,
+            \"price_overrides\": [ ... ]
+            ...
+        }
+        ```
         
+        Using the plan's discount example
+        ```json
+        {
+            ...
+            \"id\": \"price_id\",
+            \"model_type\": \"unit\",
+            \"unit_config\": {
+                \"unit_amount\": \"0.50\"
+            },
+            ...
+        }
+        ```
+        """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesRequest, base_url, '/subscriptions/{subscription_id}/unschedule_pending_plan_changes', request)
+        url = base_url.removesuffix('/') + '/subscriptions'
         
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "request", 'raw')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         
         client = self._security_client
         
-        http_res = client.request('POST', url)
+        retry_config = retries
+        if retry_config is None:
+            retry_config = utils.RetryConfig('backoff', True)
+            retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
+            
+
+        def do_request():
+            return client.request('POST', url, data=data, files=form, headers=headers)
+        
+        http_res = utils.retry(do_request, utils.Retries(retry_config, [
+            '5XX'
+        ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostSubscriptionsSubscriptionIDUnschedulePendingPlanChangesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.PostSubscriptionsRawResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Subscription])
                 res.subscription = out
 
         return res
```

### Comparing `orb-billing-0.9.3/src/orb/utils/retries.py` & `orb-billing-1.2.0/src/orb/utils/retries.py`

 * *Files identical despite different names*

### Comparing `orb-billing-0.9.3/src/orb/utils/utils.py` & `orb-billing-1.2.0/src/orb/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,91 +137,81 @@
         if field_name == 'password':
             password = value
 
     data = f'{username}:{password}'.encode()
     client.client.headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass,
-                 gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
+def generate_url(clazz: type, server_url: str, path: str, path_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> str:
     path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        if param_metadata.get('style', 'simple') == 'simple':
+            param = getattr(
+                path_params, field.name) if path_params is not None else None
+            param = _populate_from_globals(
+                field.name, param, 'pathParam', gbls)
+
+            if param is None:
+                continue
 
-        if param is None:
-            continue
+            if isinstance(param, list):
+                pp_vals: list[str] = []
+                for pp_val in param:
+                    if pp_val is None:
+                        continue
+                    pp_vals.append(_val_to_string(pp_val))
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif isinstance(param, dict):
+                pp_vals: list[str] = []
+                for pp_key in param:
+                    if param[pp_key] is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{pp_key}={_val_to_string(param[pp_key])}")
+                    else:
+                        pp_vals.append(
+                            f"{pp_key},{_val_to_string(param[pp_key])}")
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            elif not isinstance(param, (str, int, float, complex, bool)):
+                pp_vals: list[str] = []
+                param_fields: Tuple[Field, ...] = fields(param)
+                for param_field in param_fields:
+                    param_value_metadata = param_field.metadata.get(
+                        'path_param')
+                    if not param_value_metadata:
+                        continue
 
-        f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
-            serialized_params = _get_serialized_params(
-                param_metadata, f_name, param)
-            for key, value in serialized_params.items():
+                    parm_name = param_value_metadata.get(
+                        'field_name', field.name)
+
+                    param_field_val = getattr(param, param_field.name)
+                    if param_field_val is None:
+                        continue
+                    if param_metadata.get('explode'):
+                        pp_vals.append(
+                            f"{parm_name}={_val_to_string(param_field_val)}")
+                    else:
+                        pp_vals.append(
+                            f"{parm_name},{_val_to_string(param_field_val)}")
                 path = path.replace(
-                    '{' + key + '}', value, 1)
-        else:
-            if param_metadata.get('style', 'simple') == 'simple':
-                if isinstance(param, list):
-                    pp_vals: list[str] = []
-                    for pp_val in param:
-                        if pp_val is None:
-                            continue
-                        pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif isinstance(param, dict):
-                    pp_vals: list[str] = []
-                    for pp_key in param:
-                        if param[pp_key] is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
-                        else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                elif not isinstance(param, (str, int, float, complex, bool)):
-                    pp_vals: list[str] = []
-                    param_fields: Tuple[Field, ...] = fields(param)
-                    for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
-                        if not param_value_metadata:
-                            continue
-
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
-
-                        param_field_val = getattr(param, param_field.name)
-                        if param_field_val is None:
-                            continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
-                        else:
-                            pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-                else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+            else:
+                path = path.replace(
+                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -230,16 +220,15 @@
     for key, value in params.items():
         url_with_params = url_with_params.replace(
             '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[
-    str, list[str]]:
+def get_query_params(clazz: type, query_params: dataclass, gbls: dict[str, dict[str, dict[str, Any]]] = None) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
         request_metadata = field.metadata.get('request')
         if request_metadata is not None:
             continue
@@ -253,31 +242,24 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            serialized_parms = _get_serialized_params(metadata, f_name, value)
-            for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
-                else:
-                    params[key] = [value]
+            params = params | _get_serialized_query_params(
+                metadata, f_name, value)
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, ",")
-            elif style == 'pipeDelimited':
-                params = params | _get_delimited_query_params(
-                    metadata, f_name, value, "|")
+                params = params | _get_form_query_params(
+                    metadata, f_name, value)
             else:
                 raise Exception('not yet implemented')
     return params
 
 
 def get_headers(headers_params: dataclass) -> dict[str, str]:
     if headers_params is None:
@@ -296,16 +278,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
-    params: dict[str, str] = {}
+def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    params: dict[str, list[str]] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
 
@@ -328,23 +310,20 @@
                 continue
 
             if isinstance(obj_val, list):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
-                        params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    if params.get(f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                         ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(_val_to_string(val))
             else:
                 params[
                     f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
                     _val_to_string(obj_val)]
     elif isinstance(obj, dict):
         for key, value in obj.items():
             if value is None:
@@ -372,52 +351,48 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: dict, field_name: str, obj: any, array_delimiter: str) -> dict[
-    str, list[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, array_delimiter)
+def _get_form_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
+    'json':      'application/json',
+    'form':      'application/x-www-form-urlencoded',
     'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    'raw':       'application/octet-stream',
+    'string':    'text/plain',
 }
 
 
-def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[
-    str, any, any]:
+def serialize_request_body(request: dataclass, request_field_name: str, serialization_method: str) -> Tuple[str, any, any]:
     if request is None:
         return None, None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request)
+        return serialize_content_type(request_field_name, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method], request)
 
     request_val = getattr(request, request_field_name)
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
             request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
         raise Exception('invalid request type')
 
-    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(request_field_name, request_metadata.get('media_type', 'application/octet-stream'), request_val)
 
 
 def serialize_content_type(field_name: str, media_type: str, request: dataclass) -> Tuple[str, any, list[list[any]]]:
     if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request), None
     if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
@@ -482,15 +457,15 @@
                         [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
 def serialize_dict(original: dict, explode: bool, field_name, existing: Optional[dict[str, list[str]]]) -> dict[
-    str, list[str]]:
+        str, list[str]]:
     if existing is None:
         existing = []
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -522,15 +497,15 @@
             field_name = metadata.get('field_name', field.name)
 
             if metadata.get('json'):
                 form[field_name] = [marshal_json(val)]
             else:
                 if metadata.get('style', 'form') == 'form':
                     form = form | _populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")
+                        field_name, metadata.get('explode', True), val, _get_form_field_name)
                 else:
                     raise Exception(
                         f'Invalid form style for field {field.name}')
     elif isinstance(data, dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
@@ -544,16 +519,15 @@
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable, array_delimiter: str) -> \
-        dict[str, list[str]]:
+def _populate_form(field_name: str, explode: boolean, obj: any, get_field_name_func: Callable) -> dict[str, list[str]]:
     params: dict[str, list[str]] = {}
 
     if obj is None:
         return params
 
     if is_dataclass(obj):
         items = []
@@ -600,15 +574,15 @@
                 if not field_name in params:
                     params[field_name] = []
                 params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [array_delimiter.join([str(item) for item in items])]
+            params[field_name] = [','.join([str(item) for item in items])]
     else:
         params[field_name] = [_val_to_string(obj)]
 
     return params
 
 
 def _serialize_header(explode: bool, obj: any) -> str:
@@ -740,15 +714,15 @@
 
 def _val_to_string(val):
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
         return val.isoformat().replace('+00:00', 'Z')
     if isinstance(val, Enum):
-        return str(val.value)
+        return val.value
 
     return str(val)
 
 
 def _populate_from_globals(param_name: str, value: any, param_type: str, gbls: dict[str, dict[str, dict[str, Any]]]):
     if value is None and gbls is not None:
         if 'parameters' in gbls:
```

### Comparing `orb-billing-0.9.3/src/orb_billing.egg-info/SOURCES.txt` & `orb-billing-1.2.0/src/orb_billing.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,81 @@
 LICENSE.md
 README.md
 setup.py
 src/orb/__init__.py
 src/orb/availability.py
+src/orb/coupon.py
 src/orb/credits.py
 src/orb/customer.py
 src/orb/event.py
 src/orb/invoice.py
 src/orb/plan.py
 src/orb/sdk.py
 src/orb/subscription.py
 src/orb/models/__init__.py
 src/orb/models/operations/__init__.py
+src/orb/models/operations/amend_event.py
+src/orb/models/operations/delete_customers_customer_id.py
+src/orb/models/operations/deprecate_event.py
+src/orb/models/operations/get_coupons.py
+src/orb/models/operations/get_coupons_coupon_id.py
 src/orb/models/operations/get_customer_costs.py
+src/orb/models/operations/get_customer_costs_by_external_customer_id.py
+src/orb/models/operations/get_customers.py
 src/orb/models/operations/get_customers_customer_id.py
 src/orb/models/operations/get_customers_customer_id_balance_transactions.py
 src/orb/models/operations/get_customers_customer_id_credits.py
 src/orb/models/operations/get_customers_customer_id_credits_ledger.py
 src/orb/models/operations/get_customers_external_customer_id_external_customer_id.py
-src/orb/models/operations/get_external_customer_costs.py
 src/orb/models/operations/get_invoice_invoice_id.py
+src/orb/models/operations/get_invoices.py
 src/orb/models/operations/get_invoices_upcoming.py
 src/orb/models/operations/get_ping.py
+src/orb/models/operations/get_plans.py
 src/orb/models/operations/get_plans_external_plan_id.py
 src/orb/models/operations/get_plans_plan_id.py
+src/orb/models/operations/get_subscription_id_usage_by_customer.py
+src/orb/models/operations/get_subscriptions.py
+src/orb/models/operations/get_subscriptions_by_coupon.py
+src/orb/models/operations/get_subscriptions_id_usage.py
 src/orb/models/operations/get_subscriptions_subscription_id.py
-src/orb/models/operations/get_subscriptions_subscription_id_cost.py
 src/orb/models/operations/get_subscriptions_subscription_id_schedule.py
-src/orb/models/operations/get_subscriptions_subscription_id_usage.py
-src/orb/models/operations/list_customers.py
-src/orb/models/operations/list_invoices.py
-src/orb/models/operations/list_plans.py
-src/orb/models/operations/list_subscriptions.py
 src/orb/models/operations/patch_customers_customer_id_usage.py
-src/orb/models/operations/patch_external_customers_customer_id_usage.py
+src/orb/models/operations/patch_customers_external_customer_id_usage.py
+src/orb/models/operations/post_coupons.py
+src/orb/models/operations/post_coupons_coupon_id_archive.py
 src/orb/models/operations/post_customers.py
+src/orb/models/operations/post_customers_customer_id_balance_transactions.py
 src/orb/models/operations/post_customers_customer_id_credits_ledger_entry.py
 src/orb/models/operations/post_events_search.py
 src/orb/models/operations/post_ingest.py
-src/orb/models/operations/post_subscriptions.py
+src/orb/models/operations/post_invoice_line_items.py
+src/orb/models/operations/post_invoices_invoice_id_void.py
+src/orb/models/operations/post_subscriptions_json.py
+src/orb/models/operations/post_subscriptions_raw.py
 src/orb/models/operations/post_subscriptions_subscription_id_cancel.py
 src/orb/models/operations/post_subscriptions_subscription_id_schedule_plan_change.py
+src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_cancellation.py
 src/orb/models/operations/post_subscriptions_subscription_id_unschedule_pending_plan_changes.py
+src/orb/models/operations/post_subscriptions_subscription_id_update_fixed_fee_quantity.py
 src/orb/models/operations/put_customers_customer_id.py
 src/orb/models/operations/put_customers_external_customer_id_external_customer_id.py
-src/orb/models/operations/put_deprecate_events_event_id.py
-src/orb/models/operations/put_events_event_id.py
 src/orb/models/shared/__init__.py
-src/orb/models/shared/billingaddress.py
+src/orb/models/shared/coupon.py
 src/orb/models/shared/credit_ledger_entry.py
 src/orb/models/shared/customer.py
 src/orb/models/shared/customer_balance_transaction.py
+src/orb/models/shared/customer_tax_id.py
 src/orb/models/shared/event.py
 src/orb/models/shared/invoice.py
+src/orb/models/shared/invoice_line_item.py
 src/orb/models/shared/plan.py
 src/orb/models/shared/plan_phase.py
 src/orb/models/shared/price.py
 src/orb/models/shared/security.py
-src/orb/models/shared/shippingaddress.py
 src/orb/models/shared/subscription.py
 src/orb/models/shared/upcominginvoice.py
 src/orb/utils/__init__.py
 src/orb/utils/retries.py
 src/orb/utils/utils.py
 src/orb_billing.egg-info/PKG-INFO
 src/orb_billing.egg-info/SOURCES.txt
```

