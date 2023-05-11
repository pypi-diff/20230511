# Comparing `tmp/athiruma-cloud-governance-1.1.92.tar.gz` & `tmp/athiruma-cloud-governance-1.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athiruma-cloud-governance-1.1.92.tar", last modified: Wed May 10 10:37:16 2023, max compression
+gzip compressed data, was "athiruma-cloud-governance-1.1.93.tar", last modified: Thu May 11 05:54:35 2023, max compression
```

## Comparing `athiruma-cloud-governance-1.1.92.tar` & `athiruma-cloud-governance-1.1.93.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.837025 athiruma-cloud-governance-1.1.92/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/LICENSE
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/MANIFEST.in
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-10 10:37:16.837025 athiruma-cloud-governance-1.1.92/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/README.md
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.809025 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9295 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/SOURCES.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/dependency_links.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/not-zip-safe
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/requires.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-05-10 10:37:16.000000 athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/top_level.txt
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.809025 athiruma-cloud-governance-1.1.92/cloud_governance/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.809025 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.809025 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.810025 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12310 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10983 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5317 2023-05-10 09:17:19.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7250 2023-05-10 09:41:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/monitor/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/common/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudtrail/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.811025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudwatch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-04-28 14:53:44.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.812025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cost_explorer/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4803 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.812025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/dynamodb/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.813025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.813025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/iam/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-05-04 18:16:50.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.814025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/price.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.814025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/s3/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.815025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/sts/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.815025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/utils/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/utils/utils.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.815025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.816025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/cost_management/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.816025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/subscriptions/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.817025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/gcp/google_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.817025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.818025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/account/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.818025 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/classic/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.819025 athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11551 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.820025 athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/google_drive_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.820025 athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/jira.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/jira_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.821025 athiruma-cloud-governance-1.1.92/cloud_governance/common/ldap/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/ldap/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/ldap/ldap_search.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.821025 athiruma-cloud-governance-1.1.92/cloud_governance/common/logger/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/logger/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-05-09 04:30:49.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/logger/init_logger.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/logger/logger_time_stamp.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.822025 athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/gmail.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15240 2023-05-10 09:51:39.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/mail_message.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6165 2023-05-10 09:35:35.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/postfix.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.822025 athiruma-cloud-governance-1.1.92/cloud_governance/common/tool/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/tool/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/common/tool/tool.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.823025 athiruma-cloud-governance-1.1.92/cloud_governance/main/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/environment_variables.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/environment_variables_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/es_uploader.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/main.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/main/run_cloud_resource_orchestration.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.823025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.827025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-05-01 19:09:57.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_explorer.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ebs_in_use.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ebs_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_idle.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_stop.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/empty_roles.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ip_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/monthly_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/s3_inactive.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/skipped_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/zombie_snapshots.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.827025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/azure/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.827025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.829025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-05-08 04:46:20.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/tag_baremetal.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/tag_vm.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.829025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.829025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.829025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.830025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.831025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3811 2023-05-10 09:41:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.832025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.833025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.834025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.835025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.835025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.835025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.836025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gitleaks/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.836025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.836025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 10:37:16.836025 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-05-10 10:37:16.837025 athiruma-cloud-governance-1.1.92/setup.cfg
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2928 2023-05-10 10:37:00.000000 athiruma-cloud-governance-1.1.92/setup.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.399999 athiruma-cloud-governance-1.1.93/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/LICENSE
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/MANIFEST.in
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-11 05:54:35.399999 athiruma-cloud-governance-1.1.93/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/README.md
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.387998 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9295 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/SOURCES.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/dependency_links.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/not-zip-safe
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/requires.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-05-11 05:54:35.000000 athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/top_level.txt
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.387998 athiruma-cloud-governance-1.1.93/cloud_governance/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.387998 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.387998 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.387998 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12256 2023-05-11 05:50:03.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11138 2023-05-11 05:50:03.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5355 2023-05-11 05:50:03.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7250 2023-05-10 09:41:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-04-28 14:53:44.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4803 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.388999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-05-04 18:16:50.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/price.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/utils.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.389999 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/google_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.390998 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.391999 athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11551 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.391999 athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.391999 athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/jira.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/jira_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.391999 athiruma-cloud-governance-1.1.93/cloud_governance/common/ldap/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/ldap/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/ldap/ldap_search.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.391999 athiruma-cloud-governance-1.1.93/cloud_governance/common/logger/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/logger/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-05-09 04:30:49.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/logger/init_logger.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/logger/logger_time_stamp.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.392999 athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/gmail.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15240 2023-05-10 09:51:39.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/mail_message.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6165 2023-05-10 09:35:35.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/postfix.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.392999 athiruma-cloud-governance-1.1.93/cloud_governance/common/tool/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/tool/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/common/tool/tool.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.392999 athiruma-cloud-governance-1.1.93/cloud_governance/main/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-05-11 05:16:33.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/environment_variables.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/environment_variables_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/es_uploader.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/main.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/main/run_cloud_resource_orchestration.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.392999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.394999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-05-01 19:09:57.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_in_use.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_idle.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_run.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_stop.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/empty_roles.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ip_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/monthly_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/nat_gateway_unused.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/s3_inactive.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/skipped_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_snapshots.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.394999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/azure/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.394999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.395999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-05-08 04:46:20.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_vm.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.395999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.395999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.395999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.395999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.396999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3811 2023-05-10 09:41:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.396999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.397999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.397999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-05-10 09:09:25.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.398999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-05-09 04:30:34.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-11 05:54:35.399999 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-05-11 05:54:35.408999 athiruma-cloud-governance-1.1.93/setup.cfg
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2928 2023-05-11 05:54:33.000000 athiruma-cloud-governance-1.1.93/setup.py
```

### Comparing `athiruma-cloud-governance-1.1.92/LICENSE` & `athiruma-cloud-governance-1.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/PKG-INFO` & `athiruma-cloud-governance-1.1.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.92
+Version: 1.1.93
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiruma-cloud-governance-1.1.92/README.md` & `athiruma-cloud-governance-1.1.93/README.md`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/PKG-INFO` & `athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.92
+Version: 1.1.93
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/SOURCES.txt` & `athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/athiruma_cloud_governance.egg-info/requires.txt` & `athiruma-cloud-governance-1.1.93/athiruma_cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__account_name = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').strip()
         self.__cost_over_usage = CostOverUsage()
         self.jira_operations = JiraOperations()
         self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME', '')
         self.__es_index_cro = self.__environment_variables_dict.get('CRO_ES_INDEX', '')
-        self.__monitor_ticket = MonitorTickets()
 
     @typeguard.typechecked
     @logger_time_stamp
     def get_user_cost_data(self, user: str, requested_date: datetime, user_project: str = '', forecast: bool = False, duration: int = 0):
         """
         This method fetch data from the es_reports
         :param duration:
@@ -118,15 +117,15 @@
                                            f"{instance.get('instance_plan')}, {instance.get('instance_type')}, "
                                            f"{instance.get('instance_state')}, {running_days}")
                 if instance.get('instance_plan').lower() == 'spot':
                     source['total_spots'] = source.get('total_spots') + 1
                 else:
                     if instance.get('instance_plan').lower() == 'ondemand':
                         source['total_ondemand'] = source.get('total_ondemand') + 1
-        self.__monitor_ticket.verify_es_instances_state(es_data=source)
+        MonitorTickets().verify_es_instances_state(es_data=source)
         if datetime.strptime(source.get('timestamp'), "%Y-%m-%dT%H:%M:%S.%f").date() != datetime.now().date():
             source['monitored_days'] = (datetime.utcnow().date() - source.get('ticket_opened_date')).days
         source['total_instances'] = len(source.get('instances', self.ZERO))
         source['duration'] = int(instance_data[self.ZERO].get('duration'))
         source['estimated_cost'] = round(cost_estimation, self.DEFAULT_ROUND_DIGITS)
         source['actual_cost'] = user_cost
         if instance_data[self.ZERO].get('user_cro') and source.get('user_cro') != instance_data[self.ZERO].get('user_cro'):
```

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """
     This class will monitor the cost explorer reports and send alert to the user if they exceed specified amount
     """
 
     DEFAULT_ROUND_DIGITS = 3
     FORECAST_GRANULARITY = 'MONTHLY'
     FORECAST_COST_METRIC = 'UNBLENDED_COST'
+    OVER_USAGE_THRESHOLD = 0.05
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__aws_account = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').strip()
         self.__postfix_mail = Postfix()
         self.__mail_message = MailMessage()
         self.__es_host = self.__environment_variables_dict.get('es_host', '')
@@ -35,14 +36,15 @@
         self.es_index_cro = self.__environment_variables_dict.get('CRO_ES_INDEX', '')
         self.__cro_duration_days = self.__environment_variables_dict.get('CRO_DURATION_DAYS')
         self.current_end_date = datetime.utcnow()
         self.current_start_date = self.current_end_date - timedelta(days=self.__cro_duration_days)
         self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME')
         self.__ce_operations = CostExplorerOperations()
         self.es_operations = ElasticSearchOperations(es_host=self.__es_host, es_port=self.__es_port)
+        self.__over_usage_threshold = self.OVER_USAGE_THRESHOLD * self.__over_usage_amount
 
     @typeguard.typechecked
     @logger_time_stamp
     def get_cost_based_on_tag(self, start_date: str, end_date: str, tag_name: str, extra_filters: any = None, extra_operation: str = 'And', granularity: str = None, forecast: bool = False):
         """
         This method gives the cost based on the tag_name
         :param forecast:
@@ -146,15 +148,15 @@
         :return:
         """
         over_usage_users = []
         current_month_users = self.get_monthly_user_es_cost_data()
         for user in current_month_users:
             user_name = user.get('User')
             cost = round(user.get('Cost'), self.DEFAULT_ROUND_DIGITS)
-            if cost >= self.__over_usage_amount:
+            if cost >= (self.__over_usage_amount - self.__over_usage_threshold):
                 query = {  # check user opened the ticket in elastic_search
                     "query": {
                         "bool": {
                             "must": {
                                 "term": {"user": user_name}
                             },
                             "filter": {
```

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     
     PERSISTENT_RUN_DOC_ID = f'cro_run_persistence-{datetime.utcnow().date()}'
     PERSISTENT_RUN_INDEX = 'cloud_resource_orchestration_persistence_run'
     
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.cro_cost_over_usage = CostOverUsage()
-        self.cro_tagging = TagCROInstances()
-        self.cro_monitor = MonitorCROInstances()
         self.cro_reports = CollectCROReports()
         self.monitor_tickets = MonitorTickets()
         self.account = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').lower().strip()
         self.__run_active_regions = self.__environment_variables_dict.get('RUN_ACTIVE_REGIONS')
         self.__region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
 
     @logger_time_stamp
@@ -69,21 +67,23 @@
         """
         if self.__run_active_regions:
             active_regions = [region.get('RegionName') for region in boto3.client('ec2').describe_regions()['Regions']]
             logger.info(f"""*****Running CloudResourceOrchestration in all Active regions: {active_regions}*****""")
         else:
             active_regions = [self.__region]
         for active_region in active_regions:
+            cro_monitor = MonitorCROInstances(region_name=active_region)
+            cro_tagging = TagCROInstances(region_name=active_region)
             self.__environment_variables_dict.update({'AWS_DEFAULT_REGION': active_region})
             logger.info(f"""Running CloudResourceOrchestration in region: {active_region}""")
             logger.info(f"""{active_region}: -> Running CRO Tagging""")
-            tagging_response = self.cro_tagging.run()
+            tagging_response = cro_tagging.run()
             logger.info(f'Tagged instances : {tagging_response}')
             logger.info(f"""{active_region}: -> Running CRO Resource data Collection""")
-            monitor_response = self.cro_monitor.run()
+            monitor_response = cro_monitor.run()
             if monitor_response:
                 cro_reports = self.cro_reports.run(monitor_response)
                 logger.info(f'Cloud Orchestration Resources: {cro_reports}')
 
     @logger_time_stamp
     def start_cro(self):
         """
```

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/price.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/aws/utils/utils.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/gcp/google_account.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/elastic_upload.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/google_drive_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/google_drive/upload_to_gsheet.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/jira.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/jira/jira_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/ldap/ldap_search.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/logger/logger_time_stamp.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/gmail.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/mail_message.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/mail_message.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/common/mails/postfix.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/common/mails/postfix.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/main/environment_variables.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/main/environment_variables.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/main/es_uploader.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/main/main.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/main/main.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/main/run_cloud_resource_orchestration.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/main/run_cloud_resource_orchestration.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_explorer.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/cost_over_usage.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ebs_in_use.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ebs_unattached.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_idle.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_idle.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_run.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ec2_stop.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ec2_stop.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/empty_roles.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/empty_roles.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/ip_unattached.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/ip_unattached.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/monthly_report.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/monthly_report.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/nat_gateway_unused.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/nat_gateway_unused.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/s3_inactive.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/s3_inactive.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/skipped_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/skipped_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/zombie_cluster_resource.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/aws/zombie_snapshots.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/azure/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/gcp/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/cost_billing_reports.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/ibm_cost_report.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/tag_baremetal.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/ibm/tag_vm.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/ibm/tag_vm.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `athiruma-cloud-governance-1.1.93/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.92/setup.py` & `athiruma-cloud-governance-1.1.93/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.92'
+__version__ = '1.1.93'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

