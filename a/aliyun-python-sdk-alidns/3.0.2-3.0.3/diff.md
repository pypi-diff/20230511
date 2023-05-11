# Comparing `tmp/aliyun-python-sdk-alidns-3.0.2.tar.gz` & `tmp/aliyun-python-sdk-alidns-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alidns-3.0.2.tar", last modified: Thu Mar 30 03:33:00 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alidns-3.0.3.tar", last modified: Tue Apr  4 03:36:21 2023, max compression
```

## Comparing `aliyun-python-sdk-alidns-3.0.2.tar` & `aliyun-python-sdk-alidns-3.0.3.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1552 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11220 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/
--rw-r--r--   0 root         (0) root         (0)     2299 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddCustomLineRequest.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsCacheDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     6033 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     4522 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/BindInstanceDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ChangeDomainGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ChangeDomainOfDnsProductRequest.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CopyGtmConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CreatePdnsAppKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CreatePdnsUdpIpSegmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteCustomLinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsCacheDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteSubDomainRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeBatchResultCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeBatchResultDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeCustomLineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeCustomLinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDNSSLBSubDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsCacheDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddrAttributeInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddressPoolAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAvailableAlertGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2039 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceSystemCnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1478 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohAccountStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2397 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2588 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohUserInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainDnssecInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2663 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainNsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainRecordInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     3954 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainResolveStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAvailableAlertGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceSystemCnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2584 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanAvailableConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeInstanceDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheRemainQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2721 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAccountSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2536 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsOperateLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2946 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     3674 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsUdpIpSegmentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsUserInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3326 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordResolveStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2337 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3115 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsSummaryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeSubDomainRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1840 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeSupportLinesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeTransferDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ExecuteGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/GetMainDomainNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/GetTxtRecordForVerifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ModifyHichinaDomainDNSRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/MoveDomainResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/MoveGtmResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3555 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/OperateBatchDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/PausePdnsServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/PreviewGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RemovePdnsAppKeyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1593 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RemovePdnsUdpIpSegmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ResumePdnsServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RetrieveDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RollbackGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDNSSLBStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDnsGtmAccessModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1838 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDnsGtmMonitorStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDomainDnssecStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDomainRecordStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetGtmAccessModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1832 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetGtmMonitorStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2061 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SubmitIspFlushCacheTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SwitchDnsGtmInstanceStrategyModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1997 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/TransferDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UnbindInstanceDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateAppKeyStateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateCustomLineRequest.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDNSSLBWeightRequest.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     6027 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmInstanceGlobalConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2758 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmAccessStrategyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2776 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmAddressPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmInstanceGlobalConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmMonitorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2190 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmRecoveryPlanRequest.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateIspFlushCacheInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2379 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ValidateDnsGtmCnameRrCanUseRequest.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ValidatePdnsUdpIpSegmentRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2023-03-30 03:33:00.000000 aliyun-python-sdk-alidns-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11220 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddCustomLineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3344 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsCacheDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6033 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainBackupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4522 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/BindInstanceDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ChangeDomainGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ChangeDomainOfDnsProductRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CopyGtmConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CreatePdnsAppKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CreatePdnsUdpIpSegmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteCustomLinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsCacheDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteSubDomainRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeBatchResultCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeBatchResultDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeCustomLineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeCustomLinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDNSSLBSubDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsCacheDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddrAttributeInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddressPoolAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAvailableAlertGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceSystemCnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohAccountStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohUserInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainDnssecInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainNsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainRecordInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3954 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainResolveStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAvailableAlertGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceSystemCnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanAvailableConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeInstanceDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheRemainQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2721 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAccountSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsOperateLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2946 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsUdpIpSegmentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsUserInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordResolveStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3115 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsSummaryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeSubDomainRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeSupportLinesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeTransferDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ExecuteGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/GetMainDomainNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/GetTxtRecordForVerifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ModifyHichinaDomainDNSRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/MoveDomainResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/MoveGtmResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/OperateBatchDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/PausePdnsServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/PreviewGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RemovePdnsAppKeyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RemovePdnsUdpIpSegmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ResumePdnsServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RetrieveDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RollbackGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDNSSLBStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDnsGtmAccessModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDnsGtmMonitorStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDomainDnssecStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDomainRecordStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetGtmAccessModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetGtmMonitorStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SubmitIspFlushCacheTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SwitchDnsGtmInstanceStrategyModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/TransferDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UnbindInstanceDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateAppKeyStateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateCustomLineRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDNSSLBWeightRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6027 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4357 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmInstanceGlobalConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmAccessStrategyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmAddressPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmInstanceGlobalConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmMonitorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmRecoveryPlanRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateIspFlushCacheInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ValidateDnsGtmCnameRrCanUseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ValidatePdnsUdpIpSegmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-04 03:36:21.000000 aliyun-python-sdk-alidns-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-04-04 03:36:20.000000 aliyun-python-sdk-alidns-3.0.3/setup.py
```

### Comparing `aliyun-python-sdk-alidns-3.0.2/LICENSE` & `aliyun-python-sdk-alidns-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/PKG-INFO` & `aliyun-python-sdk-alidns-3.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alidns
-Version: 3.0.2
+Version: 3.0.3
 Summary: The alidns module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alidns
```

### Comparing `aliyun-python-sdk-alidns-3.0.2/README.rst` & `aliyun-python-sdk-alidns-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/PKG-INFO` & `aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alidns
-Version: 3.0.2
+Version: 3.0.3
 Summary: The alidns module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alidns
```

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyun_python_sdk_alidns.egg-info/SOURCES.txt` & `aliyun-python-sdk-alidns-3.0.3/aliyun_python_sdk_alidns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/endpoint.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddCustomLineRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddCustomLineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsCacheDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsCacheDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDnsGtmMonitorRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDnsGtmMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainBackupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainBackupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainRecordRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmMonitorRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/AddGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/AddGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/BindInstanceDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/BindInstanceDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ChangeDomainGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ChangeDomainGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ChangeDomainOfDnsProductRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ChangeDomainOfDnsProductRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CopyGtmConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CopyGtmConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CreatePdnsAppKeyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CreatePdnsAppKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/CreatePdnsUdpIpSegmentRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/CreatePdnsUdpIpSegmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteCustomLinesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteCustomLinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsCacheDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsCacheDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDnsGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainRecordRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DeleteSubDomainRecordsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DeleteSubDomainRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeBatchResultCountRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeBatchResultCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeBatchResultDetailRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeBatchResultDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeCustomLineRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeCustomLineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeCustomLinesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeCustomLinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDNSSLBSubDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDNSSLBSubDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsCacheDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsCacheDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategiesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddrAttributeInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddrAttributeInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddressPoolAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAddressPoolAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAvailableAlertGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmAvailableAlertGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceAddressPoolsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceSystemCnameRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstanceSystemCnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstancesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsGtmMonitorConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstanceRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstancesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDnsProductInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohAccountStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohAccountStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohDomainStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohSubDomainStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDohUserInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDohUserInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainDnssecInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainDnssecInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainGroupsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainNsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainNsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainRecordInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainRecordInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainRecordsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainResolveStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainResolveStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategiesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmAvailableAlertGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmAvailableAlertGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceAddressPoolsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceSystemCnameRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstanceSystemCnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmInstancesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmMonitorConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanAvailableConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanAvailableConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlansRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeGtmRecoveryPlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeInstanceDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeInstanceDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheInstancesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheRemainQuotaRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheRemainQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTaskRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTasksRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeIspFlushCacheTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAccountSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAccountSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeysRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsAppKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsOperateLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsOperateLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsRequestStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsThreatStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsUdpIpSegmentsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsUdpIpSegmentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribePdnsUserInfoRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribePdnsUserInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordLogsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordResolveStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordResolveStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsSummaryRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeRecordStatisticsSummaryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeSubDomainRecordsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeSubDomainRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeSupportLinesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeSupportLinesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeTagsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/DescribeTransferDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/DescribeTransferDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ExecuteGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ExecuteGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/GetMainDomainNameRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/GetMainDomainNameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/GetTxtRecordForVerifyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/GetTxtRecordForVerifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ListTagResourcesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ModifyHichinaDomainDNSRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ModifyHichinaDomainDNSRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/MoveDomainResourceGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/MoveDomainResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/MoveGtmResourceGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/MoveGtmResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/OperateBatchDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/OperateBatchDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/PausePdnsServiceRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/PausePdnsServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/PreviewGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/PreviewGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RemovePdnsAppKeyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RemovePdnsAppKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RemovePdnsUdpIpSegmentRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RemovePdnsUdpIpSegmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ResumePdnsServiceRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ResumePdnsServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RetrieveDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RetrieveDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/RollbackGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/RollbackGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDNSSLBStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDNSSLBStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDnsGtmAccessModeRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDnsGtmAccessModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDnsGtmMonitorStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDnsGtmMonitorStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDomainDnssecStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDomainDnssecStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetDomainRecordStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetDomainRecordStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetGtmAccessModeRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetGtmAccessModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SetGtmMonitorStatusRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SetGtmMonitorStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SubmitIspFlushCacheTaskRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SubmitIspFlushCacheTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/SwitchDnsGtmInstanceStrategyModeRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/SwitchDnsGtmInstanceStrategyModeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/TagResourcesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/TransferDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/TransferDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UnbindInstanceDomainsRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UnbindInstanceDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UntagResourcesRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateAppKeyStateRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateAppKeyStateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateCustomLineRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateCustomLineRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDNSSLBWeightRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDNSSLBWeightRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRemarkRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRemarkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsCacheDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmInstanceGlobalConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmInstanceGlobalConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDnsGtmMonitorRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDnsGtmMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainGroupRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRemarkRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRemarkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRecordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateDomainRemarkRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateDomainRemarkRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmAccessStrategyRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmAccessStrategyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmAddressPoolRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmAddressPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmInstanceGlobalConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmInstanceGlobalConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmMonitorRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmMonitorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateGtmRecoveryPlanRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateGtmRecoveryPlanRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/UpdateIspFlushCacheInstanceConfigRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/UpdateIspFlushCacheInstanceConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ValidateDnsGtmCnameRrCanUseRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ValidateDnsGtmCnameRrCanUseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/aliyunsdkalidns/request/v20150109/ValidatePdnsUdpIpSegmentRequest.py` & `aliyun-python-sdk-alidns-3.0.3/aliyunsdkalidns/request/v20150109/ValidatePdnsUdpIpSegmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alidns-3.0.2/setup.py` & `aliyun-python-sdk-alidns-3.0.3/setup.py`

 * *Files identical despite different names*

