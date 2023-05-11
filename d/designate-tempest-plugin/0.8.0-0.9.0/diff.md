# Comparing `tmp/designate-tempest-plugin-0.8.0.tar.gz` & `tmp/designate-tempest-plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/designate-tempest-plugin-0.8.0.tar", last modified: Fri Apr 24 12:42:24 2020, max compression
+gzip compressed data, was "dist/designate-tempest-plugin-0.9.0.tar", last modified: Fri Oct  2 12:24:27 2020, max compression
```

## Comparing `designate-tempest-plugin-0.8.0.tar` & `designate-tempest-plugin-0.9.0.tar`

### file list

```diff
@@ -1,137 +1,134 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9999 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8173 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      132 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/tools/pretty_flake8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4487 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/tools/pretty_flake8.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1328 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/hacking/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/query/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/query/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2813 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/query/query_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10534 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/json/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/json/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zones_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/transfer_accepts_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4294 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/pool_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5334 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/transfer_request_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/quotas_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3782 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zone_exports_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4084 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/blacklists_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6590 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/recordset_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/tsigkey_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/tld_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zone_imports_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1891 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2842 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/servers_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3371 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/records_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/domains_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3617 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/quotas_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4389 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/records_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/domains_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/servers_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5332 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6464 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7706 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_tld.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/recordset_wildcard_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9169 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_tsigkey.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/recordset_data_invalid.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11998 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_transfer_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/invalid_txt_dataset.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_unauthed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/invalid_mx_dataset.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/recordset_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/valid_txt_dataset.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/invalid_sshfp_dataset.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7732 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3538 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_transfer_accepts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones_exports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18344 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_recordset.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6379 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_recordset_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3828 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/unauthed_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7793 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_blacklists.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones_imports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7986 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3520 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_domains.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5129 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_records.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/admin/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/admin/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3770 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_recordsets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4861 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2686 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_transfer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2612 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_export.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7061 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8080 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/data_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8689 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/waiters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2585 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/releasenotes/notes/drop-py-2-7-a36c3b1d4d875e21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2020-04-24 12:41:27.000000 designate-tempest-plugin-0.8.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5266 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-04-24 12:42:24.000000 designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/not-zip-safe
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9999 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7674 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10534 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/json/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/json/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3371 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/records_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2842 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/servers_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/domains_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3617 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/quotas_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/query/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2813 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/query/query_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/query/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/quotas_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4992 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zones_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3258 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zone_imports_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/transfer_accepts_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/tld_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5334 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/transfer_request_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3782 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zone_exports_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4294 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/pool_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4084 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/blacklists_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6590 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/recordset_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/tsigkey_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1891 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2585 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8689 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/waiters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3840 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5332 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4861 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3770 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_recordsets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2686 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_transfer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2612 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_export.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5129 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_records.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3520 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_domains.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/admin/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/admin/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/valid_txt_dataset.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones_imports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7732 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3828 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/unauthed_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7706 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_tld.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18344 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_recordset.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/invalid_txt_dataset.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3538 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_transfer_accepts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_unauthed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7793 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_blacklists.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones_exports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7986 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9169 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_tsigkey.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/invalid_sshfp_dataset.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/recordset_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/invalid_mx_dataset.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6464 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6379 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_recordset_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11998 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_transfer_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/recordset_wildcard_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/recordset_data_invalid.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3514 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7061 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8080 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/data_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/servers_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/domains_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4389 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/records_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4449 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/tools/pretty_flake8.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      132 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/tools/pretty_flake8.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5178 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5313 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-02 12:24:27.000000 designate-tempest-plugin-0.9.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2020-10-02 12:23:19.000000 designate-tempest-plugin-0.9.0/releasenotes/notes/drop-py-2-7-a36c3b1d4d875e21.yaml
```

### Comparing `designate-tempest-plugin-0.8.0/doc/source/index.rst` & `designate-tempest-plugin-0.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/doc/source/conf.py` & `designate-tempest-plugin-0.9.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,34 +23,21 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = []
-
-import openstackdocstheme
+extensions = ['openstackdocstheme']
 
 html_theme = 'openstackdocs'
-html_theme_path = [openstackdocstheme.get_html_theme_path()]
 
-# We ask git for the SHA checksum
-# The git SHA checksum is used by "log-a-bug"
-git_cmd = ["/usr/bin/git", "rev-parse", "HEAD"]
-gitsha = str(subprocess.Popen(
-    git_cmd, stdout=subprocess.PIPE).communicate())[0].strip('\n')
-# tag that reported bugs will be tagged with
-bug_tag = "tempest-plugin-docs"
-# source tree
-pwd = os.getcwd()
-# html_context allows us to pass arbitrary values into the html template
-html_context = {"pwd": pwd, "gitsha": gitsha}
-# Must set this variable to include year, month, day, hours, and minutes.
-html_last_updated_fmt = '%Y-%m-%d %H:%M'
+# openstackdocstheme options
+openstackdocs_repo_name = 'openstack/designate-tempest-plugin'
+openstackdocs_bug_tag = "tempest-plugin-docs"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
@@ -93,15 +80,15 @@
 #add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 #show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = 'native'
 
 # A list of ignored prefixes for module index sorting.
 modindex_common_prefix = ["designate_tempest_plugin."]
 
 
 # -- Options for HTML output ---------------------------------------------------
```

### Comparing `designate-tempest-plugin-0.8.0/LICENSE` & `designate-tempest-plugin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/README.rst` & `designate-tempest-plugin-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/ChangeLog` & `designate-tempest-plugin-0.9.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Stop to use the \_\_future\_\_ module
+* Switch to newer openstackdocstheme version
+* Add py38 package metadata
+* Update hacking for Python3
+
 0.8.0
 -----
 
 * Cleanup py27 support
 * Limit where dnspython3 is installed
 * [ussuri][goal] Drop python 2.7 support and testing
```

### Comparing `designate-tempest-plugin-0.8.0/setup.cfg` & `designate-tempest-plugin-0.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 	Topic :: Internet :: Name Service (DNS)
 
 [files]
 packages = 
 	designate_tempest_plugin
 
 [entry_points]
```

### Comparing `designate-tempest-plugin-0.8.0/tools/pretty_flake8.py` & `designate-tempest-plugin-0.9.0/tools/pretty_flake8.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
-from __future__ import print_function
 
 import re
 import sys
 import linecache
 
 from prettytable import PrettyTable
```

### Comparing `designate-tempest-plugin-0.8.0/PKG-INFO` & `designate-tempest-plugin-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: designate-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: OpenStack DNS As A Service (Designate) Functional Tests
 Home-page: https://docs.openstack.org/designate-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -54,9 +54,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: Name Service (DNS)
 Requires-Python: >=3.6
```

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/query/query_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/query/query_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/json/base.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/json/base.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zones_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zones_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/transfer_accepts_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/transfer_accepts_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/pool_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/pool_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/transfer_request_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/transfer_request_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/base.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/base.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/quotas_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/quotas_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zone_exports_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zone_exports_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/blacklists_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/blacklists_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/recordset_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/recordset_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/tsigkey_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/tsigkey_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/tld_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/tld_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/json/zone_imports_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/json/zone_imports_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v2/__init__.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/__init__.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/servers_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/servers_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/base.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/base.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/records_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/records_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/json/domains_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/json/domains_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/v1/__init__.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/base.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/base.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/json/quotas_client.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/json/quotas_client.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/services/dns/admin/__init__.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/services/dns/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/records_schema.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/records_schema.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/domains_schema.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/domains_schema.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/schemas/v1/servers_schema.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/schemas/v1/servers_schema.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/config.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/base.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/base.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_quotas.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_tld.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_tld.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/recordset_wildcard_data.json` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/recordset_wildcard_data.json`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_tsigkey.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_tsigkey.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_transfer_request.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_transfer_request.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_unauthed.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_unauthed.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/recordset_data.json` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/recordset_data.json`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_transfer_accepts.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_transfer_accepts.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones_exports.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones_exports.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_recordset.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_recordset.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_recordset_validation.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_recordset_validation.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/unauthed_data.json` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/unauthed_data.json`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_blacklists.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_zones_imports.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_zones_imports.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v2/test_pool.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v2/test_pool.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_servers.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_servers.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_domains.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_domains.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/v1/test_records.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/v1/test_records.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/api/admin/test_quotas.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/api/admin/test_quotas.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_import.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_import.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_recordsets.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_recordsets.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_transfer.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_transfer.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/tests/scenario/v2/test_zones_export.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/tests/scenario/v2/test_zones_export.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/plugin.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/clients.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/clients.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/data_utils.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/data_utils.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/waiters.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/waiters.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin/common/models.py` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin/common/models.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/setup.py` & `designate-tempest-plugin-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `designate-tempest-plugin-0.8.0/AUTHORS` & `designate-tempest-plugin-0.9.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Emilien Macchi <emilien@redhat.com>
 Eric Larson <eric@ionrock.org>
 Erik Olof Gunnar Andersson <eandersson@blizzard.com>
 Flavio Percoco <flaper87@gmail.com>
 Ghanshyam <gmann@ghanshyammann.com>
 Graham Hayes <gr@ham.ie>
 Graham Hayes <graham.hayes@hpe.com>
+Hervé Beraud <hberaud@redhat.com>
 James E. Blair <jeblair@redhat.com>
 Jens Harbott <j.harbott@x-ion.de>
 Jordan Pittier <jordan.pittier@scality.com>
 Kiall Mac Innes <kiall@hpe.com>
 Kiall Mac Innes <kiall@macinnes.ie>
 LeopardMa <mabao@inspur.com>
 Maksym Shalamov <mshalamov@mirantis.com>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `designate-tempest-plugin-0.8.0/tox.ini` & `designate-tempest-plugin-0.9.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -75,15 +75,25 @@
 # H306 imports not in alphabetical order
 # H402 one line docstring needs punctuation
 # H404 multi line docstring should start with a summary
 # H405 multi line docstring summary not separated with an empty line
 # H904 Wrap long lines in parentheses instead of a backslash
 # E126 continuation line over-indented for hanging indent
 # E128 continuation line under-indented for visual indent
-
-ignore = H302,H306,H402,H404,H405,H904,E126,E128
+# W504 line break after binary operator
+ignore = H302,H306,H402,H404,H405,H904,E126,E128,W504
 exclude = .venv,.git,.tox,dist,doc,*openstack/common*,*openstack/deprecated*,*lib/python*,*egg,build,tools,.ropeproject
 
-
-[hacking]
-local-check-factory = designate_tempest_plugin.hacking.checks.factory
-
+[flake8:local-plugins]
+extension =
+  T102 = tempest.hacking.checks:import_no_clients_in_api_and_scenario_tests
+  T104 = tempest.hacking.checks:scenario_tests_need_service_tags
+  T105 = tempest.hacking.checks:no_setup_teardown_class_for_tests
+  T107 = tempest.hacking.checks:service_tags_not_in_module_path
+  T108 = tempest.hacking.checks:no_hyphen_at_end_of_rand_name
+  N322 = tempest.hacking.checks:no_mutable_default_args
+  T109 = tempest.hacking.checks:no_testtools_skip_decorator
+  T110 = tempest.hacking.checks:get_resources_on_service_clients
+  T111 = tempest.hacking.checks:delete_resources_on_service_clients
+  T112 = tempest.hacking.checks:dont_import_local_tempest_into_lib
+  T113 = tempest.hacking.checks:dont_use_config_in_tempest_lib
+  T114 = tempest.hacking.checks:use_rand_uuid_instead_of_uuid4
```

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/SOURCES.txt` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 designate_tempest_plugin.egg-info/not-zip-safe
 designate_tempest_plugin.egg-info/pbr.json
 designate_tempest_plugin.egg-info/requires.txt
 designate_tempest_plugin.egg-info/top_level.txt
 designate_tempest_plugin/common/__init__.py
 designate_tempest_plugin/common/models.py
 designate_tempest_plugin/common/waiters.py
-designate_tempest_plugin/hacking/__init__.py
-designate_tempest_plugin/hacking/checks.py
 designate_tempest_plugin/schemas/__init__.py
 designate_tempest_plugin/schemas/v1/__init__.py
 designate_tempest_plugin/schemas/v1/domains_schema.py
 designate_tempest_plugin/schemas/v1/records_schema.py
 designate_tempest_plugin/schemas/v1/servers_schema.py
 designate_tempest_plugin/services/__init__.py
 designate_tempest_plugin/services/dns/__init__.py
```

### Comparing `designate-tempest-plugin-0.8.0/designate_tempest_plugin.egg-info/PKG-INFO` & `designate-tempest-plugin-0.9.0/designate_tempest_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: designate-tempest-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: OpenStack DNS As A Service (Designate) Functional Tests
 Home-page: https://docs.openstack.org/designate-tempest-plugin/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -54,9 +54,10 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: Name Service (DNS)
 Requires-Python: >=3.6
```

