# Comparing `tmp/prowler-3.4.1.tar.gz` & `tmp/prowler-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowler-3.4.1.tar", max compression
+gzip compressed data, was "prowler-3.5.0.tar", max compression
```

## Comparing `prowler-3.4.1.tar` & `prowler-3.5.0.tar`

### file list

```diff
@@ -1,1306 +1,1340 @@
--rw-r--r--   0        0        0    11339 2023-04-25 11:47:11.586799 prowler-3.4.1/LICENSE
--rw-r--r--   0        0        0    13104 2023-04-25 11:47:11.586799 prowler-3.4.1/README.md
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.610799 prowler-3.4.1/prowler/__init__.py
--rw-r--r--   0        0        0     8364 2023-04-25 11:47:11.610799 prowler-3.4.1/prowler/__main__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.610799 prowler-3.4.1/prowler/compliance/aws/__init__.py
--rw-r--r--   0        0        0     6516 2023-04-25 11:47:11.610799 prowler-3.4.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
--rw-r--r--   0        0        0    17475 2023-04-25 11:47:11.610799 prowler-3.4.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
--rw-r--r--   0        0        0   260398 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/cis_1.4_aws.json
--rw-r--r--   0        0        0   287275 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/cis_1.5_aws.json
--rw-r--r--   0        0        0    15458 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/cisa_aws.json
--rw-r--r--   0        0        0   124269 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/ens_rd2022_aws.json
--rw-r--r--   0        0        0    18551 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json
--rw-r--r--   0        0        0    57257 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
--rw-r--r--   0        0        0    31059 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/ffiec_aws.json
--rw-r--r--   0        0        0    10166 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/gdpr_aws.json
--rw-r--r--   0        0        0    18763 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
--rw-r--r--   0        0        0    11774 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json
--rw-r--r--   0        0        0    31000 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/hipaa_aws.json
--rw-r--r--   0        0        0    86208 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json
--rw-r--r--   0        0        0    50559 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json
--rw-r--r--   0        0        0   243911 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json
--rw-r--r--   0        0        0    40042 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/nist_csf_1.1_aws.json
--rw-r--r--   0        0        0     8722 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/pci_3.2.1_aws.json
--rw-r--r--   0        0        0     8563 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
--rw-r--r--   0        0        0    93913 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/aws/soc2_aws.json
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/azure/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/compliance/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/config/__init__.py
--rw-r--r--   0        0        0     2352 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/config/allowlist.yaml
--rw-r--r--   0        0        0      165 2023-04-25 11:47:11.614799 prowler-3.4.1/prowler/config/checklist_example.json
--rw-r--r--   0        0        0     2725 2023-04-25 11:47:28.562922 prowler-3.4.1/prowler/config/config.py
--rw-r--r--   0        0        0     1942 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/config/config.yaml
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/banner.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/__init__.py
--rw-r--r--   0        0        0    23001 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/check.py
--rw-r--r--   0        0        0     2973 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/checks_loader.py
--rw-r--r--   0        0        0     4413 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/compliance.py
--rw-r--r--   0        0        0     3645 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/compliance_models.py
--rw-r--r--   0        0        0     3835 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/check/models.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/cli/__init__.py
--rw-r--r--   0        0        0    17295 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/cli/parser.py
--rw-r--r--   0        0        0     1885 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/logger.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/__init__.py
--rw-r--r--   0        0        0    19729 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/compliance.py
--rw-r--r--   0        0        0     6687 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/file_descriptors.py
--rw-r--r--   0        0        0    20055 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/html.py
--rw-r--r--   0        0        0     3721 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/json.py
--rw-r--r--   0        0        0    20235 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/models.py
--rw-r--r--   0        0        0    10451 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/outputs.py
--rw-r--r--   0        0        0     6058 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/outputs/summary_table.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/scan_filters/__init__.py
--rw-r--r--   0        0        0      552 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/scan_filters/scan_filters.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/utils/__init__.py
--rw-r--r--   0        0        0     2200 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/lib/utils/utils.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/__init__.py
--rw-r--r--   0        0        0    10318 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/aws_provider.py
--rw-r--r--   0        0        0   211895 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/aws_regions_by_service.json
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/allowlist/__init__.py
--rw-r--r--   0        0        0     7931 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/allowlist/allowlist.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/arn/__init__.py
--rw-r--r--   0        0        0     1902 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/arn/arn.py
--rw-r--r--   0        0        0     1932 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/arn/error.py
--rw-r--r--   0        0        0      953 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0     1178 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/quick_inventory/__init__.py
--rw-r--r--   0        0        0    13659 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/resource_api_tagging/__init__.py
--rw-r--r--   0        0        0     1585 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/security_hub/__init__.py
--rw-r--r--   0        0        0     5867 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/lib/security_hub/security_hub.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/__init__.py
--rw-r--r--   0        0        0      244 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
--rw-r--r--   0        0        0     1584 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
--rw-r--r--   0        0        0     1478 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
--rw-r--r--   0        0        0     1635 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
--rw-r--r--   0        0        0     2184 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
--rw-r--r--   0        0        0     4735 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/__init__.py
--rw-r--r--   0        0        0      200 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
--rw-r--r--   0        0        0     1753 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
--rw-r--r--   0        0        0      652 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
--rw-r--r--   0        0        0      681 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
--rw-r--r--   0        0        0     1674 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
--rw-r--r--   0        0        0      699 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
--rw-r--r--   0        0        0      769 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/account/account_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
--rw-r--r--   0        0        0     1233 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
--rw-r--r--   0        0        0     1636 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_client.py
--rw-r--r--   0        0        0     4752 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/acm/acm_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0      976 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
--rw-r--r--   0        0        0     1250 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
--rw-r--r--   0        0        0     1126 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
--rw-r--r--   0        0        0      994 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1676 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1079 2023-04-25 11:47:11.618799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
--rw-r--r--   0        0        0     5312 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1181 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1093 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
--rw-r--r--   0        0        0      234 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
--rw-r--r--   0        0        0     3806 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/__init__.py
--rw-r--r--   0        0        0      210 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
--rw-r--r--   0        0        0     1346 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
--rw-r--r--   0        0        0     1273 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
--rw-r--r--   0        0        0     1408 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1269 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1420 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
--rw-r--r--   0        0        0     1583 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
--rw-r--r--   0        0        0     3619 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/__init__.py
--rw-r--r--   0        0        0      220 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
--rw-r--r--   0        0        0     1902 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
--rw-r--r--   0        0        0       78 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
--rw-r--r--   0        0        0     2626 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/__init__.py
--rw-r--r--   0        0        0      204 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2548 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
--rw-r--r--   0        0        0     3352 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
--rw-r--r--   0        0        0     1536 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
--rw-r--r--   0        0        0     2209 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1823 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
--rw-r--r--   0        0        0     1120 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
--rw-r--r--   0        0        0     1144 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
--rw-r--r--   0        0        0     1619 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
--rw-r--r--   0        0        0     7807 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/__init__.py
--rw-r--r--   0        0        0      195 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
--rw-r--r--   0        0        0      920 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
--rw-r--r--   0        0        0     1167 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
--rw-r--r--   0        0        0      975 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
--rw-r--r--   0        0        0     6992 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
--rw-r--r--   0        0        0     1096 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
--rw-r--r--   0        0        0      928 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/__init__.py
--rw-r--r--   0        0        0      244 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_client.py
--rw-r--r--   0        0        0     4466 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
--rw-r--r--   0        0        0     1992 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1286 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/__init__.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
--rw-r--r--   0        0        0     1321 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
--rw-r--r--   0        0        0     1164 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
--rw-r--r--   0        0        0     1395 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
--rw-r--r--   0        0        0     1912 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1230 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
--rw-r--r--   0        0        0     1781 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
--rw-r--r--   0        0        0     1031 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
--rw-r--r--   0        0        0     6244 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
--rw-r--r--   0        0        0     1707 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1575 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2245 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
--rw-r--r--   0        0        0     1287 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
--rw-r--r--   0        0        0     1073 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1951 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1524 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
--rw-r--r--   0        0        0     1457 2023-04-25 11:47:11.622799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1380 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0     2232 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1393 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2755 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
--rw-r--r--   0        0        0     1730 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
--rw-r--r--   0        0        0     1956 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
--rw-r--r--   0        0        0     2892 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
--rw-r--r--   0        0        0     1565 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
--rw-r--r--   0        0        0     2894 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
--rw-r--r--   0        0        0     9085 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2391 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1462 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2397 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1450 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2415 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
--rw-r--r--   0        0        0     2600 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
--rw-r--r--   0        0        0      841 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1249 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1002 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
--rw-r--r--   0        0        0     1345 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
--rw-r--r--   0        0        0     4856 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
--rw-r--r--   0        0        0     1365 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
--rw-r--r--   0        0        0     1569 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2391 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2337 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
--rw-r--r--   0        0        0     1495 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
--rw-r--r--   0        0        0     2208 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
--rw-r--r--   0        0        0     3046 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
--rw-r--r--   0        0        0     1560 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
--rw-r--r--   0        0        0     2261 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
--rw-r--r--   0        0        0     2543 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
--rw-r--r--   0        0        0     2748 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
--rw-r--r--   0        0        0     2228 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
--rw-r--r--   0        0        0     1448 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
--rw-r--r--   0        0        0     2413 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
--rw-r--r--   0        0        0     2203 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
--rw-r--r--   0        0        0     1446 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
--rw-r--r--   0        0        0     2208 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
--rw-r--r--   0        0        0    10786 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
--rw-r--r--   0        0        0      197 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/cloudwatch/logs_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/__init__.py
--rw-r--r--   0        0        0      234 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
--rw-r--r--   0        0        0     1665 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
--rw-r--r--   0        0        0    10499 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/__init__.py
--rw-r--r--   0        0        0      210 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
--rw-r--r--   0        0        0     1241 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
--rw-r--r--   0        0        0     1049 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
--rw-r--r--   0        0        0     3606 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/__init__.py
--rw-r--r--   0        0        0      195 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/config_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
--rw-r--r--   0        0        0     1486 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
--rw-r--r--   0        0        0     3167 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/config/config_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/__init__.py
--rw-r--r--   0        0        0      254 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
--rw-r--r--   0        0        0     1191 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
--rw-r--r--   0        0        0      997 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
--rw-r--r--   0        0        0     1041 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
--rw-r--r--   0        0        0     1042 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
--rw-r--r--   0        0        0     1872 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
--rw-r--r--   0        0        0     1660 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
--rw-r--r--   0        0        0     1373 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
--rw-r--r--   0        0        0    12175 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
--rw-r--r--   0        0        0     1265 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
--rw-r--r--   0        0        0     1269 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/drs_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
--rw-r--r--   0        0        0      898 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
--rw-r--r--   0        0        0      919 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
--rw-r--r--   0        0        0     3629 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/drs/drs_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/__init__.py
--rw-r--r--   0        0        0      190 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dax_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.626799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      957 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
--rw-r--r--   0        0        0      205 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_client.py
--rw-r--r--   0        0        0     8153 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1497 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      988 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
--rw-r--r--   0        0        0      933 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
--rw-r--r--   0        0        0      843 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
--rw-r--r--   0        0        0      783 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
--rw-r--r--   0        0        0      965 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
--rw-r--r--   0        0        0     1530 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
--rw-r--r--   0        0        0      922 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
--rw-r--r--   0        0        0      849 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
--rw-r--r--   0        0        0     2037 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
--rw-r--r--   0        0        0     1107 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
--rw-r--r--   0        0        0      971 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
--rw-r--r--   0        0        0     1461 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
--rw-r--r--   0        0        0     1111 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
--rw-r--r--   0        0        0     1253 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
--rw-r--r--   0        0        0     1201 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
--rw-r--r--   0        0        0     1491 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
--rw-r--r--   0        0        0     1543 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
--rw-r--r--   0        0        0     1034 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
--rw-r--r--   0        0        0     1118 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
--rw-r--r--   0        0        0     1292 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
--rw-r--r--   0        0        0     2348 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
--rw-r--r--   0        0        0       78 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
--rw-r--r--   0        0        0     1378 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
--rw-r--r--   0        0        0     1247 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1483 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1268 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
--rw-r--r--   0        0        0     1139 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
--rw-r--r--   0        0        0     1323 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
--rw-r--r--   0        0        0     1197 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
--rw-r--r--   0        0        0     1468 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
--rw-r--r--   0        0        0     1169 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
--rw-r--r--   0        0        0     1436 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
--rw-r--r--   0        0        0     1429 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
--rw-r--r--   0        0        0     1409 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
--rw-r--r--   0        0        0     1437 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
--rw-r--r--   0        0        0     1497 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
--rw-r--r--   0        0        0     1532 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
--rw-r--r--   0        0        0     1427 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
--rw-r--r--   0        0        0     1443 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
--rw-r--r--   0        0        0     1486 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
--rw-r--r--   0        0        0     1461 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
--rw-r--r--   0        0        0     1436 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
--rw-r--r--   0        0        0     1164 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
--rw-r--r--   0        0        0     1427 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
--rw-r--r--   0        0        0     1218 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
--rw-r--r--   0        0        0     1499 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
--rw-r--r--   0        0        0     1422 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
--rw-r--r--   0        0        0     2440 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
--rw-r--r--   0        0        0     1305 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
--rw-r--r--   0        0        0     1029 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
--rw-r--r--   0        0        0     1043 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
--rw-r--r--   0        0        0     1144 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
--rw-r--r--   0        0        0     1219 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
--rw-r--r--   0        0        0    18754 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/lib/__init__.py
--rw-r--r--   0        0        0     2581 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/lib/network_acls.py
--rw-r--r--   0        0        0     3766 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ec2/lib/security_groups.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ecr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.630799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1375 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0     1302 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
--rw-r--r--   0        0        0      973 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1213 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1322 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
--rw-r--r--   0        0        0     1501 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
--rw-r--r--   0        0        0      990 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
--rw-r--r--   0        0        0     1268 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
--rw-r--r--   0        0        0     2034 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
--rw-r--r--   0        0        0    10008 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_client.py
--rw-r--r--   0        0        0     3857 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
--rw-r--r--   0        0        0     1625 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
--rw-r--r--   0        0        0     2328 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1366 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      853 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1099 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
--rw-r--r--   0        0        0      843 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0      981 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1853 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
--rw-r--r--   0        0        0     3889 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/efs/efs_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
--rw-r--r--   0        0        0      992 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
--rw-r--r--   0        0        0     1559 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
--rw-r--r--   0        0        0     1215 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
--rw-r--r--   0        0        0     1374 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
--rw-r--r--   0        0        0     1489 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
--rw-r--r--   0        0        0     4579 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/eks/eks_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1364 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1115 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
--rw-r--r--   0        0        0      823 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
--rw-r--r--   0        0        0      817 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
--rw-r--r--   0        0        0     4592 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1360 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
--rw-r--r--   0        0        0      937 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
--rw-r--r--   0        0        0      892 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
--rw-r--r--   0        0        0     1718 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
--rw-r--r--   0        0        0     1367 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
--rw-r--r--   0        0        0     1337 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
--rw-r--r--   0        0        0     1646 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
--rw-r--r--   0        0        0     1162 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
--rw-r--r--   0        0        0      888 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
--rw-r--r--   0        0        0      996 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
--rw-r--r--   0        0        0      836 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1435 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
--rw-r--r--   0        0        0      924 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
--rw-r--r--   0        0        0     7882 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
--rw-r--r--   0        0        0     1325 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
--rw-r--r--   0        0        0     1664 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
--rw-r--r--   0        0        0     1439 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
--rw-r--r--   0        0        0      917 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
--rw-r--r--   0        0        0      897 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
--rw-r--r--   0        0        0     1200 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
--rw-r--r--   0        0        0     4444 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
--rw-r--r--   0        0        0     7714 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/emr/emr_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/__init__.py
--rw-r--r--   0        0        0      200 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_client.py
--rw-r--r--   0        0        0     3995 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
--rw-r--r--   0        0        0     1219 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
--rw-r--r--   0        0        0     1940 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/globalaccelerator/__init__.py
--rw-r--r--   0        0        0      259 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
--rw-r--r--   0        0        0     2362 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/__init__.py
--rw-r--r--   0        0        0      185 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1464 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      928 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      920 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
--rw-r--r--   0        0        0     1222 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
--rw-r--r--   0        0        0      884 2023-04-25 11:47:11.634799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1632 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1361 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1623 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1352 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1644 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1322 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1574 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1622 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1600 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1293 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1591 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1284 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
--rw-r--r--   0        0        0     9722 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/glue/glue_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
--rw-r--r--   0        0        0      998 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
--rw-r--r--   0        0        0     1221 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
--rw-r--r--   0        0        0      210 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
--rw-r--r--   0        0        0     1282 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
--rw-r--r--   0        0        0     1130 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
--rw-r--r--   0        0        0      961 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
--rw-r--r--   0        0        0     7252 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
--rw-r--r--   0        0        0     1010 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
--rw-r--r--   0        0        0     2805 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2073 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2227 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
--rw-r--r--   0        0        0      802 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2088 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2238 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     2118 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     2251 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
--rw-r--r--   0        0        0     1413 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
--rw-r--r--   0        0        0     4146 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
--rw-r--r--   0        0        0     1417 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
--rw-r--r--   0        0        0     4192 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
--rw-r--r--   0        0        0     1089 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
--rw-r--r--   0        0        0     2665 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
--rw-r--r--   0        0        0     1707 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
--rw-r--r--   0        0        0     1090 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
--rw-r--r--   0        0        0     1541 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
--rw-r--r--   0        0        0     1360 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
--rw-r--r--   0        0        0     1086 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
--rw-r--r--   0        0        0     1299 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
--rw-r--r--   0        0        0     1185 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
--rw-r--r--   0        0        0     1095 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
--rw-r--r--   0        0        0     1280 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
--rw-r--r--   0        0        0     1231 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
--rw-r--r--   0        0        0     1095 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
--rw-r--r--   0        0        0     1083 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
--rw-r--r--   0        0        0     6229 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
--rw-r--r--   0        0        0     1925 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
--rw-r--r--   0        0        0     2059 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
--rw-r--r--   0        0        0     2045 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
--rw-r--r--   0        0        0     1174 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
--rw-r--r--   0        0        0     3534 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1595 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1738 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1020 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
--rw-r--r--   0        0        0     1424 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
--rw-r--r--   0        0        0     2832 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
--rw-r--r--   0        0        0     1335 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
--rw-r--r--   0        0        0      901 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
--rw-r--r--   0        0        0    21365 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
--rw-r--r--   0        0        0      940 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-25 11:47:11.638799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
--rw-r--r--   0        0        0     1698 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
--rw-r--r--   0        0        0     2671 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
--rw-r--r--   0        0        0      998 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
--rw-r--r--   0        0        0     1341 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/__init__.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
--rw-r--r--   0        0        0     1158 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
--rw-r--r--   0        0        0     1256 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
--rw-r--r--   0        0        0     4121 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
--rw-r--r--   0        0        0     1053 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
--rw-r--r--   0        0        0     1194 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1294 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2525 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0     5255 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/__init__.py
--rw-r--r--   0        0        0      190 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/macie_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
--rw-r--r--   0        0        0      894 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
--rw-r--r--   0        0        0     1785 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/macie/macie_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/__init__.py
--rw-r--r--   0        0        0      238 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_client.py
--rw-r--r--   0        0        0     6959 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1102 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1871 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0     1003 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
--rw-r--r--   0        0        0      991 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
--rw-r--r--   0        0        0      983 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1766 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     2655 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
--rw-r--r--   0        0        0     1736 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
--rw-r--r--   0        0        0      984 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
--rw-r--r--   0        0        0      239 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
--rw-r--r--   0        0        0     1816 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
--rw-r--r--   0        0        0     1548 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
--rw-r--r--   0        0        0     5605 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
--rw-r--r--   0        0        0     8903 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
--rw-r--r--   0        0        0     1473 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
--rw-r--r--   0        0        0      984 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
--rw-r--r--   0        0        0     1367 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
--rw-r--r--   0        0        0      980 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
--rw-r--r--   0        0        0      960 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
--rw-r--r--   0        0        0     1488 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
--rw-r--r--   0        0        0      947 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
--rw-r--r--   0        0        0      969 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
--rw-r--r--   0        0        0      944 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
--rw-r--r--   0        0        0     1426 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
--rw-r--r--   0        0        0      959 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
--rw-r--r--   0        0        0     1370 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
--rw-r--r--   0        0        0      892 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
--rw-r--r--   0        0        0     1510 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
--rw-r--r--   0        0        0     1367 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
--rw-r--r--   0        0        0    10647 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
--rw-r--r--   0        0        0     1543 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/__init__.py
--rw-r--r--   0        0        0      205 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
--rw-r--r--   0        0        0      973 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
--rw-r--r--   0        0        0     1204 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
--rw-r--r--   0        0        0      984 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
--rw-r--r--   0        0        0     1285 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
--rw-r--r--   0        0        0      996 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
--rw-r--r--   0        0        0     1297 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
--rw-r--r--   0        0        0      992 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
--rw-r--r--   0        0        0     4912 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/__init__.py
--rw-r--r--   0        0        0      261 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
--rw-r--r--   0        0        0      973 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
--rw-r--r--   0        0        0      940 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
--rw-r--r--   0        0        0     2344 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.642799 prowler-3.4.1/prowler/providers/aws/services/route53/__init__.py
--rw-r--r--   0        0        0      200 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
--rw-r--r--   0        0        0     1188 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
--rw-r--r--   0        0        0     1023 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
--rw-r--r--   0        0        0      998 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
--rw-r--r--   0        0        0     1058 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
--rw-r--r--   0        0        0     1249 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
--rw-r--r--   0        0        0     6911 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53_service.py
--rw-r--r--   0        0        0      221 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/route53/route53domains_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
--rw-r--r--   0        0        0     1392 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
--rw-r--r--   0        0        0     1068 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
--rw-r--r--   0        0        0     1266 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
--rw-r--r--   0        0        0      957 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
--rw-r--r--   0        0        0      917 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
--rw-r--r--   0        0        0     1123 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
--rw-r--r--   0        0        0     1426 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
--rw-r--r--   0        0        0      943 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
--rw-r--r--   0        0        0      947 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
--rw-r--r--   0        0        0     1716 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
--rw-r--r--   0        0        0     4014 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
--rw-r--r--   0        0        0     2099 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
--rw-r--r--   0        0        0     1372 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
--rw-r--r--   0        0        0      978 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
--rw-r--r--   0        0        0      175 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_client.py
--rw-r--r--   0        0        0    14801 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3_service.py
--rw-r--r--   0        0        0      196 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/s3/s3control_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/__init__.py
--rw-r--r--   0        0        0      210 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0      945 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0      966 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1412 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
--rw-r--r--   0        0        0     1037 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1361 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1063 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
--rw-r--r--   0        0        0     1524 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
--rw-r--r--   0        0        0     1091 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
--rw-r--r--   0        0        0    11132 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1119 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1040 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
--rw-r--r--   0        0        0     1106 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
--rw-r--r--   0        0        0     1005 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1042 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
--rw-r--r--   0        0        0     1100 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
--rw-r--r--   0        0        0     1072 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1341 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1054 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
--rw-r--r--   0        0        0      244 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
--rw-r--r--   0        0        0     2442 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/__init__.py
--rw-r--r--   0        0        0      220 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
--rw-r--r--   0        0        0     1315 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
--rw-r--r--   0        0        0     1296 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
--rw-r--r--   0        0        0     4490 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
--rw-r--r--   0        0        0     1051 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
--rw-r--r--   0        0        0     1259 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
--rw-r--r--   0        0        0     1267 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
--rw-r--r--   0        0        0     1041 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
--rw-r--r--   0        0        0     1316 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
--rw-r--r--   0        0        0     1271 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
--rw-r--r--   0        0        0     1095 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
--rw-r--r--   0        0        0     1353 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
--rw-r--r--   0        0        0     1020 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
--rw-r--r--   0        0        0     1275 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
--rw-r--r--   0        0        0      195 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_client.py
--rw-r--r--   0        0        0     2527 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/shield/shield_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_client.py
--rw-r--r--   0        0        0     3814 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
--rw-r--r--   0        0        0      841 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1921 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1396 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1933 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     1479 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
--rw-r--r--   0        0        0      939 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
--rw-r--r--   0        0        0     4137 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/ssm/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.646799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
--rw-r--r--   0        0        0     1974 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
--rw-r--r--   0        0        0      884 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
--rw-r--r--   0        0        0     1557 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
--rw-r--r--   0        0        0      993 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
--rw-r--r--   0        0        0     7622 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/__init__.py
--rw-r--r--   0        0        0      234 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
--rw-r--r--   0        0        0     1396 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
--rw-r--r--   0        0        0     6747 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/__init__.py
--rw-r--r--   0        0        0      244 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
--rw-r--r--   0        0        0     1272 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
--rw-r--r--   0        0        0     2972 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
--rw-r--r--   0        0        0      860 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
--rw-r--r--   0        0        0     1070 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1094 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     3142 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
--rw-r--r--   0        0        0     2056 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
--rw-r--r--   0        0        0     1214 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
--rw-r--r--   0        0        0      822 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
--rw-r--r--   0        0        0     1294 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
--rw-r--r--   0        0        0     1496 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
--rw-r--r--   0        0        0    15315 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
--rw-r--r--   0        0        0      913 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
--rw-r--r--   0        0        0     1276 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
--rw-r--r--   0        0        0      900 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
--rw-r--r--   0        0        0     1432 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/waf/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/waf/waf_client.py
--rw-r--r--   0        0        0     2645 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/waf/waf_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/wafv2/__init__.py
--rw-r--r--   0        0        0      190 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/wafv2/wafv2_client.py
--rw-r--r--   0        0        0     2724 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/wafv2/wafv2_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/__init__.py
--rw-r--r--   0        0        0      215 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_client.py
--rw-r--r--   0        0        0     3457 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
--rw-r--r--   0        0        0     2073 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
--rw-r--r--   0        0        0     1586 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/__init__.py
--rw-r--r--   0        0        0     8032 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/azure_provider.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      258 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      796 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/__init__.py
--rw-r--r--   0        0        0      205 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
--rw-r--r--   0        0        0     1182 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
--rw-r--r--   0        0        0      926 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
--rw-r--r--   0        0        0     1121 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1210 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
--rw-r--r--   0        0        0     1561 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
--rw-r--r--   0        0        0     1181 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
--rw-r--r--   0        0        0     1306 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
--rw-r--r--   0        0        0      906 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1638 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
--rw-r--r--   0        0        0     1254 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
--rw-r--r--   0        0        0     1122 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
--rw-r--r--   0        0        0     1590 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
--rw-r--r--   0        0        0     1163 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
--rw-r--r--   0        0        0     1187 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
--rw-r--r--   0        0        0     1346 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
--rw-r--r--   0        0        0     1170 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
--rw-r--r--   0        0        0     1227 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
--rw-r--r--   0        0        0     1693 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
--rw-r--r--   0        0        0     1202 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
--rw-r--r--   0        0        0     2326 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/defender/defender_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/__init__.py
--rw-r--r--   0        0        0      180 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/iam_client.py
--rw-r--r--   0        0        0     2696 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
--rw-r--r--   0        0        0      996 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
--rw-r--r--   0        0        0     1330 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
--rw-r--r--   0        0        0      200 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
--rw-r--r--   0        0        0     1354 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
--rw-r--r--   0        0        0     1765 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
--rw-r--r--   0        0        0     1265 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
--rw-r--r--   0        0        0     1399 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
--rw-r--r--   0        0        0     1156 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
--rw-r--r--   0        0        0     1246 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
--rw-r--r--   0        0        0     1151 2023-04-25 11:47:11.650799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
--rw-r--r--   0        0        0     1093 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
--rw-r--r--   0        0        0     1169 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
--rw-r--r--   0        0        0     1272 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
--rw-r--r--   0        0        0     1166 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
--rw-r--r--   0        0        0     3651 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/azure/services/storage/storage_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/allowlist.py
--rw-r--r--   0        0        0    17566 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/audit_info.py
--rw-r--r--   0        0        0      251 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/models.py
--rw-r--r--   0        0        0     4693 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/outputs.py
--rw-r--r--   0        0        0      885 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/common/quick_inventory.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/__init__.py
--rw-r--r--   0        0        0     1695 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/gcp_provider.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/lib/audit_info/__init__.py
--rw-r--r--   0        0        0      201 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/lib/audit_info/audit_info.py
--rw-r--r--   0        0        0      522 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/lib/audit_info/models.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1445 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      996 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
--rw-r--r--   0        0        0      948 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
--rw-r--r--   0        0        0     4116 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
--rw-r--r--   0        0        0     1373 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
--rw-r--r--   0        0        0      974 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
--rw-r--r--   0        0        0      266 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
--rw-r--r--   0        0        0     1262 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
--rw-r--r--   0        0        0     1408 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
--rw-r--r--   0        0        0     1011 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
--rw-r--r--   0        0        0     1182 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
--rw-r--r--   0        0        0     1216 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
--rw-r--r--   0        0        0     1203 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
--rw-r--r--   0        0        0     2058 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
--rw-r--r--   0        0        0     1302 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
--rw-r--r--   0        0        0     1207 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
--rw-r--r--   0        0        0     1219 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
--rw-r--r--   0        0        0     1618 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
--rw-r--r--   0        0        0     1310 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
--rw-r--r--   0        0        0     1323 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
--rw-r--r--   0        0        0     1955 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
--rw-r--r--   0        0        0     1466 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
--rw-r--r--   0        0        0     1745 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
--rw-r--r--   0        0        0     1410 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
--rw-r--r--   0        0        0     1326 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
--rw-r--r--   0        0        0     1368 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
--rw-r--r--   0        0        0     1104 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
--rw-r--r--   0        0        0     1492 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
--rw-r--r--   0        0        0     1046 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1319 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      991 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
--rw-r--r--   0        0        0     2153 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
--rw-r--r--   0        0        0     1350 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
--rw-r--r--   0        0        0     1702 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
--rw-r--r--   0        0        0     1232 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
--rw-r--r--   0        0        0     1319 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
--rw-r--r--   0        0        0     1860 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
--rw-r--r--   0        0        0     1201 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
--rw-r--r--   0        0        0     2002 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
--rw-r--r--   0        0        0     1190 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
--rw-r--r--   0        0        0     2238 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
--rw-r--r--   0        0        0     1210 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
--rw-r--r--   0        0        0     1583 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
--rw-r--r--   0        0        0     1179 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
--rw-r--r--   0        0        0     1428 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
--rw-r--r--   0        0        0      977 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
--rw-r--r--   0        0        0     2467 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
--rw-r--r--   0        0        0      926 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
--rw-r--r--   0        0        0     1270 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
--rw-r--r--   0        0        0     1067 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
--rw-r--r--   0        0        0      226 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
--rw-r--r--   0        0        0     2099 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/__init__.py
--rw-r--r--   0        0        0      192 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
--rw-r--r--   0        0        0      897 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
--rw-r--r--   0        0        0     1132 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
--rw-r--r--   0        0        0      827 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
--rw-r--r--   0        0        0     3489 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/compute/compute_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/__init__.py
--rw-r--r--   0        0        0      172 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
--rw-r--r--   0        0        0     1395 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
--rw-r--r--   0        0        0     1363 2023-04-25 11:47:11.654799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
--rw-r--r--   0        0        0     1038 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
--rw-r--r--   0        0        0     1133 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
--rw-r--r--   0        0        0     1317 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
--rw-r--r--   0        0        0     3292 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/iam/iam_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/__init__.py
--rw-r--r--   0        0        0      172 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
--rw-r--r--   0        0        0     1195 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
--rw-r--r--   0        0        0     1000 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
--rw-r--r--   0        0        0     1135 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
--rw-r--r--   0        0        0     4837 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/kms/kms_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/__init__.py
--rw-r--r--   0        0        0      192 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_client.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1438 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1996 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1243 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1971 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1239 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2090 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1590 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2288 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
--rw-r--r--   0        0        0     1955 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1233 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2086 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1113 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2188 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
--rw-r--r--   0        0        0     1157 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
--rw-r--r--   0        0        0     2019 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
--rw-r--r--   0        0        0     2577 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_service.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
--rw-r--r--   0        0        0     1235 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
--rw-r--r--   0        0        0     1473 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
--rw-r--r--   0        0        0        0 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/monitoring/__init__.py
--rw-r--r--   0        0        0      207 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_client.py
--rw-r--r--   0        0        0     1893 2023-04-25 11:47:11.658799 prowler-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_service.py
--rw-r--r--   0        0        0     2437 2023-04-25 11:47:28.542922 prowler-3.4.1/pyproject.toml
--rw-r--r--   0        0        0    15165 1970-01-01 00:00:00.000000 prowler-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-05-11 14:20:18.949326 prowler-3.5.0/LICENSE
+-rw-r--r--   0        0        0    13104 2023-05-11 14:20:18.949326 prowler-3.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.985327 prowler-3.5.0/prowler/__init__.py
+-rw-r--r--   0        0        0     9018 2023-05-11 14:20:18.985327 prowler-3.5.0/prowler/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.985327 prowler-3.5.0/prowler/compliance/aws/__init__.py
+-rw-r--r--   0        0        0     6516 2023-05-11 14:20:18.985327 prowler-3.5.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json
+-rw-r--r--   0        0        0    17475 2023-05-11 14:20:18.985327 prowler-3.5.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json
+-rw-r--r--   0        0        0   260398 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/cis_1.4_aws.json
+-rw-r--r--   0        0        0   287275 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/cis_1.5_aws.json
+-rw-r--r--   0        0        0    15458 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/cisa_aws.json
+-rw-r--r--   0        0        0   124269 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/ens_rd2022_aws.json
+-rw-r--r--   0        0        0    18551 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json
+-rw-r--r--   0        0        0    57257 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json
+-rw-r--r--   0        0        0    31059 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/ffiec_aws.json
+-rw-r--r--   0        0        0    10166 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/gdpr_aws.json
+-rw-r--r--   0        0        0    18763 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json
+-rw-r--r--   0        0        0    11774 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json
+-rw-r--r--   0        0        0    31000 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/hipaa_aws.json
+-rw-r--r--   0        0        0    86208 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json
+-rw-r--r--   0        0        0    50559 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json
+-rw-r--r--   0        0        0   243911 2023-05-11 14:20:18.989327 prowler-3.5.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json
+-rw-r--r--   0        0        0    40042 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/aws/nist_csf_1.1_aws.json
+-rw-r--r--   0        0        0     8722 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/aws/pci_3.2.1_aws.json
+-rw-r--r--   0        0        0     8563 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json
+-rw-r--r--   0        0        0    93913 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/aws/soc2_aws.json
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/azure/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/compliance/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/config/__init__.py
+-rw-r--r--   0        0        0     2530 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/config/allowlist.yaml
+-rw-r--r--   0        0        0      165 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/config/checklist_example.json
+-rw-r--r--   0        0        0     3194 2023-05-11 14:20:41.877398 prowler-3.5.0/prowler/config/config.py
+-rw-r--r--   0        0        0     1942 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/config/config.yaml
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/banner.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/__init__.py
+-rw-r--r--   0        0        0    23001 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/check.py
+-rw-r--r--   0        0        0     2973 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/checks_loader.py
+-rw-r--r--   0        0        0     4413 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/compliance.py
+-rw-r--r--   0        0        0     3645 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/compliance_models.py
+-rw-r--r--   0        0        0     3835 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/check/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/cli/__init__.py
+-rw-r--r--   0        0        0    17645 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/cli/parser.py
+-rw-r--r--   0        0        0     1885 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/logger.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/__init__.py
+-rw-r--r--   0        0        0    19729 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/compliance.py
+-rw-r--r--   0        0        0     6687 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/file_descriptors.py
+-rw-r--r--   0        0        0    20055 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/html.py
+-rw-r--r--   0        0        0     3721 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/json.py
+-rw-r--r--   0        0        0    20061 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/models.py
+-rw-r--r--   0        0        0    10451 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/outputs.py
+-rw-r--r--   0        0        0     5002 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/slack.py
+-rw-r--r--   0        0        0     6058 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/outputs/summary_table.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/scan_filters/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/scan_filters/scan_filters.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/utils/__init__.py
+-rw-r--r--   0        0        0     2200 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/lib/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/providers/aws/__init__.py
+-rw-r--r--   0        0        0    10318 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/providers/aws/aws_provider.py
+-rw-r--r--   0        0        0   213237 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/providers/aws/aws_regions_by_service.json
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/providers/aws/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.993327 prowler-3.5.0/prowler/providers/aws/lib/allowlist/__init__.py
+-rw-r--r--   0        0        0     8680 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/allowlist/allowlist.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/arn/__init__.py
+-rw-r--r--   0        0        0     1902 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/arn/arn.py
+-rw-r--r--   0        0        0     1932 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/arn/error.py
+-rw-r--r--   0        0        0      953 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0     1178 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/quick_inventory/__init__.py
+-rw-r--r--   0        0        0    13659 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/resource_api_tagging/__init__.py
+-rw-r--r--   0        0        0     1585 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/security_hub/__init__.py
+-rw-r--r--   0        0        0     5867 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/lib/security_hub/security_hub.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/__init__.py
+-rw-r--r--   0        0        0     1584 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json
+-rw-r--r--   0        0        0     1478 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/__init__.py
+-rw-r--r--   0        0        0     1635 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json
+-rw-r--r--   0        0        0     2184 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py
+-rw-r--r--   0        0        0     5375 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json
+-rw-r--r--   0        0        0      652 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json
+-rw-r--r--   0        0        0      681 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/__init__.py
+-rw-r--r--   0        0        0     1674 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json
+-rw-r--r--   0        0        0      699 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py
+-rw-r--r--   0        0        0      769 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/account/account_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/__init__.py
+-rw-r--r--   0        0        0     1368 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json
+-rw-r--r--   0        0        0     1233 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json
+-rw-r--r--   0        0        0     1636 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_client.py
+-rw-r--r--   0        0        0     4752 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/acm/acm_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1133 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0      976 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/__init__.py
+-rw-r--r--   0        0        0     1250 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json
+-rw-r--r--   0        0        0     1126 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/__init__.py
+-rw-r--r--   0        0        0     1087 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json
+-rw-r--r--   0        0        0      994 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1079 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py
+-rw-r--r--   0        0        0     5312 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1181 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1093 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1123 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py
+-rw-r--r--   0        0        0      234 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_client.py
+-rw-r--r--   0        0        0     3796 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/appstream/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:18.997327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1346 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1273 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json
+-rw-r--r--   0        0        0     1408 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1269 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1420 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/__init__.py
+-rw-r--r--   0        0        0     1363 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json
+-rw-r--r--   0        0        0     1583 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py
+-rw-r--r--   0        0        0     3619 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/__init__.py
+-rw-r--r--   0        0        0     1182 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json
+-rw-r--r--   0        0        0     1902 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py
+-rw-r--r--   0        0        0       78 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.metadata.json
+-rw-r--r--   0        0        0     1002 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_group_multiple_az/autoscaling_group_multiple_az.py
+-rw-r--r--   0        0        0     4192 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/__init__.py
+-rw-r--r--   0        0        0      204 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1198 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2548 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json
+-rw-r--r--   0        0        0     3352 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/__init__.py
+-rw-r--r--   0        0        0     1536 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json
+-rw-r--r--   0        0        0     2209 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1399 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1823 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/__init__.py
+-rw-r--r--   0        0        0     1272 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json
+-rw-r--r--   0        0        0     1058 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/__init__.py
+-rw-r--r--   0        0        0     1120 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json
+-rw-r--r--   0        0        0     1144 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json
+-rw-r--r--   0        0        0     1169 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py
+-rw-r--r--   0        0        0     7807 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/__init__.py
+-rw-r--r--   0        0        0      195 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_plans_exist/__init__.py
+-rw-r--r--   0        0        0     1194 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json
+-rw-r--r--   0        0        0      948 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_reportplans_exist/__init__.py
+-rw-r--r--   0        0        0     1167 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json
+-rw-r--r--   0        0        0     1138 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py
+-rw-r--r--   0        0        0     6996 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json
+-rw-r--r--   0        0        0     1096 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_exist/__init__.py
+-rw-r--r--   0        0        0     1132 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json
+-rw-r--r--   0        0        0      925 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_client.py
+-rw-r--r--   0        0        0     4466 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/__init__.py
+-rw-r--r--   0        0        0     1367 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json
+-rw-r--r--   0        0        0     1992 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1249 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1432 2023-05-11 14:20:19.001327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/__init__.py
+-rw-r--r--   0        0        0     1321 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json
+-rw-r--r--   0        0        0     1164 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/__init__.py
+-rw-r--r--   0        0        0     1395 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json
+-rw-r--r--   0        0        0     1721 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1230 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/__init__.py
+-rw-r--r--   0        0        0     1385 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json
+-rw-r--r--   0        0        0     1781 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json
+-rw-r--r--   0        0        0     1031 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py
+-rw-r--r--   0        0        0     6242 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json
+-rw-r--r--   0        0        0     1707 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1575 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2245 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/__init__.py
+-rw-r--r--   0        0        0     1287 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json
+-rw-r--r--   0        0        0     1073 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1951 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1524 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json
+-rw-r--r--   0        0        0     1457 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1380 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     2232 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1393 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2755 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json
+-rw-r--r--   0        0        0     1956 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/__init__.py
+-rw-r--r--   0        0        0     1537 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json
+-rw-r--r--   0        0        0     2892 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json
+-rw-r--r--   0        0        0     2894 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py
+-rw-r--r--   0        0        0     9652 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1496 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2391 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2397 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2415 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json
+-rw-r--r--   0        0        0     2600 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1249 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1002 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json
+-rw-r--r--   0        0        0     4856 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/__init__.py
+-rw-r--r--   0        0        0     1365 2023-05-11 14:20:19.005327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json
+-rw-r--r--   0        0        0     1569 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2391 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1498 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2337 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/__init__.py
+-rw-r--r--   0        0        0     1495 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json
+-rw-r--r--   0        0        0     2208 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json
+-rw-r--r--   0        0        0     3046 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/__init__.py
+-rw-r--r--   0        0        0     1560 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json
+-rw-r--r--   0        0        0     2261 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2543 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/__init__.py
+-rw-r--r--   0        0        0     1430 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json
+-rw-r--r--   0        0        0     2748 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/__init__.py
+-rw-r--r--   0        0        0     1432 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json
+-rw-r--r--   0        0        0     2228 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/__init__.py
+-rw-r--r--   0        0        0     1448 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json
+-rw-r--r--   0        0        0     2413 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json
+-rw-r--r--   0        0        0     2203 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/__init__.py
+-rw-r--r--   0        0        0     1446 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json
+-rw-r--r--   0        0        0     2208 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py
+-rw-r--r--   0        0        0    10786 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py
+-rw-r--r--   0        0        0      197 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/cloudwatch/logs_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/__init__.py
+-rw-r--r--   0        0        0     1540 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json
+-rw-r--r--   0        0        0     1665 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py
+-rw-r--r--   0        0        0    10499 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json
+-rw-r--r--   0        0        0     1241 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/__init__.py
+-rw-r--r--   0        0        0     1018 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json
+-rw-r--r--   0        0        0     1049 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py
+-rw-r--r--   0        0        0     3606 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/__init__.py
+-rw-r--r--   0        0        0      195 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/config_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json
+-rw-r--r--   0        0        0     1486 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py
+-rw-r--r--   0        0        0     3167 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/config/config_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/__init__.py
+-rw-r--r--   0        0        0     1191 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json
+-rw-r--r--   0        0        0      997 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json
+-rw-r--r--   0        0        0     1041 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json
+-rw-r--r--   0        0        0     1872 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/__init__.py
+-rw-r--r--   0        0        0     1098 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json
+-rw-r--r--   0        0        0     1660 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json
+-rw-r--r--   0        0        0     1373 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py
+-rw-r--r--   0        0        0    12175 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.009327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json
+-rw-r--r--   0        0        0     1269 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/drs_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/drs_job_exist/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json
+-rw-r--r--   0        0        0      919 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py
+-rw-r--r--   0        0        0     3629 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/drs/drs_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dax_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1594 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      957 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py
+-rw-r--r--   0        0        0      205 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_client.py
+-rw-r--r--   0        0        0     8153 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1497 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      988 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/__init__.py
+-rw-r--r--   0        0        0     1529 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json
+-rw-r--r--   0        0        0      933 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ami_public/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json
+-rw-r--r--   0        0        0      843 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1192 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json
+-rw-r--r--   0        0        0      783 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/__init__.py
+-rw-r--r--   0        0        0     1176 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json
+-rw-r--r--   0        0        0      965 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json
+-rw-r--r--   0        0        0      922 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/__init__.py
+-rw-r--r--   0        0        0     1239 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json
+-rw-r--r--   0        0        0      849 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/__init__.py
+-rw-r--r--   0        0        0     1057 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json
+-rw-r--r--   0        0        0     2037 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/__init__.py
+-rw-r--r--   0        0        0     1107 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json
+-rw-r--r--   0        0        0      971 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/__init__.py
+-rw-r--r--   0        0        0     1461 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json
+-rw-r--r--   0        0        0     1111 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/__init__.py
+-rw-r--r--   0        0        0     1174 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json
+-rw-r--r--   0        0        0     1253 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/__init__.py
+-rw-r--r--   0        0        0     1201 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json
+-rw-r--r--   0        0        0     1491 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/__init__.py
+-rw-r--r--   0        0        0     1543 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json
+-rw-r--r--   0        0        0     1034 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1141 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0     1118 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/__init__.py
+-rw-r--r--   0        0        0     1292 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json
+-rw-r--r--   0        0        0     2348 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py
+-rw-r--r--   0        0        0       78 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/fixtures/fixture
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json
+-rw-r--r--   0        0        0     1247 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1483 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1268 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1513 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1296 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json
+-rw-r--r--   0        0        0     1323 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json
+-rw-r--r--   0        0        0     1468 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/__init__.py
+-rw-r--r--   0        0        0     1169 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json
+-rw-r--r--   0        0        0     1436 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json
+-rw-r--r--   0        0        0     1409 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-11 14:20:19.013327 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json
+-rw-r--r--   0        0        0     1437 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json
+-rw-r--r--   0        0        0     1497 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json
+-rw-r--r--   0        0        0     1532 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/__init__.py
+-rw-r--r--   0        0        0     1164 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json
+-rw-r--r--   0        0        0     1427 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json
+-rw-r--r--   0        0        0     1443 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json
+-rw-r--r--   0        0        0     1486 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/__init__.py
+-rw-r--r--   0        0        0     1190 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json
+-rw-r--r--   0        0        0     1461 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/__init__.py
+-rw-r--r--   0        0        0     1173 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json
+-rw-r--r--   0        0        0     1436 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/__init__.py
+-rw-r--r--   0        0        0     1164 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json
+-rw-r--r--   0        0        0     1427 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/__init__.py
+-rw-r--r--   0        0        0     1218 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json
+-rw-r--r--   0        0        0     1499 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/__init__.py
+-rw-r--r--   0        0        0     1161 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json
+-rw-r--r--   0        0        0     1422 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/__init__.py
+-rw-r--r--   0        0        0     1127 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json
+-rw-r--r--   0        0        0     2440 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/__init__.py
+-rw-r--r--   0        0        0     1374 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json
+-rw-r--r--   0        0        0     1305 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json
+-rw-r--r--   0        0        0     1029 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/__init__.py
+-rw-r--r--   0        0        0     1043 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json
+-rw-r--r--   0        0        0     1144 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json
+-rw-r--r--   0        0        0     1219 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py
+-rw-r--r--   0        0        0    20408 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/lib/__init__.py
+-rw-r--r--   0        0        0     2581 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/lib/network_acls.py
+-rw-r--r--   0        0        0     3766 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ec2/lib/security_groups.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1375 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1568 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/__init__.py
+-rw-r--r--   0        0        0     1123 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json
+-rw-r--r--   0        0        0     1030 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1213 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1506 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json
+-rw-r--r--   0        0        0     1108 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json
+-rw-r--r--   0        0        0     2377 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py
+-rw-r--r--   0        0        0    13156 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_client.py
+-rw-r--r--   0        0        0     3857 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/__init__.py
+-rw-r--r--   0        0        0     1625 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json
+-rw-r--r--   0        0        0     2328 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/efs/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1366 2023-05-11 14:20:19.017328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      853 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1099 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      843 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1853 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py
+-rw-r--r--   0        0        0     3889 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/efs/efs_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json
+-rw-r--r--   0        0        0      992 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/__init__.py
+-rw-r--r--   0        0        0     1559 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json
+-rw-r--r--   0        0        0     1215 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/__init__.py
+-rw-r--r--   0        0        0     1374 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json
+-rw-r--r--   0        0        0     1489 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1020 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py
+-rw-r--r--   0        0        0     4579 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/eks/eks_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1115 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json
+-rw-r--r--   0        0        0      823 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1392 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      817 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py
+-rw-r--r--   0        0        0     4592 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1360 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0      937 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1347 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json
+-rw-r--r--   0        0        0      892 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/__init__.py
+-rw-r--r--   0        0        0     1718 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json
+-rw-r--r--   0        0        0     1367 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/__init__.py
+-rw-r--r--   0        0        0     1337 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json
+-rw-r--r--   0        0        0     1646 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/__init__.py
+-rw-r--r--   0        0        0     1162 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json
+-rw-r--r--   0        0        0      888 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/__init__.py
+-rw-r--r--   0        0        0      996 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json
+-rw-r--r--   0        0        0      836 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1435 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      924 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py
+-rw-r--r--   0        0        0     7882 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/__init__.py
+-rw-r--r--   0        0        0     1325 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json
+-rw-r--r--   0        0        0     1664 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/__init__.py
+-rw-r--r--   0        0        0     1004 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json
+-rw-r--r--   0        0        0     1439 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json
+-rw-r--r--   0        0        0      917 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/__init__.py
+-rw-r--r--   0        0        0      897 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json
+-rw-r--r--   0        0        0     1200 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/__init__.py
+-rw-r--r--   0        0        0     1018 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json
+-rw-r--r--   0        0        0     4444 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py
+-rw-r--r--   0        0        0     8244 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/emr/emr_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/fms_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/fms_policy_compliant/__init__.py
+-rw-r--r--   0        0        0     1001 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.metadata.json
+-rw-r--r--   0        0        0     1279 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/fms_policy_compliant/fms_policy_compliant.py
+-rw-r--r--   0        0        0     4538 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/fms/fms_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_client.py
+-rw-r--r--   0        0        0     3995 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/__init__.py
+-rw-r--r--   0        0        0     1219 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json
+-rw-r--r--   0        0        0     1940 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/globalaccelerator/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-11 14:20:19.021328 prowler-3.5.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_client.py
+-rw-r--r--   0        0        0     2362 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      928 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      920 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json
+-rw-r--r--   0        0        0      884 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1632 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1361 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1623 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1352 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1322 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1574 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1622 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1600 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1293 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1591 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1284 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py
+-rw-r--r--   0        0        0     9722 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/glue/glue_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json
+-rw-r--r--   0        0        0     1221 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py
+-rw-r--r--   0        0        0      210 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1282 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1130 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json
+-rw-r--r--   0        0        0      961 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py
+-rw-r--r--   0        0        0     7252 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/__init__.py
+-rw-r--r--   0        0        0     1010 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json
+-rw-r--r--   0        0        0     1933 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json
+-rw-r--r--   0        0        0     2805 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2227 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/__init__.py
+-rw-r--r--   0        0        0     1494 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json
+-rw-r--r--   0        0        0      802 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2238 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     2118 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     2251 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1413 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4146 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/__init__.py
+-rw-r--r--   0        0        0     1417 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json
+-rw-r--r--   0        0        0     4192 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json
+-rw-r--r--   0        0        0     2665 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/__init__.py
+-rw-r--r--   0        0        0     1707 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json
+-rw-r--r--   0        0        0     1090 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_root_access_key/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json
+-rw-r--r--   0        0        0     1541 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/__init__.py
+-rw-r--r--   0        0        0     1314 2023-05-11 14:20:19.025328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json
+-rw-r--r--   0        0        0     1360 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json
+-rw-r--r--   0        0        0     1086 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json
+-rw-r--r--   0        0        0     1185 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_number/__init__.py
+-rw-r--r--   0        0        0     1254 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json
+-rw-r--r--   0        0        0     1095 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/__init__.py
+-rw-r--r--   0        0        0     1280 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json
+-rw-r--r--   0        0        0     1231 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json
+-rw-r--r--   0        0        0     1095 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/__init__.py
+-rw-r--r--   0        0        0     1300 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json
+-rw-r--r--   0        0        0     1083 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/__init__.py
+-rw-r--r--   0        0        0     1223 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json
+-rw-r--r--   0        0        0     6229 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/__init__.py
+-rw-r--r--   0        0        0     1533 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json
+-rw-r--r--   0        0        0     1925 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/__init__.py
+-rw-r--r--   0        0        0     1384 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json
+-rw-r--r--   0        0        0     1967 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json
+-rw-r--r--   0        0        0     1954 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.metadata.json
+-rw-r--r--   0        0        0     4380 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_account_readonlyaccess_policy/iam_role_cross_account_readonlyaccess_policy.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/__init__.py
+-rw-r--r--   0        0        0     1172 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json
+-rw-r--r--   0        0        0     3534 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1595 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1020 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json
+-rw-r--r--   0        0        0     2832 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/__init__.py
+-rw-r--r--   0        0        0     1335 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json
+-rw-r--r--   0        0        0      901 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py
+-rw-r--r--   0        0        0    23835 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_support_role_created/__init__.py
+-rw-r--r--   0        0        0     1256 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json
+-rw-r--r--   0        0        0      940 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/__init__.py
+-rw-r--r--   0        0        0     1061 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json
+-rw-r--r--   0        0        0     1341 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json
+-rw-r--r--   0        0        0     1698 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/__init__.py
+-rw-r--r--   0        0        0     1671 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json
+-rw-r--r--   0        0        0     2671 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json
+-rw-r--r--   0        0        0     1341 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/inspector2/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:19.029328 prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/__init__.py
+-rw-r--r--   0        0        0     1158 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json
+-rw-r--r--   0        0        0     1256 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py
+-rw-r--r--   0        0        0     4121 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_are_used/__init__.py
+-rw-r--r--   0        0        0     1053 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json
+-rw-r--r--   0        0        0     1194 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1294 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1354 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2525 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0     5255 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/macie_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/macie_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json
+-rw-r--r--   0        0        0      894 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py
+-rw-r--r--   0        0        0     1785 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/macie/macie_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/__init__.py
+-rw-r--r--   0        0        0      249 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/networkfirewall_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.metadata.json
+-rw-r--r--   0        0        0     1138 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/networkfirewall_in_all_vpc/networkfirewall_in_all_vpc.py
+-rw-r--r--   0        0        0     3772 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/networkfirewall/networkfirewall_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/__init__.py
+-rw-r--r--   0        0        0      238 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_client.py
+-rw-r--r--   0        0        0     7268 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1124 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1102 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1478 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1871 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1555 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0     1003 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json
+-rw-r--r--   0        0        0      991 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json
+-rw-r--r--   0        0        0      983 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1766 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1281 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     2655 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/__init__.py
+-rw-r--r--   0        0        0     1736 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json
+-rw-r--r--   0        0        0     1046 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/__init__.py
+-rw-r--r--   0        0        0     1242 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json
+-rw-r--r--   0        0        0     1023 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json
+-rw-r--r--   0        0        0      984 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py
+-rw-r--r--   0        0        0      239 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/__init__.py
+-rw-r--r--   0        0        0     1579 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json
+-rw-r--r--   0        0        0     1816 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/__init__.py
+-rw-r--r--   0        0        0     1548 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json
+-rw-r--r--   0        0        0     5769 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py
+-rw-r--r--   0        0        0     8762 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/__init__.py
+-rw-r--r--   0        0        0     1047 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.metadata.json
+-rw-r--r--   0        0        0     1432 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_tags_policies_enabled_and_attached/organizations_tags_policies_enabled_and_attached.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/__init__.py
+-rw-r--r--   0        0        0     1473 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json
+-rw-r--r--   0        0        0      984 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/__init__.py
+-rw-r--r--   0        0        0     1367 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json
+-rw-r--r--   0        0        0     1578 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/__init__.py
+-rw-r--r--   0        0        0      961 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.metadata.json
+-rw-r--r--   0        0        0     1127 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deprecated_engine_version/rds_instance_deprecated_engine_version.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json
+-rw-r--r--   0        0        0      960 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/__init__.py
+-rw-r--r--   0        0        0     1488 2023-05-11 14:20:19.033328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json
+-rw-r--r--   0        0        0      947 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/__init__.py
+-rw-r--r--   0        0        0     1732 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json
+-rw-r--r--   0        0        0      969 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_multi_az/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json
+-rw-r--r--   0        0        0     1565 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/__init__.py
+-rw-r--r--   0        0        0     1426 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json
+-rw-r--r--   0        0        0      959 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json
+-rw-r--r--   0        0        0      892 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json
+-rw-r--r--   0        0        0     1419 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py
+-rw-r--r--   0        0        0    15407 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/__init__.py
+-rw-r--r--   0        0        0     1552 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json
+-rw-r--r--   0        0        0     1543 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/__init__.py
+-rw-r--r--   0        0        0      205 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/__init__.py
+-rw-r--r--   0        0        0     1384 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json
+-rw-r--r--   0        0        0      973 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json
+-rw-r--r--   0        0        0      984 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json
+-rw-r--r--   0        0        0      996 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json
+-rw-r--r--   0        0        0      992 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py
+-rw-r--r--   0        0        0     4912 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/__init__.py
+-rw-r--r--   0        0        0      261 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/__init__.py
+-rw-r--r--   0        0        0      973 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json
+-rw-r--r--   0        0        0     1012 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py
+-rw-r--r--   0        0        0     2402 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/__init__.py
+-rw-r--r--   0        0        0     1426 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.metadata.json
+-rw-r--r--   0        0        0     2170 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_dangling_ip_subdomain_takeover/route53_dangling_ip_subdomain_takeover.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/__init__.py
+-rw-r--r--   0        0        0     1188 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json
+-rw-r--r--   0        0        0     1023 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json
+-rw-r--r--   0        0        0     1058 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1362 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json
+-rw-r--r--   0        0        0     1303 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py
+-rw-r--r--   0        0        0     8478 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53_service.py
+-rw-r--r--   0        0        0      221 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/route53/route53domains_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/__init__.py
+-rw-r--r--   0        0        0     1392 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json
+-rw-r--r--   0        0        0     1068 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/__init__.py
+-rw-r--r--   0        0        0     1266 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json
+-rw-r--r--   0        0        0      957 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json
+-rw-r--r--   0        0        0      917 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/__init__.py
+-rw-r--r--   0        0        0     1496 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json
+-rw-r--r--   0        0        0     1123 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/__init__.py
+-rw-r--r--   0        0        0     1426 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json
+-rw-r--r--   0        0        0      943 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/__init__.py
+-rw-r--r--   0        0        0     1399 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.metadata.json
+-rw-r--r--   0        0        0      944 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json
+-rw-r--r--   0        0        0      947 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json
+-rw-r--r--   0        0        0     1716 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0     4014 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/__init__.py
+-rw-r--r--   0        0        0     1190 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json
+-rw-r--r--   0        0        0     2099 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/__init__.py
+-rw-r--r--   0        0        0     1372 2023-05-11 14:20:19.037328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json
+-rw-r--r--   0        0        0      978 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py
+-rw-r--r--   0        0        0      175 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_client.py
+-rw-r--r--   0        0        0    17431 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/s3/s3_service.py
+-rw-r--r--   0        0        0      196 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/s3/s3control_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0      945 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1094 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0      966 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1412 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1046 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json
+-rw-r--r--   0        0        0     1037 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1361 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1063 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json
+-rw-r--r--   0        0        0     1091 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py
+-rw-r--r--   0        0        0    11611 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1119 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1040 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json
+-rw-r--r--   0        0        0     1005 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1042 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json
+-rw-r--r--   0        0        0     1072 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1341 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1054 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py
+-rw-r--r--   0        0        0      244 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_client.py
+-rw-r--r--   0        0        0     2442 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_enabled/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json
+-rw-r--r--   0        0        0     1296 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py
+-rw-r--r--   0        0        0     4490 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/__init__.py
+-rw-r--r--   0        0        0     1051 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json
+-rw-r--r--   0        0        0     1259 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1045 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1267 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/__init__.py
+-rw-r--r--   0        0        0     1041 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json
+-rw-r--r--   0        0        0     1316 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/__init__.py
+-rw-r--r--   0        0        0     1021 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json
+-rw-r--r--   0        0        0     1271 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/__init__.py
+-rw-r--r--   0        0        0     1095 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json
+-rw-r--r--   0        0        0     1353 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/__init__.py
+-rw-r--r--   0        0        0     1020 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json
+-rw-r--r--   0        0        0     1275 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py
+-rw-r--r--   0        0        0      195 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_client.py
+-rw-r--r--   0        0        0     2527 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/shield/shield_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_client.py
+-rw-r--r--   0        0        0     3814 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json
+-rw-r--r--   0        0        0      841 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1340 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1938 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1396 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1933 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0      939 2023-05-11 14:20:19.041328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py
+-rw-r--r--   0        0        0     4137 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_document_secrets/__init__.py
+-rw-r--r--   0        0        0     1225 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json
+-rw-r--r--   0        0        0     1974 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/__init__.py
+-rw-r--r--   0        0        0     1142 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json
+-rw-r--r--   0        0        0      884 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json
+-rw-r--r--   0        0        0      993 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py
+-rw-r--r--   0        0        0     7622 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045328 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/__init__.py
+-rw-r--r--   0        0        0     1073 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json
+-rw-r--r--   0        0        0     1396 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py
+-rw-r--r--   0        0        0     6871 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/__init__.py
+-rw-r--r--   0        0        0     1132 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json
+-rw-r--r--   0        0        0     1478 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py
+-rw-r--r--   0        0        0     2972 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_different_regions/__init__.py
+-rw-r--r--   0        0        0      860 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json
+-rw-r--r--   0        0        0      949 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1094 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     3142 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/__init__.py
+-rw-r--r--   0        0        0     1173 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json
+-rw-r--r--   0        0        0     2056 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/__init__.py
+-rw-r--r--   0        0        0     1214 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json
+-rw-r--r--   0        0        0      831 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json
+-rw-r--r--   0        0        0     1496 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py
+-rw-r--r--   0        0        0    15645 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json
+-rw-r--r--   0        0        0     1285 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/__init__.py
+-rw-r--r--   0        0        0      900 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json
+-rw-r--r--   0        0        0     1441 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/waf/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/waf/waf_client.py
+-rw-r--r--   0        0        0     2645 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/waf/waf_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/wafv2/__init__.py
+-rw-r--r--   0        0        0      190 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/wafv2/wafv2_client.py
+-rw-r--r--   0        0        0     2724 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/wafv2/wafv2_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/__init__.py
+-rw-r--r--   0        0        0      215 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_client.py
+-rw-r--r--   0        0        0     3585 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json
+-rw-r--r--   0        0        0     1586 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.metadata.json
+-rw-r--r--   0        0        0     2344 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_vpc_2private_1public_subnets_nat/workspaces_vpc_2private_1public_subnets_nat.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/__init__.py
+-rw-r--r--   0        0        0     8032 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/azure_provider.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      258 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      796 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/__init__.py
+-rw-r--r--   0        0        0      205 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/__init__.py
+-rw-r--r--   0        0        0     1496 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json
+-rw-r--r--   0        0        0     1182 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/__init__.py
+-rw-r--r--   0        0        0      926 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json
+-rw-r--r--   0        0        0     1121 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1654 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1210 2023-05-11 14:20:19.045329 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/__init__.py
+-rw-r--r--   0        0        0     1561 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json
+-rw-r--r--   0        0        0     1181 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/__init__.py
+-rw-r--r--   0        0        0     1306 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/__init__.py
+-rw-r--r--   0        0        0      906 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1638 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/__init__.py
+-rw-r--r--   0        0        0     1254 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json
+-rw-r--r--   0        0        0     1122 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/__init__.py
+-rw-r--r--   0        0        0     1590 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json
+-rw-r--r--   0        0        0     1163 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/__init__.py
+-rw-r--r--   0        0        0     1187 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json
+-rw-r--r--   0        0        0     1346 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/__init__.py
+-rw-r--r--   0        0        0     1509 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json
+-rw-r--r--   0        0        0     1170 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json
+-rw-r--r--   0        0        0     1227 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/__init__.py
+-rw-r--r--   0        0        0     1693 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json
+-rw-r--r--   0        0        0     1202 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py
+-rw-r--r--   0        0        0     2326 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/defender/defender_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/iam_client.py
+-rw-r--r--   0        0        0     2696 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/__init__.py
+-rw-r--r--   0        0        0      996 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json
+-rw-r--r--   0        0        0     1330 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/__init__.py
+-rw-r--r--   0        0        0     1470 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py
+-rw-r--r--   0        0        0      200 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/__init__.py
+-rw-r--r--   0        0        0     1354 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1265 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1399 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1156 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json
+-rw-r--r--   0        0        0     1151 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1093 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1169 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/__init__.py
+-rw-r--r--   0        0        0     1272 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json
+-rw-r--r--   0        0        0     1166 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py
+-rw-r--r--   0        0        0     3651 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/azure/services/storage/storage_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/allowlist.py
+-rw-r--r--   0        0        0    17566 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/audit_info.py
+-rw-r--r--   0        0        0      251 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/models.py
+-rw-r--r--   0        0        0     4693 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/outputs.py
+-rw-r--r--   0        0        0      885 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/common/quick_inventory.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/__init__.py
+-rw-r--r--   0        0        0     1695 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/gcp_provider.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/lib/audit_info/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/lib/audit_info/audit_info.py
+-rw-r--r--   0        0        0      522 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/lib/audit_info/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1445 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      996 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/__init__.py
+-rw-r--r--   0        0        0     1314 2023-05-11 14:20:19.049328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json
+-rw-r--r--   0        0        0      948 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py
+-rw-r--r--   0        0        0     4116 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/__init__.py
+-rw-r--r--   0        0        0     1373 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json
+-rw-r--r--   0        0        0      974 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudresourcemanager/__init__.py
+-rw-r--r--   0        0        0      266 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_client.py
+-rw-r--r--   0        0        0     1262 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/__init__.py
+-rw-r--r--   0        0        0     1408 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json
+-rw-r--r--   0        0        0     1011 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/__init__.py
+-rw-r--r--   0        0        0     1359 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json
+-rw-r--r--   0        0        0     1182 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/__init__.py
+-rw-r--r--   0        0        0     1216 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json
+-rw-r--r--   0        0        0     1203 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/__init__.py
+-rw-r--r--   0        0        0     2058 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json
+-rw-r--r--   0        0        0     1302 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1207 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/__init__.py
+-rw-r--r--   0        0        0     1447 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json
+-rw-r--r--   0        0        0     1219 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/__init__.py
+-rw-r--r--   0        0        0     1618 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json
+-rw-r--r--   0        0        0     1310 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1442 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1323 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1955 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1466 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/__init__.py
+-rw-r--r--   0        0        0     1745 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json
+-rw-r--r--   0        0        0     1410 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/__init__.py
+-rw-r--r--   0        0        0     1326 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json
+-rw-r--r--   0        0        0     1368 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/__init__.py
+-rw-r--r--   0        0        0     1151 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json
+-rw-r--r--   0        0        0     1104 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/__init__.py
+-rw-r--r--   0        0        0     1492 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json
+-rw-r--r--   0        0        0     1046 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1319 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      991 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/__init__.py
+-rw-r--r--   0        0        0     2153 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json
+-rw-r--r--   0        0        0     1350 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/__init__.py
+-rw-r--r--   0        0        0     1702 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json
+-rw-r--r--   0        0        0     1232 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json
+-rw-r--r--   0        0        0     1319 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/__init__.py
+-rw-r--r--   0        0        0     1860 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json
+-rw-r--r--   0        0        0     1201 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/__init__.py
+-rw-r--r--   0        0        0     2002 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json
+-rw-r--r--   0        0        0     1190 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/__init__.py
+-rw-r--r--   0        0        0     2238 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json
+-rw-r--r--   0        0        0     1210 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json
+-rw-r--r--   0        0        0     1179 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/__init__.py
+-rw-r--r--   0        0        0     1428 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json
+-rw-r--r--   0        0        0      977 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py
+-rw-r--r--   0        0        0     2467 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/__init__.py
+-rw-r--r--   0        0        0     1351 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json
+-rw-r--r--   0        0        0      926 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/__init__.py
+-rw-r--r--   0        0        0     1270 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json
+-rw-r--r--   0        0        0     1067 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py
+-rw-r--r--   0        0        0      226 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_client.py
+-rw-r--r--   0        0        0     2099 2023-05-11 14:20:19.053328 prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/__init__.py
+-rw-r--r--   0        0        0     1327 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json
+-rw-r--r--   0        0        0      897 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/__init__.py
+-rw-r--r--   0        0        0     1132 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json
+-rw-r--r--   0        0        0      827 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py
+-rw-r--r--   0        0        0     3489 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/compute/compute_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json
+-rw-r--r--   0        0        0     1395 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/__init__.py
+-rw-r--r--   0        0        0     1363 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json
+-rw-r--r--   0        0        0     1038 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/__init__.py
+-rw-r--r--   0        0        0     1133 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json
+-rw-r--r--   0        0        0     1317 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py
+-rw-r--r--   0        0        0     3292 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/iam/iam_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/__init__.py
+-rw-r--r--   0        0        0      172 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/__init__.py
+-rw-r--r--   0        0        0     1195 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json
+-rw-r--r--   0        0        0     1000 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json
+-rw-r--r--   0        0        0     1135 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py
+-rw-r--r--   0        0        0     4837 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/kms/kms_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_client.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1438 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1996 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1243 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1971 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1239 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2090 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1590 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2288 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1212 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     1955 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1233 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2086 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1113 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2188 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/__init__.py
+-rw-r--r--   0        0        0     1157 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json
+-rw-r--r--   0        0        0     2019 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py
+-rw-r--r--   0        0        0     2577 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_service.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_sink_created/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json
+-rw-r--r--   0        0        0     1473 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/monitoring/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/monitoring/monitoring_client.py
+-rw-r--r--   0        0        0     1893 2023-05-11 14:20:19.057327 prowler-3.5.0/prowler/providers/gcp/services/monitoring/monitoring_service.py
+-rw-r--r--   0        0        0     2458 2023-05-11 14:20:41.845398 prowler-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    15201 1970-01-01 00:00:00.000000 prowler-3.5.0/PKG-INFO
```

### Comparing `prowler-3.4.1/LICENSE` & `prowler-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/README.md` & `prowler-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/__main__.py` & `prowler-3.5.0/prowler/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
+import os
 import sys
 
 from prowler.lib.banner import print_banner
 from prowler.lib.check.check import (
     bulk_load_checks_metadata,
     bulk_load_compliance_frameworks,
     exclude_checks_to_run,
@@ -25,14 +26,15 @@
 from prowler.lib.check.compliance import update_checks_metadata_with_compliance
 from prowler.lib.cli.parser import ProwlerArgumentParser
 from prowler.lib.logger import logger, set_logging_config
 from prowler.lib.outputs.compliance import display_compliance_table
 from prowler.lib.outputs.html import add_html_footer, fill_html_overview_statistics
 from prowler.lib.outputs.json import close_json
 from prowler.lib.outputs.outputs import extract_findings_statistics, send_to_s3_bucket
+from prowler.lib.outputs.slack import send_slack_message
 from prowler.lib.outputs.summary_table import display_summary_table
 from prowler.providers.aws.lib.security_hub.security_hub import (
     resolve_security_hub_previous_findings,
 )
 from prowler.providers.common.allowlist import set_provider_allowlist
 from prowler.providers.common.audit_info import (
     set_provider_audit_info,
@@ -165,14 +167,29 @@
         logger.error(
             "There are no checks to execute. Please, check your input arguments"
         )
 
     # Extract findings stats
     stats = extract_findings_statistics(findings)
 
+    if args.slack:
+        if "SLACK_API_TOKEN" in os.environ and "SLACK_CHANNEL_ID" in os.environ:
+            _ = send_slack_message(
+                os.environ["SLACK_API_TOKEN"],
+                os.environ["SLACK_CHANNEL_ID"],
+                stats,
+                provider,
+                audit_info,
+            )
+        else:
+            logger.critical(
+                "Slack integration needs SLACK_API_TOKEN and SLACK_CHANNEL_ID environment variables (see more in https://docs.prowler.cloud/en/latest/tutorials/integrations/#slack)."
+            )
+            sys.exit(1)
+
     if args.output_modes:
         for mode in args.output_modes:
             # Close json file if exists
             if mode == "json" or mode == "json-asff":
                 close_json(
                     audit_output_options.output_filename, args.output_directory, mode
                 )
```

### Comparing `prowler-3.4.1/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json` & `prowler-3.5.0/prowler/compliance/aws/aws_audit_manager_control_tower_guardrails_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json` & `prowler-3.5.0/prowler/compliance/aws/aws_foundational_security_best_practices_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/cis_1.4_aws.json` & `prowler-3.5.0/prowler/compliance/aws/cis_1.4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/cis_1.5_aws.json` & `prowler-3.5.0/prowler/compliance/aws/cis_1.5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/cisa_aws.json` & `prowler-3.5.0/prowler/compliance/aws/cisa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/ens_rd2022_aws.json` & `prowler-3.5.0/prowler/compliance/aws/ens_rd2022_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/fedramp_low_revision_4_aws.json` & `prowler-3.5.0/prowler/compliance/aws/fedramp_low_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json` & `prowler-3.5.0/prowler/compliance/aws/fedramp_moderate_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/ffiec_aws.json` & `prowler-3.5.0/prowler/compliance/aws/ffiec_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/gdpr_aws.json` & `prowler-3.5.0/prowler/compliance/aws/gdpr_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json` & `prowler-3.5.0/prowler/compliance/aws/gxp_21_cfr_part_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/gxp_eu_annex_11_aws.json` & `prowler-3.5.0/prowler/compliance/aws/gxp_eu_annex_11_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/hipaa_aws.json` & `prowler-3.5.0/prowler/compliance/aws/hipaa_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/nist_800_171_revision_2_aws.json` & `prowler-3.5.0/prowler/compliance/aws/nist_800_171_revision_2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/nist_800_53_revision_4_aws.json` & `prowler-3.5.0/prowler/compliance/aws/nist_800_53_revision_4_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/nist_800_53_revision_5_aws.json` & `prowler-3.5.0/prowler/compliance/aws/nist_800_53_revision_5_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/nist_csf_1.1_aws.json` & `prowler-3.5.0/prowler/compliance/aws/nist_csf_1.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/pci_3.2.1_aws.json` & `prowler-3.5.0/prowler/compliance/aws/pci_3.2.1_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/rbi_cyber_security_framework_aws.json` & `prowler-3.5.0/prowler/compliance/aws/rbi_cyber_security_framework_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/compliance/aws/soc2_aws.json` & `prowler-3.5.0/prowler/compliance/aws/soc2_aws.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/config/allowlist.yaml` & `prowler-3.5.0/prowler/config/allowlist.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-### Account, Check and/or Region can be * to apply for all the cases
-### Resources is a list that can have either Regex or Keywords
-### Tags is an optional list containing tuples of 'key=value'
+### Account, Check and/or Region can be * to apply for all the cases.
+### Resources and tags are lists that can have either Regex or Keywords.
+### Tags is an optional list that matches on tuples of 'key=value' and are "ANDed" together.
+### Use an alternation Regex to match one of multiple tags with "ORed" logic.
 ###########################  ALLOWLIST EXAMPLE  ###########################
 Allowlist:
   Accounts:
     "123456789012":
       Checks:
         "iam_user_hardware_mfa_enabled":
           Regions:
             - "us-east-1"
           Resources:
             - "user-1"           # Will ignore user-1 in check iam_user_hardware_mfa_enabled
             - "user-2"           # Will ignore user-2 in check iam_user_hardware_mfa_enabled
+        "ec2_*":
+          Regions:
+            - "*"
+          Resources:
+            - "*"                 # Will ignore every EC2 check in every account and region
         "*":
           Regions:
             - "*"
           Resources:
-            - "test"             # Will ignore every resource containing the string "test" and the tags 'test=test' and 'project=test' in account 123456789012 and every region
+            - "test"
           Tags:
-            - "test=test"        # Will ignore every resource containing the string "test" and the tags 'test=test' and 'project=test' in account 123456789012 and every region
-            - "project=test"
+            - "test=test"         # Will ignore every resource containing the string "test" and the tags 'test=test' and
+            - "project=test|project=stage" # either of ('project=test' OR project=stage) in account 123456789012 and every region
 
     "*":
       Checks:
         "s3_bucket_object_versioning":
           Regions:
             - "eu-west-1"
             - "us-east-1"
```

### Comparing `prowler-3.4.1/prowler/config/config.py` & `prowler-3.5.0/prowler/config/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 import requests
 import yaml
 
 from prowler.lib.logger import logger
 
 timestamp = datetime.today()
 timestamp_utc = datetime.now(timezone.utc).replace(tzinfo=timezone.utc)
-prowler_version = "3.4.1"
+prowler_version = "3.5.0"
 html_logo_url = "https://github.com/prowler-cloud/prowler/"
 html_logo_img = "https://user-images.githubusercontent.com/3985464/113734260-7ba06900-96fb-11eb-82bc-d4f68a1e2710.png"
+square_logo_img = "https://user-images.githubusercontent.com/38561120/235905862-9ece5bd7-9aa3-4e48-807a-3a9035eb8bfb.png"
+aws_logo = "https://user-images.githubusercontent.com/38561120/235953920-3e3fba08-0795-41dc-b480-9bea57db9f2e.png"
+azure_logo = "https://user-images.githubusercontent.com/38561120/235927375-b23e2e0f-8932-49ec-b59c-d89f61c8041d.png"
+gcp_logo = "https://user-images.githubusercontent.com/38561120/235928332-eb4accdc-c226-4391-8e97-6ca86a91cf50.png"
 
 orange_color = "\033[38;5;208m"
 banner_color = "\033[1;92m"
 
 # Compliance
 actual_directory = pathlib.Path(os.path.dirname(os.path.realpath(__file__)))
 compliance_aws_dir = f"{actual_directory}/../compliance/aws"
```

### Comparing `prowler-3.4.1/prowler/config/config.yaml` & `prowler-3.5.0/prowler/config/config.yaml`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/banner.py` & `prowler-3.5.0/prowler/lib/banner.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/check/check.py` & `prowler-3.5.0/prowler/lib/check/check.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/check/checks_loader.py` & `prowler-3.5.0/prowler/lib/check/checks_loader.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/check/compliance.py` & `prowler-3.5.0/prowler/lib/check/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/check/compliance_models.py` & `prowler-3.5.0/prowler/lib/check/compliance_models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/check/models.py` & `prowler-3.5.0/prowler/lib/check/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/cli/parser.py` & `prowler-3.5.0/prowler/lib/cli/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,19 @@
             "--ignore-exit-code-3",
             action="store_true",
             help="Failed checks do not trigger exit code 3",
         )
         common_outputs_parser.add_argument(
             "-b", "--no-banner", action="store_true", help="Hide Prowler banner"
         )
+        common_outputs_parser.add_argument(
+            "--slack",
+            action="store_true",
+            help="Send a summary of the execution with a Slack APP in your channel. Environment variables SLACK_API_TOKEN and SLACK_CHANNEL_ID are required (see more in https://docs.prowler.cloud/en/latest/tutorials/integrations/#slack).",
+        )
 
     def __init_logging_parser__(self):
         # Logging Options
         # Both options can be combined to only report to file some log level
         common_logging_parser = self.common_providers_parser.add_argument_group(
             "Logging"
         )
```

### Comparing `prowler-3.4.1/prowler/lib/logger.py` & `prowler-3.5.0/prowler/lib/logger.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/compliance.py` & `prowler-3.5.0/prowler/lib/outputs/compliance.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/file_descriptors.py` & `prowler-3.5.0/prowler/lib/outputs/file_descriptors.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/html.py` & `prowler-3.5.0/prowler/lib/outputs/html.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/json.py` & `prowler-3.5.0/prowler/lib/outputs/json.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/models.py` & `prowler-3.5.0/prowler/lib/outputs/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,14 @@
 def generate_provider_output_csv(
     provider: str, finding, audit_info, mode: str, fd, output_options
 ):
     """
     set_provider_output_options configures automatically the outputs based on the selected provider and returns the Provider_Output_Options object.
     """
     try:
-        finding_output_model = f"{provider.capitalize()}_Check_Output_{mode.upper()}"
-        output_model = getattr(importlib.import_module(__name__), finding_output_model)
         # Dynamically load the Provider_Output_Options class
         finding_output_model = f"{provider.capitalize()}_Check_Output_{mode.upper()}"
         output_model = getattr(importlib.import_module(__name__), finding_output_model)
         # Fill common data among providers
         data = fill_common_data_csv(finding)
 
         if provider == "azure":
```

### Comparing `prowler-3.4.1/prowler/lib/outputs/outputs.py` & `prowler-3.5.0/prowler/lib/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/outputs/summary_table.py` & `prowler-3.5.0/prowler/lib/outputs/summary_table.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/scan_filters/scan_filters.py` & `prowler-3.5.0/prowler/lib/scan_filters/scan_filters.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/lib/utils/utils.py` & `prowler-3.5.0/prowler/lib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/aws_provider.py` & `prowler-3.5.0/prowler/providers/aws/aws_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/aws_regions_by_service.json` & `prowler-3.5.0/prowler/providers/aws/aws_regions_by_service.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992829658575515%*

 * *Differences: {"'services'": "{'aps': {'regions': {'aws': {insert: [(1, 'ap-northeast-2'), (2, 'ap-south-1'), "*

 * *               "(9, 'eu-west-3'), (10, 'sa-east-1')]}}}, 'arc-zonal-shift': {'regions': {'aws': "*

 * *               "{insert: [(25, 'us-west-1')]}}}, 'codepipeline': {'regions': {'aws-us-gov': "*

 * *               "{insert: [(0, 'us-gov-east-1')]}}}, 'emr-serverless': {'regions': {'aws': {insert: "*

 * *               "[(0, 'ap-east-1'), (12, 'me-south-1')]}, 'aws-cn': ['cn-north-1', "*

 * *               "'cn-northwest-1']}},  […]*

```diff
@@ -732,20 +732,24 @@
                 "aws-us-gov": []
             }
         },
         "aps": {
             "regions": {
                 "aws": [
                     "ap-northeast-1",
+                    "ap-northeast-2",
+                    "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-west-1",
                     "eu-west-2",
+                    "eu-west-3",
+                    "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-2"
                 ],
                 "aws-cn": [],
                 "aws-us-gov": []
             }
@@ -774,14 +778,15 @@
                     "eu-west-2",
                     "eu-west-3",
                     "me-central-1",
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
+                    "us-west-1",
                     "us-west-2"
                 ],
                 "aws-cn": [],
                 "aws-us-gov": []
             }
         },
         "artifact": {
@@ -1933,14 +1938,15 @@
                     "us-west-2"
                 ],
                 "aws-cn": [
                     "cn-north-1",
                     "cn-northwest-1"
                 ],
                 "aws-us-gov": [
+                    "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
         "codestar": {
             "regions": {
                 "aws": [
@@ -3417,32 +3423,37 @@
                     "us-gov-west-1"
                 ]
             }
         },
         "emr-serverless": {
             "regions": {
                 "aws": [
+                    "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
+                    "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
-                "aws-cn": [],
+                "aws-cn": [
+                    "cn-north-1",
+                    "cn-northwest-1"
+                ],
                 "aws-us-gov": []
             }
         },
         "es": {
             "regions": {
                 "aws": [
                     "af-south-1",
@@ -4921,14 +4932,29 @@
                     "us-east-1",
                     "us-west-2"
                 ],
                 "aws-cn": [],
                 "aws-us-gov": []
             }
         },
+        "ivs-realtime": {
+            "regions": {
+                "aws": [
+                    "ap-northeast-1",
+                    "ap-northeast-2",
+                    "ap-south-1",
+                    "eu-central-1",
+                    "eu-west-1",
+                    "us-east-1",
+                    "us-west-2"
+                ],
+                "aws-cn": [],
+                "aws-us-gov": []
+            }
+        },
         "ivschat": {
             "regions": {
                 "aws": [
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-south-1",
                     "eu-central-1",
@@ -5090,14 +5116,15 @@
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-south-2",
                     "eu-west-1",
@@ -5275,29 +5302,33 @@
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-southeast-1",
                     "ap-southeast-2",
+                    "ap-southeast-3",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-west-1",
                     "eu-west-2",
                     "eu-west-3",
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
-                "aws-cn": [],
+                "aws-cn": [
+                    "cn-north-1",
+                    "cn-northwest-1"
+                ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
         "lex-models": {
@@ -5419,15 +5450,18 @@
                     "me-south-1",
                     "sa-east-1",
                     "us-east-1",
                     "us-east-2",
                     "us-west-1",
                     "us-west-2"
                 ],
-                "aws-cn": [],
+                "aws-cn": [
+                    "cn-north-1",
+                    "cn-northwest-1"
+                ],
                 "aws-us-gov": []
             }
         },
         "license-manager-user-subscriptions": {
             "regions": {
                 "aws": [
                     "af-south-1",
@@ -6588,14 +6622,32 @@
                 ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
+        "osis": {
+            "regions": {
+                "aws": [
+                    "ap-northeast-1",
+                    "ap-southeast-1",
+                    "ap-southeast-2",
+                    "eu-central-1",
+                    "eu-west-1",
+                    "eu-west-2",
+                    "us-east-1",
+                    "us-east-2",
+                    "us-west-1",
+                    "us-west-2"
+                ],
+                "aws-cn": [],
+                "aws-us-gov": []
+            }
+        },
         "outposts": {
             "regions": {
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
@@ -7558,14 +7610,15 @@
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
                     "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
+                    "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
                     "eu-north-1",
                     "eu-south-1",
                     "eu-south-2",
                     "eu-west-1",
@@ -7798,14 +7851,15 @@
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
                     "ap-northeast-3",
                     "ap-south-1",
+                    "ap-south-2",
                     "ap-southeast-1",
                     "ap-southeast-2",
                     "ap-southeast-3",
                     "ap-southeast-4",
                     "ca-central-1",
                     "eu-central-1",
                     "eu-central-2",
@@ -8872,38 +8926,14 @@
                 ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
-        "sumerian": {
-            "regions": {
-                "aws": [
-                    "ap-northeast-1",
-                    "ap-northeast-2",
-                    "ap-south-1",
-                    "ap-southeast-1",
-                    "ap-southeast-2",
-                    "ca-central-1",
-                    "eu-central-1",
-                    "eu-north-1",
-                    "eu-west-1",
-                    "eu-west-2",
-                    "eu-west-3",
-                    "sa-east-1",
-                    "us-east-1",
-                    "us-east-2",
-                    "us-west-1",
-                    "us-west-2"
-                ],
-                "aws-cn": [],
-                "aws-us-gov": []
-            }
-        },
         "support": {
             "regions": {
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
@@ -9265,14 +9295,32 @@
                 ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
+        "verified-access": {
+            "regions": {
+                "aws": [
+                    "ap-southeast-2",
+                    "ca-central-1",
+                    "eu-central-1",
+                    "eu-west-1",
+                    "eu-west-2",
+                    "sa-east-1",
+                    "us-east-1",
+                    "us-east-2",
+                    "us-west-1",
+                    "us-west-2"
+                ],
+                "aws-cn": [],
+                "aws-us-gov": []
+            }
+        },
         "vmwarecloudonaws": {
             "regions": {
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
@@ -9354,14 +9402,29 @@
                 ],
                 "aws-us-gov": [
                     "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
+        "vpc-lattice": {
+            "regions": {
+                "aws": [
+                    "ap-northeast-1",
+                    "ap-southeast-1",
+                    "ap-southeast-2",
+                    "eu-west-1",
+                    "us-east-1",
+                    "us-east-2",
+                    "us-west-2"
+                ],
+                "aws-cn": [],
+                "aws-us-gov": []
+            }
+        },
         "vpn": {
             "regions": {
                 "aws": [
                     "af-south-1",
                     "ap-east-1",
                     "ap-northeast-1",
                     "ap-northeast-2",
@@ -9639,14 +9702,15 @@
                     "us-east-1",
                     "us-west-2"
                 ],
                 "aws-cn": [
                     "cn-northwest-1"
                 ],
                 "aws-us-gov": [
+                    "us-gov-east-1",
                     "us-gov-west-1"
                 ]
             }
         },
         "workspaces-web": {
             "regions": {
                 "aws": [
```

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/allowlist/allowlist.py` & `prowler-3.5.0/prowler/providers/aws/lib/allowlist/allowlist.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,27 +126,41 @@
             f"{error.__class__.__name__} -- {error}[{error.__traceback__.tb_lineno}]"
         )
         sys.exit(1)
 
 
 def is_allowlisted_in_check(allowlist, audited_account, check, region, resource, tags):
     try:
-        # If there is a *, it affects to all checks
-        if "*" in allowlist["Accounts"][audited_account]["Checks"]:
-            check = "*"
-            if is_allowlisted_in_region(
-                allowlist, audited_account, check, region, resource, tags
-            ):
-                return True
-        # Check if there is the specific check
-        if check in allowlist["Accounts"][audited_account]["Checks"]:
-            if is_allowlisted_in_region(
-                allowlist, audited_account, check, region, resource, tags
-            ):
-                return True
+        for allowlisted_check in allowlist["Accounts"][audited_account][
+            "Checks"
+        ].keys():
+            # If there is a *, it affects to all checks
+            if "*" == allowlisted_check:
+                check = "*"
+                if is_allowlisted_in_region(
+                    allowlist, audited_account, check, region, resource, tags
+                ):
+                    return True
+            # Check if there is the specific check
+            elif check == allowlisted_check:
+                if is_allowlisted_in_region(
+                    allowlist, audited_account, check, region, resource, tags
+                ):
+                    return True
+            # Check if check is a regex
+            elif re.search(allowlisted_check, check):
+                if is_allowlisted_in_region(
+                    allowlist,
+                    audited_account,
+                    allowlisted_check,
+                    region,
+                    resource,
+                    tags,
+                ):
+                    return True
         return False
     except Exception as error:
         logger.critical(
             f"{error.__class__.__name__} -- {error}[{error.__traceback__.tb_lineno}]"
         )
         sys.exit(1)
 
@@ -188,21 +202,29 @@
     try:
         # Check if it is an *
         if elem == "*":
             elem = ".*"
         # Check if there are allowlisted tags
         if "Tags" in check_allowlist:
             # Check if there are resource tags
-            if tags:
-                tags_in_resource_tags = True
-                for tag in check_allowlist["Tags"]:
-                    if tag not in tags:
-                        tags_in_resource_tags = False
-                if tags_in_resource_tags and re.search(elem, resource):
-                    return True
+            if not tags or not re.search(elem, resource):
+                return False
+
+            all_allowed_tags_in_resource_tags = True
+            for allowed_tag in check_allowlist["Tags"]:
+                found_allowed_tag = False
+                for resource_tag in tags:
+                    if re.search(allowed_tag, resource_tag):
+                        found_allowed_tag = True
+                        break
+
+                if not found_allowed_tag:
+                    all_allowed_tags_in_resource_tags = False
+
+            return all_allowed_tags_in_resource_tags
         else:
             if re.search(elem, resource):
                 return True
     except Exception as error:
         logger.critical(
             f"{error.__class__.__name__} -- {error}[{error.__traceback__.tb_lineno}]"
         )
```

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/arn/arn.py` & `prowler-3.5.0/prowler/providers/aws/lib/arn/arn.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/arn/error.py` & `prowler-3.5.0/prowler/providers/aws/lib/arn/error.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/audit_info/audit_info.py` & `prowler-3.5.0/prowler/providers/aws/lib/audit_info/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/audit_info/models.py` & `prowler-3.5.0/prowler/providers/aws/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/quick_inventory/quick_inventory.py` & `prowler-3.5.0/prowler/providers/aws/lib/quick_inventory/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py` & `prowler-3.5.0/prowler/providers/aws/lib/resource_api_tagging/resource_api_tagging.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/lib/security_hub/security_hub.py` & `prowler-3.5.0/prowler/providers/aws/lib/security_hub/security_hub.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled/accessanalyzer_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py` & `prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_enabled_without_findings/accessanalyzer_enabled_without_findings.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py` & `prowler-3.5.0/prowler/providers/aws/services/accessanalyzer/accessanalyzer_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import threading
 from typing import Optional
 
+from botocore.exceptions import ClientError
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
@@ -75,18 +76,29 @@
     def __get_finding_status__(self):
         logger.info("AccessAnalyzer - Get Finding status...")
         try:
             for analyzer in self.analyzers:
                 if analyzer.status == "ACTIVE":
                     regional_client = self.regional_clients[analyzer.region]
                     for finding in analyzer.findings:
-                        finding_information = regional_client.get_finding(
-                            analyzerArn=analyzer.arn, id=finding.id
-                        )
-                        finding.status = finding_information["finding"]["status"]
+                        try:
+                            finding_information = regional_client.get_finding(
+                                analyzerArn=analyzer.arn, id=finding.id
+                            )
+                            finding.status = finding_information["finding"]["status"]
+                        except ClientError as error:
+                            if (
+                                error.response["Error"]["Code"]
+                                == "ResourceNotFoundException"
+                            ):
+                                logger.warning(
+                                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                                )
+                                finding.status = ""
+                            continue
 
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __list_findings__(self):
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py` & `prowler-3.5.0/prowler/providers/aws/services/account/account_maintain_current_contact_details/account_maintain_current_contact_details.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py` & `prowler-3.5.0/prowler/providers/aws/services/account/account_security_contact_information_is_registered/account_security_contact_information_is_registered.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py` & `prowler-3.5.0/prowler/providers/aws/services/account/account_security_questions_are_registered_in_the_aws_account/account_security_questions_are_registered_in_the_aws_account.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/account/account_service.py` & `prowler-3.5.0/prowler/providers/aws/services/account/account_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py` & `prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_expiration_check/acm_certificates_expiration_check.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/acm/acm_certificates_transparency_logs_enabled/acm_certificates_transparency_logs_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/acm/acm_service.py` & `prowler-3.5.0/prowler/providers/aws/services/acm/acm_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_authorizers_enabled/apigateway_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_client_certificate_enabled/apigateway_client_certificate_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_endpoint_public/apigateway_endpoint_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_logging_enabled/apigateway_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_service.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py` & `prowler-3.5.0/prowler/providers/aws/services/apigateway/apigateway_waf_acl_attached/apigateway_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_access_logging_enabled/apigatewayv2_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_authorizers_enabled/apigatewayv2_authorizers_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py` & `prowler-3.5.0/prowler/providers/aws/services/apigatewayv2/apigatewayv2_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
             t.start()
         for t in threads:
             t.join()
 
     def __get_apis__(self, regional_client):
         logger.info("APIGatewayv2 - Getting APIs...")
         try:
-            get_rest_apis_paginator = regional_client.get_paginator("get_apis")
-            for page in get_rest_apis_paginator.paginate():
+            get_apis_paginator = regional_client.get_paginator("get_apis")
+            for page in get_apis_paginator.paginate():
                 for apigw in page["Items"]:
                     if not self.audit_resources or (
                         is_resource_filtered(apigw["ApiId"], self.audit_resources)
                     ):
                         self.apis.append(
                             API(
                                 id=apigw["ApiId"],
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_default_internet_access_disabled/appstream_fleet_default_internet_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_maximum_session_duration/appstream_fleet_maximum_session_duration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_disconnect_timeout/appstream_fleet_session_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_fleet_session_idle_disconnect_timeout/appstream_fleet_session_idle_disconnect_timeout.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/appstream/appstream_service.py` & `prowler-3.5.0/prowler/providers/aws/services/appstream/appstream_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.metadata.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'ResourceIdTemplate'": "'arn:partition:autoscaling:region:account-id:autoScalingGroupName/resource-name'"}*

```diff
@@ -21,14 +21,14 @@
             "Terraform": ""
         },
         "Recommendation": {
             "Text": "Do not include sensitive information in user data within the launch configuration, try to use Secrets Manager instead.",
             "Url": "https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html"
         }
     },
-    "ResourceIdTemplate": "arn:partition:access-analyzer:region:account-id:analyzer/resource-id",
+    "ResourceIdTemplate": "arn:partition:autoscaling:region:account-id:autoScalingGroupName/resource-name",
     "ResourceType": "Other",
     "Risk": "The use of a hard-coded password increases the possibility of password guessing.  If hard-coded passwords are used, it is possible that malicious users gain access through the account in question.",
     "ServiceName": "autoscaling",
     "Severity": "critical",
     "SubServiceName": ""
 }
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py` & `prowler-3.5.0/prowler/providers/aws/services/autoscaling/autoscaling_find_secrets_ec2_launch_configuration/autoscaling_find_secrets_ec2_launch_configuration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/autoscaling/autoscaling_service.py` & `prowler-3.5.0/prowler/providers/aws/services/wafv2/wafv2_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,66 +3,73 @@
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
-################## AutoScaling
-class AutoScaling:
+################### WAFv2
+class WAFv2:
     def __init__(self, audit_info):
-        self.service = "autoscaling"
+        self.service = "wafv2"
         self.session = audit_info.audit_session
-        self.audited_account = audit_info.audited_account
         self.audit_resources = audit_info.audit_resources
         self.regional_clients = generate_regional_clients(self.service, audit_info)
-        self.launch_configurations = []
-        self.__threading_call__(self.__describe_launch_configurations__)
+        self.web_acls = []
+        self.__threading_call__(self.__list_web_acls__)
+        self.__threading_call__(self.__list_resources_for_web_acl__)
 
     def __get_session__(self):
         return self.session
 
     def __threading_call__(self, call):
         threads = []
         for regional_client in self.regional_clients.values():
             threads.append(threading.Thread(target=call, args=(regional_client,)))
         for t in threads:
             t.start()
         for t in threads:
             t.join()
 
-    def __describe_launch_configurations__(self, regional_client):
-        logger.info("AutoScaling - Describing Launch Configurations...")
+    def __list_web_acls__(self, regional_client):
+        logger.info("WAFv2 - Listing Regional Web ACLs...")
         try:
-            describe_launch_configurations_paginator = regional_client.get_paginator(
-                "describe_launch_configurations"
-            )
-            for page in describe_launch_configurations_paginator.paginate():
-                for configuration in page["LaunchConfigurations"]:
-                    if not self.audit_resources or (
-                        is_resource_filtered(
-                            configuration["LaunchConfigurationARN"],
-                            self.audit_resources,
-                        )
-                    ):
-                        self.launch_configurations.append(
-                            LaunchConfiguration(
-                                arn=configuration["LaunchConfigurationARN"],
-                                name=configuration["LaunchConfigurationName"],
-                                user_data=configuration["UserData"],
-                                image_id=configuration["ImageId"],
-                                region=regional_client.region,
-                            )
+            for wafv2 in regional_client.list_web_acls(Scope="REGIONAL")["WebACLs"]:
+                if not self.audit_resources or (
+                    is_resource_filtered(wafv2["ARN"], self.audit_resources)
+                ):
+                    self.web_acls.append(
+                        WebAclv2(
+                            arn=wafv2["ARN"],
+                            name=wafv2["Name"],
+                            id=wafv2["Id"],
+                            albs=[],
+                            region=regional_client.region,
                         )
+                    )
+        except Exception as error:
+            logger.error(
+                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
+    def __list_resources_for_web_acl__(self, regional_client):
+        logger.info("WAFv2 - Describing resources...")
+        try:
+            for acl in self.web_acls:
+                if acl.region == regional_client.region:
+                    for resource in regional_client.list_resources_for_web_acl(
+                        WebACLArn=acl.arn, ResourceType="APPLICATION_LOAD_BALANCER"
+                    )["ResourceArns"]:
+                        acl.albs.append(resource)
 
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
 
-class LaunchConfiguration(BaseModel):
+class WebAclv2(BaseModel):
     arn: str
     name: str
-    user_data: str
-    image_id: str
+    id: str
+    albs: list[str]
     region: str
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled/awslambda_function_invoke_api_operations_cloudtrail_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_code/awslambda_function_no_secrets_in_code.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_no_secrets_in_variables/awslambda_function_no_secrets_in_variables.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_not_publicly_accessible/awslambda_function_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_cors_policy/awslambda_function_url_cors_policy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_url_public/awslambda_function_url_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_function_using_supported_runtimes/awslambda_function_using_supported_runtimes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/awslambda/awslambda_service.py` & `prowler-3.5.0/prowler/providers/aws/services/awslambda/awslambda_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'Severity'": "'low'"}*

```diff
@@ -25,10 +25,10 @@
             "Url": ""
         }
     },
     "ResourceIdTemplate": "arn:partition:service:region:account-id:backup-plan:backup-plan-id",
     "ResourceType": "AwsBackupBackupPlan",
     "Risk": "Without a backup plan, an organization may be at risk of losing important data due to accidental deletion, system failures, or natural disasters. This can result in significant financial and reputational damage for the organization.",
     "ServiceName": "backup",
-    "Severity": "medium",
+    "Severity": "low",
     "SubServiceName": ""
 }
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_plans_exist/backup_plans_exist.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 class backup_plans_exist(Check):
     def execute(self):
         findings = []
         report = Check_Report_AWS(self.metadata())
         report.status = "FAIL"
         report.status_extended = "No Backup Plan Exist"
         report.resource_arn = ""
-        report.resource_id = "No Backups"
+        report.resource_id = "Backups"
         report.region = backup_client.region
         if backup_client.backup_plans:
             report.status = "PASS"
-            report.status_extended = f"At least one backup plan exists: { backup_client.backup_plans[0].name}"
+            report.status_extended = (
+                f"At least one backup plan exists: {backup_client.backup_plans[0].name}"
+            )
             report.resource_arn = backup_client.backup_plans[0].arn
             report.resource_id = backup_client.backup_plans[0].name
             report.region = backup_client.backup_plans[0].region
 
         findings.append(report)
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_reportplans_exist/backup_reportplans_exist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.backup.backup_client import backup_client
 
 
 class backup_reportplans_exist(Check):
     def execute(self):
         findings = []
-        report = Check_Report_AWS(self.metadata())
-        report.status = "FAIL"
-        report.status_extended = "No Backup Report Plan Exist"
-        report.resource_arn = ""
-        report.resource_id = "No Backups"
-        report.region = backup_client.region
-        if backup_client.backup_report_plans:
-            report.status = "PASS"
-            report.status_extended = f"At least one backup report plan exists: { backup_client.backup_report_plans[0].name}"
-            report.resource_arn = backup_client.backup_report_plans[0].arn
-            report.resource_id = backup_client.backup_report_plans[0].name
-            report.region = backup_client.backup_report_plans[0].region
+        # We only check report plans if backup plans exist, reducing noise
+        if backup_client.backup_plans:
+            report = Check_Report_AWS(self.metadata())
+            report.status = "FAIL"
+            report.status_extended = "No Backup Report Plan Exist"
+            report.resource_arn = ""
+            report.resource_id = "Backups"
+            report.region = backup_client.region
+            if backup_client.backup_report_plans:
+                report.status = "PASS"
+                report.status_extended = f"At least one backup report plan exists: { backup_client.backup_report_plans[0].name}"
+                report.resource_arn = backup_client.backup_report_plans[0].arn
+                report.resource_id = backup_client.backup_report_plans[0].name
+                report.region = backup_client.backup_report_plans[0].region
 
-        findings.append(report)
+            findings.append(report)
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_service.py` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                                 region=regional_client.region,
                                 name=configuration.get("BackupPlanName"),
                                 version_id=configuration.get("VersionId"),
                                 last_execution_date=configuration.get(
                                     "LastExecutionDate"
                                 ),
                                 advanced_settings=configuration.get(
-                                    "AdvancedBackupSettings"
+                                    "AdvancedBackupSettings", []
                                 ),
                             )
                         )
 
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_encrypted/backup_vaults_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.metadata.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'CheckTitle'": "'Ensure AWS Backup vaults exist'", "'Severity'": "'low'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "Categories": [],
     "CheckID": "backup_vaults_exist",
-    "CheckTitle": "Esure AWS Backup vaults exist",
+    "CheckTitle": "Ensure AWS Backup vaults exist",
     "CheckType": [
         "Recover",
         "Resilience",
         "Backup"
     ],
     "DependsOn": [],
     "Description": "This check ensures that AWS Backup vaults exist to provide a secure and durable storage location for backup data.",
@@ -25,10 +25,10 @@
             "Url": ""
         }
     },
     "ResourceIdTemplate": "arn:partition:service:region:account-id:backup-vault:backup-vault-id",
     "ResourceType": "AwsBackupBackupVault",
     "Risk": "Without an AWS Backup vault, an organization's critical data may be at risk of being lost in the event of an accidental deletion, system failures, or natural disasters.",
     "ServiceName": "backup",
-    "Severity": "medium",
+    "Severity": "low",
     "SubServiceName": ""
 }
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/backup/backup_vaults_exist/backup_vaults_exist.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class backup_vaults_exist(Check):
     def execute(self):
         findings = []
         report = Check_Report_AWS(self.metadata())
         report.status = "FAIL"
         report.status_extended = "No Backup Vault Exist"
         report.resource_arn = ""
-        report.resource_id = "No Backups"
+        report.resource_id = "Backups"
         report.region = backup_client.region
         if backup_client.backup_vaults:
             report.status = "PASS"
             report.status_extended = f"At least one backup vault exists: { backup_client.backup_vaults[0].name}"
             report.resource_arn = backup_client.backup_vaults[0].arn
             report.resource_id = backup_client.backup_vaults[0].name
             report.region = backup_client.backup_vaults[0].region
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_service.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 ]
                 # Nested Stack
                 if "RootId" in stack_details["Stacks"][0]:
                     stack.root_nested_stack = stack_details["Stacks"][0]["RootId"]
                 stack.is_nested_stack = True if stack.root_nested_stack != "" else False
 
             except ClientError as error:
-                if error.response["Error"]["Code"] != "ValidationError":
+                if error.response["Error"]["Code"] == "ValidationError":
                     logger.warning(
                         f"{stack.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                     )
                     continue
             except Exception as error:
                 logger.error(
                     f"{stack.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stack_outputs_find_secrets/cloudformation_stack_outputs_find_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudformation/cloudformation_stacks_termination_protection_enabled/cloudformation_stacks_termination_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_field_level_encryption_enabled/cloudfront_distributions_field_level_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_geo_restrictions_enabled/cloudfront_distributions_geo_restrictions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_https_enabled/cloudfront_distributions_https_enabled.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,18 @@
         findings = []
         for distribution in cloudfront_client.distributions.values():
             report = Check_Report_AWS(self.metadata())
             report.region = distribution.region
             report.resource_arn = distribution.arn
             report.resource_id = distribution.id
             report.resource_tags = distribution.tags
+
             if (
                 distribution.default_cache_config
                 and distribution.default_cache_config.viewer_protocol_policy
-                == ViewerProtocolPolicy.allow_all
-            ):
-                report.status = "FAIL"
-                report.status_extended = f"CloudFront Distribution {distribution.id} viewers can use HTTP or HTTPS"
-            elif (
-                distribution.default_cache_config
-                and distribution.default_cache_config.viewer_protocol_policy
                 == ViewerProtocolPolicy.redirect_to_https
             ):
                 report.status = "PASS"
                 report.status_extended = (
                     f"CloudFront Distribution {distribution.id} has redirect to HTTPS"
                 )
             elif (
@@ -37,10 +31,14 @@
                 and distribution.default_cache_config.viewer_protocol_policy
                 == ViewerProtocolPolicy.https_only
             ):
                 report.status = "PASS"
                 report.status_extended = (
                     f"CloudFront Distribution {distribution.id} has HTTPS only"
                 )
+            else:
+                report.status = "FAIL"
+                report.status_extended = f"CloudFront Distribution {distribution.id} viewers can use HTTP or HTTPS"
+
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_logging_enabled/cloudfront_distributions_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_deprecated_ssl_protocols/cloudfront_distributions_using_deprecated_ssl_protocols.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_distributions_using_waf/cloudfront_distributions_using_waf.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudfront/cloudfront_service.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudfront/cloudfront_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,28 +79,28 @@
                     "RestrictionType"
                 ]
                 distributions[distribution_id].web_acl_id = distribution_config[
                     "DistributionConfig"
                 ]["WebACLId"]
 
                 # Default Cache Config
-                default_chache_config = DefaultCacheConfigBehaviour(
+                default_cache_config = DefaultCacheConfigBehaviour(
                     realtime_log_config_arn=distribution_config["DistributionConfig"][
                         "DefaultCacheBehavior"
                     ].get("RealtimeLogConfigArn"),
                     viewer_protocol_policy=distribution_config["DistributionConfig"][
                         "DefaultCacheBehavior"
                     ].get("ViewerProtocolPolicy"),
                     field_level_encryption_id=distribution_config["DistributionConfig"][
                         "DefaultCacheBehavior"
                     ].get("FieldLevelEncryptionId"),
                 )
                 distributions[
                     distribution_id
-                ].default_cache_config = default_chache_config
+                ].default_cache_config = default_cache_config
 
         except Exception as error:
             logger.error(
                 f"{region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __list_tags_for_resource__(self, client, distributions, region):
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_bucket_requires_mfa_delete/cloudtrail_bucket_requires_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_cloudwatch_logging_enabled/cloudtrail_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_insights_exist/cloudtrail_insights_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_kms_encryption_enabled/cloudtrail_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_log_file_validation_enabled/cloudtrail_log_file_validation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_access_logging_enabled/cloudtrail_logs_s3_bucket_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_logs_s3_bucket_is_not_publicly_accessible/cloudtrail_logs_s3_bucket_is_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_multi_region_enabled/cloudtrail_multi_region_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_read_enabled/cloudtrail_s3_dataevents_read_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_s3_dataevents_write_enabled/cloudtrail_s3_dataevents_write_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudtrail/cloudtrail_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import threading
 from datetime import datetime
 from typing import Optional
 
+from botocore.client import ClientError
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
@@ -154,14 +155,24 @@
                         try:
                             client_insight_selectors = client.get_insight_selectors(
                                 TrailName=trail.arn
                             )
                             insight_selectors = client_insight_selectors.get(
                                 "InsightSelectors"
                             )
+                        except ClientError as error:
+                            if (
+                                error.response["Error"]["Code"]
+                                == "InsightNotEnabledException"
+                            ):
+                                continue
+                            else:
+                                logger.error(
+                                    f"{client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                                )
                         except Exception as error:
                             logger.error(
                                 f"{client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                             )
                             continue
                         if insight_selectors:
                             trail.has_insight_selectors = insight_selectors[0].get(
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_acls_alarm_configured/cloudwatch_changes_to_network_acls_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_gateways_alarm_configured/cloudwatch_changes_to_network_gateways_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_network_route_tables_alarm_configured/cloudwatch_changes_to_network_route_tables_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_changes_to_vpcs_alarm_configured/cloudwatch_changes_to_vpcs_alarm_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_cross_account_sharing_disabled/cloudwatch_cross_account_sharing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_kms_encryption_enabled/cloudwatch_log_group_kms_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_no_secrets_in_logs/cloudwatch_log_group_no_secrets_in_logs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_group_retention_policy_specific_days_enabled/cloudwatch_log_group_retention_policy_specific_days_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_aws_config_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled/cloudwatch_log_metric_filter_and_alarm_for_cloudtrail_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_authentication_failures/cloudwatch_log_metric_filter_authentication_failures.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_aws_organizations_changes/cloudwatch_log_metric_filter_aws_organizations_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk/cloudwatch_log_metric_filter_disable_or_scheduled_deletion_of_kms_cmk.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes/cloudwatch_log_metric_filter_for_s3_bucket_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_policy_changes/cloudwatch_log_metric_filter_policy_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_root_usage/cloudwatch_log_metric_filter_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_security_group_changes/cloudwatch_log_metric_filter_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_sign_in_without_mfa/cloudwatch_log_metric_filter_sign_in_without_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_log_metric_filter_unauthorized_api_calls/cloudwatch_log_metric_filter_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py` & `prowler-3.5.0/prowler/providers/aws/services/cloudwatch/cloudwatch_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py` & `prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_packages_external_public_publishing_disabled/codeartifact_packages_external_public_publishing_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codeartifact/codeartifact_service.py` & `prowler-3.5.0/prowler/providers/aws/services/codeartifact/codeartifact_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py` & `prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_older_90_days/codebuild_project_older_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py` & `prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_project_user_controlled_buildspec/codebuild_project_user_controlled_buildspec.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/codebuild/codebuild_service.py` & `prowler-3.5.0/prowler/providers/aws/services/codebuild/codebuild_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/config/config_recorder_all_regions_enabled/config_recorder_all_regions_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/config/config_service.py` & `prowler-3.5.0/prowler/providers/aws/services/config/config_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_log_forwarding_enabled/directoryservice_directory_log_forwarding_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_monitor_notifications/directoryservice_directory_monitor_notifications.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_directory_snapshots_limit/directoryservice_directory_snapshots_limit.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_ldap_certificate_expiration/directoryservice_ldap_certificate_expiration.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_radius_server_security_protocol/directoryservice_radius_server_security_protocol.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_service.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/directoryservice/directoryservice_supported_mfa_radius_enabled/directoryservice_supported_mfa_radius_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/drs/drs_job_exist/drs_job_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/drs/drs_service.py` & `prowler-3.5.0/prowler/providers/aws/services/drs/drs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_accelerator_cluster_encryption_enabled/dynamodb_accelerator_cluster_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_service.py` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             try:
                 regional_client = self.regional_clients[cluster.region]
                 # In the DAX service to call list_tags we need to pass the cluster ARN as the resource name
                 response = regional_client.list_tags(ResourceName=cluster.arn)["Tags"]
                 cluster.tags = response
 
             except ClientError as error:
-                if error.response["Error"]["Code"] != "InvalidARNFault":
+                if error.response["Error"]["Code"] == "InvalidARNFault":
                     logger.warning(
                         f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                     )
                     continue
 
             except Exception as error:
                 logger.error(
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_kms_cmk_encryption_enabled/dynamodb_tables_kms_cmk_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/dynamodb/dynamodb_tables_pitr_enabled/dynamodb_tables_pitr_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ami_public/ec2_ami_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_default_encryption/ec2_ebs_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_public_snapshot/ec2_ebs_public_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_snapshots_encrypted/ec2_ebs_snapshots_encrypted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_ebs_volume_encryption/ec2_ebs_volume_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_shodan/ec2_elastic_ip_shodan.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_elastic_ip_unassgined/ec2_elastic_ip_unassgined.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_imdsv2_enabled/ec2_instance_imdsv2_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_internet_facing_with_instance_profile/ec2_instance_internet_facing_with_instance_profile.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_managed_by_ssm/ec2_instance_managed_by_ssm.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_older_than_specific_days/ec2_instance_older_than_specific_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_profile_attached/ec2_instance_profile_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_public_ip/ec2_instance_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_instance_secrets_user_data/ec2_instance_secrets_user_data.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_any_port/ec2_networkacl_allow_ingress_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_22/ec2_networkacl_allow_ingress_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_networkacl_allow_ingress_tcp_port_3389/ec2_networkacl_allow_ingress_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_any_port/ec2_securitygroup_allow_ingress_from_internet_to_any_port.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018/ec2_securitygroup_allow_ingress_from_internet_to_port_mongodb_27017_27018.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21/ec2_securitygroup_allow_ingress_from_internet_to_tcp_ftp_port_20_21.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_22.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_3389.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_cassandra_7199_9160_8888.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_elasticsearch_kibana_9200_9300_5601.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_kafka_9092.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_memcached_11211.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_mysql_3306.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_oracle_1521_2483.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_postgres_5432.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_redis_6379.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_sql_server_1433_1434.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23/ec2_securitygroup_allow_ingress_from_internet_to_tcp_port_telnet_23.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_allow_wide_open_public_ipv4/ec2_securitygroup_allow_wide_open_public_ipv4.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_default_restrict_traffic/ec2_securitygroup_default_restrict_traffic.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_from_launch_wizard/ec2_securitygroup_from_launch_wizard.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_not_used/ec2_securitygroup_not_used.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_securitygroup_with_many_ingress_egress_rules/ec2_securitygroup_with_many_ingress_egress_rules.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/ec2_service.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/ec2_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         self.security_groups = []
         self.__threading_call__(self.__describe_security_groups__)
         self.network_acls = []
         self.__threading_call__(self.__describe_network_acls__)
         self.snapshots = []
         self.__threading_call__(self.__describe_snapshots__)
         self.__get_snapshot_public__()
-        self.__threading_call__(self.__describe_network_interfaces__)
+        self.network_interfaces = []
+        self.__threading_call__(self.__describe_public_network_interfaces__)
+        self.__threading_call__(self.__describe_sg_network_interfaces__)
         self.images = []
         self.__threading_call__(self.__describe_images__)
         self.volumes = []
         self.__threading_call__(self.__describe_volumes__)
         self.ebs_encryption_by_default = []
         self.__threading_call__(self.__get_ebs_encryption_by_default__)
         self.elastic_ips = []
@@ -216,18 +218,45 @@
                     continue
 
             except Exception as error:
                 logger.error(
                     f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                 )
 
-    def __describe_network_interfaces__(self, regional_client):
+    def __describe_public_network_interfaces__(self, regional_client):
         logger.info("EC2 - Describing Network Interfaces...")
         try:
-            # Get SGs Network Interfaces
+            # Get Network Interfaces with Public IPs
+            describe_network_interfaces_paginator = regional_client.get_paginator(
+                "describe_network_interfaces"
+            )
+            for page in describe_network_interfaces_paginator.paginate():
+                for interface in page["NetworkInterfaces"]:
+                    if interface.get("Association"):
+                        self.network_interfaces.append(
+                            NetworkInterface(
+                                public_ip=interface["Association"]["PublicIp"],
+                                type=interface["InterfaceType"],
+                                private_ip=interface["PrivateIpAddress"],
+                                subnet_id=interface["SubnetId"],
+                                vpc_id=interface["VpcId"],
+                                region=regional_client.region,
+                                tags=interface.get("TagSet"),
+                            )
+                        )
+
+        except Exception as error:
+            logger.error(
+                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
+    def __describe_sg_network_interfaces__(self, regional_client):
+        logger.info("EC2 - Describing Network Interfaces...")
+        try:
+            # Get Network Interfaces for Security Groups
             for sg in self.security_groups:
                 regional_client = self.regional_clients[sg.region]
                 describe_network_interfaces_paginator = regional_client.get_paginator(
                     "describe_network_interfaces"
                 )
                 for page in describe_network_interfaces_paginator.paginate(
                     Filters=[
@@ -237,15 +266,14 @@
                                 sg.id,
                             ],
                         },
                     ],
                 ):
                     for interface in page["NetworkInterfaces"]:
                         sg.network_interfaces.append(interface["NetworkInterfaceId"])
-
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __get_instance_user_data__(self):
         logger.info("EC2 - Gettting instance user data...")
@@ -421,14 +449,24 @@
     id: str
     arn: str
     region: str
     entries: list[dict]
     tags: Optional[list] = []
 
 
+class NetworkInterface(BaseModel):
+    public_ip: str
+    private_ip: str
+    type: str
+    subnet_id: str
+    vpc_id: str
+    region: str
+    tags: Optional[list] = []
+
+
 class ElasticIP(BaseModel):
     public_ip: Optional[str]
     association_id: Optional[str]
     arn: str
     allocation_id: Optional[str]
     region: str
     tags: Optional[list] = []
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/lib/network_acls.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/lib/network_acls.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ec2/lib/security_groups.py` & `prowler-3.5.0/prowler/providers/aws/services/ec2/lib/security_groups.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_registry_scan_images_on_push_enabled/ecr_registry_scan_images_on_push_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
-from prowler.providers.aws.services.ecr.ecr_client import ecr_client
+from prowler.providers.aws.services.rds.rds_client import rds_client
 
 
-class ecr_registry_scan_images_on_push_enabled(Check):
+class rds_instance_no_public_access(Check):
     def execute(self):
         findings = []
-        for registry in ecr_client.registries:
+        for db_instance in rds_client.db_instances:
             report = Check_Report_AWS(self.metadata())
-            report.region = registry.region
-            report.resource_id = registry.id
-            report.resource_tags = registry.tags
-            report.status = "FAIL"
-            report.status_extended = f"ECR registry {registry.id} has {registry.scan_type} scanning without scan on push"
-            if registry.rules:
+            report.region = db_instance.region
+            report.resource_id = db_instance.id
+            report.resource_tags = db_instance.tags
+            if not db_instance.public:
                 report.status = "PASS"
-                report.status_extended = f"ECR registry {registry.id} has {registry.scan_type} scan with scan on push"
-                filters = True
-                for rule in registry.rules:
-                    if not rule.scan_filters or "'*'" in str(rule.scan_filters):
-                        filters = False
-                if filters:
-                    report.status = "FAIL"
-                    report.status_extended = f"ECR registry {registry.id} has {registry.scan_type} scanning with scan on push but with repository filters"
+                report.status_extended = (
+                    f"RDS Instance {db_instance.id} is not Publicly Accessible."
+                )
+            else:
+                report.status = "FAIL"
+                report.status_extended = (
+                    f"RDS Instance {db_instance.id} is set as Publicly Accessible."
+                )
 
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_lifecycle_policy_enabled/ecr_repositories_lifecycle_policy_enabled.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.ecr.ecr_client import ecr_client
 
 
 class ecr_repositories_lifecycle_policy_enabled(Check):
     def execute(self):
         findings = []
-        for repository in ecr_client.repositories:
-            report = Check_Report_AWS(self.metadata())
-            report.region = repository.region
-            report.resource_id = repository.name
-            report.resource_arn = repository.arn
-            report.resource_tags = repository.tags
-            report.status = "FAIL"
-            report.status_extended = (
-                f"Repository {repository.name} has no lifecycle policy"
-            )
-            if repository.lyfecicle_policy:
-                report.status = "PASS"
-                report.status_extended = (
-                    f"Repository {repository.name} has lifecycle policy"
-                )
+        for registry in ecr_client.registries.values():
+            for repository in registry.repositories:
+                report = Check_Report_AWS(self.metadata())
+                report.region = repository.region
+                report.resource_id = repository.name
+                report.resource_arn = repository.arn
+                report.resource_tags = repository.tags
+                report.status = "FAIL"
+                report.status_extended = f"Repository {repository.name} has not a lifecycle policy configured"
+                if repository.lifecycle_policy:
+                    report.status = "PASS"
+                    report.status_extended = f"Repository {repository.name} has a lifecycle policy configured"
 
-            findings.append(report)
+                findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_not_publicly_accessible/ecr_repositories_not_publicly_accessible.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.ecr.ecr_client import ecr_client
 
 
 class ecr_repositories_not_publicly_accessible(Check):
     def execute(self):
         findings = []
-        for repository in ecr_client.repositories:
-            report = Check_Report_AWS(self.metadata())
-            report.region = repository.region
-            report.resource_id = repository.name
-            report.resource_arn = repository.arn
-            report.resource_tags = repository.tags
-            report.status = "PASS"
-            report.status_extended = f"Repository {repository.name} is not open"
-            if repository.policy:
-                for statement in repository.policy["Statement"]:
-                    if statement["Effect"] == "Allow":
-                        if "*" in statement["Principal"] or (
-                            "AWS" in statement["Principal"]
-                            and "*" in statement["Principal"]["AWS"]
-                        ):
-                            report.status = "FAIL"
-                            report.status_extended = f"Repository {repository.name} policy may allow anonymous users to perform actions (Principal: '*')"
-                            break
+        for registry in ecr_client.registries.values():
+            for repository in registry.repositories:
+                report = Check_Report_AWS(self.metadata())
+                report.region = repository.region
+                report.resource_id = repository.name
+                report.resource_arn = repository.arn
+                report.resource_tags = repository.tags
+                report.status = "PASS"
+                report.status_extended = (
+                    f"Repository {repository.name} is not publicly accesible"
+                )
+                if repository.policy:
+                    for statement in repository.policy["Statement"]:
+                        if statement["Effect"] == "Allow":
+                            if "*" in statement["Principal"] or (
+                                "AWS" in statement["Principal"]
+                                and "*" in statement["Principal"]["AWS"]
+                            ):
+                                report.status = "FAIL"
+                                report.status_extended = f"Repository {repository.name} policy may allow anonymous users to perform actions (Principal: '*')"
+                                break
 
-            findings.append(report)
+                findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_images_on_push_enabled/ecr_repositories_scan_images_on_push_enabled.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.ecr.ecr_client import ecr_client
 
 
 class ecr_repositories_scan_images_on_push_enabled(Check):
     def execute(self):
         findings = []
-        for repository in ecr_client.repositories:
-            report = Check_Report_AWS(self.metadata())
-            report.region = repository.region
-            report.resource_id = repository.name
-            report.resource_arn = repository.arn
-            report.resource_tags = repository.tags
-            report.status = "PASS"
-            report.status_extended = (
-                f"ECR repository {repository.name} has scan on push enabled"
-            )
-            if not repository.scan_on_push:
-                report.status = "FAIL"
+        for registry in ecr_client.registries.values():
+            for repository in registry.repositories:
+                report = Check_Report_AWS(self.metadata())
+                report.region = repository.region
+                report.resource_id = repository.name
+                report.resource_arn = repository.arn
+                report.resource_tags = repository.tags
+                report.status = "PASS"
                 report.status_extended = (
-                    f"ECR repository {repository.name} has scan on push disabled"
+                    f"ECR repository {repository.name} has scan on push enabled"
                 )
+                if not repository.scan_on_push:
+                    report.status = "FAIL"
+                    report.status_extended = (
+                        f"ECR repository {repository.name} has scan on push disabled"
+                    )
 
-            findings.append(report)
+                findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py` & `prowler-3.5.0/prowler/providers/aws/services/ecr/ecr_repositories_scan_vulnerabilities_in_latest_image/ecr_repositories_scan_vulnerabilities_in_latest_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.ecr.ecr_client import ecr_client
 
 
 class ecr_repositories_scan_vulnerabilities_in_latest_image(Check):
     def execute(self):
         findings = []
-        for repository in ecr_client.repositories:
-            for image in repository.images_details:
-                report = Check_Report_AWS(self.metadata())
-                report.region = repository.region
-                report.resource_id = repository.name
-                report.resource_arn = repository.arn
-                report.resource_tags = repository.tags
-                report.status = "PASS"
-                report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} scanned without findings"
-                if not image.scan_findings_status:
-                    report.status = "FAIL"
-                    report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} without a scan"
-                elif image.scan_findings_status == "FAILED":
-                    report.status = "FAIL"
-                    report.status_extended = (
-                        f"ECR repository {repository.name} with scan status FAILED"
-                    )
-                elif image.scan_findings_status != "FAILED":
-                    if image.scan_findings_severity_count and (
-                        image.scan_findings_severity_count.critical
-                        or image.scan_findings_severity_count.high
-                        or image.scan_findings_severity_count.medium
-                    ):
+        for registry in ecr_client.registries.values():
+            for repository in registry.repositories:
+                # First check if the repository has images
+                if len(repository.images_details) > 0:
+                    # We only want to check the latest image pushed
+                    image = repository.images_details[-1]
+
+                    report = Check_Report_AWS(self.metadata())
+                    report.region = repository.region
+                    report.resource_id = repository.name
+                    report.resource_arn = repository.arn
+                    report.resource_tags = repository.tags
+                    report.status = "PASS"
+                    report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} scanned without findings"
+                    if not image.scan_findings_status:
+                        report.status = "FAIL"
+                        report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} without a scan"
+                    elif image.scan_findings_status == "FAILED":
                         report.status = "FAIL"
-                        report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} scanned with findings: CRITICAL->{image.scan_findings_severity_count.critical}, HIGH->{image.scan_findings_severity_count.high}, MEDIUM->{image.scan_findings_severity_count.medium} "
+                        report.status_extended = (
+                            f"ECR repository {repository.name} with scan status FAILED"
+                        )
+                    elif image.scan_findings_status != "FAILED":
+                        if image.scan_findings_severity_count and (
+                            image.scan_findings_severity_count.critical
+                            or image.scan_findings_severity_count.high
+                            or image.scan_findings_severity_count.medium
+                        ):
+                            report.status = "FAIL"
+                            report.status_extended = f"ECR repository {repository.name} has imageTag {image.latest_tag} scanned with findings: CRITICAL->{image.scan_findings_severity_count.critical}, HIGH->{image.scan_findings_severity_count.high}, MEDIUM->{image.scan_findings_severity_count.medium} "
 
-                findings.append(report)
+                    findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_service.py` & `prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py` & `prowler-3.5.0/prowler/providers/aws/services/ecs/ecs_task_definitions_no_environment_secrets/ecs_task_definitions_no_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_encryption_at_rest_enabled/efs_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_have_backup_enabled/efs_have_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_not_publicly_accessible/efs_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/efs/efs_service.py` & `prowler-3.5.0/prowler/providers/aws/services/efs/efs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_cluster_kms_cmk_encryption_in_secrets_enabled/eks_cluster_kms_cmk_encryption_in_secrets_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_endpoint_access_restricted/eks_control_plane_endpoint_access_restricted.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_control_plane_logging_all_types_enabled/eks_control_plane_logging_all_types_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_endpoints_not_publicly_accessible/eks_endpoints_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/eks/eks_service.py` & `prowler-3.5.0/prowler/providers/aws/services/eks/eks_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_insecure_ssl_ciphers/elb_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_internet_facing/elb_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_logging_enabled/elb_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_service.py` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py` & `prowler-3.5.0/prowler/providers/aws/services/elb/elb_ssl_listeners/elb_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_deletion_protection/elbv2_deletion_protection.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_desync_mitigation_mode/elbv2_desync_mitigation_mode.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_insecure_ssl_ciphers/elbv2_insecure_ssl_ciphers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_internet_facing/elbv2_internet_facing.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_listeners_underneath/elbv2_listeners_underneath.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_logging_enabled/elbv2_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_service.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_ssl_listeners/elbv2_ssl_listeners.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py` & `prowler-3.5.0/prowler/providers/aws/services/elbv2/elbv2_waf_acl_attached/elbv2_waf_acl_attached.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_account_public_block_enabled/emr_cluster_account_public_block_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_master_nodes_no_public_ip/emr_cluster_master_nodes_no_public_ip.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_cluster_publicly_accesible/emr_cluster_publicly_accesible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/emr/emr_service.py` & `prowler-3.5.0/prowler/providers/aws/services/emr/emr_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import threading
 from enum import Enum
 from typing import Optional
 
+from botocore.client import ClientError
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
@@ -67,18 +68,27 @@
             )
 
     def __describe_cluster__(self, regional_client):
         logger.info("EMR - Describing Clusters...")
         try:
             for cluster in self.clusters.values():
                 if cluster.region == regional_client.region:
-                    describe_cluster_parameters = {"ClusterId": cluster.id}
-                    cluster_info = regional_client.describe_cluster(
-                        **describe_cluster_parameters
-                    )
+                    try:
+                        describe_cluster_parameters = {"ClusterId": cluster.id}
+                        cluster_info = regional_client.describe_cluster(
+                            **describe_cluster_parameters
+                        )
+                    except ClientError as error:
+                        if error.response["Error"]["Code"] == "InvalidRequestException":
+                            logger.warning(
+                                f"{regional_client.region} --"
+                                f" {error.__class__.__name__}[{error.__traceback__.tb_lineno}]:"
+                                f" {error}"
+                            )
+                        continue
 
                     # Master Node Security Groups
                     master_node_security_group = cluster_info["Cluster"][
                         "Ec2InstanceAttributes"
                     ].get("EmrManagedMasterSecurityGroup")
                     master_node_additional_security_groups = None
                     if (
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_service.py` & `prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py` & `prowler-3.5.0/prowler/providers/aws/services/glacier/glacier_vaults_policy_public_access/glacier_vaults_policy_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py` & `prowler-3.5.0/prowler/providers/aws/services/globalaccelerator/globalaccelerator_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_connection_passwords_encryption_enabled/glue_data_catalogs_connection_passwords_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_data_catalogs_metadata_encryption_enabled/glue_data_catalogs_metadata_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_database_connections_ssl_enabled/glue_database_connections_ssl_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_cloudwatch_logs_encryption_enabled/glue_development_endpoints_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_job_bookmark_encryption_enabled/glue_development_endpoints_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_development_endpoints_s3_encryption_enabled/glue_development_endpoints_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_amazon_s3_encryption_enabled/glue_etl_jobs_amazon_s3_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_cloudwatch_logs_encryption_enabled/glue_etl_jobs_cloudwatch_logs_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_etl_jobs_job_bookmark_encryption_enabled/glue_etl_jobs_job_bookmark_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/glue/glue_service.py` & `prowler-3.5.0/prowler/providers/aws/services/glue/glue_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_centrally_managed/guardduty_centrally_managed.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_is_enabled/guardduty_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_no_high_severity_findings/guardduty_no_high_severity_findings.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/guardduty/guardduty_service.py` & `prowler-3.5.0/prowler/providers/aws/services/guardduty/guardduty_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_administrator_access_with_mfa/iam_administrator_access_with_mfa.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_avoid_root_usage/iam_avoid_root_usage.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_aws_attached_policy_no_administrative_privileges/iam_aws_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_check_saml_providers_sts/iam_check_saml_providers_sts.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_attached_policy_no_administrative_privileges/iam_customer_attached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_customer_unattached_policy_no_administrative_privileges/iam_customer_unattached_policy_no_administrative_privileges.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_30_days_credentials/iam_disable_30_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_45_days_credentials/iam_disable_45_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_disable_90_days_credentials/iam_disable_90_days_credentials.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_custom_policy_permissive_role_assumption/iam_no_custom_policy_permissive_role_assumption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_expired_server_certificates_stored/iam_no_expired_server_certificates_stored.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_no_root_access_key/iam_no_root_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_expires_passwords_within_90_days_or_less/iam_password_policy_expires_passwords_within_90_days_or_less.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_lowercase/iam_password_policy_lowercase.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_minimum_length_14/iam_password_policy_minimum_length_14.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_number/iam_password_policy_number.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_reuse_24/iam_password_policy_reuse_24.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_symbol/iam_password_policy_symbol.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_password_policy_uppercase/iam_password_policy_uppercase.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_allows_privilege_escalation/iam_policy_allows_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_attached_only_to_group_or_roles/iam_policy_attached_only_to_group_or_roles.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.iam.iam_client import iam_client
 
-critical_service = "cloudtrail"
+critical_service = "kms"
 
 
-class iam_policy_no_full_access_to_cloudtrail(Check):
+class iam_policy_no_full_access_to_kms(Check):
     def execute(self) -> Check_Report_AWS:
         findings = []
         for policy in iam_client.policies:
             # Check only custom policies
             if policy.type == "Custom":
                 report = Check_Report_AWS(self.metadata())
                 report.region = iam_client.region
                 report.resource_arn = policy.arn
                 report.resource_id = policy.name
                 report.resource_tags = policy.tags
                 report.status = "PASS"
                 report.status_extended = f"Custom Policy {policy.name} does not allow '{critical_service}:*' privileges"
                 if policy.document:
-                    # Check the statements, if one includes critical_service:* stop iterating over the rest
-                    if type(policy.document.get("Statement")) != list:
-                        policy_statements = [policy.document.get("Statement")]
+                    if type(policy.document["Statement"]) != list:
+                        policy_statements = [policy.document["Statement"]]
                     else:
-                        policy_statements = policy.document.get("Statement")
+                        policy_statements = policy.document["Statement"]
+                    # Check the statements, if one includes kms:* stop iterating over the rest
                     for statement in policy_statements:
-                        # Check policies with "Effect": "Allow" with "Action": "*" over "Resource": "*".
                         if (
-                            statement.get("Effect") == "Allow"
-                            and critical_service + ":*" in statement.get("Action")
+                            statement["Effect"] == "Allow"
+                            and "Action" in statement
+                            and critical_service + ":*" in statement["Action"]
                             and (
-                                statement.get("Resource") == "*"
-                                or statement.get("Resource") == ["*"]
+                                statement["Resource"] == "*"
+                                or statement["Resource"] == ["*"]
                             )
                         ):
                             report.status = "FAIL"
                             report.status_extended = f"Custom Policy {policy.name} allows '{critical_service}:*' privileges"
                             break
+
                 findings.append(report)
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_kms/iam_policy_no_full_access_to_kms.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_policy_no_full_access_to_cloudtrail/iam_policy_no_full_access_to_cloudtrail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.iam.iam_client import iam_client
 
-critical_service = "kms"
+critical_service = "cloudtrail"
 
 
-class iam_policy_no_full_access_to_kms(Check):
+class iam_policy_no_full_access_to_cloudtrail(Check):
     def execute(self) -> Check_Report_AWS:
         findings = []
         for policy in iam_client.policies:
             # Check only custom policies
             if policy.type == "Custom":
                 report = Check_Report_AWS(self.metadata())
                 report.region = iam_client.region
                 report.resource_arn = policy.arn
                 report.resource_id = policy.name
                 report.resource_tags = policy.tags
                 report.status = "PASS"
                 report.status_extended = f"Custom Policy {policy.name} does not allow '{critical_service}:*' privileges"
                 if policy.document:
-                    # Check the statements, if one includes critical_service:* stop iterating over the rest
-                    if type(policy.document.get("Statement")) != list:
-                        policy_statements = [policy.document.get("Statement")]
+                    if type(policy.document["Statement"]) != list:
+                        policy_statements = [policy.document["Statement"]]
                     else:
-                        policy_statements = policy.document.get("Statement")
+                        policy_statements = policy.document["Statement"]
+                    # Check the statements, if one includes kms:* stop iterating over the rest
                     for statement in policy_statements:
-                        # Check policies with "Effect": "Allow" with "Action": "*" over "Resource": "*".
                         if (
-                            statement.get("Effect") == "Allow"
-                            and critical_service + ":*" in statement.get("Action")
+                            statement["Effect"] == "Allow"
+                            and "Action" in statement
+                            and critical_service + ":*" in statement["Action"]
                             and (
-                                statement.get("Resource") == "*"
-                                or statement.get("Resource") == ["*"]
+                                statement["Resource"] == "*"
+                                or statement["Resource"] == ["*"]
                             )
                         ):
                             report.status = "FAIL"
                             report.status_extended = f"Custom Policy {policy.name} allows '{critical_service}:*' privileges"
                             break
                 findings.append(report)
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.metadata.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'ResourceType'": "'AwsIamRole'"}*

```diff
@@ -20,13 +20,13 @@
         },
         "Recommendation": {
             "Text": "Use the aws:SourceArn and aws:SourceAccount global condition context keys in trust relationship policies to limit the permissions that a service has to a specific resource",
             "Url": "https://docs.aws.amazon.com/IAM/latest/UserGuide/confused-deputy.html#cross-service-confused-deputy-prevention"
         }
     },
     "ResourceIdTemplate": "arn:partition:service:region:account-id:resource-id",
-    "ResourceType": "AwsIamPolicy",
+    "ResourceType": "AwsIamRole",
     "Risk": "Allow attackers to gain unauthorized access to resources",
     "ServiceName": "iam",
     "Severity": "high",
     "SubServiceName": ""
 }
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_role_cross_service_confused_deputy_prevention/iam_role_cross_service_confused_deputy_prevention.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_hardware_mfa_enabled/iam_root_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_root_mfa_enabled/iam_root_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_rotate_access_key_90_days/iam_rotate_access_key_90_days.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_securityaudit_role_created/iam_securityaudit_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_service.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,46 @@
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
 def is_service_role(role):
-    if "Statement" in role["AssumeRolePolicyDocument"]:
-        for statement in role["AssumeRolePolicyDocument"]["Statement"]:
-            if (
-                statement["Effect"] == "Allow"
-                and (
-                    "sts:AssumeRole" in statement["Action"]
-                    or "sts:*" in statement["Action"]
-                    or "*" in statement["Action"]
-                )
-                # This is what defines a service role
-                and "Service" in statement["Principal"]
-            ):
-                return True
+    try:
+        if "Statement" in role["AssumeRolePolicyDocument"]:
+            if type(role["AssumeRolePolicyDocument"]["Statement"]) == list:
+                for statement in role["AssumeRolePolicyDocument"]["Statement"]:
+                    if (
+                        statement["Effect"] == "Allow"
+                        and (
+                            "sts:AssumeRole" in statement["Action"]
+                            or "sts:*" in statement["Action"]
+                            or "*" in statement["Action"]
+                        )
+                        # This is what defines a service role
+                        and "Service" in statement["Principal"]
+                    ):
+                        return True
+            else:
+                statement = role["AssumeRolePolicyDocument"]["Statement"]
+                if (
+                    statement["Effect"] == "Allow"
+                    and (
+                        "sts:AssumeRole" in statement["Action"]
+                        or "sts:*" in statement["Action"]
+                        or "*" in statement["Action"]
+                    )
+                    # This is what defines a service role
+                    and "Service" in statement["Principal"]
+                ):
+                    return True
+    except Exception as error:
+        logger.error(
+            f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+        )
     return False
 
 
 ################## IAM
 class IAM:
     def __init__(self, audit_info):
         self.service = "iam"
@@ -46,14 +65,15 @@
         self.account_summary = self.__get_account_summary__()
         self.virtual_mfa_devices = self.__list_virtual_mfa_devices__()
         self.credential_report = self.__get_credential_report__()
         self.groups = self.__get_groups__()
         self.__get_group_users__()
         self.__list_attached_group_policies__()
         self.__list_attached_user_policies__()
+        self.__list_attached_role_policies__()
         self.__list_inline_user_policies__()
         self.__list_mfa_devices__()
         self.password_policy = self.__get_password_policy__()
         support_policy_arn = (
             "arn:aws:iam::aws:policy/aws-service-role/AWSSupportServiceRolePolicy"
         )
         self.entities_role_attached_to_support_policy = (
@@ -115,15 +135,15 @@
             # Convert credential report to list of dictionaries
             credential = self.client.get_credential_report()["Content"].decode("utf-8")
             credential_lines = credential.split("\n")
             csv_reader = csv.DictReader(credential_lines, delimiter=",")
             credential_list = list(csv_reader)
 
         except ClientError as error:
-            if error.response["Error"]["Code"] != "LimitExceededException":
+            if error.response["Error"]["Code"] == "LimitExceededException":
                 logger.warning(
                     f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                 )
 
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
@@ -334,14 +354,35 @@
                 user.attached_policies = attached_user_policies
 
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
+    def __list_attached_role_policies__(self):
+        logger.info("IAM - List Attached User Policies...")
+        try:
+            for role in self.roles:
+                attached_role_policies = []
+                list_attached_role_policies_paginator = self.client.get_paginator(
+                    "list_attached_role_policies"
+                )
+                for page in list_attached_role_policies_paginator.paginate(
+                    RoleName=role.name
+                ):
+                    for policy in page["AttachedPolicies"]:
+                        attached_role_policies.append(policy)
+
+                role.attached_policies = attached_role_policies
+
+        except Exception as error:
+            logger.error(
+                f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
     def __list_inline_user_policies__(self):
         logger.info("IAM - List Inline User Policies...")
         try:
             for user in self.users:
                 inline_user_policies = []
                 get_user_inline_policies_paginator = self.client.get_paginator(
                     "list_user_policies"
@@ -453,32 +494,51 @@
         finally:
             return server_certificates
 
     def __list_tags_for_resource__(self):
         logger.info("IAM - List Tags...")
         try:
             for role in self.roles:
-                response = self.client.list_role_tags(RoleName=role.name)["Tags"]
-                role.tags = response
+                try:
+                    response = self.client.list_role_tags(RoleName=role.name)["Tags"]
+                    role.tags = response
+                except ClientError as error:
+                    if error.response["Error"]["Code"] == "NoSuchEntityException":
+                        role.tags = []
+
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
+
         try:
             for user in self.users:
-                response = self.client.list_user_tags(UserName=user.name)["Tags"]
-                user.tags = response
+                try:
+                    response = self.client.list_user_tags(UserName=user.name)["Tags"]
+                    user.tags = response
+                except ClientError as error:
+                    if error.response["Error"]["Code"] == "NoSuchEntityException":
+                        user.tags = []
+
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
+
         try:
             for policy in self.policies:
-                response = self.client.list_policy_tags(PolicyArn=policy.arn)["Tags"]
-                policy.tags = response
+                try:
+                    response = self.client.list_policy_tags(PolicyArn=policy.arn)[
+                        "Tags"
+                    ]
+                    policy.tags = response
+                except ClientError as error:
+                    if error.response["Error"]["Code"] == "NoSuchEntityException":
+                        policy.tags = []
+
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
 
 class MFADevice(BaseModel):
@@ -497,14 +557,15 @@
 
 
 class Role(BaseModel):
     name: str
     arn: str
     assume_role_policy: dict
     is_service_role: bool
+    attached_policies: list[dict] = []
     tags: Optional[list] = []
 
 
 class Group(BaseModel):
     name: str
     arn: str
     attached_policies: list[dict] = []
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_support_role_created/iam_support_role_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_hardware_mfa_enabled/iam_user_hardware_mfa_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_mfa_enabled_console_access/iam_user_mfa_enabled_console_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_no_setup_initial_access_key/iam_user_no_setup_initial_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py` & `prowler-3.5.0/prowler/providers/aws/services/iam/iam_user_two_active_access_key/iam_user_two_active_access_key.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py` & `prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_findings_exist/inspector2_findings_exist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/inspector2/inspector2_service.py` & `prowler-3.5.0/prowler/providers/aws/services/inspector2/inspector2_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_are_used/kms_cmk_are_used.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_cmk_rotation_enabled/kms_cmk_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/kms/kms_service.py` & `prowler-3.5.0/prowler/providers/aws/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/macie/macie_is_enabled/macie_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/macie/macie_service.py` & `prowler-3.5.0/prowler/providers/aws/services/macie/macie_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import threading
-from json import loads
+from json import JSONDecodeError, loads
 from typing import Optional
 
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
@@ -75,17 +75,24 @@
                             PublishingLoggingOption(
                                 name=logging_key,
                                 enabled=describe_domain["DomainConfig"][
                                     "LogPublishingOptions"
                                 ]["Options"][logging_key]["Enabled"],
                             )
                         )
-                domain.access_policy = loads(
-                    describe_domain["DomainConfig"]["AccessPolicies"]["Options"]
-                )
+                try:
+                    domain.access_policy = loads(
+                        describe_domain["DomainConfig"]["AccessPolicies"]["Options"]
+                    )
+                except JSONDecodeError as error:
+                    logger.error(
+                        f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                    )
+                    continue
+
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __describe_domain__(self, regional_clients):
         logger.info("OpenSearch - describing domain configurations...")
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_audit_logging_enabled/opensearch_service_domains_audit_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_cloudwatch_logging_enabled/opensearch_service_domains_cloudwatch_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_encryption_at_rest_enabled/opensearch_service_domains_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_https_communications_enforced/opensearch_service_domains_https_communications_enforced.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_internal_user_database_enabled/opensearch_service_domains_internal_user_database_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_node_to_node_encryption_enabled/opensearch_service_domains_node_to_node_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_not_publicly_accessible/opensearch_service_domains_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_updated_to_the_latest_service_software_version/opensearch_service_domains_updated_to_the_latest_service_software_version.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py` & `prowler-3.5.0/prowler/providers/aws/services/opensearch/opensearch_service_domains_use_cognito_authentication_for_kibana/opensearch_service_domains_use_cognito_authentication_for_kibana.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_account_part_of_organizations/organizations_account_part_of_organizations.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_delegated_administrators/organizations_delegated_administrators.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_scp_check_deny_regions/organizations_scp_check_deny_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,18 @@
                         f"No SCP policies exist at the organization {org.id} level"
                     )
                 else:
                     # We use this flag if we find a statement that is restricting regions but not all the configured ones:
                     is_region_restricted_statement = False
 
                     for policy in org.policies:
+                        # We only check SCP policies here
+                        if policy.type != "SERVICE_CONTROL_POLICY":
+                            continue
+
                         # Statements are not always list
                         statements = policy.content.get("Statement")
                         if type(policy.content["Statement"]) is not list:
                             statements = [policy.content.get("Statement")]
 
                         for statement in statements:
                             # Deny if Condition = {"StringNotEquals": {"aws:RequestedRegion": [region1, region2]}}
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/organizations/organizations_service.py` & `prowler-3.5.0/prowler/providers/aws/services/organizations/organizations_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 from botocore.client import ClientError
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
+available_organizations_policies = [
+    "SERVICE_CONTROL_POLICY",
+    "TAG_POLICY",
+    "BACKUP_POLICY",
+    "AISERVICES_OPT_OUT_POLICY",
+]
+
 
 ################## Organizations
 class Organizations:
     def __init__(self, audit_info):
         self.service = "organizations"
         self.session = audit_info.audit_session
         self.audited_account = audit_info.audited_account
@@ -32,21 +39,16 @@
         try:
             # Check if Organizations is in-use
             try:
                 organization_desc = self.client.describe_organization()["Organization"]
                 organization_arn = organization_desc.get("Arn")
                 organization_id = organization_desc.get("Id")
                 organization_master_id = organization_desc.get("MasterAccountId")
-                organization_available_policy_types = organization_desc.get(
-                    "AvailablePolicyTypes"
-                )
                 # Fetch policies for organization:
-                organization_policies = self.__list_policies__(
-                    organization_available_policy_types
-                )
+                organization_policies = self.__list_policies__()
                 # Fetch delegated administrators for organization:
                 organization_delegated_administrator = (
                     self.__list_delegated_administrators__()
                 )
             except ClientError as error:
                 if (
                     error.response["Error"]["Code"]
@@ -91,27 +93,25 @@
 
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     # I'm using list_policies instead of list_policies_for_target, because the last one only returns "Attached directly" policies but not "Inherited from..." policies.
-    def __list_policies__(self, enabled_policy_types):
+    def __list_policies__(self):
         logger.info("Organizations - List policies...")
 
         try:
             list_policies_paginator = self.client.get_paginator("list_policies")
-            for policy_type in enabled_policy_types:
+            for policy_type in available_organizations_policies:
                 logger.info(
                     "Organizations - List policies... - Type: %s",
-                    policy_type.get("Type"),
+                    policy_type,
                 )
-                for page in list_policies_paginator.paginate(
-                    Filter=policy_type.get("Type")
-                ):
+                for page in list_policies_paginator.paginate(Filter=policy_type):
                     for policy in page["Policies"]:
                         policy_content = self.__describe_policy__(policy.get("Id"))
                         policy_targets = self.__list_targets_for_policy__(
                             policy.get("Id")
                         )
                         self.policies.append(
                             Policy(
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_backup_enabled/rds_instance_backup_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_deletion_protection/rds_instance_deletion_protection.py` & `prowler-3.5.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from prowler.lib.check.models import Check, Check_Report_AWS
-from prowler.providers.aws.services.rds.rds_client import rds_client
+from prowler.lib.check.models import Check, Check_Report_GCP
+from prowler.providers.gcp.services.compute.compute_client import compute_client
 
 
-class rds_instance_deletion_protection(Check):
-    def execute(self):
+class compute_instance_public_ip(Check):
+    def execute(self) -> Check_Report_GCP:
         findings = []
-        for db_instance in rds_client.db_instances:
-            report = Check_Report_AWS(self.metadata())
-            report.region = db_instance.region
-            report.resource_id = db_instance.id
-            report.resource_tags = db_instance.tags
-            if db_instance.deletion_protection:
-                report.status = "PASS"
-                report.status_extended = (
-                    f"RDS Instance {db_instance.id} deletion protection is enabled."
-                )
-            else:
+        for instance in compute_client.instances:
+            report = Check_Report_GCP(self.metadata())
+            report.project_id = compute_client.project_id
+            report.resource_id = instance.id
+            report.resource_name = instance.name
+            report.location = instance.zone
+            report.status = "PASS"
+            report.status_extended = f"VM Instance {instance.name} has not a public IP"
+            if instance.public_ip:
                 report.status = "FAIL"
-                report.status_extended = (
-                    f"RDS Instance {db_instance.id} deletion protection is not enabled."
-                )
-
+                report.status_extended = f"VM Instance {instance.name} has a public IP"
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_enhanced_monitoring_enabled/rds_instance_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_integration_cloudwatch_logs/rds_instance_integration_cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_minor_version_upgrade_enabled/rds_instance_minor_version_upgrade_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_multi_az/rds_instance_multi_az.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.rds.rds_client import rds_client
 
 
-class rds_instance_multi_az(Check):
+class rds_instance_storage_encrypted(Check):
     def execute(self):
         findings = []
         for db_instance in rds_client.db_instances:
             report = Check_Report_AWS(self.metadata())
             report.region = db_instance.region
             report.resource_id = db_instance.id
             report.resource_tags = db_instance.tags
-            if db_instance.multi_az:
+            if db_instance.encrypted:
                 report.status = "PASS"
-                report.status_extended = (
-                    f"RDS Instance {db_instance.id} has multi-AZ enabled."
-                )
+                report.status_extended = f"RDS Instance {db_instance.id} is encrypted."
             else:
                 report.status = "FAIL"
                 report.status_extended = (
-                    f"RDS Instance {db_instance.id} does not have multi-AZ enabled."
+                    f"RDS Instance {db_instance.id} is not encrypted."
                 )
 
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_no_public_access/rds_instance_no_public_access.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-from prowler.lib.check.models import Check, Check_Report_AWS
-from prowler.providers.aws.services.rds.rds_client import rds_client
+from prowler.lib.check.models import Check, Check_Report_GCP
+from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class rds_instance_no_public_access(Check):
-    def execute(self):
+class cloudsql_instance_public_ip(Check):
+    def execute(self) -> Check_Report_GCP:
         findings = []
-        for db_instance in rds_client.db_instances:
-            report = Check_Report_AWS(self.metadata())
-            report.region = db_instance.region
-            report.resource_id = db_instance.id
-            report.resource_tags = db_instance.tags
-            if not db_instance.public:
-                report.status = "PASS"
-                report.status_extended = (
-                    f"RDS Instance {db_instance.id} is not Publicly Accessible."
-                )
-            else:
+        for instance in cloudsql_client.instances:
+            report = Check_Report_GCP(self.metadata())
+            report.project_id = cloudsql_client.project_id
+            report.resource_id = instance.name
+            report.resource_name = instance.name
+            report.location = instance.region
+            report.status = "PASS"
+            report.status_extended = (
+                f"Database Instance {instance.name} has not a public IP"
+            )
+            if instance.public_ip:
                 report.status = "FAIL"
                 report.status_extended = (
-                    f"RDS Instance {db_instance.id} is set as Publicly Accessible."
+                    f"Database Instance {instance.name} has a public IP"
                 )
-
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_storage_encrypted/rds_instance_storage_encrypted.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from prowler.lib.check.models import Check, Check_Report_AWS
-from prowler.providers.aws.services.rds.rds_client import rds_client
+from prowler.lib.check.models import Check, Check_Report_GCP
+from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class rds_instance_storage_encrypted(Check):
-    def execute(self):
+class cloudsql_instance_postgres_log_error_verbosity_flag(Check):
+    def execute(self) -> Check_Report_GCP:
         findings = []
-        for db_instance in rds_client.db_instances:
-            report = Check_Report_AWS(self.metadata())
-            report.region = db_instance.region
-            report.resource_id = db_instance.id
-            report.resource_tags = db_instance.tags
-            if db_instance.encrypted:
-                report.status = "PASS"
-                report.status_extended = f"RDS Instance {db_instance.id} is encrypted."
-            else:
+        for instance in cloudsql_client.instances:
+            if "POSTGRES" in instance.version:
+                report = Check_Report_GCP(self.metadata())
+                report.project_id = cloudsql_client.project_id
+                report.resource_id = instance.name
+                report.resource_name = instance.name
+                report.location = instance.region
                 report.status = "FAIL"
-                report.status_extended = (
-                    f"RDS Instance {db_instance.id} is not encrypted."
-                )
-
-            findings.append(report)
+                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_error_verbosity' flag set to 'default'"
+                for flag in instance.flags:
+                    if (
+                        flag["name"] == "log_error_verbosity"
+                        and flag["value"] == "default"
+                    ):
+                        report.status = "PASS"
+                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_error_verbosity' flag set to 'default'"
+                        break
+                findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_instance_transport_encrypted/rds_instance_transport_encrypted.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     def execute(self):
         findings = []
         supported_engines = ["sqlserver", "postgres"]
         for db_instance in rds_client.db_instances:
             report = Check_Report_AWS(self.metadata())
             report.region = db_instance.region
             report.resource_id = db_instance.id
+            report.resource_tags = db_instance.tags
             report.status = "FAIL"
             report.status_extended = (
                 f"RDS Instance {db_instance.id} connections are not encrypted."
             )
             # Check only RDS SQL Server or PostgreSQL engines (Aurora not supported)
             if (
                 any(engine in db_instance.engine for engine in supported_engines)
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_service.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,22 +14,26 @@
     def __init__(self, audit_info):
         self.service = "rds"
         self.session = audit_info.audit_session
         self.audited_account = audit_info.audited_account
         self.audit_resources = audit_info.audit_resources
         self.regional_clients = generate_regional_clients(self.service, audit_info)
         self.db_instances = []
+        self.db_clusters = {}
         self.db_snapshots = []
+        self.db_engines = {}
         self.db_cluster_snapshots = []
         self.__threading_call__(self.__describe_db_instances__)
         self.__threading_call__(self.__describe_db_parameters__)
         self.__threading_call__(self.__describe_db_snapshots__)
         self.__threading_call__(self.__describe_db_snapshot_attributes__)
+        self.__threading_call__(self.__describe_db_clusters__)
         self.__threading_call__(self.__describe_db_cluster_snapshots__)
         self.__threading_call__(self.__describe_db_cluster_snapshot_attributes__)
+        self.__threading_call__(self.__describe_db_engine_versions__)
 
     def __get_session__(self):
         return self.session
 
     def __threading_call__(self, call):
         threads = []
         for regional_client in self.regional_clients.values():
@@ -54,14 +58,15 @@
                     ):
                         if instance["Engine"] != "docdb":
                             self.db_instances.append(
                                 DBInstance(
                                     id=instance["DBInstanceIdentifier"],
                                     endpoint=instance.get("Endpoint"),
                                     engine=instance["Engine"],
+                                    engine_version=instance["EngineVersion"],
                                     status=instance["DBInstanceStatus"],
                                     public=instance["PubliclyAccessible"],
                                     encrypted=instance["StorageEncrypted"],
                                     auto_minor_version_upgrade=instance[
                                         "AutoMinorVersionUpgrade"
                                     ],
                                     backup_retention_period=instance.get(
@@ -75,14 +80,15 @@
                                         "EnhancedMonitoringResourceArn"
                                     ),
                                     parameter_groups=[
                                         item["DBParameterGroupName"]
                                         for item in instance["DBParameterGroups"]
                                     ],
                                     multi_az=instance["MultiAZ"],
+                                    cluster_id=instance.get("DBClusterIdentifier"),
                                     region=regional_client.region,
                                     tags=instance.get("TagList"),
                                 )
                             )
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
@@ -143,24 +149,68 @@
                     response = regional_client.describe_db_snapshot_attributes(
                         DBSnapshotIdentifier=snapshot.id
                     )["DBSnapshotAttributesResult"]
                     for att in response["DBSnapshotAttributes"]:
                         if "all" in att["AttributeValues"]:
                             snapshot.public = True
             except ClientError as error:
-                if error.response["Error"]["Code"] != "DBSnapshotNotFound":
+                if error.response["Error"]["Code"] == "DBSnapshotNotFound":
                     logger.warning(
                         f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                     )
                     continue
             except Exception as error:
                 logger.error(
                     f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                 )
 
+    def __describe_db_clusters__(self, regional_client):
+        logger.info("RDS - Describe Clusters...")
+        try:
+            describe_db_clusters_paginator = regional_client.get_paginator(
+                "describe_db_clusters"
+            )
+            for page in describe_db_clusters_paginator.paginate():
+                for cluster in page["DBClusters"]:
+                    if not self.audit_resources or (
+                        is_resource_filtered(
+                            cluster["DBClusterIdentifier"], self.audit_resources
+                        )
+                    ):
+                        if cluster["Engine"] != "docdb":
+                            db_cluster = DBCluster(
+                                id=cluster["DBClusterIdentifier"],
+                                endpoint=cluster.get("Endpoint"),
+                                engine=cluster["Engine"],
+                                status=cluster["Status"],
+                                public=cluster.get("PubliclyAccessible", False),
+                                encrypted=cluster["StorageEncrypted"],
+                                auto_minor_version_upgrade=cluster.get(
+                                    "AutoMinorVersionUpgrade", False
+                                ),
+                                backup_retention_period=cluster.get(
+                                    "BackupRetentionPeriod"
+                                ),
+                                cloudwatch_logs=cluster.get(
+                                    "EnabledCloudwatchLogsExports"
+                                ),
+                                deletion_protection=cluster["DeletionProtection"],
+                                parameter_group=cluster["DBClusterParameterGroup"],
+                                multi_az=cluster["MultiAZ"],
+                                region=regional_client.region,
+                                tags=cluster.get("TagList"),
+                            )
+                            self.db_clusters[
+                                cluster["DBClusterIdentifier"]
+                            ] = db_cluster
+        except Exception as error:
+            logger.error(
+                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
     def __describe_db_cluster_snapshots__(self, regional_client):
         logger.info("RDS - Describe Cluster Snapshots...")
         try:
             describe_db_snapshots_paginator = regional_client.get_paginator(
                 "describe_db_cluster_snapshots"
             )
             for page in describe_db_snapshots_paginator.paginate():
@@ -198,30 +248,79 @@
                             snapshot.public = True
 
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
+    def __describe_db_engine_versions__(self, regional_client):
+        logger.info("RDS - Describe Engine Versions...")
+        try:
+            describe_db_engine_versions_paginator = regional_client.get_paginator(
+                "describe_db_engine_versions"
+            )
+            for page in describe_db_engine_versions_paginator.paginate():
+                for engine in page["DBEngineVersions"]:
+                    if regional_client.region not in self.db_engines:
+                        self.db_engines[regional_client.region] = {}
+                    if engine["Engine"] not in self.db_engines[regional_client.region]:
+                        db_engine = DBEngine(
+                            region=regional_client.region,
+                            engine=engine["Engine"],
+                            engine_versions=[engine["EngineVersion"]],
+                            engine_description=engine["DBEngineDescription"],
+                        )
+                        self.db_engines[regional_client.region][
+                            engine["Engine"]
+                        ] = db_engine
+                    else:
+                        self.db_engines[regional_client.region][
+                            engine["Engine"]
+                        ].engine_versions.append(engine["EngineVersion"])
+
+        except Exception as error:
+            logger.error(
+                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
 
 class DBInstance(BaseModel):
     id: str
     endpoint: Optional[dict]
     engine: str
+    engine_version: str
     status: str
     public: bool
     encrypted: bool
     backup_retention_period: int = 0
     cloudwatch_logs: Optional[list]
     deletion_protection: bool
     auto_minor_version_upgrade: bool
     enhanced_monitoring_arn: Optional[str]
     multi_az: bool
     parameter_groups: list[str] = []
     parameters: list[dict] = []
+    cluster_id: Optional[str]
+    region: str
+    tags: Optional[list] = []
+
+
+class DBCluster(BaseModel):
+    id: str
+    endpoint: Optional[str]
+    engine: str
+    status: str
+    public: bool
+    encrypted: bool
+    backup_retention_period: int = 0
+    cloudwatch_logs: Optional[list]
+    deletion_protection: bool
+    auto_minor_version_upgrade: bool
+    multi_az: bool
+    parameter_group: Optional[str]
     region: str
     tags: Optional[list] = []
 
 
 class DBSnapshot(BaseModel):
     id: str
     instance_id: str
@@ -232,7 +331,14 @@
 
 class ClusterSnapshot(BaseModel):
     id: str
     cluster_id: str
     public: bool = False
     region: str
     tags: Optional[list] = []
+
+
+class DBEngine(BaseModel):
+    region: str
+    engine: str
+    engine_versions: list[str]
+    engine_description: str
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py` & `prowler-3.5.0/prowler/providers/aws/services/rds/rds_snapshots_public_access/rds_snapshots_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_audit_logging/redshift_cluster_audit_logging.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automated_snapshot/redshift_cluster_automated_snapshot.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_automatic_upgrades/redshift_cluster_automatic_upgrades.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_cluster_public_access/redshift_cluster_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/redshift/redshift_service.py` & `prowler-3.5.0/prowler/providers/aws/services/redshift/redshift_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py` & `prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_indexes_found/resourceexplorer2_indexes_found.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     def execute(self):
         findings = []
         report = Check_Report_AWS(self.metadata())
         report.status = "FAIL"
         report.status_extended = "No Resource Explorer Indexes found"
         report.region = resource_explorer_2_client.region
         report.resource_arn = "NoResourceExplorer"
+        report.resource_id = resource_explorer_2_client.audited_account
         if resource_explorer_2_client.indexes:
             report.region = resource_explorer_2_client.indexes[0].region
             report.resource_arn = resource_explorer_2_client.indexes[0].arn
             report.status = "PASS"
             report.status_extended = f"Resource Explorer Indexes found: {len(resource_explorer_2_client.indexes)}"
         findings.append(report)
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py` & `prowler-3.5.0/prowler/providers/aws/services/resourceexplorer2/resourceexplorer2_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ################################ ResourceExplorer2
 class ResourceExplorer2:
     def __init__(self, audit_info):
         self.service = "resource-explorer-2"
         self.session = audit_info.audit_session
         self.audit_resources = audit_info.audit_resources
+        self.audited_account = audit_info.audited_account
         self.regional_clients = generate_regional_clients(self.service, audit_info)
         # If the region is not set in the audit profile,
         # we pick the first region from the regional clients list
         self.region = (
             audit_info.profile_region
             if audit_info.profile_region
             else list(self.regional_clients.keys())[0]
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_privacy_protection_enabled/route53_domains_privacy_protection_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_domains_transferlock_enabled/route53_domains_transferlock_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_public_hosted_zones_cloudwatch_logging_enabled/route53_public_hosted_zones_cloudwatch_logging_enabled.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     def execute(self) -> Check_Report_AWS:
         findings = []
 
         for hosted_zone in route53_client.hosted_zones.values():
             if not hosted_zone.private_zone:
                 report = Check_Report_AWS(self.metadata())
                 report.resource_id = hosted_zone.id
+                report.resource_arn = hosted_zone.arn
                 report.resource_tags = hosted_zone.tags
                 report.region = hosted_zone.region
                 if (
                     hosted_zone.logging_config
                     and hosted_zone.logging_config.cloudwatch_log_group_arn
                 ):
                     report.status = "PASS"
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/route53/route53_service.py` & `prowler-3.5.0/prowler/providers/aws/services/route53/route53_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 class Route53:
     def __init__(self, audit_info):
         self.service = "route53"
         self.session = audit_info.audit_session
         self.audited_partition = audit_info.audited_partition
         self.audit_resources = audit_info.audit_resources
         self.hosted_zones = {}
+        self.record_sets = []
         global_client = generate_regional_clients(
             self.service, audit_info, global_service=True
         )
         if global_client:
             self.client = list(global_client.values())[0]
             self.region = self.client.region
             self.__list_hosted_zones__()
             self.__list_query_logging_configs__()
             self.__list_tags_for_resource__()
+            self.__list_resource_record_sets__()
 
     def __get_session__(self):
         return self.session
 
     def __list_hosted_zones__(self):
         logger.info("Route53 - Listing Hosting Zones...")
         try:
@@ -51,14 +53,44 @@
                         )
 
         except Exception as error:
             logger.error(
                 f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
+    def __list_resource_record_sets__(self):
+        logger.info("Route53 - Listing Hosting Zones...")
+        try:
+            list_resource_record_sets_paginator = self.client.get_paginator(
+                "list_resource_record_sets"
+            )
+            for zone_id in self.hosted_zones.keys():
+                for page in list_resource_record_sets_paginator.paginate(
+                    HostedZoneId=zone_id
+                ):
+                    for record in page["ResourceRecordSets"]:
+                        self.record_sets.append(
+                            RecordSet(
+                                name=record["Name"],
+                                type=record["Type"],
+                                records=[
+                                    resource_record["Value"]
+                                    for resource_record in record["ResourceRecords"]
+                                ],
+                                is_alias=True if "AliasTarget" in record else False,
+                                hosted_zone_id=zone_id,
+                                region=self.region,
+                            )
+                        )
+
+        except Exception as error:
+            logger.error(
+                f"{self.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
     def __list_query_logging_configs__(self):
         logger.info("Route53 - Listing Query Logging Configs...")
         try:
             for hosted_zone in self.hosted_zones.values():
                 list_query_logging_configs_paginator = self.client.get_paginator(
                     "list_query_logging_configs"
                 )
@@ -101,14 +133,23 @@
     name: str
     private_zone: bool
     logging_config: LoggingConfig = None
     region: str
     tags: Optional[list] = []
 
 
+class RecordSet(BaseModel):
+    name: str
+    type: str
+    is_alias: bool
+    records: list = []
+    hosted_zone_id: str
+    region: str
+
+
 ################## Route53Domains
 class Route53Domains:
     def __init__(self, audit_info):
         self.service = "route53domains"
         self.session = audit_info.audit_session
         self.audited_account = audit_info.audited_account
         self.domains = {}
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_account_level_public_access_blocks/s3_account_level_public_access_blocks.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_acl_prohibited/s3_bucket_acl_prohibited.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_default_encryption/s3_bucket_default_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_level_public_access_block/s3_bucket_level_public_access_block.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_no_mfa_delete/s3_bucket_no_mfa_delete.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_versioning/s3_bucket_object_versioning.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_policy_public_write_access/s3_bucket_policy_public_write_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_public_access/s3_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_secure_transport_policy/s3_bucket_secure_transport_policy.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_server_access_logging_enabled/s3_bucket_server_access_logging_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/s3/s3_service.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.__threading_call__(self.__get_bucket_versioning__)
         self.__threading_call__(self.__get_bucket_logging__)
         self.__threading_call__(self.__get_bucket_policy__)
         self.__threading_call__(self.__get_bucket_acl__)
         self.__threading_call__(self.__get_public_access_block__)
         self.__threading_call__(self.__get_bucket_encryption__)
         self.__threading_call__(self.__get_bucket_ownership_controls__)
+        self.__threading_call__(self.__get_object_lock_configuration__)
         self.__threading_call__(self.__get_bucket_tagging__)
 
     def __get_session__(self):
         return self.session
 
     def __threading_call__(self, call):
         threads = []
@@ -118,14 +119,23 @@
             bucket.encryption = regional_client.get_bucket_encryption(
                 Bucket=bucket.name
             )["ServerSideEncryptionConfiguration"]["Rules"][0][
                 "ApplyServerSideEncryptionByDefault"
             ][
                 "SSEAlgorithm"
             ]
+        except ClientError as error:
+            if error.response["Error"]["Code"] == "NoSuchBucket":
+                logger.warning(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+            else:
+                logger.error(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
         except Exception as error:
             if "ServerSideEncryptionConfigurationNotFoundError" in str(error):
                 bucket.encryption = None
             elif regional_client:
                 logger.error(
                     f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                 )
@@ -163,32 +173,43 @@
             )["PublicAccessBlockConfiguration"]
             bucket.public_access_block = PublicAccessBlock(
                 block_public_acls=public_access_block["BlockPublicAcls"],
                 ignore_public_acls=public_access_block["IgnorePublicAcls"],
                 block_public_policy=public_access_block["BlockPublicPolicy"],
                 restrict_public_buckets=public_access_block["RestrictPublicBuckets"],
             )
-        except Exception as error:
-            if "NoSuchPublicAccessBlockConfiguration" in str(error):
+        except ClientError as error:
+            if error.response["Error"]["Code"] == "NoSuchBucket":
+                logger.warning(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+            elif (
+                error.response["Error"]["Code"]
+                == "NoSuchPublicAccessBlockConfiguration"
+            ):
                 # Set all block as False
                 bucket.public_access_block = PublicAccessBlock(
                     block_public_acls=False,
                     ignore_public_acls=False,
                     block_public_policy=False,
                     restrict_public_buckets=False,
                 )
             else:
-                if regional_client:
-                    logger.error(
-                        f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
-                    )
-                else:
-                    logger.error(
-                        f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
-                    )
+                logger.error(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+        except Exception as error:
+            if regional_client:
+                logger.error(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+            else:
+                logger.error(
+                    f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
 
     def __get_bucket_acl__(self, bucket):
         logger.info("S3 - Get buckets acl...")
         try:
             grantees = []
             regional_client = self.regional_clients[bucket.region]
             acl_grants = regional_client.get_bucket_acl(Bucket=bucket.name)["Grants"]
@@ -237,18 +258,45 @@
     def __get_bucket_ownership_controls__(self, bucket):
         logger.info("S3 - Get buckets ownership controls...")
         try:
             regional_client = self.regional_clients[bucket.region]
             bucket.ownership = regional_client.get_bucket_ownership_controls(
                 Bucket=bucket.name
             )["OwnershipControls"]["Rules"][0]["ObjectOwnership"]
-        except Exception as error:
-            if "OwnershipControlsNotFoundError" in str(error):
+        except ClientError as error:
+            if error.response["Error"]["Code"] == "NoSuchBucket":
+                logger.warning(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+            elif error.response["Error"]["Code"] == "OwnershipControlsNotFoundError":
                 bucket.ownership = None
             else:
+                logger.error(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+        except Exception as error:
+            if regional_client:
+                logger.error(
+                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+            else:
+                logger.error(
+                    f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                )
+
+    def __get_object_lock_configuration__(self, bucket):
+        logger.info("S3 - Get buckets ownership controls...")
+        try:
+            regional_client = self.regional_clients[bucket.region]
+            regional_client.get_object_lock_configuration(Bucket=bucket.name)
+            bucket.object_lock = True
+        except Exception as error:
+            if "ObjectLockConfigurationNotFoundError" in str(error):
+                bucket.object_lock = False
+            else:
                 if regional_client:
                     logger.error(
                         f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                     )
                 else:
                     logger.error(
                         f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
@@ -261,17 +309,22 @@
             bucket_tags = regional_client.get_bucket_tagging(Bucket=bucket.name)[
                 "TagSet"
             ]
             bucket.tags = bucket_tags
         except ClientError as error:
             bucket.tags = []
             if error.response["Error"]["Code"] != "NoSuchTagSet":
-                logger.error(
-                    f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
-                )
+                if error.response["Error"]["Code"] == "NoSuchBucket":
+                    logger.warning(
+                        f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                    )
+                else:
+                    logger.error(
+                        f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                    )
         except Exception as error:
             if regional_client:
                 logger.error(
                     f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                 )
             else:
                 logger.error(
@@ -345,9 +398,10 @@
     public_access_block: Optional[PublicAccessBlock]
     acl_grantees: list[ACL_Grantee] = []
     policy: dict = {}
     encryption: Optional[str]
     region: str
     logging_target_bucket: Optional[str]
     ownership: Optional[str]
+    object_lock: bool = False
     mfa_delete: bool = False
     tags: Optional[list] = []
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_network_isolation_enabled/sagemaker_models_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_models_vpc_settings_configured/sagemaker_models_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_encryption_enabled/sagemaker_notebook_instance_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_root_access_disabled/sagemaker_notebook_instance_root_access_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_vpc_settings_configured/sagemaker_notebook_instance_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_notebook_instance_without_direct_internet_access_configured/sagemaker_notebook_instance_without_direct_internet_access_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_service.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import threading
 from typing import Optional
 
+from botocore.client import ClientError
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.lib.scan_filters.scan_filters import is_resource_filtered
 from prowler.providers.aws.aws_provider import generate_regional_clients
 
 
@@ -111,17 +112,27 @@
             )
 
     def __describe_notebook_instance__(self, regional_clients):
         logger.info("SageMaker - describing notebook instances...")
         try:
             for notebook_instance in self.sagemaker_notebook_instances:
                 regional_client = regional_clients[notebook_instance.region]
-                describe_notebook_instance = regional_client.describe_notebook_instance(
-                    NotebookInstanceName=notebook_instance.name
-                )
+                try:
+                    describe_notebook_instance = (
+                        regional_client.describe_notebook_instance(
+                            NotebookInstanceName=notebook_instance.name
+                        )
+                    )
+                except ClientError as error:
+                    if error.response["Error"]["Code"] == "ValidationException":
+                        logger.warning(
+                            f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                        )
+
+                    continue
                 if (
                     "RootAccess" in describe_notebook_instance
                     and describe_notebook_instance["RootAccess"] == "Enabled"
                 ):
                     notebook_instance.root_access = True
                 if "SubnetId" in describe_notebook_instance:
                     notebook_instance.subnet_id = describe_notebook_instance["SubnetId"]
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_intercontainer_encryption_enabled/sagemaker_training_jobs_intercontainer_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_network_isolation_enabled/sagemaker_training_jobs_network_isolation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_volume_and_output_encryption_enabled/sagemaker_training_jobs_volume_and_output_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py` & `prowler-3.5.0/prowler/providers/aws/services/sagemaker/sagemaker_training_jobs_vpc_settings_configured/sagemaker_training_jobs_vpc_settings_configured.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_automatic_rotation_enabled/secretsmanager_automatic_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py` & `prowler-3.5.0/prowler/providers/aws/services/secretsmanager/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_enabled/securityhub_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/securityhub/securityhub_service.py` & `prowler-3.5.0/prowler/providers/aws/services/securityhub/securityhub_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_associated_elastic_ips/shield_advanced_protection_in_associated_elastic_ips.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_classic_load_balancers/shield_advanced_protection_in_classic_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_cloudfront_distributions/shield_advanced_protection_in_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_global_accelerators/shield_advanced_protection_in_global_accelerators.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_internet_facing_load_balancers/shield_advanced_protection_in_internet_facing_load_balancers.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_advanced_protection_in_route53_hosted_zones/shield_advanced_protection_in_route53_hosted_zones.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/shield/shield_service.py` & `prowler-3.5.0/prowler/providers/aws/services/shield/shield_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sns/sns_service.py` & `prowler-3.5.0/prowler/providers/aws/services/sns/sns_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_kms_encryption_at_rest_enabled/sns_topics_kms_encryption_at_rest_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/sns/sns_topics_not_publicly_accessible/sns_topics_not_publicly_accessible.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         for topic in sns_client.topics:
             report = Check_Report_AWS(self.metadata())
             report.region = topic.region
             report.resource_id = topic.name
             report.resource_arn = topic.arn
             report.resource_tags = topic.tags
             report.status = "PASS"
-            report.status_extended = f"SNS topic {topic.name} without public access"
+            report.status_extended = f"SNS topic {topic.name} is not publicly accesible"
             if topic.policy:
                 for statement in topic.policy["Statement"]:
                     # Only check allow statements
                     if statement["Effect"] == "Allow":
                         if (
                             "*" in statement["Principal"]
                             or (
@@ -27,16 +27,16 @@
                                 "CanonicalUser" in statement["Principal"]
                                 and "*" in statement["Principal"]["CanonicalUser"]
                             )
                         ):
                             if "Condition" not in statement:
                                 report.status = "FAIL"
                                 report.status_extended = (
-                                    f"SNS topic {topic.name} policy with public access"
+                                    f"SNS topic {topic.name} is publicly accesible"
                                 )
                             else:
-                                report.status = "FAIL"
-                                report.status_extended = f"SNS topic {topic.name} policy with public access but has a Condition"
+                                report.status = "PASS"
+                                report.status_extended = f"SNS topic {topic.name} is publicly accesible but has a Condition that could filter it"
 
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_not_publicly_accessible/sqs_queues_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_queues_server_side_encryption_enabled/sqs_queues_server_side_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/sqs/sqs_service.py` & `prowler-3.5.0/prowler/providers/aws/services/sqs/sqs_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_document_secrets/ssm_document_secrets.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_documents_set_as_public/ssm_documents_set_as_public.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_managed_compliant_patching/ssm_managed_compliant_patching.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssm/ssm_service.py` & `prowler-3.5.0/prowler/providers/aws/services/ssm/ssm_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py` & `prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_enabled_with_plans/ssmincidents_enabled_with_plans.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py` & `prowler-3.5.0/prowler/providers/aws/services/ssmincidents/ssmincidents_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,20 @@
             t.start()
         for t in threads:
             t.join()
 
     def __list_replication_sets__(self):
         logger.info("SSMIncidents - Listing Replication Sets...")
         try:
-            regional_client = self.regional_clients[self.region]
-            list_replication_sets = regional_client.list_replication_sets()[
-                "replicationSetArns"
+            regional_client = self.regional_clients[
+                list(self.regional_clients.keys())[0]
             ]
+            list_replication_sets = regional_client.list_replication_sets().get(
+                "replicationSetArns"
+            )
             if list_replication_sets:
                 replication_set = list_replication_sets[0]
                 if not self.audit_resources or (
                     is_resource_filtered(replication_set, self.audit_resources)
                 ):
                     self.replication_set = [
                         ReplicationSet(
@@ -70,14 +72,16 @@
             logger.error(
                 f"{error.__class__.__name__}:{error.__traceback__.tb_lineno} -- {error}"
             )
 
     def __get_replication_set__(self):
         logger.info("SSMIncidents - Getting Replication Sets...")
         try:
+            if not self.replication_set:
+                return
             replication_set = self.replication_set[0]
             for regional_client in self.regional_clients.values():
                 try:
                     get_replication_set = regional_client.get_replication_set(
                         arn=replication_set.arn
                     )["replicationSet"]
                     replication_set.status = get_replication_set["status"]
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py` & `prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_errors_and_warnings/trustedadvisor_errors_and_warnings.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 
 class trustedadvisor_errors_and_warnings(Check):
     def execute(self):
         findings = []
         if trustedadvisor_client.enabled:
             if trustedadvisor_client.checks:
                 for check in trustedadvisor_client.checks:
-                    report = Check_Report_AWS(self.metadata())
-                    report.region = check.region
-                    report.resource_id = check.id
-                    report.status = "FAIL"
-                    report.status_extended = f"Trusted Advisor check {check.name} is in state {check.status}."
-                    if check.status == "ok":
-                        report.status = "PASS"
-                    findings.append(report)
+                    if (
+                        check.status != "not_available"
+                    ):  # avoid not_available checks since there are no resources that apply
+                        report = Check_Report_AWS(self.metadata())
+                        report.region = check.region
+                        report.resource_id = check.id
+                        report.status = "FAIL"
+                        report.status_extended = f"Trusted Advisor check {check.name} is in state {check.status}."
+                        if check.status == "ok":
+                            report.status = "PASS"
+                        findings.append(report)
         else:
             report = Check_Report_AWS(self.metadata())
             report.status = "INFO"
             report.status_extended = "Amazon Web Services Premium Support Subscription is required to use this service."
             report.resource_id = trustedadvisor_client.account
             report.region = trustedadvisor_client.region
             findings.append(report)
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py` & `prowler-3.5.0/prowler/providers/aws/services/trustedadvisor/trustedadvisor_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_different_regions/vpc_different_regions.py` & `prowler-3.5.0/prowler/providers/aws/services/s3/s3_bucket_object_lock/s3_bucket_object_lock.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
-from prowler.providers.aws.services.vpc.vpc_client import vpc_client
+from prowler.providers.aws.services.s3.s3_client import s3_client
 
 
-class vpc_different_regions(Check):
+class s3_bucket_object_lock(Check):
     def execute(self):
         findings = []
-        region = None
-        for vpc in vpc_client.vpcs:
-            if not vpc.default:
-                report = Check_Report_AWS(self.metadata())
-                # This is a global check under the vpc service: region, resource_id and tags are not relevant here but we keep them for consistency
-                report.region = vpc.region
-                report.resource_id = vpc.id
-                report.resource_tags = vpc.tags
+        for bucket in s3_client.buckets:
+            report = Check_Report_AWS(self.metadata())
+            report.region = bucket.region
+            report.resource_id = bucket.name
+            report.resource_arn = bucket.arn
+            report.resource_tags = bucket.tags
+            if bucket.object_lock:
+                report.status = "PASS"
+                report.status_extended = (
+                    f"S3 Bucket {bucket.name} has Object Lock enabled."
+                )
+            else:
                 report.status = "FAIL"
-                report.status_extended = f"VPCs found only in one region {vpc.region}."
-                if region and vpc.region != region:
-                    report.status = "PASS"
-                    report.status_extended = "VPCs found in more than one region."
-                    break
-                region = vpc.region
-
-        findings.append(report)
+                report.status_extended = (
+                    f"S3 Bucket {bucket.name} has Object Lock disabled."
+                )
+            findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_connections_trust_boundaries/vpc_endpoint_connections_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_endpoint_services_allowed_principals_trust_boundaries/vpc_endpoint_services_allowed_principals_trust_boundaries.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_flow_logs_enabled/vpc_flow_logs_enabled.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.vpc.vpc_client import vpc_client
 
 
 class vpc_flow_logs_enabled(Check):
     def execute(self):
         findings = []
-        for vpc in vpc_client.vpcs:
+        for vpc in vpc_client.vpcs.values():
             report = Check_Report_AWS(self.metadata())
             report.region = vpc.region
             report.resource_tags = vpc.tags
             if vpc.flow_log:
                 report.status = "PASS"
                 report.status_extended = f"VPC {vpc.id} Flow logs are enabled."
                 report.resource_id = vpc.id
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_peering_routing_tables_with_least_privilege/vpc_peering_routing_tables_with_least_privilege.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_service.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,32 @@
 class VPC:
     def __init__(self, audit_info):
         self.service = "ec2"
         self.session = audit_info.audit_session
         self.audited_account = audit_info.audited_account
         self.audit_resources = audit_info.audit_resources
         self.regional_clients = generate_regional_clients(self.service, audit_info)
-        self.vpcs = []
+        self.vpcs = {}
         self.vpc_peering_connections = []
         self.vpc_endpoints = []
         self.vpc_endpoint_services = []
         self.__threading_call__(self.__describe_vpcs__)
         self.__threading_call__(self.__describe_vpc_peering_connections__)
         self.__threading_call__(self.__describe_vpc_endpoints__)
         self.__threading_call__(self.__describe_vpc_endpoint_services__)
         self.__describe_flow_logs__()
         self.__describe_peering_route_tables__()
         self.__describe_vpc_endpoint_service_permissions__()
-        self.vpc_subnets = []
+        self.vpc_subnets = {}
         self.__threading_call__(self.__describe_vpc_subnets__)
+        self.region = (
+            audit_info.profile_region
+            if audit_info.profile_region
+            else list(self.regional_clients.keys())[0]
+        )
 
     def __get_session__(self):
         return self.session
 
     def __threading_call__(self, call):
         threads = []
         for regional_client in self.regional_clients.values():
@@ -48,22 +53,20 @@
         try:
             describe_vpcs_paginator = regional_client.get_paginator("describe_vpcs")
             for page in describe_vpcs_paginator.paginate():
                 for vpc in page["Vpcs"]:
                     if not self.audit_resources or (
                         is_resource_filtered(vpc["VpcId"], self.audit_resources)
                     ):
-                        self.vpcs.append(
-                            VPCs(
-                                id=vpc["VpcId"],
-                                default=vpc["IsDefault"],
-                                cidr_block=vpc["CidrBlock"],
-                                region=regional_client.region,
-                                tags=vpc.get("Tags"),
-                            )
+                        self.vpcs[vpc["VpcId"]] = VPCs(
+                            id=vpc["VpcId"],
+                            default=vpc["IsDefault"],
+                            cidr_block=vpc["CidrBlock"],
+                            region=regional_client.region,
+                            tags=vpc.get("Tags"),
                         )
         except Exception as error:
             logger.error(
                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
     def __describe_vpc_peering_connections__(self, regional_client):
@@ -131,15 +134,15 @@
             logger.error(
                 f"{error.__class__.__name__}:{error.__traceback__.tb_lineno} -- {error}"
             )
 
     def __describe_flow_logs__(self):
         logger.info("VPC - Describing flow logs...")
         try:
-            for vpc in self.vpcs:
+            for vpc in self.vpcs.values():
                 regional_client = self.regional_clients[vpc.region]
                 flow_logs = regional_client.describe_flow_logs(
                     Filters=[
                         {
                             "Name": "resource-id",
                             "Values": [
                                 vpc.id,
@@ -268,34 +271,37 @@
                                                 "Name": "association.main",
                                                 "Values": ["true"],
                                             }
                                         ]
                                     )
                                 )
                             public = False
+                            nat_gateway = False
                             for route in route_tables_for_subnet.get("RouteTables")[
                                 0
                             ].get("Routes"):
                                 if "GatewayId" in route and "igw" in route["GatewayId"]:
                                     public = True
-                                    break
+                                if "NatGatewayId" in route:
+                                    nat_gateway = True
                             # Add it to to list of vpc_subnets and to the VPC object
                             object = VpcSubnet(
                                 id=subnet["SubnetId"],
                                 default=subnet["DefaultForAz"],
                                 vpc_id=subnet["VpcId"],
                                 cidr_block=subnet["CidrBlock"],
                                 region=regional_client.region,
                                 availability_zone=subnet["AvailabilityZone"],
                                 public=public,
+                                nat_gateway=nat_gateway,
                                 tags=subnet.get("Tags"),
                             )
-                            self.vpc_subnets.append(object)
+                            self.vpc_subnets[subnet["SubnetId"]] = object
                             # Add it to the VPC object
-                            for vpc in self.vpcs:
+                            for vpc in self.vpcs.values():
                                 if vpc.id == subnet["VpcId"]:
                                     vpc.subnets.append(object)
                         except Exception as error:
                             logger.error(
                                 f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
                             )
         except Exception as error:
@@ -307,14 +313,15 @@
 class VpcSubnet(BaseModel):
     id: str
     default: bool
     vpc_id: str
     cidr_block: str
     availability_zone: str
     public: bool
+    nat_gateway: bool
     region: str
     tags: Optional[list] = []
 
 
 class VPCs(BaseModel):
     id: str
     default: bool
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_different_az/vpc_subnet_different_az.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.vpc.vpc_client import vpc_client
 
 
 class vpc_subnet_different_az(Check):
     def execute(self):
         findings = []
-        for vpc in vpc_client.vpcs:
+        for vpc in vpc_client.vpcs.values():
             report = Check_Report_AWS(self.metadata())
             report.region = vpc.region
             report.resource_tags = vpc.tags
             report.status = "FAIL"
             report.status_extended = f"VPC {vpc.id} has no subnets."
             report.resource_id = vpc.id
             if vpc.subnets:
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py` & `prowler-3.5.0/prowler/providers/aws/services/vpc/vpc_subnet_separate_private_public/vpc_subnet_separate_private_public.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from prowler.lib.check.models import Check, Check_Report_AWS
 from prowler.providers.aws.services.vpc.vpc_client import vpc_client
 
 
 class vpc_subnet_separate_private_public(Check):
     def execute(self):
         findings = []
-        for vpc in vpc_client.vpcs:
+        for vpc in vpc_client.vpcs.values():
             report = Check_Report_AWS(self.metadata())
             report.region = vpc.region
             report.resource_tags = vpc.tags
             report.status = "FAIL"
             report.status_extended = f"VPC {vpc.id} has no subnets."
             report.resource_id = vpc.id
             if vpc.subnets:
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/waf/waf_service.py` & `prowler-3.5.0/prowler/providers/aws/services/waf/waf_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/wafv2/wafv2_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,66 @@
-import threading
-
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
-from prowler.lib.scan_filters.scan_filters import is_resource_filtered
-from prowler.providers.aws.aws_provider import generate_regional_clients
+from prowler.providers.gcp.gcp_provider import generate_client
 
 
-################### WAFv2
-class WAFv2:
+################## CloudSQL
+class CloudSQL:
     def __init__(self, audit_info):
-        self.service = "wafv2"
-        self.session = audit_info.audit_session
-        self.audit_resources = audit_info.audit_resources
-        self.regional_clients = generate_regional_clients(self.service, audit_info)
-        self.web_acls = []
-        self.__threading_call__(self.__list_web_acls__)
-        self.__threading_call__(self.__list_resources_for_web_acl__)
-
-    def __get_session__(self):
-        return self.session
-
-    def __threading_call__(self, call):
-        threads = []
-        for regional_client in self.regional_clients.values():
-            threads.append(threading.Thread(target=call, args=(regional_client,)))
-        for t in threads:
-            t.start()
-        for t in threads:
-            t.join()
+        self.service = "sqladmin"
+        self.api_version = "v1"
+        self.project_id = audit_info.project_id
+        self.client = generate_client(self.service, self.api_version, audit_info)
+        self.instances = []
+        self.__get_instances__()
 
-    def __list_web_acls__(self, regional_client):
-        logger.info("WAFv2 - Listing Regional Web ACLs...")
+    def __get_instances__(self):
         try:
-            for wafv2 in regional_client.list_web_acls(Scope="REGIONAL")["WebACLs"]:
-                if not self.audit_resources or (
-                    is_resource_filtered(wafv2["ARN"], self.audit_resources)
-                ):
-                    self.web_acls.append(
-                        WebAclv2(
-                            arn=wafv2["ARN"],
-                            name=wafv2["Name"],
-                            id=wafv2["Id"],
-                            albs=[],
-                            region=regional_client.region,
+            request = self.client.instances().list(project=self.project_id)
+            while request is not None:
+                response = request.execute()
+
+                for instance in response.get("items", []):
+                    public_ip = False
+                    for address in instance.get("ipAddresses", []):
+                        if address["type"] == "PRIMARY":
+                            public_ip = True
+                    self.instances.append(
+                        Instance(
+                            name=instance["name"],
+                            version=instance["databaseVersion"],
+                            region=instance["region"],
+                            ip_addresses=instance.get("ipAddresses", []),
+                            public_ip=public_ip,
+                            ssl=instance["settings"]["ipConfiguration"].get(
+                                "requireSsl", False
+                            ),
+                            automated_backups=instance["settings"][
+                                "backupConfiguration"
+                            ]["enabled"],
+                            authorized_networks=instance["settings"]["ipConfiguration"][
+                                "authorizedNetworks"
+                            ],
+                            flags=instance["settings"].get("databaseFlags", []),
                         )
                     )
-        except Exception as error:
-            logger.error(
-                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
-            )
-
-    def __list_resources_for_web_acl__(self, regional_client):
-        logger.info("WAFv2 - Describing resources...")
-        try:
-            for acl in self.web_acls:
-                if acl.region == regional_client.region:
-                    for resource in regional_client.list_resources_for_web_acl(
-                        WebACLArn=acl.arn, ResourceType="APPLICATION_LOAD_BALANCER"
-                    )["ResourceArns"]:
-                        acl.albs.append(resource)
 
+                request = self.client.instances().list_next(
+                    previous_request=request, previous_response=response
+                )
         except Exception as error:
             logger.error(
-                f"{regional_client.region} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+                f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
 
-class WebAclv2(BaseModel):
-    arn: str
+class Instance(BaseModel):
     name: str
-    id: str
-    albs: list[str]
+    version: str
+    ip_addresses: list
     region: str
+    public_ip: bool
+    authorized_networks: list
+    ssl: bool
+    automated_backups: bool
+    flags: list
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_service.py` & `prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,19 +41,21 @@
                 for workspace in page["Workspaces"]:
                     if not self.audit_resources or (
                         is_resource_filtered(
                             workspace["WorkspaceId"], self.audit_resources
                         )
                     ):
                         workspace_to_append = WorkSpace(
-                            id=workspace["WorkspaceId"], region=regional_client.region
+                            id=workspace.get("WorkspaceId"),
+                            region=regional_client.region,
+                            subnet_id=workspace.get("SubnetId"),
                         )
                         if (
                             "UserVolumeEncryptionEnabled" in workspace
-                            and workspace["UserVolumeEncryptionEnabled"]
+                            and workspace.get("UserVolumeEncryptionEnabled")
                         ):
                             workspace_to_append.user_volume_encryption_enabled = True
                         if (
                             "RootVolumeEncryptionEnabled" in workspace
                             and workspace["RootVolumeEncryptionEnabled"]
                         ):
                             workspace_to_append.root_volume_encryption_enabled = True
@@ -81,8 +83,9 @@
 
 class WorkSpace(BaseModel):
     id: str
     arn: str = ""
     region: str
     user_volume_encryption_enabled: bool = None
     root_volume_encryption_enabled: bool = None
+    subnet_id: str = None
     tags: Optional[list] = []
```

### Comparing `prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py` & `prowler-3.5.0/prowler/providers/aws/services/workspaces/workspaces_volume_encryption_enabled/workspaces_volume_encryption_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/azure_provider.py` & `prowler-3.5.0/prowler/providers/azure/azure_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/lib/audit_info/models.py` & `prowler-3.5.0/prowler/providers/azure/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_app_services_is_on/defender_ensure_defender_for_app_services_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_arm_is_on/defender_ensure_defender_for_arm_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_azure_sql_databases_is_on/defender_ensure_defender_for_azure_sql_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_containers_is_on/defender_ensure_defender_for_containers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_cosmosdb_is_on/defender_ensure_defender_for_cosmosdb_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_databases_is_on/defender_ensure_defender_for_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_dns_is_on/defender_ensure_defender_for_dns_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_keyvault_is_on/defender_ensure_defender_for_keyvault_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_os_relational_databases_is_on/defender_ensure_defender_for_os_relational_databases_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_server_is_on/defender_ensure_defender_for_server_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_sql_servers_is_on/defender_ensure_defender_for_sql_servers_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_ensure_defender_for_storage_is_on/defender_ensure_defender_for_storage_is_on.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/defender/defender_service.py` & `prowler-3.5.0/prowler/providers/azure/services/defender/defender_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/iam/iam_service.py` & `prowler-3.5.0/prowler/providers/azure/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py` & `prowler-3.5.0/prowler/providers/azure/services/iam/iam_subscription_roles_owner_custom_not_created/iam_subscription_roles_owner_custom_not_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_blob_public_access_level_is_disabled/storage_blob_public_access_level_is_disabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_default_network_access_rule_is_denied/storage_default_network_access_rule_is_denied.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_azure_services_are_trusted_to_access_is_enabled/storage_ensure_azure_services_are_trusted_to_access_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_encryption_with_customer_managed_keys/storage_ensure_encryption_with_customer_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_ensure_minimum_tls_version_12/storage_ensure_minimum_tls_version_12.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_infrastructure_encryption_is_enabled/storage_infrastructure_encryption_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_secure_transfer_required_is_enabled/storage_secure_transfer_required_is_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/azure/services/storage/storage_service.py` & `prowler-3.5.0/prowler/providers/azure/services/storage/storage_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/common/allowlist.py` & `prowler-3.5.0/prowler/providers/common/allowlist.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/common/audit_info.py` & `prowler-3.5.0/prowler/providers/common/audit_info.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/common/outputs.py` & `prowler-3.5.0/prowler/providers/common/outputs.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/common/quick_inventory.py` & `prowler-3.5.0/prowler/providers/common/quick_inventory.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/gcp_provider.py` & `prowler-3.5.0/prowler/providers/gcp/gcp_provider.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/lib/audit_info/models.py` & `prowler-3.5.0/prowler/providers/gcp/lib/audit_info/models.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_cmk_encryption/bigquery_dataset_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_dataset_public_access/bigquery_dataset_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py` & `prowler-3.5.0/prowler/providers/gcp/services/bigquery/bigquery_table_cmk_encryption/bigquery_table_cmk_encryption.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudresourcemanager/cloudresourcemanager_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_automated_backups/cloudsql_instance_automated_backups.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_local_infile_flag/cloudsql_instance_mysql_local_infile_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_mysql_skip_show_database_flag/cloudsql_instance_mysql_skip_show_database_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_enable_pgaudit_flag/cloudsql_instance_postgres_enable_pgaudit_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_connections_flag/cloudsql_instance_postgres_log_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_disconnections_flag/cloudsql_instance_postgres_log_disconnections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_error_verbosity_flag/cloudsql_instance_postgres_log_error_verbosity_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class cloudsql_instance_postgres_log_error_verbosity_flag(Check):
+class cloudsql_instance_postgres_log_min_duration_statement_flag(Check):
     def execute(self) -> Check_Report_GCP:
         findings = []
         for instance in cloudsql_client.instances:
             if "POSTGRES" in instance.version:
                 report = Check_Report_GCP(self.metadata())
                 report.project_id = cloudsql_client.project_id
                 report.resource_id = instance.name
                 report.resource_name = instance.name
                 report.location = instance.region
                 report.status = "FAIL"
-                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_error_verbosity' flag set to 'default'"
+                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_min_duration_statement' flag set to '-1'"
                 for flag in instance.flags:
                     if (
-                        flag["name"] == "log_error_verbosity"
-                        and flag["value"] == "default"
+                        flag["name"] == "log_min_duration_statement"
+                        and flag["value"] == "-1"
                     ):
                         report.status = "PASS"
-                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_error_verbosity' flag set to 'default'"
+                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_min_duration_statement' flag set to '-1'"
                         break
                 findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_duration_statement_flag/cloudsql_instance_postgres_log_min_duration_statement_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class cloudsql_instance_postgres_log_min_duration_statement_flag(Check):
+class cloudsql_instance_postgres_log_min_error_statement_flag(Check):
     def execute(self) -> Check_Report_GCP:
+        desired_log_min_error_statement = "error"
         findings = []
         for instance in cloudsql_client.instances:
             if "POSTGRES" in instance.version:
                 report = Check_Report_GCP(self.metadata())
                 report.project_id = cloudsql_client.project_id
                 report.resource_id = instance.name
                 report.resource_name = instance.name
                 report.location = instance.region
                 report.status = "FAIL"
-                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_min_duration_statement' flag set to '-1'"
+                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_min_error_statement' flag set minimum to '{desired_log_min_error_statement}'"
                 for flag in instance.flags:
                     if (
-                        flag["name"] == "log_min_duration_statement"
-                        and flag["value"] == "-1"
+                        flag["name"] == "log_min_error_statement"
+                        and flag["value"] == desired_log_min_error_statement
                     ):
                         report.status = "PASS"
-                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_min_duration_statement' flag set to '-1'"
+                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_min_error_statement' flag set minimum to '{desired_log_min_error_statement}'"
                         break
                 findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_error_statement_flag/cloudsql_instance_postgres_log_min_error_statement_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class cloudsql_instance_postgres_log_min_error_statement_flag(Check):
+class cloudsql_instance_postgres_log_statement_flag(Check):
     def execute(self) -> Check_Report_GCP:
-        desired_log_min_error_statement = "error"
+        desired_log_statement = "ddl"
         findings = []
         for instance in cloudsql_client.instances:
             if "POSTGRES" in instance.version:
                 report = Check_Report_GCP(self.metadata())
                 report.project_id = cloudsql_client.project_id
                 report.resource_id = instance.name
                 report.resource_name = instance.name
                 report.location = instance.region
                 report.status = "FAIL"
-                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_min_error_statement' flag set minimum to '{desired_log_min_error_statement}'"
+                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_statement' flag set to '{desired_log_statement}'"
                 for flag in instance.flags:
                     if (
-                        flag["name"] == "log_min_error_statement"
-                        and flag["value"] == desired_log_min_error_statement
+                        flag["name"] == "log_statement"
+                        and flag["value"] == desired_log_statement
                     ):
                         report.status = "PASS"
-                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_min_error_statement' flag set minimum to '{desired_log_min_error_statement}'"
+                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_statement' flag set to '{desired_log_statement}'"
                         break
                 findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_min_messages_flag/cloudsql_instance_postgres_log_min_messages_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_postgres_log_statement_flag/cloudsql_instance_postgres_log_statement_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class cloudsql_instance_postgres_log_statement_flag(Check):
+class cloudsql_instance_sqlserver_trace_flag(Check):
     def execute(self) -> Check_Report_GCP:
-        desired_log_statement = "ddl"
         findings = []
         for instance in cloudsql_client.instances:
-            if "POSTGRES" in instance.version:
+            if "SQLSERVER" in instance.version:
                 report = Check_Report_GCP(self.metadata())
                 report.project_id = cloudsql_client.project_id
                 report.resource_id = instance.name
                 report.resource_name = instance.name
                 report.location = instance.region
-                report.status = "FAIL"
-                report.status_extended = f"PostgreSQL Instance {instance.name} has not 'log_statement' flag set to '{desired_log_statement}'"
+                report.status = "PASS"
+                report.status_extended = f"SQL Server Instance {instance.name} has '3625 (trace flag)' flag set to 'on'"
                 for flag in instance.flags:
-                    if (
-                        flag["name"] == "log_statement"
-                        and flag["value"] == desired_log_statement
-                    ):
-                        report.status = "PASS"
-                        report.status_extended = f"PostgreSQL Instance {instance.name} has 'log_statement' flag set to '{desired_log_statement}'"
+                    if flag["name"] == "3625" and flag["value"] == "off":
+                        report.status = "FAIL"
+                        report.status_extended = f"SQL Server Instance {instance.name} has '3625 (trace flag)' flag set to 'off'"
                         break
                 findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_private_ip_assignment/cloudsql_instance_private_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_access/cloudsql_instance_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_public_ip/cloudsql_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_contained_database_authentication_flag/cloudsql_instance_sqlserver_contained_database_authentication_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag/cloudsql_instance_sqlserver_cross_db_ownership_chaining_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_external_scripts_enabled_flag/cloudsql_instance_sqlserver_external_scripts_enabled_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_remote_access_flag/cloudsql_instance_sqlserver_remote_access_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_trace_flag/cloudsql_instance_sqlserver_trace_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
 
 
-class cloudsql_instance_sqlserver_trace_flag(Check):
+class cloudsql_instance_ssl_connections(Check):
     def execute(self) -> Check_Report_GCP:
         findings = []
         for instance in cloudsql_client.instances:
-            if "SQLSERVER" in instance.version:
-                report = Check_Report_GCP(self.metadata())
-                report.project_id = cloudsql_client.project_id
-                report.resource_id = instance.name
-                report.resource_name = instance.name
-                report.location = instance.region
-                report.status = "PASS"
-                report.status_extended = f"SQL Server Instance {instance.name} has '3625 (trace flag)' flag set to 'on'"
-                for flag in instance.flags:
-                    if flag["name"] == "3625" and flag["value"] == "off":
-                        report.status = "FAIL"
-                        report.status_extended = f"SQL Server Instance {instance.name} has '3625 (trace flag)' flag set to 'off'"
-                        break
-                findings.append(report)
+            report = Check_Report_GCP(self.metadata())
+            report.project_id = cloudsql_client.project_id
+            report.resource_id = instance.name
+            report.resource_name = instance.name
+            report.location = instance.region
+            report.status = "PASS"
+            report.status_extended = (
+                f"Database Instance {instance.name} requires SSL connections"
+            )
+            if not instance.ssl:
+                report.status = "FAIL"
+                report.status_extended = f"Database Instance {instance.name} does not require SSL connections"
+            findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_connections_flag/cloudsql_instance_sqlserver_user_connections_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_sqlserver_user_options_flag/cloudsql_instance_sqlserver_user_options_flag.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_instance_ssl_connections/cloudsql_instance_ssl_connections.py` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
-from prowler.providers.gcp.services.cloudsql.cloudsql_client import cloudsql_client
+from prowler.providers.gcp.services.cloudresourcemanager.cloudresourcemanager_client import (
+    cloudresourcemanager_client,
+)
+from prowler.providers.gcp.services.iam.iam_client import iam_client
 
 
-class cloudsql_instance_ssl_connections(Check):
+class iam_sa_no_administrative_privileges(Check):
     def execute(self) -> Check_Report_GCP:
         findings = []
-        for instance in cloudsql_client.instances:
+        for account in iam_client.service_accounts:
             report = Check_Report_GCP(self.metadata())
-            report.project_id = cloudsql_client.project_id
-            report.resource_id = instance.name
-            report.resource_name = instance.name
-            report.location = instance.region
+            report.project_id = iam_client.project_id
+            report.resource_id = account.email
+            report.resource_name = account.name
+            report.location = iam_client.region
             report.status = "PASS"
             report.status_extended = (
-                f"Database Instance {instance.name} requires SSL connections"
+                f"Account {account.email} has no administrative privileges"
             )
-            if not instance.ssl:
-                report.status = "FAIL"
-                report.status_extended = f"Database Instance {instance.name} does not require SSL connections"
+            for binding in cloudresourcemanager_client.bindings:
+                if f"serviceAccount:{account.email}" in binding.members and (
+                    "admin" in binding.role.lower()
+                    or "owner" in binding.role.lower()
+                    or "editor" in binding.role.lower()
+                ):
+                    report.status = "FAIL"
+                    report.status_extended = f"Account {account.email} has administrative privileges with {binding.role}"
             findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudsql/cloudsql_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/compute/compute_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,102 @@
 from pydantic import BaseModel
 
 from prowler.lib.logger import logger
 from prowler.providers.gcp.gcp_provider import generate_client
 
 
-################## CloudSQL
-class CloudSQL:
+################## Compute
+class Compute:
     def __init__(self, audit_info):
-        self.service = "sqladmin"
+        self.service = "compute"
         self.api_version = "v1"
         self.project_id = audit_info.project_id
         self.client = generate_client(self.service, self.api_version, audit_info)
+        self.zones = []
         self.instances = []
+        self.networks = []
+        self.__get_zones__()
         self.__get_instances__()
+        self.__get_networks__()
+
+    def __get_zones__(self):
+        try:
+            request = self.client.zones().list(project=self.project_id)
+            while request is not None:
+                response = request.execute()
+
+                for zone in response.get("items", []):
+                    self.zones.append(zone["name"])
+
+                request = self.client.zones().list_next(
+                    previous_request=request, previous_response=response
+                )
+        except Exception as error:
+            logger.error(
+                f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
 
     def __get_instances__(self):
         try:
-            request = self.client.instances().list(project=self.project_id)
+            for zone in self.zones:
+                request = self.client.instances().list(
+                    project=self.project_id, zone=zone
+                )
+                while request is not None:
+                    response = request.execute()
+
+                    for instance in response.get("items", []):
+                        public_ip = False
+                        for interface in instance["networkInterfaces"]:
+                            for config in interface.get("accessConfigs", []):
+                                if "natIP" in config:
+                                    public_ip = True
+                        self.instances.append(
+                            Instance(
+                                name=instance["name"],
+                                id=instance["id"],
+                                zone=zone,
+                                public_ip=public_ip,
+                            )
+                        )
+
+                    request = self.client.instances().list_next(
+                        previous_request=request, previous_response=response
+                    )
+        except Exception as error:
+            logger.error(
+                f"{zone} -- {error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
+            )
+
+    def __get_networks__(self):
+        try:
+            request = self.client.networks().list(project=self.project_id)
             while request is not None:
                 response = request.execute()
 
-                for instance in response.get("items", []):
-                    public_ip = False
-                    for address in instance.get("ipAddresses", []):
-                        if address["type"] == "PRIMARY":
-                            public_ip = True
-                    self.instances.append(
-                        Instance(
-                            name=instance["name"],
-                            version=instance["databaseVersion"],
-                            region=instance["region"],
-                            ip_addresses=instance.get("ipAddresses", []),
-                            public_ip=public_ip,
-                            ssl=instance["settings"]["ipConfiguration"].get(
-                                "requireSsl", False
-                            ),
-                            automated_backups=instance["settings"][
-                                "backupConfiguration"
-                            ]["enabled"],
-                            authorized_networks=instance["settings"]["ipConfiguration"][
-                                "authorizedNetworks"
-                            ],
-                            flags=instance["settings"].get("databaseFlags", []),
+                for network in response.get("items", []):
+                    self.networks.append(
+                        Network(
+                            name=network["name"],
+                            id=network["id"],
                         )
                     )
 
-                request = self.client.instances().list_next(
+                request = self.client.networks().list_next(
                     previous_request=request, previous_response=response
                 )
         except Exception as error:
             logger.error(
                 f"{error.__class__.__name__}[{error.__traceback__.tb_lineno}]: {error}"
             )
 
 
 class Instance(BaseModel):
     name: str
-    version: str
-    ip_addresses: list
-    region: str
+    id: str
+    zone: str
     public_ip: bool
-    authorized_networks: list
-    ssl: bool
-    automated_backups: bool
-    flags: list
+
+
+class Network(BaseModel):
+    name: str
+    id: str
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_public_access/cloudstorage_bucket_public_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_bucket_uniform_bucket_level_access/cloudstorage_bucket_uniform_bucket_level_access.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/cloudstorage/cloudstorage_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/compute/compute_instance_public_ip/compute_instance_public_ip.py` & `prowler-3.5.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from prowler.lib.check.models import Check, Check_Report_GCP
 from prowler.providers.gcp.services.compute.compute_client import compute_client
 
 
-class compute_instance_public_ip(Check):
+class compute_network_default_in_use(Check):
     def execute(self) -> Check_Report_GCP:
         findings = []
-        for instance in compute_client.instances:
-            report = Check_Report_GCP(self.metadata())
-            report.project_id = compute_client.project_id
-            report.resource_id = instance.id
-            report.resource_name = instance.name
-            report.location = instance.zone
-            report.status = "PASS"
-            report.status_extended = f"VM Instance {instance.name} has not a public IP"
-            if instance.public_ip:
+        report = Check_Report_GCP(self.metadata())
+        report.project_id = compute_client.project_id
+        report.resource_id = "default"
+        report.resource_name = "default"
+        report.location = "global"
+        report.status = "PASS"
+        report.status_extended = "Default network does not exist"
+        for network in compute_client.networks:
+            if network.name == "default":
                 report.status = "FAIL"
-                report.status_extended = f"VM Instance {instance.name} has a public IP"
-            findings.append(report)
+                report.status_extended = "Default network is in use"
+
+        findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/compute/compute_network_default_in_use/compute_network_default_in_use.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_administrative_privileges/iam_sa_no_administrative_privileges.py` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,26 @@
+from datetime import datetime
+
 from prowler.lib.check.models import Check, Check_Report_GCP
-from prowler.providers.gcp.services.cloudresourcemanager.cloudresourcemanager_client import (
-    cloudresourcemanager_client,
-)
 from prowler.providers.gcp.services.iam.iam_client import iam_client
 
 
-class iam_sa_no_administrative_privileges(Check):
+class iam_sa_user_managed_key_rotate_90_days(Check):
     def execute(self) -> Check_Report_GCP:
         findings = []
         for account in iam_client.service_accounts:
-            report = Check_Report_GCP(self.metadata())
-            report.project_id = iam_client.project_id
-            report.resource_id = account.email
-            report.resource_name = account.name
-            report.location = iam_client.region
-            report.status = "PASS"
-            report.status_extended = (
-                f"Account {account.email} has no administrative privileges"
-            )
-            for binding in cloudresourcemanager_client.bindings:
-                if f"serviceAccount:{account.email}" in binding.members and (
-                    "admin" in binding.role.lower()
-                    or "owner" in binding.role.lower()
-                    or "editor" in binding.role.lower()
-                ):
-                    report.status = "FAIL"
-                    report.status_extended = f"Account {account.email} has administrative privileges with {binding.role}"
-            findings.append(report)
+            for key in account.keys:
+                if key.type == "USER_MANAGED":
+                    last_rotated = (datetime.now() - key.valid_after).days
+                    report = Check_Report_GCP(self.metadata())
+                    report.project_id = iam_client.project_id
+                    report.resource_id = key.name
+                    report.resource_name = account.email
+                    report.location = iam_client.region
+                    report.status = "PASS"
+                    report.status_extended = f"User-managed key {key.name} for account {account.email} was rotated over the last 90 days ({last_rotated} days ago)"
+                    if last_rotated > 90:
+                        report.status = "FAIL"
+                        report.status_extended = f"User-managed key {key.name} for account {account.email} was not rotated over the last 90 days ({last_rotated} days ago)"
+                    findings.append(report)
 
         return findings
```

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_no_user_managed_keys/iam_sa_no_user_managed_keys.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_sa_user_managed_key_rotate_90_days/iam_sa_user_managed_key_rotate_90_days.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/iam/iam_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/iam/iam_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py` & `prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_not_publicly_accessible/kms_key_not_publicly_accessible.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/kms/kms_key_rotation_enabled/kms_key_rotation_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/kms/kms_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/kms/kms_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_audit_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled/logging_log_metric_filter_and_alert_for_bucket_permission_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled/logging_log_metric_filter_and_alert_for_custom_role_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled/logging_log_metric_filter_and_alert_for_project_ownership_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled/logging_log_metric_filter_and_alert_for_sql_instance_configuration_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_firewall_rule_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled/logging_log_metric_filter_and_alert_for_vpc_network_route_changes_enabled.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.metadata.json`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py` & `prowler-3.5.0/prowler/providers/gcp/services/logging/logging_sink_created/logging_sink_created.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/prowler/providers/gcp/services/monitoring/monitoring_service.py` & `prowler-3.5.0/prowler/providers/gcp/services/monitoring/monitoring_service.py`

 * *Files identical despite different names*

### Comparing `prowler-3.4.1/pyproject.toml` & `prowler-3.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,52 +18,53 @@
   "Pepe Fagoaga <pepe@verica.io>"
 ]
 name = "prowler"
 packages = [
   {include = "prowler"}
 ]
 readme = "README.md"
-version = "3.4.1"
+version = "3.5.0"
 
 [tool.poetry.dependencies]
 alive-progress = "3.1.1"
 arnparse = "0.0.2"
 azure-identity = "1.12.0"
 azure-mgmt-authorization = "3.0.0"
 azure-mgmt-security = "5.0.0"
 azure-mgmt-storage = "21.0.0"
 azure-mgmt-subscription = "3.1.1"
 azure-storage-blob = "12.16.0"
-boto3 = "1.26.115"
-botocore = "1.29.115"
+boto3 = "1.26.125"
+botocore = "1.29.125"
 colorama = "0.4.6"
 detect-secrets = "1.4.0"
-google-api-python-client = "2.84.0"
-mkdocs = {version = "1.4.2", optional = true}
-mkdocs-material = {version = "9.1.6", optional = true}
+google-api-python-client = "2.86.0"
+mkdocs = {version = "1.4.3", optional = true}
+mkdocs-material = {version = "9.1.8", optional = true}
 msgraph-core = "0.2.2"
 pydantic = "1.10.7"
 python = "^3.9"
 schema = "0.7.5"
 shodan = "1.28.0"
+slack-sdk = "3.21.3"
 tabulate = "0.9.0"
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material"]
 
 [tool.poetry.group.dev.dependencies]
 bandit = "1.7.5"
 black = "22.12.0"
-coverage = "7.2.3"
-docker = "6.0.1"
+coverage = "7.2.5"
+docker = "6.1.1"
 flake8 = "6.0.0"
 freezegun = "1.2.2"
-moto = "4.1.8"
+moto = "4.1.9"
 openapi-spec-validator = "0.5.6"
-pylint = "2.17.3"
+pylint = "2.17.4"
 pytest = "7.3.1"
 pytest-xdist = "3.2.1"
 safety = "2.3.5"
 sure = "2.0.1"
 vulture = "2.7"
 
 [tool.poetry.scripts]
```

### Comparing `prowler-3.4.1/PKG-INFO` & `prowler-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowler
-Version: 3.4.1
+Version: 3.5.0
 Summary: Prowler is an Open Source security tool to perform Cloud Security best practices assessments, audits, incident response, continuous monitoring, hardening and forensics readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001, GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks.
 License: Apache-2.0
 Author: Toni de la Fuente
 Author-email: toni@blyx.com
 Maintainer: Sergio Garcia
 Maintainer-email: sergio@verica.io
 Requires-Python: >=3.9,<4.0
@@ -20,25 +20,26 @@
 Requires-Dist: arnparse (==0.0.2)
 Requires-Dist: azure-identity (==1.12.0)
 Requires-Dist: azure-mgmt-authorization (==3.0.0)
 Requires-Dist: azure-mgmt-security (==5.0.0)
 Requires-Dist: azure-mgmt-storage (==21.0.0)
 Requires-Dist: azure-mgmt-subscription (==3.1.1)
 Requires-Dist: azure-storage-blob (==12.16.0)
-Requires-Dist: boto3 (==1.26.115)
-Requires-Dist: botocore (==1.29.115)
+Requires-Dist: boto3 (==1.26.125)
+Requires-Dist: botocore (==1.29.125)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: detect-secrets (==1.4.0)
-Requires-Dist: google-api-python-client (==2.84.0)
-Requires-Dist: mkdocs (==1.4.2) ; extra == "docs"
-Requires-Dist: mkdocs-material (==9.1.6) ; extra == "docs"
+Requires-Dist: google-api-python-client (==2.86.0)
+Requires-Dist: mkdocs (==1.4.3) ; extra == "docs"
+Requires-Dist: mkdocs-material (==9.1.8) ; extra == "docs"
 Requires-Dist: msgraph-core (==0.2.2)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: schema (==0.7.5)
 Requires-Dist: shodan (==1.28.0)
+Requires-Dist: slack-sdk (==3.21.3)
 Requires-Dist: tabulate (==0.9.0)
 Project-URL: Changelog, https://github.com/prowler-cloud/prowler/releases
 Project-URL: Documentation, https://docs.prowler.cloud
 Project-URL: Homepage, https://github.com/prowler-cloud/prowler
 Project-URL: Issue tracker, https://github.com/prowler-cloud/prowler/issues
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prowler Version: 3.4.1 Summary: Prowler is an Open
+Metadata-Version: 2.1 Name: prowler Version: 3.5.0 Summary: Prowler is an Open
 Source security tool to perform Cloud Security best practices assessments,
 audits, incident response, continuous monitoring, hardening and forensics
 readiness. It contains more than 240 controls covering CIS, PCI-DSS, ISO27001,
 GDPR, HIPAA, FFIEC, SOC2, AWS FTR, ENS and custom security frameworks. License:
 Apache-2.0 Author: Toni de la Fuente Author-email: toni@blyx.com Maintainer:
 Sergio Garcia Maintainer-email: sergio@verica.io Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
@@ -11,24 +11,25 @@
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Provides-Extra:
 docs Requires-Dist: alive-progress (==3.1.1) Requires-Dist: arnparse (==0.0.2)
 Requires-Dist: azure-identity (==1.12.0) Requires-Dist: azure-mgmt-
 authorization (==3.0.0) Requires-Dist: azure-mgmt-security (==5.0.0) Requires-
 Dist: azure-mgmt-storage (==21.0.0) Requires-Dist: azure-mgmt-subscription
 (==3.1.1) Requires-Dist: azure-storage-blob (==12.16.0) Requires-Dist: boto3
-(==1.26.115) Requires-Dist: botocore (==1.29.115) Requires-Dist: colorama
+(==1.26.125) Requires-Dist: botocore (==1.29.125) Requires-Dist: colorama
 (==0.4.6) Requires-Dist: detect-secrets (==1.4.0) Requires-Dist: google-api-
-python-client (==2.84.0) Requires-Dist: mkdocs (==1.4.2) ; extra == "docs"
-Requires-Dist: mkdocs-material (==9.1.6) ; extra == "docs" Requires-Dist:
+python-client (==2.86.0) Requires-Dist: mkdocs (==1.4.3) ; extra == "docs"
+Requires-Dist: mkdocs-material (==9.1.8) ; extra == "docs" Requires-Dist:
 msgraph-core (==0.2.2) Requires-Dist: pydantic (==1.10.7) Requires-Dist: schema
-(==0.7.5) Requires-Dist: shodan (==1.28.0) Requires-Dist: tabulate (==0.9.0)
-Project-URL: Changelog, https://github.com/prowler-cloud/prowler/releases
-Project-URL: Documentation, https://docs.prowler.cloud Project-URL: Homepage,
-https://github.com/prowler-cloud/prowler Project-URL: Issue tracker, https://
-github.com/prowler-cloud/prowler/issues Description-Content-Type: text/markdown
+(==0.7.5) Requires-Dist: shodan (==1.28.0) Requires-Dist: slack-sdk (==3.21.3)
+Requires-Dist: tabulate (==0.9.0) Project-URL: Changelog, https://github.com/
+prowler-cloud/prowler/releases Project-URL: Documentation, https://
+docs.prowler.cloud Project-URL: Homepage, https://github.com/prowler-cloud/
+prowler Project-URL: Issue tracker, https://github.com/prowler-cloud/prowler/
+issues Description-Content-Type: text/markdown
                 [https://github.com/prowler-cloud/prowler/blob/
         62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-
 dark.png?raw=True#gh-dark-mode-only] [https://github.com/prowler-cloud/prowler/
       blob/62c1ce73bbcdd6b9e5ba03dfcae26dfd165defd9/docs/img/prowler-pro-
                     light.png?raw=True#gh-light-mode-only]
   See all the things you and your team can do with ProwlerPro at prowler.pro
 ===============================================================================
```

