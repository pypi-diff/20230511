# Comparing `tmp/python-neutronclient-8.2.1.tar.gz` & `tmp/python-neutronclient-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-neutronclient-8.2.1.tar", last modified: Wed Jan  4 13:40:19 2023, max compression
+gzip compressed data, was "python-neutronclient-9.0.0.tar", last modified: Fri Feb 17 10:24:31 2023, max compression
```

## Comparing `python-neutronclient-8.2.1.tar` & `python-neutronclient-9.0.0.tar`

### file list

```diff
@@ -1,454 +1,446 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13283 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46125 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.684565 python-neutronclient-8.2.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.684565 python-neutronclient-8.2.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.688565 python-neutronclient-8.2.1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/neutron-reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18699 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/neutron.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.672565 python-neutronclient-8.2.1/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.688565 python-neutronclient-8.2.1/doc/source/cli/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/bgp-dynamic-routing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/firewall-group.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/firewall-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/firewall-rule.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/network-log.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/network-trunk.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/networking-bgpvpn.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/networking-sfc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/subnet-onboard.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/vpn-endpoint-group.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/vpn-ike-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/vpn-ipsec-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/vpn-ipsec-site-connection.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc/v2/vpn-service.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/cli/osc_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2105 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.692565 python-neutronclient-8.2.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9492 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/contributor/cli_option_guideline.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3756 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/contributor/client_command_extensions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15534 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/contributor/transition_to_osc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.692565 python-neutronclient-8.2.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/doc/source/reference/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6876 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutron_test.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.692565 python-neutronclient-8.2.1/neutronclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16747 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.692565 python-neutronclient-8.2.1/neutronclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/clientmanager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6744 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3434 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3764 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/serializer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8051 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/common/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.692565 python-neutronclient-8.2.1/neutronclient/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2250 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.696565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30910 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12421 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/agentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4472 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1410 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/availability_zone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.700565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/dragentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4366 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/peer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10237 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/speaker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.700565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/contrib/_fox_sockets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2563 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.700565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5690 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3237 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/flavor_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5525 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/floatingip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.700565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8207 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewallpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5730 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewallrule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.700565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2731 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/pool.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.704565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5350 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/l7policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/l7rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5308 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6935 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/vip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4069 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/metering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9334 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12956 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6090 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/purge.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.704565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3463 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/bandwidth_limit_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/dscp_marking_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3844 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/minimum_bandwidth_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9437 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11540 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14072 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/securitygroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/servicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10497 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4222 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/tag.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.704565 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ikepolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9114 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ipsec_site_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4566 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ipsecpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4342 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/vpnservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.704565 python-neutronclient-8.2.1/neutronclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2234 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.704565 python-neutronclient-8.2.1/neutronclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.708565 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5494 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_dragent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6972 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_peer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12320 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_speaker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.708565 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15142 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16604 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallrule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.708565 python-neutronclient-8.2.1/neutronclient/osc/v2/lbaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/lbaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.708565 python-neutronclient-8.2.1/neutronclient/osc/v2/logging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/logging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11550 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/logging/network_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.708565 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15967 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/network_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/port_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10347 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/resource_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4309 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/router_association.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12775 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_flow_classifier.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14731 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_chain.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8519 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_pair.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11959 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9214 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_service_graph.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/osc/v2/subnet_onboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/subnet_onboard/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/subnet_onboard/subnet_onboard.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/osc/v2/trunk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/trunk/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13876 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/trunk/network_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8104 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9098 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ikepolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14913 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ipsec_site_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9330 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ipsecpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4312 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8519 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/vpnservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24286 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.712565 python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_fwaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_vpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.716565 python-neutronclient-8.2.1/neutronclient/tests/functional/core/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_cli_formatter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_clientlib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8183 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_readonly_neutron.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_subnet_create.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.716565 python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/fwaas
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1107 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/gate_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2143 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/post_test_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/vpnaas
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.720565 python-neutronclient-8.2.1/neutronclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.720565 python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_dragentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9584 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_peer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12211 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_speaker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6166 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/test_cli20_flavor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/test_cli20_flavor_profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/fw/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/fw/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7297 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewall.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10373 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewallpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11582 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewallrule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8574 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4816 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6731 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8196 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_vip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_healthmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10740 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_l7policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8108 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_l7rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8968 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_listener.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9606 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7717 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_member.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9008 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_pool.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.724565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.728565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4920 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_dragent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_peer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5264 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_speaker.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1914 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.728565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10581 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26025 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24925 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31042 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallrule.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.728565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/lbaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/lbaas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.728565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2490 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26685 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/test_network_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.728565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7630 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20474 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11876 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_resource_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11328 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_router_association.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.732565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9117 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/fakes.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14512 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_flow_classifier.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    21491 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_chain.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11357 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_pair.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18310 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_pair_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12153 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_service_graph.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.732565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/subnet_onboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/subnet_onboard/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/subnet_onboard/test_network_onboard_subnets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.732565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/trunk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/trunk/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/trunk/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25905 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/trunk/test_network_trunk.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.732565 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5531 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6271 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8904 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11390 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ikepolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13688 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsec_site_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10760 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsecpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10153 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_vpnservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.736565 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6205 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_bandwidth_limit_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_dscp_marking_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_minimum_bandwidth_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3341 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5814 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_casual_args.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49363 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7608 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3652 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_agents.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8710 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_agentschedulers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_az.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8241 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_floatingips.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3969 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_metering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31638 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35069 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5755 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_rbac.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19484 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30857 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_securitygroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_servicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30473 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9368 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9447 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_client_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_command_meta.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10337 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_name_or_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4035 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14278 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.736565 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6110 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9647 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ikepolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14702 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ipsec_site_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10287 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ipsecpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_vpnservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6025 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.736565 python-neutronclient-8.2.1/neutronclient/v2_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/v2_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116801 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/v2_0/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/neutronclient/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.736565 python-neutronclient-8.2.1/python_neutronclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18504 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31596 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-01-04 13:40:19.000000 python-neutronclient-8.2.1/python_neutronclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.680565 python-neutronclient-8.2.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.752565 python-neutronclient-8.2.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/Define-IpAddressAlreadyAllocatedClient-exception-e8600ca5ba1c7f45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-aggressive-negotiation-mode-5218b1baff930eb8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-auto-allocated-topology-delete-aaccd60bd0f2e7b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-get-me-a-network-5ab2d60bf6f257b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-l7-content-policies-capability-0f17cd06f044c83c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-lb-status-tree-723f23c09617de3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-neutron-purge-a89e3d1179dce4b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-new-session-clear-option-3c0b78ebc133a10c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-no-shared-option-to-qos-policy-update-56ac41fb3af7e309.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-osc-dynamic-routing-support-11130b2f440c0ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-osc-trunk-commands-7e77283a369729c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-quota-default-show-c2ab35b791dcdcbc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-rbac-qos-type-support-c42e31fadd7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-service-graph-ce4a25b3e32d70a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-sfc-commands.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-shared-pools-support-6f79b565afad3e47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-subnet-onboard-e60772bc4984f698.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-support-to-floating-ip-port-forwardings-9dc838a5c5727eb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/add-tag-support-bad62d60ecc7075c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/availability-zone-support-8e66f55e46b7ef9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/bgp-dynamic-routing-b97a1c81d3007049.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/bug-1676922-81341b70bc6f055a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/bulk-delete-support-94a353db08efec8d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/default-subnetpool-support-c0d34870e9d3e814.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/deprecate-bgp-speaker-show-dragents-2fcce99cf6bb5b60.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/deprecate-cli-7be1123817969439.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/direct-physical-vnic-port-create-736d8b2600faf22b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/docs-improvements-17e31babe38e2962.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/drop-nuage-commands-df10aab6ccd77ed2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/drop-python-2.7-f615ebae463b2143.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/drop-python-3-6-and-3-7-73767fa0bbe89a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/drop-xml-support-41babecb1784d996.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/dscp_qos-4a26d3c0363624b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/extraroute-atomic-b11919d8e33b0d92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/fix-exception-typeerror-4.1.0-b37d738146575ed5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/fix-quota-update-zero-args-d596c4169c2d2e30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/fix-rbac-create-command-dd40a474f0f092db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/fix-token-endpoint-auth-support-26bf7ee12e4ec833.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/global_request_id-56856a93b982a6b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/keystonev3-7f9ede9c21b30841.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/log-request-id-64bef955b8292c18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/minimum-packet-rate-34576b8fd98a3034.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/network-ip-availability-ac9a462f42fe9db4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/neutron-cli-deprecation-398823c87270a296.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/no-new-binding-code-b03c9abbcaf2839e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/osprofiler-support-9ba539761ae437e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/paket_rate_limit-1266a2a30f18727f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/port-bindings-c3f36bd76ece0a71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/qos_minimum_bandwidth-dc4adb23c51de30b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/quota-update-for-LB-b21e7bc9e4a10f3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/quota-update-for-rbac-192a8e65bf481941.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/relnotes-from-3.0.0-d7306f5af5e3868d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/remote_fwg-0f5362e5be8b2e84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/remove-case-dependency-773ccb3237c38e81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/remove-deprecated-option-b53f5d7e6a16ce95.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/remove-public-and-private-parameters-d683e7c30ecedc3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/return-request-id-to-caller-15b1d23a4ddc27a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/segments-8557f5b0caa5ee26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/sfc-tap-service-function-support-a05242f25f79066b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/show-tenant-id-admin-listing-dc13ee7eb889d418.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/start-using-reno-9081b3e4c1951fdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-bgpvpn-route-control-aeda3e698486f73b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-firewall-group-resource-type-5ad1b69cabcb4aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-fwaasv2-cli-7f21676c551f8ae0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-logging-cli-cd02d3bb03367106.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-networking-bgpvpn-cli-fdd0cc3a5b14983d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-routes-advertise-9356a38cf3e2fe5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-vni-in-networking-bgpvpn-cli-d284b73b40b79495.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/support-vpnaas-cli-9478fb7cfe603e26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/notes/tag-support-subnet-port-subnetpool-router-6250ec4714ee8690.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.752565 python-neutronclient-8.2.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6585 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/old_relnotes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32963 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-01-04 13:40:19.756565 python-neutronclient-8.2.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/tools/neutron.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2624 2023-01-04 13:39:48.000000 python-neutronclient-8.2.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13283 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46273 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.212708 python-neutronclient-9.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.212708 python-neutronclient-9.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.212708 python-neutronclient-9.0.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2309 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/neutron-reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18699 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/neutron.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.204707 python-neutronclient-9.0.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/doc/source/cli/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1503 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/bgp-dynamic-routing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/firewall-group.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/firewall-policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/firewall-rule.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/network-log.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/networking-bgpvpn.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/networking-sfc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/subnet-onboard.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/vpn-endpoint-group.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/vpn-ike-policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/vpn-ipsec-policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/vpn-ipsec-site-connection.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc/v2/vpn-service.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/cli/osc_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2105 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9492 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/contributor/cli_option_guideline.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3756 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/contributor/client_command_extensions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15534 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/contributor/transition_to_osc.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3433 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/doc/source/reference/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6876 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutron_test.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/neutronclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16747 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/neutronclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/clientmanager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6744 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3434 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3764 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/serializer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8051 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2593 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/common/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.216708 python-neutronclient-9.0.0/neutronclient/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2250 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.220708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30910 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2863 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12421 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/agentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4472 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1410 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/availability_zone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.220708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/dragentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4366 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/peer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10237 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/speaker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.220708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/contrib/_fox_sockets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2563 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.220708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5690 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3237 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/flavor_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5525 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/floatingip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.220708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8207 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewallpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5730 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewallrule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2731 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3909 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5350 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/l7policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4776 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/l7rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5308 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6935 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/vip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4069 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/metering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9334 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12956 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6090 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/purge.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3463 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/bandwidth_limit_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/dscp_marking_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3844 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/minimum_bandwidth_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9437 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11540 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14072 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/securitygroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/servicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10497 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4222 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/tag.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4377 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ikepolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9114 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ipsec_site_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4566 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ipsecpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4342 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/vpnservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2234 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4437 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.224708 python-neutronclient-9.0.0/neutronclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.228708 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5494 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_dragent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6972 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_peer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12320 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_speaker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.228708 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15142 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16604 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallrule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.228708 python-neutronclient-9.0.0/neutronclient/osc/v2/lbaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/lbaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.228708 python-neutronclient-9.0.0/neutronclient/osc/v2/logging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/logging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11550 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/logging/network_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.228708 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15967 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/network_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12226 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/port_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10347 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/resource_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4309 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/router_association.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12775 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_flow_classifier.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14731 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_chain.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8519 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_pair.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11959 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_pair_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9214 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_service_graph.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/osc/v2/subnet_onboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/subnet_onboard/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2091 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/subnet_onboard/subnet_onboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8104 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9098 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ikepolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14913 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ipsec_site_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9330 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ipsecpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4312 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8519 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/vpnservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24286 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_fwaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_vpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/tests/functional/core/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_cli_formatter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2366 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_clientlib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8183 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5377 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_readonly_neutron.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1533 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_subnet_create.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.232708 python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/fwaas
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1107 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2143 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/vpnaas
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2753 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_dragentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9584 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_peer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12211 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_speaker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6166 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/test_cli20_flavor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/test_cli20_flavor_profile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/fw/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/fw/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7297 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewall.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10373 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewallpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11582 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewallrule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8574 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4816 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6731 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8196 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_vip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_healthmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10740 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_l7policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8108 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_l7rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8968 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_listener.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9606 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7717 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_member.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9008 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.240708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4920 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_dragent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_peer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5264 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_speaker.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1914 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10581 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26025 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24925 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31042 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallrule.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/lbaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/lbaas/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2490 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26685 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/test_network_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7630 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20474 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11876 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_resource_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11328 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_router_association.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     9117 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/fakes.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    14512 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_flow_classifier.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    21491 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_chain.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11357 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_pair.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18310 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_pair_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12153 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_service_graph.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.244708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/subnet_onboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/subnet_onboard/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/subnet_onboard/test_network_onboard_subnets.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.248708 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5531 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6271 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8904 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11390 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ikepolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13688 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsec_site_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10760 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsecpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10153 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_vpnservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.248708 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6205 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_bandwidth_limit_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_dscp_marking_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_minimum_bandwidth_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1697 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3341 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5814 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_casual_args.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49363 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7608 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3652 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_agents.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8710 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_agentschedulers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_az.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8241 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_floatingips.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3969 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_metering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31638 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35069 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5755 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_rbac.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19484 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30857 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_securitygroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2178 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_servicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30473 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9368 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9447 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_client_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_command_meta.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5616 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10337 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_name_or_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4035 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14278 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6368 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4101 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.248708 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6110 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9647 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ikepolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14702 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ipsec_site_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10287 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ipsecpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6152 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_vpnservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6025 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.248708 python-neutronclient-9.0.0/neutronclient/v2_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/v2_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116617 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/v2_0/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/neutronclient/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.248708 python-neutronclient-9.0.0/python_neutronclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18224 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31031 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-02-17 10:24:31.000000 python-neutronclient-9.0.0/python_neutronclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.208708 python-neutronclient-9.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.256708 python-neutronclient-9.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/Define-IpAddressAlreadyAllocatedClient-exception-e8600ca5ba1c7f45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-aggressive-negotiation-mode-5218b1baff930eb8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-auto-allocated-topology-delete-aaccd60bd0f2e7b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-get-me-a-network-5ab2d60bf6f257b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-l7-content-policies-capability-0f17cd06f044c83c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-lb-status-tree-723f23c09617de3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-neutron-purge-a89e3d1179dce4b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-new-session-clear-option-3c0b78ebc133a10c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-no-shared-option-to-qos-policy-update-56ac41fb3af7e309.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-osc-dynamic-routing-support-11130b2f440c0ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-osc-trunk-commands-7e77283a369729c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-quota-default-show-c2ab35b791dcdcbc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-rbac-qos-type-support-c42e31fadd7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-service-graph-ce4a25b3e32d70a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-sfc-commands.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-shared-pools-support-6f79b565afad3e47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-subnet-onboard-e60772bc4984f698.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-support-to-floating-ip-port-forwardings-9dc838a5c5727eb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/add-tag-support-bad62d60ecc7075c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/availability-zone-support-8e66f55e46b7ef9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/bgp-dynamic-routing-b97a1c81d3007049.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/bug-1676922-81341b70bc6f055a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/bulk-delete-support-94a353db08efec8d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/default-subnetpool-support-c0d34870e9d3e814.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/deprecate-bgp-speaker-show-dragents-2fcce99cf6bb5b60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/deprecate-cli-7be1123817969439.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/direct-physical-vnic-port-create-736d8b2600faf22b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/docs-improvements-17e31babe38e2962.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/drop-nuage-commands-df10aab6ccd77ed2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/drop-python-2.7-f615ebae463b2143.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/drop-python-3-6-and-3-7-73767fa0bbe89a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/drop-xml-support-41babecb1784d996.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/dscp_qos-4a26d3c0363624b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/extraroute-atomic-b11919d8e33b0d92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/fix-exception-typeerror-4.1.0-b37d738146575ed5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/fix-quota-update-zero-args-d596c4169c2d2e30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/fix-rbac-create-command-dd40a474f0f092db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/fix-token-endpoint-auth-support-26bf7ee12e4ec833.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/global_request_id-56856a93b982a6b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/keystonev3-7f9ede9c21b30841.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/log-request-id-64bef955b8292c18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/minimum-packet-rate-34576b8fd98a3034.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/network-ip-availability-ac9a462f42fe9db4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/neutron-cli-deprecation-398823c87270a296.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/no-new-binding-code-b03c9abbcaf2839e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/osprofiler-support-9ba539761ae437e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/paket_rate_limit-1266a2a30f18727f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/port-bindings-c3f36bd76ece0a71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/qos_minimum_bandwidth-dc4adb23c51de30b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/quota-update-for-LB-b21e7bc9e4a10f3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/quota-update-for-rbac-192a8e65bf481941.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/relnotes-from-3.0.0-d7306f5af5e3868d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/remote_fwg-0f5362e5be8b2e84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/remove-case-dependency-773ccb3237c38e81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/remove-deprecated-option-b53f5d7e6a16ce95.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/remove-public-and-private-parameters-d683e7c30ecedc3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/return-request-id-to-caller-15b1d23a4ddc27a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/segments-8557f5b0caa5ee26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/sfc-tap-service-function-support-a05242f25f79066b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/show-tenant-id-admin-listing-dc13ee7eb889d418.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/start-using-reno-9081b3e4c1951fdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-bgpvpn-route-control-aeda3e698486f73b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-firewall-group-resource-type-5ad1b69cabcb4aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-fwaasv2-cli-7f21676c551f8ae0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-logging-cli-cd02d3bb03367106.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-networking-bgpvpn-cli-fdd0cc3a5b14983d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-routes-advertise-9356a38cf3e2fe5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-vni-in-networking-bgpvpn-cli-d284b73b40b79495.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/support-vpnaas-cli-9478fb7cfe603e26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/notes/tag-support-subnet-port-subnetpool-router-6250ec4714ee8690.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6585 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/old_relnotes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32391 2023-02-17 10:24:31.264709 python-neutronclient-9.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-17 10:24:31.260708 python-neutronclient-9.0.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/tools/neutron.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2023-02-17 10:24:04.000000 python-neutronclient-9.0.0/tox.ini
```

### Comparing `python-neutronclient-8.2.1/.pylintrc` & `python-neutronclient-9.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/.zuul.yaml` & `python-neutronclient-9.0.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/AUTHORS` & `python-neutronclient-9.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/CONTRIBUTING.rst` & `python-neutronclient-9.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/ChangeLog` & `python-neutronclient-9.0.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+9.0.0
+-----
+
+* Remove CLI warning message
+* Move network trunk commands from python-neutronclient
+* Tox4: add allowlist\_externals where necessary
+
 8.2.1
 -----
 
 * Fix help sentence in network log create --enable
 
 8.2.0
 -----
```

### Comparing `python-neutronclient-8.2.1/HACKING.rst` & `python-neutronclient-9.0.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/LICENSE` & `python-neutronclient-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/PKG-INFO` & `python-neutronclient-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-neutronclient
-Version: 8.2.1
+Version: 9.0.0
 Summary: CLI and Client Library for OpenStack Networking
 Home-page: https://docs.openstack.org/python-neutronclient/latest/
 Author: OpenStack Networking Project
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-neutronclient-8.2.1/README.rst` & `python-neutronclient-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/index.rst` & `python-neutronclient-9.0.0/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/neutron-reference.rst` & `python-neutronclient-9.0.0/doc/source/cli/neutron-reference.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/neutron.rst` & `python-neutronclient-9.0.0/doc/source/cli/neutron.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/bgp-dynamic-routing.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/bgp-dynamic-routing.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/firewall-group.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/firewall-group.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/firewall-policy.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/firewall-policy.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/networking-bgpvpn.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/networking-bgpvpn.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/networking-sfc.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/networking-sfc.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc/v2/subnet-onboard.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc/v2/subnet-onboard.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/cli/osc_plugins.rst` & `python-neutronclient-9.0.0/doc/source/cli/osc_plugins.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/conf.py` & `python-neutronclient-9.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/contributor/cli_option_guideline.rst` & `python-neutronclient-9.0.0/doc/source/contributor/cli_option_guideline.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/contributor/client_command_extensions.rst` & `python-neutronclient-9.0.0/doc/source/contributor/client_command_extensions.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/contributor/index.rst` & `python-neutronclient-9.0.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/contributor/transition_to_osc.rst` & `python-neutronclient-9.0.0/doc/source/contributor/transition_to_osc.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/index.rst` & `python-neutronclient-9.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/doc/source/reference/index.rst` & `python-neutronclient-9.0.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutron_test.sh` & `python-neutronclient-9.0.0/neutron_test.sh`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/_i18n.py` & `python-neutronclient-9.0.0/neutronclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/client.py` & `python-neutronclient-9.0.0/neutronclient/client.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/clientmanager.py` & `python-neutronclient-9.0.0/neutronclient/common/clientmanager.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/constants.py` & `python-neutronclient-9.0.0/neutronclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/exceptions.py` & `python-neutronclient-9.0.0/neutronclient/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/extension.py` & `python-neutronclient-9.0.0/neutronclient/common/extension.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/serializer.py` & `python-neutronclient-9.0.0/neutronclient/common/serializer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/utils.py` & `python-neutronclient-9.0.0/neutronclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/common/validators.py` & `python-neutronclient-9.0.0/neutronclient/common/validators.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/client.py` & `python-neutronclient-9.0.0/neutronclient/neutron/client.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/__init__.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/__init__.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/address_scope.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/address_scope.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/agent.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/agent.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/agentscheduler.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/agentscheduler.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/auto_allocated_topology.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/availability_zone.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/availability_zone.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/dragentscheduler.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/dragentscheduler.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/peer.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/peer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/bgp/speaker.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/bgp/speaker.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/contrib/_fox_sockets.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/contrib/_fox_sockets.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/dns.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/dns.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/extension.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/extension.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/flavor.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/flavor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/flavor/flavor_profile.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/flavor/flavor_profile.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/floatingip.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/floatingip.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewall.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewall.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewallpolicy.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewallpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/fw/firewallrule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/fw/firewallrule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/healthmonitor.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/healthmonitor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/member.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/member.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/pool.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/pool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/healthmonitor.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/healthmonitor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/l7policy.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/l7policy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/l7rule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/l7rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/listener.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/listener.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/loadbalancer.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/member.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/member.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/v2/pool.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/v2/pool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/lb/vip.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/lb/vip.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/metering.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/metering.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/network.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/network.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/network_ip_availability.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/port.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/port.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/purge.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/purge.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/bandwidth_limit_rule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/bandwidth_limit_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/dscp_marking_rule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/dscp_marking_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/minimum_bandwidth_rule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/minimum_bandwidth_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/policy.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/policy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/qos/rule.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/qos/rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/quota.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/quota.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/rbac.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/rbac.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/router.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/router.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/securitygroup.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/securitygroup.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/servicetype.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/servicetype.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/subnet.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/subnet.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/subnetpool.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/subnetpool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/tag.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/tag.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/endpoint_group.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/endpoint_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ikepolicy.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ikepolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ipsec_site_connection.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ipsec_site_connection.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/ipsecpolicy.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/ipsecpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/utils.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/neutron/v2_0/vpn/vpnservice.py` & `python-neutronclient-9.0.0/neutronclient/neutron/v2_0/vpn/vpnservice.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/plugin.py` & `python-neutronclient-9.0.0/neutronclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/utils.py` & `python-neutronclient-9.0.0/neutronclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_dragent.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_peer.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_peer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/bgp_speaker.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/bgp_speaker.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/dynamic_routing/constants.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/dynamic_routing/constants.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/constants.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/constants.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallgroup.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallgroup.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallpolicy.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/fwaas/firewallrule.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/fwaas/firewallrule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/logging/network_log.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/logging/network_log.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/bgpvpn.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/bgpvpn.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/constants.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/constants.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/network_association.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/network_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/port_association.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/port_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/resource_association.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/resource_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/networking_bgpvpn/router_association.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/networking_bgpvpn/router_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_flow_classifier.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_flow_classifier.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_chain.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_chain.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_pair.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_pair.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_port_pair_group.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_port_pair_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/sfc/sfc_service_graph.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/sfc/sfc_service_graph.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/subnet_onboard/subnet_onboard.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/subnet_onboard/subnet_onboard.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/utils.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/endpoint_group.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/endpoint_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ikepolicy.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ikepolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ipsec_site_connection.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ipsec_site_connection.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/ipsecpolicy.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/ipsecpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/utils.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/osc/v2/vpnaas/vpnservice.py` & `python-neutronclient-9.0.0/neutronclient/osc/v2/vpnaas/vpnservice.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/shell.py` & `python-neutronclient-9.0.0/neutronclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_fwaas.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_fwaas.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_vpn.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/adv-svcs/test_readonly_neutron_vpn.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/base.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_cli_formatter.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_cli_formatter.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_clientlib.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_clientlib.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_common.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_common.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_purge.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_purge.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_readonly_neutron.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_readonly_neutron.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/core/test_subnet_create.py` & `python-neutronclient-9.0.0/neutronclient/tests/functional/core/test_subnet_create.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/gate_hook.sh` & `python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/functional/hooks/post_test_hook.sh` & `python-neutronclient-9.0.0/neutronclient/tests/functional/hooks/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_dragentscheduler.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_dragentscheduler.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_peer.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_peer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/bgp/test_cli20_speaker.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/bgp/test_cli20_speaker.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/test_cli20_flavor.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/test_cli20_flavor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/flavor/test_cli20_flavor_profile.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/flavor/test_cli20_flavor_profile.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewall.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewall.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewallpolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewallpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/fw/test_cli20_firewallrule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/fw/test_cli20_firewallrule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_healthmonitor.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_healthmonitor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_member.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_member.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_pool.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_pool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/test_cli20_vip.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/test_cli20_vip.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_healthmonitor.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_healthmonitor.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_l7policy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_l7policy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_l7rule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_l7rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_listener.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_listener.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_loadbalancer.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_member.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_member.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/lb/v2/test_cli20_pool.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/lb/v2/test_cli20_pool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_dragent.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_dragent.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_peer.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_peer.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_speaker.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/dynamic_routing/test_bgp_speaker.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/common.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/common.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallgroup.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallgroup.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallpolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/fwaas/test_firewallrule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/fwaas/test_firewallrule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/logging/test_network_log.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/logging/test_network_log.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_bgpvpn.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_resource_association.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_resource_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_router_association.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/networking_bgpvpn/test_router_association.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_flow_classifier.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_flow_classifier.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_chain.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_chain.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_pair.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_pair.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_port_pair_group.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_port_pair_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/sfc/test_service_graph.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/sfc/test_service_graph.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/subnet_onboard/test_network_onboard_subnets.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/subnet_onboard/test_network_onboard_subnets.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/common.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/common.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/fakes.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/fakes.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_endpoint_group.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ikepolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ikepolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsec_site_connection.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsec_site_connection.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsecpolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_ipsecpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/osc/v2/vpnaas/test_vpnservice.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/osc/v2/vpnaas/test_vpnservice.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_bandwidth_limit_rule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_bandwidth_limit_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_dscp_marking_rule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_dscp_marking_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_minimum_bandwidth_rule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_minimum_bandwidth_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_policy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_policy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/qos/test_cli20_rule.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/qos/test_cli20_rule.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_auto_allocated_topology.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_casual_args.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_casual_args.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_address_scope.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_address_scope.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_agents.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_agents.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_agentschedulers.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_agentschedulers.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_az.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_az.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_extensions.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_extensions.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_floatingips.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_floatingips.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_metering.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_metering.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_network.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_network.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_network_ip_availability.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_port.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_port.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_purge.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_purge.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_rbac.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_rbac.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_router.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_router.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_securitygroup.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_securitygroup.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_servicetype.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_servicetype.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_subnet.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_subnet.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_subnetpool.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_subnetpool.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_cli20_tag.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_cli20_tag.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_client_extension.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_client_extension.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_command_meta.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_command_meta.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_exceptions.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_http.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_http.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_name_or_id.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_name_or_id.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_quota.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_quota.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_shell.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_utils.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/test_validators.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_endpoint_group.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ikepolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ikepolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ipsec_site_connection.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ipsec_site_connection.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_ipsecpolicy.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_ipsecpolicy.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_cli20_vpnservice.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_cli20_vpnservice.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/tests/unit/vpn/test_utils.py` & `python-neutronclient-9.0.0/neutronclient/tests/unit/vpn/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/neutronclient/v2_0/client.py` & `python-neutronclient-9.0.0/neutronclient/v2_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,17 +246,14 @@
     EXTED_PLURALS = {}
 
     @debtcollector.renames.renamed_kwarg(
         'tenant_id', 'project_id', replace=True)
     def __init__(self, **kwargs):
         """Initialize a new client for the Neutron v2.0 API."""
         super(ClientBase, self).__init__()
-        _logger.warning("The python binding code in neutronclient will be "
-                        "deprecated in favor of OpenstackSDK, please use "
-                        "that!")
         self.retries = kwargs.pop('retries', 0)
         self.raise_errors = kwargs.pop('raise_errors', True)
         self.httpclient = client.construct_http_client(**kwargs)
         self.version = '2.0'
         self.action_prefix = "/v%s" % (self.version)
         self.retry_interval = 1
```

### Comparing `python-neutronclient-8.2.1/neutronclient/version.py` & `python-neutronclient-9.0.0/neutronclient/version.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/python_neutronclient.egg-info/PKG-INFO` & `python-neutronclient-9.0.0/python_neutronclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-neutronclient
-Version: 8.2.1
+Version: 9.0.0
 Summary: CLI and Client Library for OpenStack Networking
 Home-page: https://docs.openstack.org/python-neutronclient/latest/
 Author: OpenStack Networking Project
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `python-neutronclient-8.2.1/python_neutronclient.egg-info/SOURCES.txt` & `python-neutronclient-9.0.0/python_neutronclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 doc/source/cli/neutron.rst
 doc/source/cli/osc_plugins.rst
 doc/source/cli/osc/v2/bgp-dynamic-routing.rst
 doc/source/cli/osc/v2/firewall-group.rst
 doc/source/cli/osc/v2/firewall-policy.rst
 doc/source/cli/osc/v2/firewall-rule.rst
 doc/source/cli/osc/v2/network-log.rst
-doc/source/cli/osc/v2/network-trunk.rst
 doc/source/cli/osc/v2/networking-bgpvpn.rst
 doc/source/cli/osc/v2/networking-sfc.rst
 doc/source/cli/osc/v2/subnet-onboard.rst
 doc/source/cli/osc/v2/vpn-endpoint-group.rst
 doc/source/cli/osc/v2/vpn-ike-policy.rst
 doc/source/cli/osc/v2/vpn-ipsec-policy.rst
 doc/source/cli/osc/v2/vpn-ipsec-site-connection.rst
@@ -145,16 +144,14 @@
 neutronclient/osc/v2/sfc/sfc_flow_classifier.py
 neutronclient/osc/v2/sfc/sfc_port_chain.py
 neutronclient/osc/v2/sfc/sfc_port_pair.py
 neutronclient/osc/v2/sfc/sfc_port_pair_group.py
 neutronclient/osc/v2/sfc/sfc_service_graph.py
 neutronclient/osc/v2/subnet_onboard/__init__.py
 neutronclient/osc/v2/subnet_onboard/subnet_onboard.py
-neutronclient/osc/v2/trunk/__init__.py
-neutronclient/osc/v2/trunk/network_trunk.py
 neutronclient/osc/v2/vpnaas/__init__.py
 neutronclient/osc/v2/vpnaas/endpoint_group.py
 neutronclient/osc/v2/vpnaas/ikepolicy.py
 neutronclient/osc/v2/vpnaas/ipsec_site_connection.py
 neutronclient/osc/v2/vpnaas/ipsecpolicy.py
 neutronclient/osc/v2/vpnaas/utils.py
 neutronclient/osc/v2/vpnaas/vpnservice.py
@@ -258,17 +255,14 @@
 neutronclient/tests/unit/osc/v2/sfc/test_flow_classifier.py
 neutronclient/tests/unit/osc/v2/sfc/test_port_chain.py
 neutronclient/tests/unit/osc/v2/sfc/test_port_pair.py
 neutronclient/tests/unit/osc/v2/sfc/test_port_pair_group.py
 neutronclient/tests/unit/osc/v2/sfc/test_service_graph.py
 neutronclient/tests/unit/osc/v2/subnet_onboard/__init__.py
 neutronclient/tests/unit/osc/v2/subnet_onboard/test_network_onboard_subnets.py
-neutronclient/tests/unit/osc/v2/trunk/__init__.py
-neutronclient/tests/unit/osc/v2/trunk/fakes.py
-neutronclient/tests/unit/osc/v2/trunk/test_network_trunk.py
 neutronclient/tests/unit/osc/v2/vpnaas/__init__.py
 neutronclient/tests/unit/osc/v2/vpnaas/common.py
 neutronclient/tests/unit/osc/v2/vpnaas/fakes.py
 neutronclient/tests/unit/osc/v2/vpnaas/test_endpoint_group.py
 neutronclient/tests/unit/osc/v2/vpnaas/test_ikepolicy.py
 neutronclient/tests/unit/osc/v2/vpnaas/test_ipsec_site_connection.py
 neutronclient/tests/unit/osc/v2/vpnaas/test_ipsecpolicy.py
```

### Comparing `python-neutronclient-8.2.1/python_neutronclient.egg-info/entry_points.txt` & `python-neutronclient-9.0.0/python_neutronclient.egg-info/entry_points.txt`

 * *Files 5% similar despite different names*

```diff
@@ -323,21 +323,14 @@
 network_log_create = neutronclient.osc.v2.logging.network_log:CreateNetworkLog
 network_log_delete = neutronclient.osc.v2.logging.network_log:DeleteNetworkLog
 network_log_list = neutronclient.osc.v2.logging.network_log:ListNetworkLog
 network_log_set = neutronclient.osc.v2.logging.network_log:SetNetworkLog
 network_log_show = neutronclient.osc.v2.logging.network_log:ShowNetworkLog
 network_loggable_resources_list = neutronclient.osc.v2.logging.network_log:ListLoggableResource
 network_onboard_subnets = neutronclient.osc.v2.subnet_onboard.subnet_onboard:NetworkOnboardSubnets
-network_subport_list = neutronclient.osc.v2.trunk.network_trunk:ListNetworkSubport
-network_trunk_create = neutronclient.osc.v2.trunk.network_trunk:CreateNetworkTrunk
-network_trunk_delete = neutronclient.osc.v2.trunk.network_trunk:DeleteNetworkTrunk
-network_trunk_list = neutronclient.osc.v2.trunk.network_trunk:ListNetworkTrunk
-network_trunk_set = neutronclient.osc.v2.trunk.network_trunk:SetNetworkTrunk
-network_trunk_show = neutronclient.osc.v2.trunk.network_trunk:ShowNetworkTrunk
-network_trunk_unset = neutronclient.osc.v2.trunk.network_trunk:UnsetNetworkTrunk
 sfc_flow_classifier_create = neutronclient.osc.v2.sfc.sfc_flow_classifier:CreateSfcFlowClassifier
 sfc_flow_classifier_delete = neutronclient.osc.v2.sfc.sfc_flow_classifier:DeleteSfcFlowClassifier
 sfc_flow_classifier_list = neutronclient.osc.v2.sfc.sfc_flow_classifier:ListSfcFlowClassifier
 sfc_flow_classifier_set = neutronclient.osc.v2.sfc.sfc_flow_classifier:SetSfcFlowClassifier
 sfc_flow_classifier_show = neutronclient.osc.v2.sfc.sfc_flow_classifier:ShowSfcFlowClassifier
 sfc_port_chain_create = neutronclient.osc.v2.sfc.sfc_port_chain:CreateSfcPortChain
 sfc_port_chain_delete = neutronclient.osc.v2.sfc.sfc_port_chain:DeleteSfcPortChain
```

### Comparing `python-neutronclient-8.2.1/releasenotes/notes/add-tag-support-bad62d60ecc7075c.yaml` & `python-neutronclient-9.0.0/releasenotes/notes/add-tag-support-bad62d60ecc7075c.yaml`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/releasenotes/notes/bug-1676922-81341b70bc6f055a.yaml` & `python-neutronclient-9.0.0/releasenotes/notes/bug-1676922-81341b70bc6f055a.yaml`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/releasenotes/notes/relnotes-from-3.0.0-d7306f5af5e3868d.yaml` & `python-neutronclient-9.0.0/releasenotes/notes/relnotes-from-3.0.0-d7306f5af5e3868d.yaml`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/releasenotes/source/conf.py` & `python-neutronclient-9.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/releasenotes/source/old_relnotes.rst` & `python-neutronclient-9.0.0/releasenotes/source/old_relnotes.rst`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/requirements.txt` & `python-neutronclient-9.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/setup.cfg` & `python-neutronclient-9.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,14 @@
 
 [entry_points]
 console_scripts = 
 	neutron = neutronclient.shell:main
 openstack.cli.extension = 
 	neutronclient = neutronclient.osc.plugin
 openstack.neutronclient.v2 = 
-	network_subport_list = neutronclient.osc.v2.trunk.network_trunk:ListNetworkSubport
-	network_trunk_create = neutronclient.osc.v2.trunk.network_trunk:CreateNetworkTrunk
-	network_trunk_delete = neutronclient.osc.v2.trunk.network_trunk:DeleteNetworkTrunk
-	network_trunk_list = neutronclient.osc.v2.trunk.network_trunk:ListNetworkTrunk
-	network_trunk_set = neutronclient.osc.v2.trunk.network_trunk:SetNetworkTrunk
-	network_trunk_show = neutronclient.osc.v2.trunk.network_trunk:ShowNetworkTrunk
-	network_trunk_unset = neutronclient.osc.v2.trunk.network_trunk:UnsetNetworkTrunk
 	sfc_flow_classifier_create = neutronclient.osc.v2.sfc.sfc_flow_classifier:CreateSfcFlowClassifier
 	sfc_flow_classifier_delete = neutronclient.osc.v2.sfc.sfc_flow_classifier:DeleteSfcFlowClassifier
 	sfc_flow_classifier_list = neutronclient.osc.v2.sfc.sfc_flow_classifier:ListSfcFlowClassifier
 	sfc_flow_classifier_set = neutronclient.osc.v2.sfc.sfc_flow_classifier:SetSfcFlowClassifier
 	sfc_flow_classifier_show = neutronclient.osc.v2.sfc.sfc_flow_classifier:ShowSfcFlowClassifier
 	sfc_port_chain_create = neutronclient.osc.v2.sfc.sfc_port_chain:CreateSfcPortChain
 	sfc_port_chain_delete = neutronclient.osc.v2.sfc.sfc_port_chain:DeleteSfcPortChain
```

### Comparing `python-neutronclient-8.2.1/setup.py` & `python-neutronclient-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/test-requirements.txt` & `python-neutronclient-9.0.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/tools/neutron.bash_completion` & `python-neutronclient-9.0.0/tools/neutron.bash_completion`

 * *Files identical despite different names*

### Comparing `python-neutronclient-8.2.1/tox.ini` & `python-neutronclient-9.0.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tox]
 envlist = py39,pep8
 minversion = 3.18.0
-skipsdist = True
+skipsdist = False
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 setenv = VIRTUAL_ENV={envdir}
          LANG=en_US.UTF-8
          LANGUAGE=en_US:en
          LC_ALL=C
          PYTHONWARNINGS=default::DeprecationWarning
 usedevelop = True
-install_command = pip install {opts} {packages}
 deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 # Delete bytecodes from normal directories before running tests.
 # Note that bytecodes in dot directories will not be deleted
 # to keep bytecodes of python modules installed into virtualenvs.
-commands = sh -c "find . -type d -name '.?*' -prune -o \
+commands = bash -c "find . -type d -name '.?*' -prune -o \
            \( -type d -name '__pycache__' -o -type f -name '*.py[co]' \) \
            -print0 | xargs -0 rm -rf"
            stestr run {posargs}
-allowlist_externals = sh
+allowlist_externals = bash
 
 [testenv:pep8]
 commands =
   flake8
   {[testenv:bandit]commands}
 distribute = false
```

