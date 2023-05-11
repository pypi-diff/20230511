# Comparing `tmp/mypy-boto3-route53resolver-1.26.133.tar.gz` & `tmp/mypy-boto3-route53resolver-1.26.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53resolver-1.26.133.tar", last modified: Thu May 11 19:32:36 2023, max compression
+gzip compressed data, was "mypy-boto3-route53resolver-1.26.87.tar", last modified: Wed Mar  8 20:35:46 2023, max compression
```

## Comparing `mypy-boto3-route53resolver-1.26.133.tar` & `mypy-boto3-route53resolver-1.26.87.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:36.501508 mypy-boto3-route53resolver-1.26.133/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-05-11 19:32:36.501508 mypy-boto3-route53resolver-1.26.133/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23103 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:36.501508 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55189 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-11 19:32:22.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57065 2023-05-11 19:32:23.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57024 2023-05-11 19:32:22.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 19:32:21.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:32:36.501508 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 19:32:36.000000 mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 19:32:36.501508 mypy-boto3-route53resolver-1.26.133/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-11 19:32:20.000000 mypy-boto3-route53resolver-1.26.133/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.194592 mypy-boto3-route53resolver-1.26.87/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-03-08 20:35:46.194592 mypy-boto3-route53resolver-1.26.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.178592 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-03-08 20:35:13.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55189 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-03-08 20:35:13.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13647 2023-03-08 20:35:13.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19616 2023-03-08 20:35:13.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-03-08 20:35:13.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56913 2023-03-08 20:35:14.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56872 2023-03-08 20:35:14.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 20:35:46.194592 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-08 20:35:46.000000 mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 20:35:46.194592 mypy-boto3-route53resolver-1.26.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-08 20:35:12.000000 mypy-boto3-route53resolver-1.26.87/setup.py
```

### Comparing `mypy-boto3-route53resolver-1.26.133/LICENSE` & `mypy-boto3-route53resolver-1.26.87/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-route53resolver-1.26.133/PKG-INFO` & `mypy-boto3-route53resolver-1.26.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.26.133
-Summary: Type annotations for boto3.Route53Resolver 1.26.133 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.87
+Summary: Type annotations for boto3.Route53Resolver 1.26.87 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,14 +422,15 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
@@ -452,78 +453,68 @@
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -552,38 +543,47 @@
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
     ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
@@ -597,42 +597,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-route53resolver-1.26.133/README.md` & `mypy-boto3-route53resolver-1.26.87/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -390,14 +390,15 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
@@ -420,78 +421,68 @@
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -520,38 +511,47 @@
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
     ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
@@ -565,42 +565,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__init__.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__init__.pyi` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/__main__.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Resolver 1.26.133\nVersion:         1.26.133\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.Route53Resolver 1.26.87\nVersion:         1.26.87\nBuilder"
+        " version: 7.12.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.133")
+    print("1.26.87")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/client.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/client.pyi` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/literals.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
@@ -64,15 +63,14 @@
     "Route53ResolverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionType = Literal["ALERT", "ALLOW", "BLOCK"]
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
@@ -312,15 +310,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -382,15 +379,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -477,15 +473,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -527,25 +522,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/literals.pyi` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActionType",
     "AutodefinedReverseFlagType",
     "BlockOverrideDnsTypeType",
     "BlockResponseType",
     "FirewallDomainImportOperationType",
     "FirewallDomainListStatusType",
@@ -63,14 +64,15 @@
     "Route53ResolverServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActionType = Literal["ALERT", "ALLOW", "BLOCK"]
 AutodefinedReverseFlagType = Literal["DISABLE", "ENABLE", "USE_LOCAL_RESOURCE_SETTING"]
 BlockOverrideDnsTypeType = Literal["CNAME"]
 BlockResponseType = Literal["NODATA", "NXDOMAIN", "OVERRIDE"]
 FirewallDomainImportOperationType = Literal["REPLACE"]
 FirewallDomainListStatusType = Literal[
     "COMPLETE", "COMPLETE_IMPORT_FAILED", "DELETING", "IMPORTING", "UPDATING"
@@ -310,15 +312,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -380,15 +381,14 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
@@ -475,15 +475,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -525,25 +524,21 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/paginator.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,45 +104,45 @@
 class ListFirewallConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
         """
 
 
 class ListFirewallDomainListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
         """
 
 
 class ListFirewallDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
     """
 
     def paginate(
-        self, *, FirewallDomainListId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FirewallDomainListId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
         """
 
 
@@ -155,30 +155,30 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 
 class ListFirewallRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
         """
 
 
@@ -190,30 +190,30 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 
 class ListResolverConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
         """
 
 
@@ -223,30 +223,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 
 class ListResolverEndpointIpAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
     """
 
     def paginate(
-        self, *, ResolverEndpointId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResolverEndpointId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointIpAddressesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
         """
 
 
@@ -256,15 +256,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 
@@ -276,15 +276,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 
@@ -296,15 +296,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 
@@ -314,15 +314,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 
@@ -332,28 +332,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/paginator.pyi` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -101,43 +101,43 @@
 class ListFirewallConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallconfigspaginator)
         """
 
 class ListFirewallDomainListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainlistspaginator)
         """
 
 class ListFirewallDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
     """
 
     def paginate(
-        self, *, FirewallDomainListId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FirewallDomainListId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewalldomainspaginator)
         """
 
 class ListFirewallRuleGroupAssociationsPaginator(Paginator):
@@ -149,29 +149,29 @@
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str = ...,
         VpcId: str = ...,
         Priority: int = ...,
         Status: FirewallRuleGroupAssociationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupassociationspaginator)
         """
 
 class ListFirewallRuleGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRuleGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulegroupspaginator)
         """
 
 class ListFirewallRulesPaginator(Paginator):
@@ -182,29 +182,29 @@
 
     def paginate(
         self,
         *,
         FirewallRuleGroupId: str,
         Priority: int = ...,
         Action: ActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFirewallRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listfirewallrulespaginator)
         """
 
 class ListResolverConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverconfigspaginator)
         """
 
 class ListResolverDnssecConfigsPaginator(Paginator):
@@ -213,29 +213,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverDnssecConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverdnssecconfigspaginator)
         """
 
 class ListResolverEndpointIpAddressesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
     """
 
     def paginate(
-        self, *, ResolverEndpointId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResolverEndpointId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointIpAddressesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointipaddressespaginator)
         """
 
 class ListResolverEndpointsPaginator(Paginator):
@@ -244,15 +244,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverendpointspaginator)
         """
 
 class ListResolverQueryLogConfigAssociationsPaginator(Paginator):
@@ -263,15 +263,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigassociationspaginator)
         """
 
 class ListResolverQueryLogConfigsPaginator(Paginator):
@@ -282,15 +282,15 @@
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverQueryLogConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverquerylogconfigspaginator)
         """
 
 class ListResolverRuleAssociationsPaginator(Paginator):
@@ -299,15 +299,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRuleAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverruleassociationspaginator)
         """
 
 class ListResolverRulesPaginator(Paginator):
@@ -316,27 +316,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResolverRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listresolverrulespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/type_defs.py` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "FirewallRuleGroupAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "IpAddressUpdateTypeDef",
     "ResolverEndpointTypeDef",
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
@@ -80,78 +80,68 @@
     "FirewallConfigTypeDef",
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     "GetResolverRuleAssociationRequestRequestTypeDef",
     "GetResolverRulePolicyRequestRequestTypeDef",
-    "GetResolverRulePolicyResponseTypeDef",
     "GetResolverRuleRequestRequestTypeDef",
     "ImportFirewallDomainsRequestRequestTypeDef",
-    "ImportFirewallDomainsResponseTypeDef",
     "IpAddressResponseTypeDef",
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
-    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
-    "ListFirewallDomainsResponseTypeDef",
-    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
-    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
-    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
-    "PutResolverRulePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
-    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    "GetResolverRulePolicyResponseTypeDef",
+    "ImportFirewallDomainsResponseTypeDef",
+    "ListFirewallDomainsResponseTypeDef",
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    "PutResolverRulePolicyResponseTypeDef",
+    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     "DisassociateResolverEndpointIpAddressRequestRequestTypeDef",
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     "CreateResolverEndpointResponseTypeDef",
     "DeleteResolverEndpointResponseTypeDef",
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
@@ -180,38 +170,47 @@
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
     "ResolverRuleTypeDef",
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestRequestTypeDef",
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverEndpointsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestRequestTypeDef",
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
     "ListResolverRulesRequestRequestTypeDef",
     "GetFirewallConfigResponseTypeDef",
     "ListFirewallConfigsResponseTypeDef",
     "UpdateFirewallConfigResponseTypeDef",
     "ListFirewallDomainListsResponseTypeDef",
     "ListFirewallRuleGroupsResponseTypeDef",
     "GetResolverConfigResponseTypeDef",
     "ListResolverConfigsResponseTypeDef",
     "UpdateResolverConfigResponseTypeDef",
     "GetResolverDnssecConfigResponseTypeDef",
     "ListResolverDnssecConfigsResponseTypeDef",
     "UpdateResolverDnssecConfigResponseTypeDef",
     "ListResolverEndpointIpAddressesResponseTypeDef",
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "UpdateResolverEndpointRequestRequestTypeDef",
     "UpdateResolverRuleRequestRequestTypeDef",
     "CreateResolverRuleResponseTypeDef",
     "DeleteResolverRuleResponseTypeDef",
     "GetResolverRuleResponseTypeDef",
     "ListResolverRulesResponseTypeDef",
     "UpdateResolverRuleResponseTypeDef",
@@ -241,14 +240,25 @@
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
@@ -309,22 +319,20 @@
     "_OptionalAssociateResolverRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class AssociateResolverRuleRequestRequestTypeDef(
     _RequiredAssociateResolverRuleRequestRequestTypeDef,
     _OptionalAssociateResolverRuleRequestRequestTypeDef,
 ):
     pass
 
-
 ResolverRuleAssociationTypeDef = TypedDict(
     "ResolverRuleAssociationTypeDef",
     {
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
@@ -387,22 +395,20 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
     },
     total=False,
 )
 
-
 class CreateFirewallRuleRequestRequestTypeDef(
     _RequiredCreateFirewallRuleRequestRequestTypeDef,
     _OptionalCreateFirewallRuleRequestRequestTypeDef,
 ):
     pass
 
-
 FirewallRuleTypeDef = TypedDict(
     "FirewallRuleTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
         "Name": str,
         "Priority": int,
@@ -429,19 +435,17 @@
     {
         "Ip": str,
         "Ipv6": str,
     },
     total=False,
 )
 
-
 class IpAddressRequestTypeDef(_RequiredIpAddressRequestTypeDef, _OptionalIpAddressRequestTypeDef):
     pass
 
-
 ResolverQueryLogConfigTypeDef = TypedDict(
     "ResolverQueryLogConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "Status": ResolverQueryLogConfigStatusType,
         "ShareStatus": ShareStatusType,
@@ -600,22 +604,14 @@
 GetFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "FirewallRuleGroupPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 
@@ -672,22 +668,14 @@
 GetResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ResolverQueryLogConfigPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
     },
 )
 
@@ -701,22 +689,14 @@
 GetResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "GetResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverRulePolicyResponseTypeDef = TypedDict(
-    "GetResolverRulePolicyResponseTypeDef",
-    {
-        "ResolverRulePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRuleRequestRequestTypeDef = TypedDict(
     "GetResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
     },
 )
 
@@ -725,25 +705,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": Literal["REPLACE"],
         "DomainFileUrl": str,
     },
 )
 
-ImportFirewallDomainsResponseTypeDef = TypedDict(
-    "ImportFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IpAddressResponseTypeDef = TypedDict(
     "IpAddressResponseTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
@@ -751,70 +720,42 @@
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
-ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListFirewallConfigsRequestRequestTypeDef = TypedDict(
     "ListFirewallConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallDomainListsRequestRequestTypeDef = TypedDict(
     "ListFirewallDomainListsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "FirewallDomainListId": str,
-    },
-)
-_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
-    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFirewallDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallDomainsRequestRequestTypeDef",
     {
         "FirewallDomainListId": str,
     },
 )
 _OptionalListFirewallDomainsRequestRequestTypeDef = TypedDict(
@@ -822,99 +763,42 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFirewallDomainsRequestRequestTypeDef(
     _RequiredListFirewallDomainsRequestRequestTypeDef,
     _OptionalListFirewallDomainsRequestRequestTypeDef,
 ):
     pass
 
-
-ListFirewallDomainsResponseTypeDef = TypedDict(
-    "ListFirewallDomainsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Domains": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
-        {
-            "FirewallRuleGroupId": str,
-            "VpcId": str,
-            "Priority": int,
-            "Status": FirewallRuleGroupAssociationStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListFirewallRuleGroupAssociationsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "VpcId": str,
         "Priority": int,
         "Status": FirewallRuleGroupAssociationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "FirewallRuleGroupId": str,
-    },
-)
-_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "Priority": int,
-        "Action": ActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
-    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFirewallRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallRulesRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 _OptionalListFirewallRulesRequestRequestTypeDef = TypedDict(
@@ -924,60 +808,28 @@
         "Action": ActionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
-
-ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "ResolverEndpointId": str,
-    },
-)
-_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
-    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
     "_RequiredListResolverEndpointIpAddressesRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
@@ -985,44 +837,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResolverEndpointIpAddressesRequestRequestTypeDef(
     _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef,
     _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1030,91 +858,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PutFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "FirewallRuleGroupPolicy": str,
     },
 )
 
-PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverQueryLogConfigPolicy": str,
     },
 )
 
-PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "PutResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverRulePolicy": str,
     },
 )
 
-PutResolverRulePolicyResponseTypeDef = TypedDict(
-    "PutResolverRulePolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1132,25 +913,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": FirewallDomainUpdateOperationType,
         "Domains": Sequence[str],
     },
 )
 
-UpdateFirewallDomainsResponseTypeDef = TypedDict(
-    "UpdateFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     {
         "FirewallRuleGroupAssociationId": str,
     },
 )
 _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
@@ -1159,22 +929,20 @@
         "Priority": int,
         "MutationProtection": MutationProtectionStatusType,
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateFirewallRuleGroupAssociationRequestRequestTypeDef(
     _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
@@ -1188,22 +956,20 @@
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateFirewallRuleRequestRequestTypeDef(
     _RequiredUpdateFirewallRuleRequestRequestTypeDef,
     _OptionalUpdateFirewallRuleRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateIpAddressTypeDef = TypedDict(
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
@@ -1239,22 +1005,20 @@
     {
         "MutationProtection": MutationProtectionStatusType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class AssociateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredAssociateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalAssociateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFirewallDomainListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallDomainListRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "Name": str,
     },
 )
@@ -1262,22 +1026,20 @@
     "_OptionalCreateFirewallDomainListRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFirewallDomainListRequestRequestTypeDef(
     _RequiredCreateFirewallDomainListRequestRequestTypeDef,
     _OptionalCreateFirewallDomainListRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleGroupRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "Name": str,
     },
 )
@@ -1285,22 +1047,20 @@
     "_OptionalCreateFirewallRuleGroupRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1309,77 +1069,154 @@
     "_OptionalCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateResolverQueryLogConfigRequestRequestTypeDef(
     _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef,
     _OptionalCreateResolverQueryLogConfigRequestRequestTypeDef,
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "AssociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "DisassociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "FirewallRuleGroupPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ResolverQueryLogConfigPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverRulePolicyResponseTypeDef = TypedDict(
+    "GetResolverRulePolicyResponseTypeDef",
+    {
+        "ResolverRulePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportFirewallDomainsResponseTypeDef = TypedDict(
+    "ImportFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallDomainsResponseTypeDef = TypedDict(
+    "ListFirewallDomainsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Domains": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverRulePolicyResponseTypeDef = TypedDict(
+    "PutResolverRulePolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDomainsResponseTypeDef = TypedDict(
+    "UpdateFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverEndpointIpAddressRequestRequestTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1395,215 +1232,215 @@
     },
 )
 
 AssociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverEndpointResponseTypeDef = TypedDict(
     "CreateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverEndpointResponseTypeDef = TypedDict(
     "DeleteResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverEndpointResponseTypeDef = TypedDict(
     "GetResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DisassociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigAssociationResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigAssociationResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverRuleResponseTypeDef = TypedDict(
     "DisassociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleAssociationResponseTypeDef = TypedDict(
     "GetResolverRuleAssociationResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallDomainListResponseTypeDef = TypedDict(
     "DeleteFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallDomainListResponseTypeDef = TypedDict(
     "GetFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleGroupResponseTypeDef = TypedDict(
     "CreateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleGroupResponseTypeDef = TypedDict(
     "DeleteFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleResponseTypeDef = TypedDict(
     "CreateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleResponseTypeDef = TypedDict(
     "DeleteFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1618,54 +1455,52 @@
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
     },
     total=False,
 )
 
-
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
     _OptionalCreateResolverEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 CreateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "CreateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DeleteResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1680,22 +1515,20 @@
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateResolverRuleRequestRequestTypeDef(
     _RequiredCreateResolverRuleRequestRequestTypeDef,
     _OptionalCreateResolverRuleRequestRequestTypeDef,
 ):
     pass
 
-
 ResolverRuleConfigTypeDef = TypedDict(
     "ResolverRuleConfigTypeDef",
     {
         "Name": str,
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
     },
@@ -1719,239 +1552,367 @@
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
-ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverDnssecConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverDnssecConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverEndpointsRequestRequestTypeDef = TypedDict(
     "ListResolverEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRuleAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverRuleAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRulesRequestRequestTypeDef = TypedDict(
     "ListResolverRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFirewallConfigResponseTypeDef = TypedDict(
     "GetFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverDnssecConfigResponseTypeDef = TypedDict(
     "GetResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "FirewallDomainListId": str,
+    },
+)
+_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
+    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+):
+    pass
+
+ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+        {
+            "FirewallRuleGroupId": str,
+            "VpcId": str,
+            "Priority": int,
+            "Status": FirewallRuleGroupAssociationStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "FirewallRuleGroupId": str,
+    },
+)
+_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "Priority": int,
+        "Action": ActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
+    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+):
+    pass
+
+ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "ResolverEndpointId": str,
+    },
+)
+_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
+    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+):
+    pass
+
+ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
@@ -1960,64 +1921,62 @@
         "Name": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
         "UpdateIpAddresses": Sequence[UpdateIpAddressTypeDef],
     },
     total=False,
 )
 
-
 class UpdateResolverEndpointRequestRequestTypeDef(
     _RequiredUpdateResolverEndpointRequestRequestTypeDef,
     _OptionalUpdateResolverEndpointRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateResolverRuleRequestRequestTypeDef = TypedDict(
     "UpdateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "Config": ResolverRuleConfigTypeDef,
     },
 )
 
 CreateResolverRuleResponseTypeDef = TypedDict(
     "CreateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverRuleResponseTypeDef = TypedDict(
     "DeleteResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleResponseTypeDef = TypedDict(
     "GetResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver/type_defs.pyi` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "FirewallRuleGroupAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "IpAddressUpdateTypeDef",
     "ResolverEndpointTypeDef",
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     "ResolverQueryLogConfigAssociationTypeDef",
     "AssociateResolverRuleRequestRequestTypeDef",
     "ResolverRuleAssociationTypeDef",
     "FirewallDomainListTypeDef",
@@ -79,78 +81,68 @@
     "FirewallConfigTypeDef",
     "FirewallDomainListMetadataTypeDef",
     "FirewallRuleGroupMetadataTypeDef",
     "GetFirewallConfigRequestRequestTypeDef",
     "GetFirewallDomainListRequestRequestTypeDef",
     "GetFirewallRuleGroupAssociationRequestRequestTypeDef",
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
     "GetFirewallRuleGroupRequestRequestTypeDef",
     "GetResolverConfigRequestRequestTypeDef",
     "ResolverConfigTypeDef",
     "GetResolverDnssecConfigRequestRequestTypeDef",
     "ResolverDnssecConfigTypeDef",
     "GetResolverEndpointRequestRequestTypeDef",
     "GetResolverQueryLogConfigAssociationRequestRequestTypeDef",
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     "GetResolverRuleAssociationRequestRequestTypeDef",
     "GetResolverRulePolicyRequestRequestTypeDef",
-    "GetResolverRulePolicyResponseTypeDef",
     "GetResolverRuleRequestRequestTypeDef",
     "ImportFirewallDomainsRequestRequestTypeDef",
-    "ImportFirewallDomainsResponseTypeDef",
     "IpAddressResponseTypeDef",
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListFirewallConfigsRequestRequestTypeDef",
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
     "ListFirewallDomainListsRequestRequestTypeDef",
-    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
     "ListFirewallDomainsRequestRequestTypeDef",
-    "ListFirewallDomainsResponseTypeDef",
-    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
     "ListFirewallRuleGroupsRequestRequestTypeDef",
-    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
     "ListFirewallRulesRequestRequestTypeDef",
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
     "ListResolverConfigsRequestRequestTypeDef",
-    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
     "ListResolverEndpointIpAddressesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
     "PutResolverRulePolicyRequestRequestTypeDef",
-    "PutResolverRulePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFirewallConfigRequestRequestTypeDef",
     "UpdateFirewallDomainsRequestRequestTypeDef",
-    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     "UpdateFirewallRuleRequestRequestTypeDef",
     "UpdateIpAddressTypeDef",
     "UpdateResolverConfigRequestRequestTypeDef",
     "UpdateResolverDnssecConfigRequestRequestTypeDef",
     "AssociateFirewallRuleGroupRequestRequestTypeDef",
     "CreateFirewallDomainListRequestRequestTypeDef",
     "CreateFirewallRuleGroupRequestRequestTypeDef",
     "CreateResolverQueryLogConfigRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateFirewallRuleGroupResponseTypeDef",
     "DisassociateFirewallRuleGroupResponseTypeDef",
     "GetFirewallRuleGroupAssociationResponseTypeDef",
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    "GetResolverRulePolicyResponseTypeDef",
+    "ImportFirewallDomainsResponseTypeDef",
+    "ListFirewallDomainsResponseTypeDef",
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    "PutResolverRulePolicyResponseTypeDef",
+    "UpdateFirewallDomainsResponseTypeDef",
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     "DisassociateResolverEndpointIpAddressRequestRequestTypeDef",
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     "CreateResolverEndpointResponseTypeDef",
     "DeleteResolverEndpointResponseTypeDef",
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
@@ -179,38 +171,47 @@
     "CreateResolverQueryLogConfigResponseTypeDef",
     "DeleteResolverQueryLogConfigResponseTypeDef",
     "GetResolverQueryLogConfigResponseTypeDef",
     "ListResolverQueryLogConfigsResponseTypeDef",
     "CreateResolverRuleRequestRequestTypeDef",
     "ResolverRuleConfigTypeDef",
     "ResolverRuleTypeDef",
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
     "ListResolverDnssecConfigsRequestRequestTypeDef",
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
     "ListResolverEndpointsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
     "ListResolverRuleAssociationsRequestRequestTypeDef",
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
     "ListResolverRulesRequestRequestTypeDef",
     "GetFirewallConfigResponseTypeDef",
     "ListFirewallConfigsResponseTypeDef",
     "UpdateFirewallConfigResponseTypeDef",
     "ListFirewallDomainListsResponseTypeDef",
     "ListFirewallRuleGroupsResponseTypeDef",
     "GetResolverConfigResponseTypeDef",
     "ListResolverConfigsResponseTypeDef",
     "UpdateResolverConfigResponseTypeDef",
     "GetResolverDnssecConfigResponseTypeDef",
     "ListResolverDnssecConfigsResponseTypeDef",
     "UpdateResolverDnssecConfigResponseTypeDef",
     "ListResolverEndpointIpAddressesResponseTypeDef",
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    "ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    "ListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    "ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "UpdateResolverEndpointRequestRequestTypeDef",
     "UpdateResolverRuleRequestRequestTypeDef",
     "CreateResolverRuleResponseTypeDef",
     "DeleteResolverRuleResponseTypeDef",
     "GetResolverRuleResponseTypeDef",
     "ListResolverRulesResponseTypeDef",
     "UpdateResolverRuleResponseTypeDef",
@@ -240,14 +241,25 @@
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 IpAddressUpdateTypeDef = TypedDict(
     "IpAddressUpdateTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
@@ -308,20 +320,22 @@
     "_OptionalAssociateResolverRuleRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class AssociateResolverRuleRequestRequestTypeDef(
     _RequiredAssociateResolverRuleRequestRequestTypeDef,
     _OptionalAssociateResolverRuleRequestRequestTypeDef,
 ):
     pass
 
+
 ResolverRuleAssociationTypeDef = TypedDict(
     "ResolverRuleAssociationTypeDef",
     {
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
@@ -384,20 +398,22 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
     },
     total=False,
 )
 
+
 class CreateFirewallRuleRequestRequestTypeDef(
     _RequiredCreateFirewallRuleRequestRequestTypeDef,
     _OptionalCreateFirewallRuleRequestRequestTypeDef,
 ):
     pass
 
+
 FirewallRuleTypeDef = TypedDict(
     "FirewallRuleTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
         "Name": str,
         "Priority": int,
@@ -424,17 +440,19 @@
     {
         "Ip": str,
         "Ipv6": str,
     },
     total=False,
 )
 
+
 class IpAddressRequestTypeDef(_RequiredIpAddressRequestTypeDef, _OptionalIpAddressRequestTypeDef):
     pass
 
+
 ResolverQueryLogConfigTypeDef = TypedDict(
     "ResolverQueryLogConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "Status": ResolverQueryLogConfigStatusType,
         "ShareStatus": ShareStatusType,
@@ -593,22 +611,14 @@
 GetFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "GetFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "FirewallRuleGroupPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "GetFirewallRuleGroupRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 
@@ -665,22 +675,14 @@
 GetResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "GetResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ResolverQueryLogConfigPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "GetResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
     },
 )
 
@@ -694,22 +696,14 @@
 GetResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "GetResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-GetResolverRulePolicyResponseTypeDef = TypedDict(
-    "GetResolverRulePolicyResponseTypeDef",
-    {
-        "ResolverRulePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRuleRequestRequestTypeDef = TypedDict(
     "GetResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
     },
 )
 
@@ -718,25 +712,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": Literal["REPLACE"],
         "DomainFileUrl": str,
     },
 )
 
-ImportFirewallDomainsResponseTypeDef = TypedDict(
-    "ImportFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IpAddressResponseTypeDef = TypedDict(
     "IpAddressResponseTypeDef",
     {
         "IpId": str,
         "SubnetId": str,
         "Ip": str,
         "Ipv6": str,
@@ -744,68 +727,42 @@
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
-ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
-    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListFirewallConfigsRequestRequestTypeDef = TypedDict(
     "ListFirewallConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
-    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallDomainListsRequestRequestTypeDef = TypedDict(
     "ListFirewallDomainListsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "FirewallDomainListId": str,
-    },
-)
-_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
-    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFirewallDomainsRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallDomainsRequestRequestTypeDef",
     {
         "FirewallDomainListId": str,
     },
 )
 _OptionalListFirewallDomainsRequestRequestTypeDef = TypedDict(
@@ -813,95 +770,44 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFirewallDomainsRequestRequestTypeDef(
     _RequiredListFirewallDomainsRequestRequestTypeDef,
     _OptionalListFirewallDomainsRequestRequestTypeDef,
 ):
     pass
 
-ListFirewallDomainsResponseTypeDef = TypedDict(
-    "ListFirewallDomainsResponseTypeDef",
-    {
-        "NextToken": str,
-        "Domains": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
-        {
-            "FirewallRuleGroupId": str,
-            "VpcId": str,
-            "Priority": int,
-            "Status": FirewallRuleGroupAssociationStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
 
 ListFirewallRuleGroupAssociationsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "VpcId": str,
         "Priority": int,
         "Status": FirewallRuleGroupAssociationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
-    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFirewallRuleGroupsRequestRequestTypeDef = TypedDict(
     "ListFirewallRuleGroupsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "FirewallRuleGroupId": str,
-    },
-)
-_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
-    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
-    {
-        "Priority": int,
-        "Action": ActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
-    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFirewallRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListFirewallRulesRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
     },
 )
 _OptionalListFirewallRulesRequestRequestTypeDef = TypedDict(
@@ -911,56 +817,30 @@
         "Action": ActionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFirewallRulesRequestRequestTypeDef(
     _RequiredListFirewallRulesRequestRequestTypeDef, _OptionalListFirewallRulesRequestRequestTypeDef
 ):
     pass
 
-ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
-    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListResolverConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "ResolverEndpointId": str,
-    },
-)
-_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
-    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
-    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
     "_RequiredListResolverEndpointIpAddressesRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef = TypedDict(
@@ -968,39 +848,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResolverEndpointIpAddressesRequestRequestTypeDef(
     _RequiredListResolverEndpointIpAddressesRequestRequestTypeDef,
     _OptionalListResolverEndpointIpAddressesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
 
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
@@ -1009,89 +871,46 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 PutFirewallRuleGroupPolicyRequestRequestTypeDef = TypedDict(
     "PutFirewallRuleGroupPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "FirewallRuleGroupPolicy": str,
     },
 )
 
-PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
-    "PutFirewallRuleGroupPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverQueryLogConfigPolicyRequestRequestTypeDef = TypedDict(
     "PutResolverQueryLogConfigPolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverQueryLogConfigPolicy": str,
     },
 )
 
-PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
-    "PutResolverQueryLogConfigPolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResolverRulePolicyRequestRequestTypeDef = TypedDict(
     "PutResolverRulePolicyRequestRequestTypeDef",
     {
         "Arn": str,
         "ResolverRulePolicy": str,
     },
 )
 
-PutResolverRulePolicyResponseTypeDef = TypedDict(
-    "PutResolverRulePolicyResponseTypeDef",
-    {
-        "ReturnValue": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1109,25 +928,14 @@
     {
         "FirewallDomainListId": str,
         "Operation": FirewallDomainUpdateOperationType,
         "Domains": Sequence[str],
     },
 )
 
-UpdateFirewallDomainsResponseTypeDef = TypedDict(
-    "UpdateFirewallDomainsResponseTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Status": FirewallDomainListStatusType,
-        "StatusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef",
     {
         "FirewallRuleGroupAssociationId": str,
     },
 )
 _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef = TypedDict(
@@ -1136,20 +944,22 @@
         "Priority": int,
         "MutationProtection": MutationProtectionStatusType,
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateFirewallRuleGroupAssociationRequestRequestTypeDef(
     _RequiredUpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     _OptionalUpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFirewallRuleRequestRequestTypeDef",
     {
         "FirewallRuleGroupId": str,
         "FirewallDomainListId": str,
     },
 )
@@ -1163,20 +973,22 @@
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateFirewallRuleRequestRequestTypeDef(
     _RequiredUpdateFirewallRuleRequestRequestTypeDef,
     _OptionalUpdateFirewallRuleRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateIpAddressTypeDef = TypedDict(
     "UpdateIpAddressTypeDef",
     {
         "IpId": str,
         "Ipv6": str,
     },
 )
@@ -1212,20 +1024,22 @@
     {
         "MutationProtection": MutationProtectionStatusType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class AssociateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredAssociateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalAssociateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFirewallDomainListRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallDomainListRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "Name": str,
     },
 )
@@ -1233,20 +1047,22 @@
     "_OptionalCreateFirewallDomainListRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFirewallDomainListRequestRequestTypeDef(
     _RequiredCreateFirewallDomainListRequestRequestTypeDef,
     _OptionalCreateFirewallDomainListRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateFirewallRuleGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleGroupRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "Name": str,
     },
 )
@@ -1254,20 +1070,22 @@
     "_OptionalCreateFirewallRuleGroupRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFirewallRuleGroupRequestRequestTypeDef(
     _RequiredCreateFirewallRuleGroupRequestRequestTypeDef,
     _OptionalCreateFirewallRuleGroupRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
     },
@@ -1276,75 +1094,156 @@
     "_OptionalCreateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateResolverQueryLogConfigRequestRequestTypeDef(
     _RequiredCreateResolverQueryLogConfigRequestRequestTypeDef,
     _OptionalCreateResolverQueryLogConfigRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "AssociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFirewallRuleGroupResponseTypeDef = TypedDict(
     "DisassociateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "GetFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "FirewallRuleGroupPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "GetResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ResolverQueryLogConfigPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResolverRulePolicyResponseTypeDef = TypedDict(
+    "GetResolverRulePolicyResponseTypeDef",
+    {
+        "ResolverRulePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportFirewallDomainsResponseTypeDef = TypedDict(
+    "ImportFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallDomainsResponseTypeDef = TypedDict(
+    "ListFirewallDomainsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Domains": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupAssociationsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroupAssociations": List[FirewallRuleGroupAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFirewallRuleGroupPolicyResponseTypeDef = TypedDict(
+    "PutFirewallRuleGroupPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverQueryLogConfigPolicyResponseTypeDef = TypedDict(
+    "PutResolverQueryLogConfigPolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResolverRulePolicyResponseTypeDef = TypedDict(
+    "PutResolverRulePolicyResponseTypeDef",
+    {
+        "ReturnValue": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFirewallDomainsResponseTypeDef = TypedDict(
+    "UpdateFirewallDomainsResponseTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Status": FirewallDomainListStatusType,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleGroupAssociationResponseTypeDef = TypedDict(
     "UpdateFirewallRuleGroupAssociationResponseTypeDef",
     {
         "FirewallRuleGroupAssociation": FirewallRuleGroupAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverEndpointIpAddressRequestRequestTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
@@ -1360,215 +1259,215 @@
     },
 )
 
 AssociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "AssociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverEndpointResponseTypeDef = TypedDict(
     "CreateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverEndpointResponseTypeDef = TypedDict(
     "DeleteResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverEndpointIpAddressResponseTypeDef = TypedDict(
     "DisassociateResolverEndpointIpAddressResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverEndpointResponseTypeDef = TypedDict(
     "GetResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointsResponseTypeDef = TypedDict(
     "ListResolverEndpointsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverEndpoints": List[ResolverEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverEndpointResponseTypeDef = TypedDict(
     "UpdateResolverEndpointResponseTypeDef",
     {
         "ResolverEndpoint": ResolverEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DisassociateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigAssociationResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigAssociationResponseTypeDef",
     {
         "ResolverQueryLogConfigAssociation": ResolverQueryLogConfigAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigAssociationsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigAssociations": List[ResolverQueryLogConfigAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateResolverRuleResponseTypeDef = TypedDict(
     "AssociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateResolverRuleResponseTypeDef = TypedDict(
     "DisassociateResolverRuleResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleAssociationResponseTypeDef = TypedDict(
     "GetResolverRuleAssociationResponseTypeDef",
     {
         "ResolverRuleAssociation": ResolverRuleAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRuleAssociationsResponseTypeDef = TypedDict(
     "ListResolverRuleAssociationsResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRuleAssociations": List[ResolverRuleAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallDomainListResponseTypeDef = TypedDict(
     "CreateFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallDomainListResponseTypeDef = TypedDict(
     "DeleteFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallDomainListResponseTypeDef = TypedDict(
     "GetFirewallDomainListResponseTypeDef",
     {
         "FirewallDomainList": FirewallDomainListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleGroupResponseTypeDef = TypedDict(
     "CreateFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleGroupResponseTypeDef = TypedDict(
     "DeleteFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFirewallRuleGroupResponseTypeDef = TypedDict(
     "GetFirewallRuleGroupResponseTypeDef",
     {
         "FirewallRuleGroup": FirewallRuleGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFirewallRuleResponseTypeDef = TypedDict(
     "CreateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteFirewallRuleResponseTypeDef = TypedDict(
     "DeleteFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRulesResponseTypeDef = TypedDict(
     "ListFirewallRulesResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRules": List[FirewallRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallRuleResponseTypeDef = TypedDict(
     "UpdateFirewallRuleResponseTypeDef",
     {
         "FirewallRule": FirewallRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverEndpointRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1583,52 +1482,54 @@
         "Name": str,
         "Tags": Sequence[TagTypeDef],
         "ResolverEndpointType": ResolverEndpointTypeType,
     },
     total=False,
 )
 
+
 class CreateResolverEndpointRequestRequestTypeDef(
     _RequiredCreateResolverEndpointRequestRequestTypeDef,
     _OptionalCreateResolverEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 CreateResolverQueryLogConfigResponseTypeDef = TypedDict(
     "CreateResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverQueryLogConfigResponseTypeDef = TypedDict(
     "DeleteResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverQueryLogConfigResponseTypeDef = TypedDict(
     "GetResolverQueryLogConfigResponseTypeDef",
     {
         "ResolverQueryLogConfig": ResolverQueryLogConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverQueryLogConfigsResponseTypeDef = TypedDict(
     "ListResolverQueryLogConfigsResponseTypeDef",
     {
         "NextToken": str,
         "TotalCount": int,
         "TotalFilteredCount": int,
         "ResolverQueryLogConfigs": List[ResolverQueryLogConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResolverRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
@@ -1643,20 +1544,22 @@
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateResolverRuleRequestRequestTypeDef(
     _RequiredCreateResolverRuleRequestRequestTypeDef,
     _OptionalCreateResolverRuleRequestRequestTypeDef,
 ):
     pass
 
+
 ResolverRuleConfigTypeDef = TypedDict(
     "ResolverRuleConfigTypeDef",
     {
         "Name": str,
         "TargetIps": Sequence[TargetAddressTypeDef],
         "ResolverEndpointId": str,
     },
@@ -1680,239 +1583,375 @@
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
     total=False,
 )
 
-ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
-    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverDnssecConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverDnssecConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
-    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverEndpointsRequestRequestTypeDef = TypedDict(
     "ListResolverEndpointsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
-    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverQueryLogConfigsRequestRequestTypeDef = TypedDict(
     "ListResolverQueryLogConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
         "SortBy": str,
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
-    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRuleAssociationsRequestRequestTypeDef = TypedDict(
     "ListResolverRuleAssociationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
-    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResolverRulesRequestRequestTypeDef = TypedDict(
     "ListResolverRulesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFirewallConfigResponseTypeDef = TypedDict(
     "GetFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallConfigsResponseTypeDef = TypedDict(
     "ListFirewallConfigsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallConfigs": List[FirewallConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFirewallConfigResponseTypeDef = TypedDict(
     "UpdateFirewallConfigResponseTypeDef",
     {
         "FirewallConfig": FirewallConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallDomainListsResponseTypeDef = TypedDict(
     "ListFirewallDomainListsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallDomainLists": List[FirewallDomainListMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFirewallRuleGroupsResponseTypeDef = TypedDict(
     "ListFirewallRuleGroupsResponseTypeDef",
     {
         "NextToken": str,
         "FirewallRuleGroups": List[FirewallRuleGroupMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverConfigResponseTypeDef = TypedDict(
     "GetResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverConfigsResponseTypeDef = TypedDict(
     "ListResolverConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverConfigs": List[ResolverConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverConfigResponseTypeDef = TypedDict(
     "UpdateResolverConfigResponseTypeDef",
     {
         "ResolverConfig": ResolverConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverDnssecConfigResponseTypeDef = TypedDict(
     "GetResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverDnssecConfigsResponseTypeDef = TypedDict(
     "ListResolverDnssecConfigsResponseTypeDef",
     {
         "NextToken": str,
         "ResolverDnssecConfigs": List[ResolverDnssecConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverDnssecConfigResponseTypeDef = TypedDict(
     "UpdateResolverDnssecConfigResponseTypeDef",
     {
         "ResolverDNSSECConfig": ResolverDnssecConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverEndpointIpAddressesResponseTypeDef = TypedDict(
     "ListResolverEndpointIpAddressesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "IpAddresses": List[IpAddressResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef = TypedDict(
+    "ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef = TypedDict(
+    "ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "FirewallDomainListId": str,
+    },
+)
+_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef(
+    _RequiredListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    _OptionalListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+):
+    pass
+
+
+ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef",
+        {
+            "FirewallRuleGroupId": str,
+            "VpcId": str,
+            "Priority": int,
+            "Status": FirewallRuleGroupAssociationStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef = TypedDict(
+    "ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "FirewallRuleGroupId": str,
+    },
+)
+_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef = TypedDict(
+    "_OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef",
+    {
+        "Priority": int,
+        "Action": ActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFirewallRulesRequestListFirewallRulesPaginateTypeDef(
+    _RequiredListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    _OptionalListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+):
+    pass
+
+
+ListResolverConfigsRequestListResolverConfigsPaginateTypeDef = TypedDict(
+    "ListResolverConfigsRequestListResolverConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef = TypedDict(
+    "ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "ResolverEndpointId": str,
+    },
+)
+_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef = TypedDict(
+    "_OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef(
+    _RequiredListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    _OptionalListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+):
+    pass
+
+
+ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef = TypedDict(
+    "ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef = TypedDict(
+    "ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef = TypedDict(
+    "ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResolverRulesRequestListResolverRulesPaginateTypeDef = TypedDict(
+    "ListResolverRulesRequestListResolverRulesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
 )
 _OptionalUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
@@ -1921,62 +1960,64 @@
         "Name": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
         "UpdateIpAddresses": Sequence[UpdateIpAddressTypeDef],
     },
     total=False,
 )
 
+
 class UpdateResolverEndpointRequestRequestTypeDef(
     _RequiredUpdateResolverEndpointRequestRequestTypeDef,
     _OptionalUpdateResolverEndpointRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateResolverRuleRequestRequestTypeDef = TypedDict(
     "UpdateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "Config": ResolverRuleConfigTypeDef,
     },
 )
 
 CreateResolverRuleResponseTypeDef = TypedDict(
     "CreateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResolverRuleResponseTypeDef = TypedDict(
     "DeleteResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverRuleResponseTypeDef = TypedDict(
     "GetResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolverRulesResponseTypeDef = TypedDict(
     "ListResolverRulesResponseTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResolverRules": List[ResolverRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverRuleResponseTypeDef = TypedDict(
     "UpdateResolverRuleResponseTypeDef",
     {
         "ResolverRule": ResolverRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/PKG-INFO` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.26.133
-Summary: Type annotations for boto3.Route53Resolver 1.26.133 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.87
+Summary: Type annotations for boto3.Route53Resolver 1.26.87 service generated with mypy-boto3-builder 7.12.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.26.133](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.26.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -422,14 +422,15 @@
 `mypy_boto3_route53resolver.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_route53resolver.type_defs import (
     TagTypeDef,
     FirewallRuleGroupAssociationTypeDef,
+    ResponseMetadataTypeDef,
     IpAddressUpdateTypeDef,
     ResolverEndpointTypeDef,
     AssociateResolverQueryLogConfigRequestRequestTypeDef,
     ResolverQueryLogConfigAssociationTypeDef,
     AssociateResolverRuleRequestRequestTypeDef,
     ResolverRuleAssociationTypeDef,
     FirewallDomainListTypeDef,
@@ -452,78 +453,68 @@
     FirewallConfigTypeDef,
     FirewallDomainListMetadataTypeDef,
     FirewallRuleGroupMetadataTypeDef,
     GetFirewallConfigRequestRequestTypeDef,
     GetFirewallDomainListRequestRequestTypeDef,
     GetFirewallRuleGroupAssociationRequestRequestTypeDef,
     GetFirewallRuleGroupPolicyRequestRequestTypeDef,
-    GetFirewallRuleGroupPolicyResponseTypeDef,
     GetFirewallRuleGroupRequestRequestTypeDef,
     GetResolverConfigRequestRequestTypeDef,
     ResolverConfigTypeDef,
     GetResolverDnssecConfigRequestRequestTypeDef,
     ResolverDnssecConfigTypeDef,
     GetResolverEndpointRequestRequestTypeDef,
     GetResolverQueryLogConfigAssociationRequestRequestTypeDef,
     GetResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    GetResolverQueryLogConfigPolicyResponseTypeDef,
     GetResolverQueryLogConfigRequestRequestTypeDef,
     GetResolverRuleAssociationRequestRequestTypeDef,
     GetResolverRulePolicyRequestRequestTypeDef,
-    GetResolverRulePolicyResponseTypeDef,
     GetResolverRuleRequestRequestTypeDef,
     ImportFirewallDomainsRequestRequestTypeDef,
-    ImportFirewallDomainsResponseTypeDef,
     IpAddressResponseTypeDef,
-    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListFirewallConfigsRequestRequestTypeDef,
-    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
     ListFirewallDomainListsRequestRequestTypeDef,
-    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
     ListFirewallDomainsRequestRequestTypeDef,
-    ListFirewallDomainsResponseTypeDef,
-    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
     ListFirewallRuleGroupAssociationsRequestRequestTypeDef,
-    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
     ListFirewallRuleGroupsRequestRequestTypeDef,
-    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
     ListFirewallRulesRequestRequestTypeDef,
-    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
     ListResolverConfigsRequestRequestTypeDef,
-    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
     ListResolverEndpointIpAddressesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutFirewallRuleGroupPolicyRequestRequestTypeDef,
-    PutFirewallRuleGroupPolicyResponseTypeDef,
     PutResolverQueryLogConfigPolicyRequestRequestTypeDef,
-    PutResolverQueryLogConfigPolicyResponseTypeDef,
     PutResolverRulePolicyRequestRequestTypeDef,
-    PutResolverRulePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFirewallConfigRequestRequestTypeDef,
     UpdateFirewallDomainsRequestRequestTypeDef,
-    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationRequestRequestTypeDef,
     UpdateFirewallRuleRequestRequestTypeDef,
     UpdateIpAddressTypeDef,
     UpdateResolverConfigRequestRequestTypeDef,
     UpdateResolverDnssecConfigRequestRequestTypeDef,
     AssociateFirewallRuleGroupRequestRequestTypeDef,
     CreateFirewallDomainListRequestRequestTypeDef,
     CreateFirewallRuleGroupRequestRequestTypeDef,
     CreateResolverQueryLogConfigRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateFirewallRuleGroupResponseTypeDef,
     DisassociateFirewallRuleGroupResponseTypeDef,
     GetFirewallRuleGroupAssociationResponseTypeDef,
+    GetFirewallRuleGroupPolicyResponseTypeDef,
+    GetResolverQueryLogConfigPolicyResponseTypeDef,
+    GetResolverRulePolicyResponseTypeDef,
+    ImportFirewallDomainsResponseTypeDef,
+    ListFirewallDomainsResponseTypeDef,
     ListFirewallRuleGroupAssociationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutFirewallRuleGroupPolicyResponseTypeDef,
+    PutResolverQueryLogConfigPolicyResponseTypeDef,
+    PutResolverRulePolicyResponseTypeDef,
+    UpdateFirewallDomainsResponseTypeDef,
     UpdateFirewallRuleGroupAssociationResponseTypeDef,
     AssociateResolverEndpointIpAddressRequestRequestTypeDef,
     DisassociateResolverEndpointIpAddressRequestRequestTypeDef,
     AssociateResolverEndpointIpAddressResponseTypeDef,
     CreateResolverEndpointResponseTypeDef,
     DeleteResolverEndpointResponseTypeDef,
     DisassociateResolverEndpointIpAddressResponseTypeDef,
@@ -552,38 +543,47 @@
     CreateResolverQueryLogConfigResponseTypeDef,
     DeleteResolverQueryLogConfigResponseTypeDef,
     GetResolverQueryLogConfigResponseTypeDef,
     ListResolverQueryLogConfigsResponseTypeDef,
     CreateResolverRuleRequestRequestTypeDef,
     ResolverRuleConfigTypeDef,
     ResolverRuleTypeDef,
-    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
     ListResolverDnssecConfigsRequestRequestTypeDef,
-    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
     ListResolverEndpointsRequestRequestTypeDef,
-    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
     ListResolverQueryLogConfigAssociationsRequestRequestTypeDef,
-    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
     ListResolverQueryLogConfigsRequestRequestTypeDef,
-    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
     ListResolverRuleAssociationsRequestRequestTypeDef,
-    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
     ListResolverRulesRequestRequestTypeDef,
     GetFirewallConfigResponseTypeDef,
     ListFirewallConfigsResponseTypeDef,
     UpdateFirewallConfigResponseTypeDef,
     ListFirewallDomainListsResponseTypeDef,
     ListFirewallRuleGroupsResponseTypeDef,
     GetResolverConfigResponseTypeDef,
     ListResolverConfigsResponseTypeDef,
     UpdateResolverConfigResponseTypeDef,
     GetResolverDnssecConfigResponseTypeDef,
     ListResolverDnssecConfigsResponseTypeDef,
     UpdateResolverDnssecConfigResponseTypeDef,
     ListResolverEndpointIpAddressesResponseTypeDef,
+    ListFirewallConfigsRequestListFirewallConfigsPaginateTypeDef,
+    ListFirewallDomainListsRequestListFirewallDomainListsPaginateTypeDef,
+    ListFirewallDomainsRequestListFirewallDomainsPaginateTypeDef,
+    ListFirewallRuleGroupAssociationsRequestListFirewallRuleGroupAssociationsPaginateTypeDef,
+    ListFirewallRuleGroupsRequestListFirewallRuleGroupsPaginateTypeDef,
+    ListFirewallRulesRequestListFirewallRulesPaginateTypeDef,
+    ListResolverConfigsRequestListResolverConfigsPaginateTypeDef,
+    ListResolverDnssecConfigsRequestListResolverDnssecConfigsPaginateTypeDef,
+    ListResolverEndpointIpAddressesRequestListResolverEndpointIpAddressesPaginateTypeDef,
+    ListResolverEndpointsRequestListResolverEndpointsPaginateTypeDef,
+    ListResolverQueryLogConfigAssociationsRequestListResolverQueryLogConfigAssociationsPaginateTypeDef,
+    ListResolverQueryLogConfigsRequestListResolverQueryLogConfigsPaginateTypeDef,
+    ListResolverRuleAssociationsRequestListResolverRuleAssociationsPaginateTypeDef,
+    ListResolverRulesRequestListResolverRulesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     UpdateResolverEndpointRequestRequestTypeDef,
     UpdateResolverRuleRequestRequestTypeDef,
     CreateResolverRuleResponseTypeDef,
     DeleteResolverRuleResponseTypeDef,
     GetResolverRuleResponseTypeDef,
     ListResolverRulesResponseTypeDef,
     UpdateResolverRuleResponseTypeDef,
@@ -597,42 +597,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-route53resolver-1.26.133/mypy_boto3_route53resolver.egg-info/SOURCES.txt` & `mypy-boto3-route53resolver-1.26.87/mypy_boto3_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.26.133/setup.py` & `mypy-boto3-route53resolver-1.26.87/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-route53resolver.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-route53resolver",
-    version="1.26.133",
+    version="1.26.87",
     packages=["mypy_boto3_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Resolver 1.26.133 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Route53Resolver 1.26.87 service generated with"
+        " mypy-boto3-builder 7.12.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

