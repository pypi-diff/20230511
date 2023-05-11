# Comparing `tmp/neutron-lib-3.5.0.tar.gz` & `tmp/neutron-lib-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-lib-3.5.0.tar", last modified: Thu Apr 13 10:18:55 2023, max compression
+gzip compressed data, was "neutron-lib-3.6.0.tar", last modified: Thu May 11 08:57:32 2023, max compression
```

## Comparing `neutron-lib-3.5.0.tar` & `neutron-lib-3.6.0.tar`

### file list

```diff
@@ -1,1458 +1,1485 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8204 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49263 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.704768 neutron-lib-3.5.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.724768 neutron-lib-3.5.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6867 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.740768 neutron-lib-3.5.0/api-ref/source/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6686 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/address-groups.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4827 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/address-scopes.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/agents.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/auto-topology.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/availability_zones.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgp_dragent_scheduler.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgp_peer.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgp_speaker.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6129 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-bgpvpns.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-network_associations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6246 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-overview.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-port_associations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-router_associations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/dhcp-agent-scheduler.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/extensions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7735 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/fip-port-forwarding.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/fip64.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/firewall_log.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13258 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/flavors.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/floatingippools.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13621 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/floatingips.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26223 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/fwaas-v2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19876 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/intro.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/l3-agent-scheduler.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5172 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/l3-conntrack-helper.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10752 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/local-ips.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/logging.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/logging_resource.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9255 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/metering.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/network-ip-availability.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8316 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/network_segment_ranges.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21787 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/networks.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   187466 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25052 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/ports.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37090 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/qos.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/quota_details.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4595 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/quotas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5064 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/rbac-policy.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/router-interface-fip.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5775 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/router-ndp-proxy.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23475 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/routers.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.740768 neutron-lib-3.5.0/api-ref/source/v2/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.744768 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-add-addresses-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-add-addresses-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-remove-addresses-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-remove-addresses-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-groups/address-groups-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.744768 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scope-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scope-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scope-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scope-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scope-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scopes-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.748768 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-dhcp-network-add-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-dhcp-networks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-l3-router-add-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-l3-router-remove-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-l3-routers-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4574 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agents-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/network-dhcp-agent-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/agents/router-l3-agent-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.748768 neutron-lib-3.5.0/api-ref/source/v2/samples/auto-topology/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/auto-topology/topo-show-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.748768 neutron-lib-3.5.0/api-ref/source/v2/samples/availability-zones/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/availability-zones/azs-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.752768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_peer-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_peer-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_peer-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_peer-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_network-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_network-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_peer-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_peer-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_dragent_host-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_routes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_remove_network-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_remove_peer-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/dragent_add_speaker-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/dragent_list_agents_hosting_speaker-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/dragent_list_speakers-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.708768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.752768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpns-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.756768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/network_associations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-show-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.756768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.756768 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.760768 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.760768 neutron-lib-3.5.0/api-ref/source/v2/samples/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/extensions/extension-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4352 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/extensions/extensions-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.764768 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-groups-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-insert-rule-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-insert-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-remove-rule-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-remove-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rules-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.764768 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_log-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_log-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_log-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_log-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_log-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_logs-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.772768 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-insert-rule-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-insert-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-remove-rule-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-remove-rule-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-policy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewalls-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.776768 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-associate-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-associate-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavor-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/flavors-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profile-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profile-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profile-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profile-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profile-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profiles-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.780768 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floating-ip-pools-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4078 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floating-ips-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.780768 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local-ip-list-associations-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local-ips-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip_association-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip_association-create-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.780768 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resources-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.784768 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/logs/loggable_resources-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.788768 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-delete-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-delete-response-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-delete-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-delete-response-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-show-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rules-list-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-show-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-labels-list-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-labels-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.788768 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.788768 neutron-lib-3.5.0/api-ref/source/v2/samples/network-ip-availability/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-list.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-show.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.792768 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_ranges-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.796768 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-bulk-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-bulk-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-provider-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/version-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/networks/versions-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.796768 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.800768 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3160 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2791 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1796 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-resource-request-new-format.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4725 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-bind-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-bulk-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-bulk-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3539 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.812768 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/bandwidth_limit_rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/dscp_marking_rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/packet_rate_limit_rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/rule_type-details-bandwidth_limit-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/rule_type-details-dscp_marking-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/qos/rule_types-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.812768 neutron-lib-3.5.0/api-ref/source/v2/samples/quota_details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/quota_details/quota-details-show-for-project-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.812768 neutron-lib-3.5.0/api-ref/source/v2/samples/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/quotas/quotas-list-for-project-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/quotas/quotas-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/quotas/quotas-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/quotas/quotas-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.812768 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.816768 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-add-extraroutes-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-add-extraroutes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-add-interface-request-with-port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-add-interface-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-add-interface-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-remove-extraroutes-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-remove-extraroutes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-remove-interface-request-with-port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-remove-interface-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-remove-interface-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3586 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/routers/routers-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.824768 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-delete-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-delete-response-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-delete-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-delete-response-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2845 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-show-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3745 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-groups-list-request-json-http.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-groups-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.824768 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segment-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segment-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segment-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segment-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segment-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segments-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/service-type-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.828768 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-add-prefixes-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-add-prefixes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-remove-prefixes-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-remove-prefixes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1676 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpools-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnets-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.832768 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/taf-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/taas/tas-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.832768 neutron-lib-3.5.0/api-ref/source/v2/samples/tag/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/tag/tag-obtain-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/tag/tag-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/tag/tag-update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.836768 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-add-subports-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-add-subports-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-details-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-list-subports-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-remove-subports-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-remove-subports-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunks-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunks-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.840768 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1034 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connections-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-groups-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservices-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5863 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/security-group-rules.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8605 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/security-groups.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/segments.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/service-providers.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/subnetpool_prefix_ops.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8016 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/subnetpools.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16497 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/subnets.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/taas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3459 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/trunk-details.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10324 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/trunk.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30735 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/api-ref/source/v2/vpnaas.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.840768 neutron-lib-3.5.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.844768 neutron-lib-3.5.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7519 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.844768 neutron-lib-3.5.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/api_attributes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/api_converters.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/api_extensions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3468 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/api_validators.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25986 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/callbacks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/consuming.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6006 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/conventions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/db_model_query.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/internals.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/releasing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3871 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/review-guidelines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5407 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/contributor/rpc_api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.844768 neutron-lib-3.5.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.848768 neutron-lib-3.5.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.848768 neutron-lib-3.5.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/user/hacking.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.848768 neutron-lib-3.5.0/neutron_lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.852769 neutron-lib-3.5.0/neutron_lib/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.852769 neutron-lib-3.5.0/neutron_lib/agent/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/l2_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/l3_extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.852769 neutron-lib-3.5.0/neutron_lib/agent/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/linux/interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/agent/topics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.856768 neutron-lib-3.5.0/neutron_lib/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/attributes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12708 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/converters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.892769 neutron-lib-3.5.0/neutron_lib/api/definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12093 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/_dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3214 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/address_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3800 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/agent_resources_synced.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/agent_sort_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/allowedaddresspairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2069 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/availability_zone_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4815 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgp_4byte_asn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgp_dragentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8213 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5626 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_routes_control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_net_assoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_port_assoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_router_assoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_vni.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/data_plane_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1610 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/default_subnetpools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/dhcpagentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/dns_domain_keywords.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/dns_domain_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/ecmp_routes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/empty_string_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/expose_l3_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/expose_port_forwarding_in_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/external_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/extra_dhcp_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/extraroute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/extraroute_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/filter_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip_distributed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_description.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_detail.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_port_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1283 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/fip_port_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10326 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/firewall_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6221 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5143 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/floating_ip_port_forwarding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/floatingip_autodelete_internal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2071 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/floatingip_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/flowclassifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/ip_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1795 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/ip_substring_port_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1334 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l2_adjacency.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7216 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_gw_mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_ha_mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4418 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/l3_port_ip_change_not_allowed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/logging_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3986 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/metering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2101 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/metering_source_and_destination_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/multiprovidernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_cascade_delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2684 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_mtu_writable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5805 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/network_segment_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/pagination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4610 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_hint_ovs_tx_steering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_hints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_mac_address_override.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_mac_address_regenerate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_numa_affinity_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_resource_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_resource_request_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3004 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/port_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9310 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/portbindings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4331 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/portbindings_extended.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/project_default_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/project_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4011 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/provider_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6023 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_bw_limit_direction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_bw_minimum_ingress.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_fip_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_gateway_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_port_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2337 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_minimum_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_minimum_rule_alias.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1330 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rule_type_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rule_type_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4363 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rules_alias.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/quota_check_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_address_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/revisionifmatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/router_admin_state_down_before_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/router_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/router_interface_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/routerservicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_normalized_cidr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_port_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_remote_address_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_shared_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/segment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/segments_peer_subnet_host_routes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/servicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9536 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/sort_key_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/sorting.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/standard_attr_segment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/stateful_security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6714 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_dns_publish_fixed_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_onboard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_segmentid_enforce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2583 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_segmentid_writable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_service_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5028 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/subnetpool_prefix_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/tag_ports_during_bulk_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/trunk_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/uplink_status_propagation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/vlan_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/vlantransparent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16736 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/vpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/vpn_endpoint_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/definitions/vpn_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9771 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/faults.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.892769 neutron-lib-3.5.0/neutron_lib/api/validators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48743 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/validators/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/validators/allowedaddresspairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/validators/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7622 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/validators/dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/api/validators/multiprovidernet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.892769 neutron-lib-3.5.0/neutron_lib/callbacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5489 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8882 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/priority_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/callbacks/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23420 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7057 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.896769 neutron-lib-3.5.0/neutron_lib/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18283 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3658 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/model_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15590 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/model_query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7409 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/quota_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/resource_extend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2913 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/sqlalchemytypes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10604 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/standard_attr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/db/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.900769 neutron-lib-3.5.0/neutron_lib/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27488 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/address_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/allowedaddresspairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/dhcpagentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/external_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/extraroute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6276 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/firewall_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1938 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/l3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1736 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/l3_ext_ha_mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/metering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/multiprovidernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/network_segment_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/placement.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/port_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4401 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/vlantransparent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6509 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/exceptions/vpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14371 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/fixture.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.904769 neutron-lib-3.5.0/neutron_lib/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8160 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3577 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/hacking/translation_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.712768 neutron-lib-3.5.0/neutron_lib/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.712768 neutron-lib-3.5.0/neutron_lib/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.904769 neutron-lib-3.5.0/neutron_lib/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43266 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/locale/zh_CN/LC_MESSAGES/neutron_lib.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.904769 neutron-lib-3.5.0/neutron_lib/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12869 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/common_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3072 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.904769 neutron-lib-3.5.0/neutron_lib/objects/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/extensions/standardattributes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.904769 neutron-lib-3.5.0/neutron_lib/objects/logapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/logapi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/logapi/event_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2575 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/objects/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/placement/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/placement/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35293 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/placement/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/placement/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13632 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/placement/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/directory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/plugins/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47814 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/ml2/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6350 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/ml2/ovs_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15070 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/plugins/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/policy/_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12972 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/services/logapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/logapi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/logapi/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.908769 neutron-lib-3.5.0/neutron_lib/services/qos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/qos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/qos/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2280 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/qos/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.912769 neutron-lib-3.5.0/neutron_lib/services/trunk/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/trunk/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/services/trunk/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.912769 neutron-lib-3.5.0/neutron_lib/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8340 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4237 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/_post_mortem_debug.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.912769 neutron-lib-3.5.0/neutron_lib/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/etc/dummy_policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/etc/neutron_lib.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/etc/no_policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/etc/policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/tools.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.916769 neutron-lib-3.5.0/neutron_lib/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.916769 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.916769 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.916769 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/agent/linux/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.916769 neutron-lib-3.5.0/neutron_lib/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.948769 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9764 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/ip_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test__dummy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_address_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_admin_state_down_before_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent_resources_synced.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent_sort_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_auto_allocated_topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_availability_zone_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp_4byte_asn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp_dragentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_net_assoc_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_port_assoc_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_router_assoc_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_routes_control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_stdattrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_vni.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_data_plane_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_default_subnetpools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dhcpagentscheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dns_domain_ports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dvr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_empty_string_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_expose_l3_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_expose_port_forwarding_in_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_external_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extra_dhcp_opt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extraroute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extraroute_atomic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_filter_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip_distributed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip_port_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_firewall_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_port_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floatingip_autodelete_internal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floatingip_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_flowclassifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_ip_substring_port_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l2_adjancency.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_conntrack_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_gw_mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ha_mode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ndp_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_port_ip_change_not_allowed.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_local_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_logging_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_metering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_metering_source_and_destination_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2074 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_multiprovidernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_cascade_delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_ip_availability.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_mtu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_mtu_writable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_segment_range.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_pagination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_device_profile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_hint_ovs_tx_steering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_hints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_mac_address_regenerate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_numa_affinity_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_portbindings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_portbindings_extended.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_project_default_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_project_id.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_provider_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_limit_direction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_minimum_ingress.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_fip_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_gateway_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_port_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule_alias.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rules_alias.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_quota_check_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_scope.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_bgpvpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_revisionifmatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_router_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_router_interface_fip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_routerservicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_normalized_cidr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_port_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_remote_address_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_shared_filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_segment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_segment_peer_subnet_host_routes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_servicetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sort_key_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sorting.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_standard_attr_segment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_stateful_security_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_dns_publish_fixed_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_onboard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_enforce.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_writable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_service_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnetpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnetpool_prefix_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_taas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_tag_ports_during_bulk_creation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_trunk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_trunk_details.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_uplink_status_propagation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vlan_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vlantransparent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn_endpoint_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13717 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_attributes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16450 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_conversions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8283 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_faults.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.952769 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4046 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_allowedaddresspairs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6835 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_dns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_multiprovidernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57538 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.952769 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_callback_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4222 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16985 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6123 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_registry.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.952769 neutron-lib-3.5.0/neutron_lib/tests/unit/clients/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/clients/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8718 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_model_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_model_query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_resource_extend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9414 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_sqlalchemytypes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4261 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_standard_attr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5603 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/exceptions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/exceptions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10579 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/exceptions/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/fake_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8681 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/hacking/test_checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/legacy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/legacy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14628 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/objects/test_common_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/objects/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.956769 neutron-lib-3.5.0/neutron_lib/tests/unit/placement/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/placement/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38627 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/placement/test_client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13448 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/placement/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/ml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/ml2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/ml2/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3509 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/test_directory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11954 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/policy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/policy/test__engine.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/services/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/services/qos/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/services/qos/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/services/qos/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2587 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/services/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10923 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/test_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/test_neutron_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19828 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/test_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5070 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/test_worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.960769 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7911 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_runtime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.964769 neutron-lib-3.5.0/neutron_lib/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1468 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/file.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6928 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3985 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5052 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/runtime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/utils/upgrade_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/neutron_lib/worker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.852769 neutron-lib-3.5.0/neutron_lib.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78656 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-04-13 10:18:54.000000 neutron-lib-3.5.0/neutron_lib.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.720768 neutron-lib-3.5.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.044769 neutron-lib-3.5.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Add-new-dns_domain_keywords-api-extension-436c2c3a091d15eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Add-oneline-string-validator-aa4e1ccad9d8d5c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Adds-PORT_FORWARDING_FLOATINGIP_KEY-ee2c7d164bea04b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Move-RBAC-share-actions-to-lib-constants-736d881f127c83d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Rehome-missing-ovs-constants-c398aa6462c9eb5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/Rehome-ovs-constants-to-separate-module-07ce93971dd1d7dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-a-getter-for-a-newly-added-option-2082877bf7dd136b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-action-status-3dbfe2490a0d231a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-api-extension-sort-key-validation-b42f5839671fe5f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-availability_zone_filter-extension-e91e1e5e822e4133.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-base-upgrade-checks-class-f6da1d501663d8c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-broadcast-mac-constant-ec00b18a883bf875.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-can-port-be-bound-to-virtual-bridge-5d6db8785e58fcb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-convert-to-string-524541aa6224f66f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-description-field-in-port-forwarding-9da781b1e38ca858.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-directory-is-loaded-e9da5b65824dddad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-empty-string-filtering-api-extension-44cb392025dc359c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-exception-pkg-5a14389891abf358.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-address-group-5e306d90666982aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-security-groups-normalized-cidr-ef7521b226090d7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-security-groups-remote-address-group-c71dbb57b61a1dba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-standard-attr-segment-8c721741589bf10b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-supported-be6f7069856d2891.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-extension-uplink-status-propagation-6b6050d6609c19c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-filter-validation-api-extension-15cc667d5498f163.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-fip-distributed-extension-ce44e8df264d44b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-fip-pf-detail-extension-fa8cd3b3857901d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-floatingip-pools-extension-17a1ee5c7eafc989.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-ip-hopopt-to-protocol-dictionary-3cbe54bb5056f790.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-ip-substring-filtering-extension-06bb0c1f738ee330.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-ipinip-protocol-ab9287f9b698f34c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-is-default-to-network-d16a2e6bcfae943a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-is_filter-keyword-to-attribute-maps-3fa31e91c353d033.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-is_sort_key-keyword-to-attribute-map-75342446d99f4490.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-local-ip-extension-fb4a18f5a6525f1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-network-address-scope-affinity-error-8f6b4493a92142d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-network-cascade-delete-api-extension-f418e44b37c2b2ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-network-segment-range-overlap-exception-e8b4b2b425c51c80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-network-segment-range-plugin-constant-9e80453919162c89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-ovo-registry-27cb7d4ac76d4dc8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-placement-report-plugin-constant-a6a4146c2e39cba3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-port-binding-resource-73f9800dbda121ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-port-bindings-resource-messages-rpc-1382ba9842561cdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-port-mac-address-override-shim-extension-fb11c4f40c12a99b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-port-ranges-support-in-port-forwarding-417da8ef7e2ec140.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-port_details-to-floatingip-a2a3c95cc54737ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-quota-check-limit-api-extension-8e39299644d41f74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-rbac-address-group-39c22aeb30241b11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-rbac-address-scope-dc4683772b205632.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-rbac-bgpvpn-cf6c9346822268f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-rbac-security-groups-2e47acd9eac3a320.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-rbac-subnetpool-bb63d4cef1d06e73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-retrieve-sort-keys-from-attribute-map-ae53d67e0be2ace0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-router-not-found-in-factory-exception-e2bf9431549ff9b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-sg-shared-filtering-api-extension-6c3628cfda6ba6ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-support-for-fetching-specific-column-in-OVO-81b764b203849776.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-traffic-control-exceptions-0e137dae3a556d54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-two-fields-to-duplicated-entry-exception-75b0e07c6e1cc6ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-type-driver-methods-for-network-segment-range-e6d300d430d97dd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-validate-cidr-848c9171dcbcf57c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-validator-pkg-a6565a2d4fbfa1d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-vif-type-agilio-ovs-6bee5b2557aca10e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-vni-to-bgpvpn-7531df9fa4f8955b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add-vnic-virtio-forwarder-portbinding-f7f87dfbef456ed1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add_QuotaDriverAPI_abc_class-1d02d0823a8886a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add_fwg_group-9252d07f1011613d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/add_qos_pps_rule_api_def-dae7c6e67904781b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/admin-state-down-before-update-c06fb3a551fe499f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/advsvc-role-support-d4f1c532264b729a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/agent-resources-synced-e70828841faf7acd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/agent_extensions-2b497ff33c6dc3e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/alembic-branches-6d5947d141efd26e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/allocations_api-1ae5fd78c83353df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/api-definition-base-d2e9514c5ee2ef5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bgpvpn-api-def-22c7072575316ddd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bgpvpn-api-ref-f0294d9ddec726a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bgpvpn-routes-control-51cd95d6ab265cb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bgpvpn_rt_fix-6d02db6a1c22f002.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/boilerplate-ext-descriptor-a5cec8b9b900cbfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bug-1877254-2b997b3911e98079.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bug-1921150-a38bef3c1be69650.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/bug-1957175-6b2705d4772df7de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/callback_priority-2ded960e17bd5db9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/change_placement_client_method_names_b26bb71425f42db3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/cidr_for_canonical_format-4e7925d76a27a19d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/cleanup-unused-l3-attr-def-f0eab40813d17a2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/client-id-number-dhcp-option-a099f927eb8f99af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/conntrack-helper-parent-resource-mapping-95a4a2cb6f6536fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/context-manager-23538670cd9c701f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/context-public-6df198b77027c224.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/core-attributes-43e6969f1b187e5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/correct-dhcp-ipv4-port-numbers-6e22c6aa26009cdc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/create-netmtu-writable-extension-284892119ef6595c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/data-plane-status-ext-c3452a01ef5007ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/default_overrides_none-ecc8dcf2c9c37e5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/deprecate-api-utils-4f86288591c95679.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/deprecate-remote_ip_prefix-in-metering-label-rules-308b3d430bc213b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/directory-fixture-083c5c5f365670d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/disable-port-number-zero-2fb484a802f099a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/dns-api-def-bc24a58f56c5fbfb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/dns-domain-ports-ext-39a069119e79e59b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/drop-python-2-7-f46dfa10169f70db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/drop-python-3-6-and-3-7-daba9483fa3d9b3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/enable-hacking-check-H904-f512ecc98c0a4033.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/ethertype_validator-2d608a46c237e214.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/events_l3_flavors-053714858ced693d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/expose-and-enhance-callback-api-714cce65a3c44fe7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/expose-port-forwarding-in-fip-a7880506cea0ad1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extend-segment-methods-with-filters-6e74953ae2d3b828.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extension-fixture-b7fd61384f1a4d1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extension_descriptor-04025e86249cc94c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extra-dhcp-opt-public-vars-ec4e1c2dcac43d69.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extraroute-atomic-apidef-80a7c6d4a773c701.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/extraroute-atomic-apidef-additive-fb783d66c08618d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fip64-0c6bb38417d602f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fix-api-list-validation-collect-duplicates-f4d45bf5d5abbdff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fix-warnfixture-c9457c50d0d5c5a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/floatingip-autodelete-internal-dep-8e544fad694d1275.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/floatingip-autodelete-internal-f08675d8d64d34c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/floatingip-portforwarding-17c284080541bc78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/flush_on_subtransaction-99ef11dfb56b706d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fwaas-api-def-a6f03db369177b4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fwaas-exceptions-e580766205b466d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/fwaas_converters_validators-c310900b4386146e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/gateway-ip-qos-ext-d3ffb5f517c9f713.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/hacking-check-n537-280ec39c061d9dd7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/interconnection-api-def-cbec5e4f77852fe7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/introduce-logging-api-031d00eb84d5d061.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/introduce-source-and-destination-ip-prefixes-into-metering-label-rules-3d62fccbca8e67b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/introduce_subnetpool_prefix_ops_extension-e37874c936d2554c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/ipv6-canonical-address-13900a784f847ce3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/ipv6_address_usage-ef3d65ad5aa5798b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-agent-extensions-ha-state-change-837140efe4187a99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-agent-extensions-update-network-e4887f7f258e40f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-apidef-exceptions-ee57b9df1c7443d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-apidefs-d028c708c22ef2a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-conntrack-helper-validator-654ccafb296e5f21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-ndp-proxy-71eee0cba8565dad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-port-ip-change-not-allow-2c98e13c08b5ee85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3-support-ecmp-91a8aa61e3a73037.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/l3_conntrack_helper-f186bcdcc31bcaf2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/logging-api-ref-fafb884367ca60a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/logging-resource-api-cecf33e3be468eb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/mac-generator-f927df2fe57300c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/mechanism_driver_supported_extensions-67e1b0b763571ae9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/mechanismdriver-connectivity-00dc679a3f307345.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/migrate-public-to-shared-0c67b32f9c37c751.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/move-get-random-mac-98f47d81cb34483d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/move-segment-range-types-to-lib-constants-d45c6959607e9136.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/moved-netmtu-extension-5999348000adcfaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/network-ip-availability-pagging-support-cc01592cd477fd02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/network-segment-range-ext-2b93b7fa42310c25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/new-hacking-check-no-log-translations-4a430a38aeb06452.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/new-policy-module-f5638e23fe91a287.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/new-validator-range-or-none-dc8d557ec1f2622a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/new-vif-details-parameters-71e70ab5e7c26c45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/one-hacking-factory-01053e8e3d88c3d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/oslo-db-jitter-c4d13cc81755203e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-NoAuthClient-for-fullstack-tests-17b4ab512417d638.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-binding-exceptions-6362d52391b7023e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-bump-latest-supported-version-to-1-20-fe96751dab42399b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-bump-latest-supported-version-to-1-23-83589217b7b079fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-do-not-swallow-exceptions-c33c9a9224a27551.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-move-9f292ae2067c119c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-optional-rp-generations-44d1f1055d5496be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-return-f4f22d244e7b174a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-client-update-ensure-rp-9e5c3cf34d49b212.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-constants-f2629b98f6fe148f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-resource-provider-functions-17ec45f714ea2b23.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/placement-utils-a66e6b302d2bc8f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/plugin-directory-55861f4098813ba6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/policy-in-code-1e73cabebd41d66e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/policy-redux-25c26836219fd02d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/populate-dict-defaults-3f205c414f21bf54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-device-profile-ffa9628ef6395c68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-hint-ovs-tx-steering-cfa15582a74fb6a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-hints-8273fa5b7454a8ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-mac-address-regenerate-cc33d03216b5bc3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-mac-sanitization-d2b6ee77b66cb815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-numa-affinity-policy-9e6d1bafd3c6af36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-range-compared-as-int-4d07fe030206f818.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-resource-request-cb520720cd19523b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/port-resource-request-groups-d4a01b55d5fe5fa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/portbindings-apidef-3d7893bcb94d7f61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/portbindings-extended-3a89560ee63824e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/propagate_uplink_status_defaults_to_true-07dcdc20f20db594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/provider-net-apidef-9ebe9f56840c79f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/public-service-classes-e52d7c79a075b799.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/public-sql-fixtures-35d0aa74a368e217.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-bw-minimum-ingress-cff397e598b6fa3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-dscp-mark-44-56934a357af4b1ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-fip-network-policy-ded58703313ae248.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-plugin-parent-resource-mapping-ab5208caba9eda01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-port-network-policy-c64c57cf2ccec725.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-pps-minimum-1f9a5433d7d4fecd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-pps-minimum-rule-alias-2d0e711bde2aa1e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-rule-type-filter-dbac0ec80ce342f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-rules-alias-ext-c13417dcb3d81130.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/qos-rules-alias-ext-fix-3f3f7dd21837cfec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/quota-driver-api-get-workers-f540a81235dbf48d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-address-scope-apidef-f4e8bb74be61729a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-agent-apidef-7a2dde6a9810f55c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-allowedaddrpairs-apidef-cd342b9a57a2dfdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-api-faults-cf30246e5e5bf8b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-autotopology-apidef-4a77e8ba0c783f7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-az-apidef-1e63cbd2359994fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-common-constants-52f39a79e8eabd7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-common-constants-8ac9580e52fd3618.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-common-exceptions-eda074ddb02349ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-common-rpc-5d84a9fe0faa71b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-core-api-defs-390735ff3bd5d2ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-db-api-63300ddab6a41e28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-db-api-event-listeners-2fb5256166e2a4e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-db-model-query-234b1559f3728a5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-db-utils-3076bf724caa31ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dftsnetpool-apidef-4de5d75d2a63dec9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dhcp-table-constants-779598680f803e2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dhcpagentscheduler-apidef-1f7729fb5834dcd2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dhcpopts-apidef-389ab9d8935e5e0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dvr-apidef-a6aa415152457c9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dvr-related-leftover-constants-2cf329794166b3f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-dynamic-routing-apidef-3d78ae209ec59858.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-externalnet-apidef-d377f87da900eabe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-extraroute-apidef-e14e72e03ce18ead.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-flavors-apidef-ef84b2c1c7eaeed7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-get-port-binding-98765e77c627e57d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-get-updatable-fields-82fd87d402d63ca2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-getphysmtu-plugin-fn-5875e352e3a14af3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ipalloc-apidef-dee59cfffd903b7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ipv6pdprefix-const-d3b39992df4adef8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-l2adjacency-apidef-f91bf184d90122c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-l3extgwmode-apidef-8f83e0f6cf0515e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-l3exthamode-apidef-9b3ef0956edb3883.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-l3flavors-apidef-da5e9b5d46df5cc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-linuxinterfacedriver-874c5e17f2675eab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-metering-apidef-d9a0e70cbecc2bcc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ml2-api-extaliases-4db48e113893c7a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ml2-driverapi-363db4b8fa42f8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ml2-mechdriver-cc86d3a2fe4c2822.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-modelquery-2079a43163def870.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-multiprovidernet-apidef-367e57772e931758.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-netaz-apidef-74e962ef682380bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-netipavail-apidef-d03558ac48b71333.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-numaaffinitypoliciesenumfield-e1e2e8bfe4df4153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-obj-commontypes-f8dfca432bf4583b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-obj-logeventtypes-b31e7c6492ca6615.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-obj-stdattrs-06c4df5bb1fca3f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ovo-exceptions-fbddfeea582ef3f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ovs-constants-3a11c9ad0d44132a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-ovs-firewall-constants-522a307ff8ef4a78.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-pagination-apidef-9aebf1c7a6bcb58b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-placement-api-client-a9ac5d96ca8570aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-plugin-constants-ebf350dfd989957a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-plugin-utils-39e3f839c0538de9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-plugin-utils-create-fns-9b8591f5222bff66.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-port-dev-util-ea6f4a5c4da42f6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-projid-apidef-a433b1b003f27a20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-provider-network-attribute-updates-supported-ea02a526ef297053.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-psec-apidef-bd9344ec1e6066b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qos-apidef-0dbe094b8b21a580.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qos-driverbase-f729875b2ad74ce0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qos-fip-apidef-a2e4d49af177be85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qosbwldir-apidef-f0e3f778f2f980c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qosdft-apidef-b70596ca11c08803.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-qosrtdetails-apidef-2276ec66a0e545ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-rbac-policy-callbacks-24fa12ad1ab4c443.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-resource-extend-7eee483ec4146801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-revisionifmatch-apidef-574ac0a930cdaf3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-routeraz-apidef-efc5f202e04b8272.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-routersvctype-apidef-1d9d712fd5383eb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-runtime-utils-acb4451326cbe4d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-secgrp-portfilter-apidef-6723062419531d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-segment-apidef-a5f81adb834328f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-shared-const-d847b2e190122425.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-sorting-apidef-1547f093da322c14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-sqlalchemytypes-14817eb6694463db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-stdattr-d834900d3fd3c2e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-subnetservicetypes-apidef-31e2e9564c746317.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-svctype-apidef-9002b2e2bcbeec8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-testools-6fba053249e14d42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-timecost-90dcfc8c7f7280f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-topics-ca451e72c8c9603a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-trunk-callback-resources-be40f8382490ef0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-trunk-consts-407e4590e9386d19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-unstable-test-decorator-a062301ac7d7a082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-vlantransp-apidef-1cd7d3ace9042686.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome-worker-b7e9c7f477bdb926.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rehome_taas_apidef-5fb00d84da32b958.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-ensure_dir-aed59b616e02a2bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-hacking-check-n523-014d163a5ae23adb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-neutron-interconnection-api-definition-4ff88c583f2fe47b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-neutron-lib-from-db-profiling-38436898d8e45b37.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-registry-notify-76a2f6eb6bbf41bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove-resource-classes-constants-81f01eaed9ac463d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/remove_label-801d7a1b13f179fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/reset-db-retry-settings-49e51cef4c842f69.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/resource-provider-uuid5-namespace-f7276ba1945ce82f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/responsible_for_ports_allocation-5599dc59b3c98db2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/revert-review-400408-4999a9159689c0c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rm-apiutils-fa30241be7ca5162.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/rm-dup-pluginconst-085d0fcee4e931b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/routed-networks-hostroutes-fb43abf942b154ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/router-interface-fip-1e79b7909f8b264f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/separate-hacking-factories-6fc36b38de95662a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/service-plugin-base-a42c2241a2fe0d26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/setproctitle_for_workers-e8805fcaf34026ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/sfc-api-def-4f46632eadfe895a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/sqlalchemy-1-3-0-b0a2b15b10ae526f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/sqlalchemy-2.0-c794885886a62fa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/stateful-security-group-a1ece5472f029dc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/std_attributes_bgpvpn-5a1c63f68d1ff6be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subnet-dns-publish-fixed-ip-031d78bbc85a419e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subnet-onboard-allow-create-update-subnets-74a4be6e9e97bbb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subnet-onboard-api-definition-f4918ff1f1d12c97.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subnet_segment_id_policy_enforce-cd8053c51417d373.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subnet_segmentid_writable-e28a85033272f05d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/subresource-update-attrmap-and-classmethods-76accdd5c56a3bd4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/support-custom-filter-f4a15bb5b38b7d3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/support-rarp-protocol-44f5c67784e74db4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/tag-ports-during-bulk-creation-ext-3dd2e68d99157a19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/traffic-control-constants-b8120d1bea0681bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/transaction_constraint-d3f93c2ced4a74c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/trunk-api-08bfdcdd80f7e666.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/update-hacking-check-n536-2f63898bea693125.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/update-segment-api-definition-d7297e73e76a754c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/update-subnet-onboard-api-267a9a37f6426d64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/validator_check_route_loopback-bc2166b10a754c77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/validator_ip_or_subnet_or_none-0175f906a9113954.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/vhost-vdpa-cc35f8d0ff9b3c4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/vnic-accelerator-eaf9b583d60e76ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/vnic-type-remote-managed-c0809926fcd30e93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/vnic-type-smart-nic-45dd5a22a9d1aa63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/notes/vpn-api-def-52970461fac0f7d2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9132 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.720768 neutron-lib-3.5.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:54.720768 neutron-lib-3.5.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2023-04-13 10:18:55.052769 neutron-lib-3.5.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-13 10:18:55.048769 neutron-lib-3.5.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tools/api_report.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      835 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tools/check_samples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1379 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1203 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tools/migration_report.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    46254 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tools/pyir.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4151 2023-04-13 10:18:27.000000 neutron-lib-3.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8271 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49722 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      663 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.595515 neutron-lib-3.6.0/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.603515 neutron-lib-3.6.0/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6867 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.611515 neutron-lib-3.6.0/api-ref/source/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6686 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/address-groups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4827 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/address-scopes.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/agents.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/auto-topology.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/availability_zones.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgp_dragent_scheduler.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgp_peer.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9537 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgp_speaker.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6129 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-bgpvpns.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-network_associations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6246 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-overview.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-port_associations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5836 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-router_associations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/dhcp-agent-scheduler.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/extensions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7735 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/fip-port-forwarding.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/fip64.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/firewall_log.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13258 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/flavors.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/floatingippools.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13621 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/floatingips.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25886 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/fwaas-v2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19876 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/intro.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/l3-agent-scheduler.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5172 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/l3-conntrack-helper.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10752 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/local-ips.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/logging.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/logging_resource.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9255 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/metering.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/network-ip-availability.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8316 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/network_segment_ranges.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22107 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/networks.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   188397 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29739 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/ports.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37090 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/qos.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/quota_details.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4595 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/quotas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5064 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/rbac-policy.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/router-interface-fip.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5775 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/router-ndp-proxy.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33304 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/routers.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.611515 neutron-lib-3.6.0/api-ref/source/v2/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.611515 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-add-addresses-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-add-addresses-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-remove-addresses-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-remove-addresses-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-groups/address-groups-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.611515 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scope-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scope-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scope-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scope-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scope-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scopes-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.611515 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-dhcp-network-add-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-dhcp-networks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-l3-router-add-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-l3-router-remove-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-l3-routers-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4574 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agents-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/network-dhcp-agent-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/agents/router-l3-agent-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.615516 neutron-lib-3.6.0/api-ref/source/v2/samples/auto-topology/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/auto-topology/topo-show-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.615516 neutron-lib-3.6.0/api-ref/source/v2/samples/availability-zones/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/availability-zones/azs-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.615516 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_peer-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_peer-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_peer-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_peer-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_network-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_network-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_peer-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_add_peer-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_dragent_host-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_routes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_remove_network-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_remove_peer-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/dragent_add_speaker-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/dragent_list_agents_hosting_speaker-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/dragent_list_speakers-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.595515 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.615516 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpns-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.619516 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/network_associations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/network_associations/network_association-show-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.619516 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/port_associations/port_association-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.619516 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/router_associations/router_association-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.619516 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/conntrack_helpers/conntrack-helper-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.619516 neutron-lib-3.6.0/api-ref/source/v2/samples/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/extensions/extension-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4352 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/extensions/extensions-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.623515 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-groups-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-insert-rule-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-insert-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-remove-rule-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-remove-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-policy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rules-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.623515 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_log-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_log-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_log-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_log-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_log-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_logs-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.627516 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-insert-rule-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-insert-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-remove-rule-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-remove-rule-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-policy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewalls-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.627516 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-associate-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-associate-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavor-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/flavors-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profile-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profile-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profile-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profile-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profile-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profiles-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.631516 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floating-ip-pools-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4078 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floating-ips-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.631516 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local-ip-list-associations-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local-ips-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip_association-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip_association-create-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.631516 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resources-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.631516 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/logs/loggable_resources-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.631516 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-delete-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-delete-response-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-delete-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-delete-response-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-show-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rules-list-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-show-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-labels-list-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-labels-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.635516 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxy-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.635516 neutron-lib-3.6.0/api-ref/source/v2/samples/network-ip-availability/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-list.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-show.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.635516 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1699 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_ranges-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.635516 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1419 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1164 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-bulk-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-bulk-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2232 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3058 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-provider-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/version-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/networks/versions-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.635516 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.639515 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-add-allowed-address-pairs-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-add-allowed-address-pairs-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3237 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2791 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1796 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-remove-allowed-address-pairs-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-remove-allowed-address-pairs-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-resource-request-new-format.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4725 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-bind-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-bulk-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-bulk-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3539 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.639515 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/bandwidth_limit_rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/dscp_marking_rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_bandwidth_rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/minimum_packet_rate_rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rule-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/packet_rate_limit_rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/rule_type-details-bandwidth_limit-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/rule_type-details-dscp_marking-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/qos/rule_types-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.639515 neutron-lib-3.6.0/api-ref/source/v2/samples/quota_details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/quota_details/quota-details-show-for-project-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.643516 neutron-lib-3.6.0/api-ref/source/v2/samples/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/quotas/quotas-list-for-project-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/quotas/quotas-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/quotas/quotas-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/quotas/quotas-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.643516 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/rbac_policy/rbac-policy-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.643516 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-external-gateways-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-external-gateways-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-extraroutes-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-extraroutes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-interface-request-with-port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-interface-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-add-interface-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-external-gateways-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1969 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-external-gateways-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-extraroutes-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-extraroutes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-interface-request-with-port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-interface-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-remove-interface-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-external-gateways-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-external-gateways-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3586 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/routers/routers-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.647516 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-delete-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-delete-response-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-delete-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-delete-response-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2845 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-show-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3745 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-groups-list-request-json-http.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-groups-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.647516 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segment-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segment-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segment-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segment-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segment-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segments-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/service-type-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.647516 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-add-prefixes-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-add-prefixes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-remove-prefixes-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-remove-prefixes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1676 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpools-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnets-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.647516 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/taf-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/taas/tas-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.647516 neutron-lib-3.6.0/api-ref/source/v2/samples/tag/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/tag/tag-obtain-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/tag/tag-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/tag/tag-update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.651516 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-add-subports-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-add-subports-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-details-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-list-subports-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-remove-subports-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-remove-subports-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunks-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunks-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.651516 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      600 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1034 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connections-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-groups-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservices-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5863 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/security-group-rules.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8605 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/security-groups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/segments.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/service-providers.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1669 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/subnetpool_prefix_ops.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8016 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/subnetpools.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16497 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/subnets.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/taas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3459 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/trunk-details.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10324 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/trunk.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30735 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/api-ref/source/v2/vpnaas.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.651516 neutron-lib-3.6.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.651516 neutron-lib-3.6.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7519 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4637 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/api_attributes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/api_converters.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/api_extensions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3468 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/api_validators.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25986 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/callbacks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1747 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/consuming.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6006 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/conventions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/db_model_query.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/internals.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/releasing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3871 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/review-guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5407 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/contributor/rpc_api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/user/hacking.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/neutron_lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/neutron_lib/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/neutron_lib/agent/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1989 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/l2_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1988 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/l3_extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.659516 neutron-lib-3.6.0/neutron_lib/agent/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/linux/interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2266 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/agent/topics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.659516 neutron-lib-3.6.0/neutron_lib/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/attributes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12708 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/converters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.675516 neutron-lib-3.6.0/neutron_lib/api/definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12639 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/_dummy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3214 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/address_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3800 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/agent_resources_synced.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/agent_sort_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/allowedaddresspairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/allowedaddresspairs_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2069 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/availability_zone_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5007 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgp_4byte_asn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgp_dragentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8213 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5626 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_routes_control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_net_assoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_port_assoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_router_assoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2774 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_vni.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/data_plane_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1610 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/default_subnetpools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/dhcpagentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/dns_domain_keywords.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/dns_domain_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/ecmp_routes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/empty_string_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/expose_l3_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/expose_port_forwarding_in_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/external_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/extra_dhcp_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/extraroute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/extraroute_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/filter_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip_distributed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_description.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_detail.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_port_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1283 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/fip_port_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10326 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/firewall_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/firewall_v2_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6221 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5143 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/floating_ip_port_forwarding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/floatingip_autodelete_internal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2071 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/floatingip_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/flowclassifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/ip_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1795 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/ip_substring_port_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1334 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l2_adjacency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7216 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_enable_default_route_bfd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_enable_default_route_ecmp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_gw_mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_gw_multihoming.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_ha_mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4418 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/l3_port_ip_change_not_allowed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/logging_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3986 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/metering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2101 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/metering_source_and_destination_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2614 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/multiprovidernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_cascade_delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_ha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2684 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_mtu_writable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5805 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/network_segment_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/pagination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4610 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_hint_ovs_tx_steering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_hints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_mac_address_override.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_mac_address_regenerate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_numa_affinity_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_resource_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_resource_request_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3004 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/port_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9310 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/portbindings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4331 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/portbindings_extended.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/project_default_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/project_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4011 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/provider_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6023 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1869 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_bw_limit_direction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_bw_minimum_ingress.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_fip_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_gateway_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_port_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2337 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_minimum_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_minimum_rule_alias.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1330 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rule_type_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rule_type_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4363 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rules_alias.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/quota_check_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_address_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/revisionifmatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/router_admin_state_down_before_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/router_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/router_interface_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1352 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/routerservicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_normalized_cidr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1800 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_port_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_remote_address_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_shared_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4049 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/segment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/segments_peer_subnet_host_routes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/servicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9536 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/sort_key_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/sorting.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/standard_attr_segment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/stateful_security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6714 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_dns_publish_fixed_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_onboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_segmentid_enforce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2583 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_segmentid_writable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_service_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5028 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/subnetpool_prefix_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/tag_ports_during_bulk_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/trunk_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/uplink_status_propagation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/vlan_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/vlantransparent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16736 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/vpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2802 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/vpn_endpoint_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/definitions/vpn_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9771 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/faults.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.675516 neutron-lib-3.6.0/neutron_lib/api/validators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50203 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/validators/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/validators/allowedaddresspairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/validators/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7622 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/validators/dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/api/validators/multiprovidernet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.675516 neutron-lib-3.6.0/neutron_lib/callbacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5489 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8882 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/priority_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/callbacks/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23549 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7057 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.675516 neutron-lib-3.6.0/neutron_lib/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18077 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3962 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/model_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15590 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/model_query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7409 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/quota_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5582 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/resource_extend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2913 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/sqlalchemytypes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10604 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/standard_attr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27488 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/address_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/allowedaddresspairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/dhcpagentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/external_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/extraroute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6276 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/firewall_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1938 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/l3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/l3_ext_gw_multihoming.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1736 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/l3_ext_ha_mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/metering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/multiprovidernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/network_segment_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/placement.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/port_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4401 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/vlantransparent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6509 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/exceptions/vpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14371 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8160 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3577 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/hacking/translation_checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.599515 neutron-lib-3.6.0/neutron_lib/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.599515 neutron-lib-3.6.0/neutron_lib/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43266 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/locale/zh_CN/LC_MESSAGES/neutron_lib.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12869 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/common_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3072 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/objects/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/extensions/standardattributes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/objects/logapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/logapi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/logapi/event_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1926 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2575 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/objects/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/placement/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/placement/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35293 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/placement/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/placement/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13632 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/placement/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/directory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/plugins/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47814 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/ml2/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6449 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/ml2/ovs_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15070 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/plugins/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/policy/_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12972 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/services/logapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/logapi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/logapi/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/services/qos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/qos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7165 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/qos/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2280 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/qos/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/services/trunk/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/trunk/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/services/trunk/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.679516 neutron-lib-3.6.0/neutron_lib/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8340 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4237 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/_post_mortem_debug.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/etc/dummy_policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/etc/neutron_lib.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        4 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/etc/no_policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/etc/policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/tools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/agent/linux/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.683516 neutron-lib-3.6.0/neutron_lib/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.699516 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9764 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/ip_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test__dummy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_address_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_admin_state_down_before_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent_resources_synced.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent_sort_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_auto_allocated_topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_availability_zone_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp_4byte_asn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp_dragentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_net_assoc_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_port_assoc_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_router_assoc_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_routes_control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_vni.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_data_plane_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_default_subnetpools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dhcpagentscheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dns_domain_ports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dvr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_empty_string_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_expose_l3_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_expose_port_forwarding_in_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_external_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extra_dhcp_opt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extraroute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extraroute_atomic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_filter_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip_distributed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip_port_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_firewall_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_firewall_v2_stdattrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_port_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floatingip_autodelete_internal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floatingip_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_flowclassifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_ip_substring_port_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l2_adjancency.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_conntrack_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_enable_default_route_bfd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_enable_default_route_ecmp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_gw_mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ha_mode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_multi_ext_gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ndp_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_port_ip_change_not_allowed.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_local_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1217 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_logging_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_metering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_metering_source_and_destination_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2074 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_multiprovidernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_cascade_delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_ip_availability.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_mtu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_mtu_writable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_segment_range.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_pagination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_device_profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_hint_ovs_tx_steering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_hints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_mac_address_regenerate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_numa_affinity_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      843 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_portbindings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_portbindings_extended.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_project_default_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_project_id.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_provider_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1258 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_limit_direction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_minimum_ingress.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_fip_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_gateway_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_port_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule_alias.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1116 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rules_alias.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_quota_check_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_scope.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_bgpvpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_revisionifmatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_router_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_router_interface_fip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_routerservicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_normalized_cidr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_port_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_remote_address_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_shared_filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_segment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_segment_peer_subnet_host_routes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_servicetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sort_key_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sorting.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_standard_attr_segment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_stateful_security_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_dns_publish_fixed_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_onboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_enforce.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_writable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_service_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnetpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnetpool_prefix_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_taas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_tag_ports_during_bulk_creation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_trunk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_trunk_details.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_uplink_status_propagation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vlan_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vlantransparent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn_endpoint_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13717 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_attributes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16450 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_conversions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8283 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_faults.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.699516 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4046 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_allowedaddresspairs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6835 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_dns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1918 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_multiprovidernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57538 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.699516 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_callback_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4222 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16985 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6123 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_registry.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.699516 neutron-lib-3.6.0/neutron_lib/tests/unit/clients/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/clients/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8718 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_model_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_model_query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_resource_extend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9414 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_sqlalchemytypes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4261 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_standard_attr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5603 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/exceptions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/exceptions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10579 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/exceptions/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/fake_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8681 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/hacking/test_checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/legacy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/legacy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14628 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/objects/test_common_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/objects/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/placement/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/placement/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38627 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/placement/test_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13448 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/placement/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/ml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/ml2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/ml2/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3509 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/test_directory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11954 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/policy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/policy/test__engine.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/services/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/services/qos/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/services/qos/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/services/qos/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2587 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/services/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10923 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/test_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/test_neutron_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19828 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/test_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5070 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/test_worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.703516 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7911 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3773 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4710 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_runtime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.707516 neutron-lib-3.6.0/neutron_lib/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1468 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/file.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6928 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3985 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5052 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/runtime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/utils/upgrade_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/neutron_lib/worker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.655516 neutron-lib-3.6.0/neutron_lib.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    80493 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-05-11 08:57:32.000000 neutron-lib-3.6.0/neutron_lib.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.599515 neutron-lib-3.6.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.735516 neutron-lib-3.6.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Add-new-dns_domain_keywords-api-extension-436c2c3a091d15eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Add-oneline-string-validator-aa4e1ccad9d8d5c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Adds-PORT_FORWARDING_FLOATINGIP_KEY-ee2c7d164bea04b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Move-RBAC-share-actions-to-lib-constants-736d881f127c83d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Rehome-missing-ovs-constants-c398aa6462c9eb5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/Rehome-ovs-constants-to-separate-module-07ce93971dd1d7dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-a-getter-for-a-newly-added-option-2082877bf7dd136b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-action-status-3dbfe2490a0d231a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-api-extension-sort-key-validation-b42f5839671fe5f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-availability_zone_filter-extension-e91e1e5e822e4133.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-base-upgrade-checks-class-f6da1d501663d8c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-broadcast-mac-constant-ec00b18a883bf875.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-can-port-be-bound-to-virtual-bridge-5d6db8785e58fcb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-convert-to-string-524541aa6224f66f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-description-field-in-port-forwarding-9da781b1e38ca858.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-directory-is-loaded-e9da5b65824dddad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-empty-string-filtering-api-extension-44cb392025dc359c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-exception-pkg-5a14389891abf358.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-address-group-5e306d90666982aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-security-groups-normalized-cidr-ef7521b226090d7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-security-groups-remote-address-group-c71dbb57b61a1dba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-standard-attr-fwaasv2-7e9250015afbe112.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-standard-attr-segment-8c721741589bf10b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-supported-be6f7069856d2891.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-extension-uplink-status-propagation-6b6050d6609c19c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-filter-validation-api-extension-15cc667d5498f163.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-fip-distributed-extension-ce44e8df264d44b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-fip-pf-detail-extension-fa8cd3b3857901d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-floatingip-pools-extension-17a1ee5c7eafc989.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-ip-hopopt-to-protocol-dictionary-3cbe54bb5056f790.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-ip-substring-filtering-extension-06bb0c1f738ee330.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-ipinip-protocol-ab9287f9b698f34c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-is-default-to-network-d16a2e6bcfae943a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-is_filter-keyword-to-attribute-maps-3fa31e91c353d033.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-is_sort_key-keyword-to-attribute-map-75342446d99f4490.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-local-ip-extension-fb4a18f5a6525f1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-network-address-scope-affinity-error-8f6b4493a92142d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-network-cascade-delete-api-extension-f418e44b37c2b2ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-network-segment-range-overlap-exception-e8b4b2b425c51c80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-network-segment-range-plugin-constant-9e80453919162c89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-ovo-registry-27cb7d4ac76d4dc8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-ovs-port-type-dpdk-b00f5bda3161773f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-placement-report-plugin-constant-a6a4146c2e39cba3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-port-binding-resource-73f9800dbda121ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-port-bindings-resource-messages-rpc-1382ba9842561cdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-port-mac-address-override-shim-extension-fb11c4f40c12a99b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-port-ranges-support-in-port-forwarding-417da8ef7e2ec140.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-port_details-to-floatingip-a2a3c95cc54737ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-quota-check-limit-api-extension-8e39299644d41f74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-rbac-address-group-39c22aeb30241b11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-rbac-address-scope-dc4683772b205632.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-rbac-bgpvpn-cf6c9346822268f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-rbac-security-groups-2e47acd9eac3a320.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-rbac-subnetpool-bb63d4cef1d06e73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-retrieve-sort-keys-from-attribute-map-ae53d67e0be2ace0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-router-not-found-in-factory-exception-e2bf9431549ff9b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-sg-shared-filtering-api-extension-6c3628cfda6ba6ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-support-for-fetching-specific-column-in-OVO-81b764b203849776.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-traffic-control-exceptions-0e137dae3a556d54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-two-fields-to-duplicated-entry-exception-75b0e07c6e1cc6ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-type-driver-methods-for-network-segment-range-e6d300d430d97dd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-validate-cidr-848c9171dcbcf57c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-validator-pkg-a6565a2d4fbfa1d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-vif-type-agilio-ovs-6bee5b2557aca10e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-vni-to-bgpvpn-7531df9fa4f8955b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add-vnic-virtio-forwarder-portbinding-f7f87dfbef456ed1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add_QuotaDriverAPI_abc_class-1d02d0823a8886a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      372 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add_fwg_group-9252d07f1011613d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/add_qos_pps_rule_api_def-dae7c6e67904781b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/admin-state-down-before-update-c06fb3a551fe499f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/advsvc-role-support-d4f1c532264b729a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/agent-resources-synced-e70828841faf7acd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/agent_extensions-2b497ff33c6dc3e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/alembic-branches-6d5947d141efd26e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/allocations_api-1ae5fd78c83353df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/allowedaddresspairs-atomic-apidef-6f9d6865854vwfrs
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/api-definition-base-d2e9514c5ee2ef5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bgpvpn-api-def-22c7072575316ddd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bgpvpn-api-ref-f0294d9ddec726a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bgpvpn-routes-control-51cd95d6ab265cb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bgpvpn_rt_fix-6d02db6a1c22f002.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/boilerplate-ext-descriptor-a5cec8b9b900cbfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bug-1877254-2b997b3911e98079.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bug-1921150-a38bef3c1be69650.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/bug-1957175-6b2705d4772df7de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/callback_priority-2ded960e17bd5db9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/change_placement_client_method_names_b26bb71425f42db3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/cidr_for_canonical_format-4e7925d76a27a19d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/cleanup-unused-l3-attr-def-f0eab40813d17a2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/client-id-number-dhcp-option-a099f927eb8f99af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/conntrack-helper-parent-resource-mapping-95a4a2cb6f6536fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/context-manager-23538670cd9c701f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/context-public-6df198b77027c224.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/core-attributes-43e6969f1b187e5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/correct-dhcp-ipv4-port-numbers-6e22c6aa26009cdc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/create-netmtu-writable-extension-284892119ef6595c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/data-plane-status-ext-c3452a01ef5007ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/default_overrides_none-ecc8dcf2c9c37e5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/deprecate-api-utils-4f86288591c95679.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/deprecate-remote_ip_prefix-in-metering-label-rules-308b3d430bc213b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/directory-fixture-083c5c5f365670d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/disable-port-number-zero-2fb484a802f099a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/dns-api-def-bc24a58f56c5fbfb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/dns-domain-ports-ext-39a069119e79e59b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/drop-python-2-7-f46dfa10169f70db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/drop-python-3-6-and-3-7-daba9483fa3d9b3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/enable-hacking-check-H904-f512ecc98c0a4033.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/ethertype_validator-2d608a46c237e214.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/events_l3_flavors-053714858ced693d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/expose-and-enhance-callback-api-714cce65a3c44fe7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/expose-port-forwarding-in-fip-a7880506cea0ad1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extend-segment-methods-with-filters-6e74953ae2d3b828.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extension-fixture-b7fd61384f1a4d1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extension_descriptor-04025e86249cc94c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extra-dhcp-opt-public-vars-ec4e1c2dcac43d69.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extraroute-atomic-apidef-80a7c6d4a773c701.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/extraroute-atomic-apidef-additive-fb783d66c08618d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fip64-0c6bb38417d602f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fix-api-list-validation-collect-duplicates-f4d45bf5d5abbdff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fix-warnfixture-c9457c50d0d5c5a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/floatingip-autodelete-internal-dep-8e544fad694d1275.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/floatingip-autodelete-internal-f08675d8d64d34c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/floatingip-portforwarding-17c284080541bc78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/flush_on_subtransaction-99ef11dfb56b706d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fwaas-api-def-a6f03db369177b4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fwaas-exceptions-e580766205b466d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/fwaas_converters_validators-c310900b4386146e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/gateway-ip-qos-ext-d3ffb5f517c9f713.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/hacking-check-n537-280ec39c061d9dd7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/interconnection-api-def-cbec5e4f77852fe7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/introduce-logging-api-031d00eb84d5d061.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/introduce-source-and-destination-ip-prefixes-into-metering-label-rules-3d62fccbca8e67b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/introduce_subnetpool_prefix_ops_extension-e37874c936d2554c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/ipv6-canonical-address-13900a784f847ce3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/ipv6_address_usage-ef3d65ad5aa5798b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-agent-extensions-ha-state-change-837140efe4187a99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-agent-extensions-update-network-e4887f7f258e40f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-apidef-exceptions-ee57b9df1c7443d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-apidefs-d028c708c22ef2a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-conntrack-helper-validator-654ccafb296e5f21.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-ext-gw-multihoming-1a7b556c541923cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-ndp-proxy-71eee0cba8565dad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-port-ip-change-not-allow-2c98e13c08b5ee85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3-support-ecmp-91a8aa61e3a73037.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/l3_conntrack_helper-f186bcdcc31bcaf2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/logging-api-ref-fafb884367ca60a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/logging-resource-api-cecf33e3be468eb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/mac-generator-f927df2fe57300c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/mechanism_driver_supported_extensions-67e1b0b763571ae9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/mechanismdriver-connectivity-00dc679a3f307345.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/migrate-public-to-shared-0c67b32f9c37c751.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/move-get-random-mac-98f47d81cb34483d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/move-segment-range-types-to-lib-constants-d45c6959607e9136.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/moved-netmtu-extension-5999348000adcfaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/network-ha-e6e0c3202b084762.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/network-ip-availability-pagging-support-cc01592cd477fd02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/network-segment-range-ext-2b93b7fa42310c25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/new-hacking-check-no-log-translations-4a430a38aeb06452.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/new-policy-module-f5638e23fe91a287.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/new-validator-range-or-none-dc8d557ec1f2622a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/new-vif-details-parameters-71e70ab5e7c26c45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/one-hacking-factory-01053e8e3d88c3d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/oslo-db-jitter-c4d13cc81755203e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-NoAuthClient-for-fullstack-tests-17b4ab512417d638.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-binding-exceptions-6362d52391b7023e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-bump-latest-supported-version-to-1-20-fe96751dab42399b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-bump-latest-supported-version-to-1-23-83589217b7b079fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-do-not-swallow-exceptions-c33c9a9224a27551.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-move-9f292ae2067c119c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-optional-rp-generations-44d1f1055d5496be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-return-f4f22d244e7b174a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-client-update-ensure-rp-9e5c3cf34d49b212.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-constants-f2629b98f6fe148f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-resource-provider-functions-17ec45f714ea2b23.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/placement-utils-a66e6b302d2bc8f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/plugin-directory-55861f4098813ba6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/policy-in-code-1e73cabebd41d66e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/policy-redux-25c26836219fd02d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/populate-dict-defaults-3f205c414f21bf54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-device-profile-ffa9628ef6395c68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-hint-ovs-tx-steering-cfa15582a74fb6a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-hints-8273fa5b7454a8ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-mac-address-regenerate-cc33d03216b5bc3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-mac-sanitization-d2b6ee77b66cb815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-numa-affinity-policy-9e6d1bafd3c6af36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-range-compared-as-int-4d07fe030206f818.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-resource-request-cb520720cd19523b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/port-resource-request-groups-d4a01b55d5fe5fa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/portbindings-apidef-3d7893bcb94d7f61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/portbindings-extended-3a89560ee63824e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/propagate_uplink_status_defaults_to_true-07dcdc20f20db594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/provider-net-apidef-9ebe9f56840c79f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/public-service-classes-e52d7c79a075b799.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/public-sql-fixtures-35d0aa74a368e217.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-bw-minimum-ingress-cff397e598b6fa3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-dscp-mark-44-56934a357af4b1ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-fip-network-policy-ded58703313ae248.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-plugin-parent-resource-mapping-ab5208caba9eda01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-port-network-policy-c64c57cf2ccec725.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-pps-minimum-1f9a5433d7d4fecd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-pps-minimum-rule-alias-2d0e711bde2aa1e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-rule-type-filter-dbac0ec80ce342f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-rules-alias-ext-c13417dcb3d81130.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/qos-rules-alias-ext-fix-3f3f7dd21837cfec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/quota-driver-api-get-workers-f540a81235dbf48d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-address-scope-apidef-f4e8bb74be61729a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-agent-apidef-7a2dde6a9810f55c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-allowedaddrpairs-apidef-cd342b9a57a2dfdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-api-faults-cf30246e5e5bf8b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-autotopology-apidef-4a77e8ba0c783f7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-az-apidef-1e63cbd2359994fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-common-constants-52f39a79e8eabd7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-common-constants-8ac9580e52fd3618.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-common-exceptions-eda074ddb02349ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-common-rpc-5d84a9fe0faa71b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-core-api-defs-390735ff3bd5d2ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-db-api-63300ddab6a41e28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-db-api-event-listeners-2fb5256166e2a4e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-db-model-query-234b1559f3728a5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-db-utils-3076bf724caa31ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dftsnetpool-apidef-4de5d75d2a63dec9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dhcp-table-constants-779598680f803e2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dhcpagentscheduler-apidef-1f7729fb5834dcd2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dhcpopts-apidef-389ab9d8935e5e0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dvr-apidef-a6aa415152457c9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dvr-related-leftover-constants-2cf329794166b3f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-dynamic-routing-apidef-3d78ae209ec59858.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-externalnet-apidef-d377f87da900eabe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-extraroute-apidef-e14e72e03ce18ead.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-flavors-apidef-ef84b2c1c7eaeed7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-get-port-binding-98765e77c627e57d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-get-updatable-fields-82fd87d402d63ca2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-getphysmtu-plugin-fn-5875e352e3a14af3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ipalloc-apidef-dee59cfffd903b7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ipv6pdprefix-const-d3b39992df4adef8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-l2adjacency-apidef-f91bf184d90122c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-l3extgwmode-apidef-8f83e0f6cf0515e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-l3exthamode-apidef-9b3ef0956edb3883.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-l3flavors-apidef-da5e9b5d46df5cc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-linuxinterfacedriver-874c5e17f2675eab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-metering-apidef-d9a0e70cbecc2bcc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ml2-api-extaliases-4db48e113893c7a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ml2-driverapi-363db4b8fa42f8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ml2-mechdriver-cc86d3a2fe4c2822.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-modelquery-2079a43163def870.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-multiprovidernet-apidef-367e57772e931758.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-netaz-apidef-74e962ef682380bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-netipavail-apidef-d03558ac48b71333.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-numaaffinitypoliciesenumfield-e1e2e8bfe4df4153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-obj-commontypes-f8dfca432bf4583b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-obj-logeventtypes-b31e7c6492ca6615.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-obj-stdattrs-06c4df5bb1fca3f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ovo-exceptions-fbddfeea582ef3f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ovs-constants-3a11c9ad0d44132a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-ovs-firewall-constants-522a307ff8ef4a78.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-pagination-apidef-9aebf1c7a6bcb58b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-placement-api-client-a9ac5d96ca8570aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-plugin-constants-ebf350dfd989957a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-plugin-utils-39e3f839c0538de9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-plugin-utils-create-fns-9b8591f5222bff66.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-port-dev-util-ea6f4a5c4da42f6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-projid-apidef-a433b1b003f27a20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-provider-network-attribute-updates-supported-ea02a526ef297053.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-psec-apidef-bd9344ec1e6066b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qos-apidef-0dbe094b8b21a580.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qos-driverbase-f729875b2ad74ce0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qos-fip-apidef-a2e4d49af177be85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qosbwldir-apidef-f0e3f778f2f980c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qosdft-apidef-b70596ca11c08803.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-qosrtdetails-apidef-2276ec66a0e545ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-rbac-policy-callbacks-24fa12ad1ab4c443.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-resource-extend-7eee483ec4146801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-revisionifmatch-apidef-574ac0a930cdaf3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-routeraz-apidef-efc5f202e04b8272.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-routersvctype-apidef-1d9d712fd5383eb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-runtime-utils-acb4451326cbe4d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-secgrp-portfilter-apidef-6723062419531d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-segment-apidef-a5f81adb834328f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-shared-const-d847b2e190122425.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-sorting-apidef-1547f093da322c14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-sqlalchemytypes-14817eb6694463db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-stdattr-d834900d3fd3c2e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-subnetservicetypes-apidef-31e2e9564c746317.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-svctype-apidef-9002b2e2bcbeec8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-testools-6fba053249e14d42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-timecost-90dcfc8c7f7280f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-topics-ca451e72c8c9603a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-trunk-callback-resources-be40f8382490ef0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-trunk-consts-407e4590e9386d19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-unstable-test-decorator-a062301ac7d7a082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-vlantransp-apidef-1cd7d3ace9042686.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome-worker-b7e9c7f477bdb926.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rehome_taas_apidef-5fb00d84da32b958.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-ensure_dir-aed59b616e02a2bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-hacking-check-n523-014d163a5ae23adb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-neutron-interconnection-api-definition-4ff88c583f2fe47b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-neutron-lib-from-db-profiling-38436898d8e45b37.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-registry-notify-76a2f6eb6bbf41bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove-resource-classes-constants-81f01eaed9ac463d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/remove_label-801d7a1b13f179fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/reset-db-retry-settings-49e51cef4c842f69.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/resource-provider-uuid5-namespace-f7276ba1945ce82f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/responsible_for_ports_allocation-5599dc59b3c98db2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/revert-review-400408-4999a9159689c0c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rm-apiutils-fa30241be7ca5162.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/rm-dup-pluginconst-085d0fcee4e931b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/routed-networks-hostroutes-fb43abf942b154ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/router-interface-fip-1e79b7909f8b264f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/separate-hacking-factories-6fc36b38de95662a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/service-plugin-base-a42c2241a2fe0d26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/setproctitle_for_workers-e8805fcaf34026ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/sfc-api-def-4f46632eadfe895a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/sqlalchemy-1-3-0-b0a2b15b10ae526f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/sqlalchemy-2.0-c794885886a62fa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/stateful-security-group-a1ece5472f029dc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/std_attributes_bgpvpn-5a1c63f68d1ff6be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subnet-dns-publish-fixed-ip-031d78bbc85a419e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subnet-onboard-allow-create-update-subnets-74a4be6e9e97bbb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subnet-onboard-api-definition-f4918ff1f1d12c97.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subnet_segment_id_policy_enforce-cd8053c51417d373.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subnet_segmentid_writable-e28a85033272f05d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/subresource-update-attrmap-and-classmethods-76accdd5c56a3bd4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/support-custom-filter-f4a15bb5b38b7d3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/support-rarp-protocol-44f5c67784e74db4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/tag-ports-during-bulk-creation-ext-3dd2e68d99157a19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/traffic-control-constants-b8120d1bea0681bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/transaction_constraint-d3f93c2ced4a74c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/trunk-api-08bfdcdd80f7e666.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/update-hacking-check-n536-2f63898bea693125.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/update-segment-api-definition-d7297e73e76a754c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/update-subnet-onboard-api-267a9a37f6426d64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/validator_check_route_loopback-bc2166b10a754c77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/validator_ip_or_subnet_or_none-0175f906a9113954.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/vhost-vdpa-cc35f8d0ff9b3c4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/vnic-accelerator-eaf9b583d60e76ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/vnic-type-remote-managed-c0809926fcd30e93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/vnic-type-smart-nic-45dd5a22a9d1aa63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/notes/vpn-api-def-52970461fac0f7d2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9132 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.599515 neutron-lib-3.6.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.599515 neutron-lib-3.6.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 08:57:32.739516 neutron-lib-3.6.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2683 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tools/api_report.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      835 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tools/check_samples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1379 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1203 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tools/migration_report.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    46254 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tools/pyir.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4151 2023-05-11 08:57:05.000000 neutron-lib-3.6.0/tox.ini
```

### Comparing `neutron-lib-3.5.0/.pylintrc` & `neutron-lib-3.6.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/.zuul.yaml` & `neutron-lib-3.6.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/AUTHORS` & `neutron-lib-3.6.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 Nate Johnston <nate_johnston@cable.comcast.com>
 Ngo Quoc Cuong <cuongnq@vn.fujitsu.com>
 Nguyen Hai Truong <truongnh@vn.fujitsu.com>
 Nguyen Phuong An <AnNP@vn.fujitsu.com>
 Nurmatov Mamatisa <nurmatov.mamatisa@huawei.com>
 Oleg Bondarev <obondarev@mirantis.com>
 Oleg Bondarev <oleg.bondarev@huawei.com>
+Oleksii Butenko <obu-plv@napatech.comm>
 Omer Anson <omer.anson@toganetworks.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Pablo Iranzo Gómez <Pablo.Iranzo@redhat.com>
 Paul Carver <pcarver@att.com>
 Paul Michali <pc@michali.net>
 Pavel Gluschak <trustytwelve@gmail.com>
 Pawel Suder <pawel@suder.info>
@@ -179,14 +180,15 @@
 gugug <gu.jin@99cloud.net>
 huangtianhua <huangtianhua@huawei.com>
 kpdev <kinpaa@gmail.com>
 leiyashuai <leiyashuai@inspur.com>
 lidong <lidongbj@inspur.com>
 lijunjie <lijunjie@cloudin.cn>
 lilintan <lintan.li@easystack.cn>
+liushy <liuxie_11@163.com>
 longqianzhao <longqian.zhao@intel.com>
 maliangyi <maliangyi@inspur.com>
 melissaml <ma.lei@99cloud.net>
 nanaboat <prince.a.owusu.boateng@intel.com>
 nicky <qi.ni@intel.com>
 nizam <abdul.nizamuddin@nectechnologies.in>
 pandatt <guojy8993@163.com>
```

### Comparing `neutron-lib-3.5.0/CONTRIBUTING.rst` & `neutron-lib-3.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/ChangeLog` & `neutron-lib-3.6.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+3.6.0
+-----
+
+* New \`\`network-ha\`\` API definition
+* Remove an unused exception
+* DPDK datapath type added
+* Add a shim extension standard-attr-fwaas-v2
+* port-hint-ovs-tx-steering: Add missing api-ref response sample
+* Drop "\_\_autocommit=False" from context manager
+* New api-def: allowedaddresspairs-atomic
+* ext-gw-multihoming: api-def and api-ref
+* doc: Remove fwaas v2 deprecation message
+* FUP Suppress IPv6 metadata DAD failure and delete address
+
 3.5.0
 -----
 
 * Return properly elevated context by get\_admin\_context() helper
 * port-hints: api-ref: Add field length limitation
 * api-ref: describe which protocols are enabled for stateless SG
 * api-ref: add semantics for stateless security group api
```

### Comparing `neutron-lib-3.5.0/HACKING.rst` & `neutron-lib-3.6.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/LICENSE` & `neutron-lib-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/PKG-INFO` & `neutron-lib-3.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-lib
-Version: 3.5.0
+Version: 3.6.0
 Summary: Neutron shared routines and utilities
 Home-page: https://docs.openstack.org/neutron-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `neutron-lib-3.5.0/README.rst` & `neutron-lib-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/conf.py` & `neutron-lib-3.6.0/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/address-groups.inc` & `neutron-lib-3.6.0/api-ref/source/v2/address-groups.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/address-scopes.inc` & `neutron-lib-3.6.0/api-ref/source/v2/address-scopes.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/agents.inc` & `neutron-lib-3.6.0/api-ref/source/v2/agents.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/auto-topology.inc` & `neutron-lib-3.6.0/api-ref/source/v2/auto-topology.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/availability_zones.inc` & `neutron-lib-3.6.0/api-ref/source/v2/availability_zones.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgp_dragent_scheduler.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgp_dragent_scheduler.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgp_peer.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgp_peer.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgp_speaker.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgp_speaker.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-bgpvpns.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-bgpvpns.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-network_associations.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-network_associations.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-overview.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-overview.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-port_associations.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-port_associations.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/bgpvpn-router_associations.inc` & `neutron-lib-3.6.0/api-ref/source/v2/bgpvpn-router_associations.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/dhcp-agent-scheduler.inc` & `neutron-lib-3.6.0/api-ref/source/v2/dhcp-agent-scheduler.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/extensions.inc` & `neutron-lib-3.6.0/api-ref/source/v2/extensions.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/fip-port-forwarding.inc` & `neutron-lib-3.6.0/api-ref/source/v2/fip-port-forwarding.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/firewall_log.inc` & `neutron-lib-3.6.0/api-ref/source/v2/firewall_log.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/flavors.inc` & `neutron-lib-3.6.0/api-ref/source/v2/flavors.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/floatingippools.inc` & `neutron-lib-3.6.0/api-ref/source/v2/floatingippools.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/floatingips.inc` & `neutron-lib-3.6.0/api-ref/source/v2/floatingips.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/fwaas-v2.inc` & `neutron-lib-3.6.0/api-ref/source/v2/fwaas-v2.inc`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,13 @@
 .. -*- rst -*-
 
 ================================================================================
 FWaaS v2.0 (CURRENT) (fwaas, firewall_groups, firewall_policies, firewall_rules)
 ================================================================================
 
-.. warning::
-
-    Due to lack of maintenance of the ``neutron-fwaas`` project, the reference
-    implementation of the FWaaS API, is now deprecated and unmaintained
-    anymore.
-    This document describes the FWaaS API definitions without any official
-    implementation.
-    This API can be implemented by some third party solutions.
-
 Use the Firewall-as-a-Service (FWaaS) v2.0 extension to deploy
 firewall groups to protect your networks.
 
 The FWaaS extension enables you to:
 
 - Apply firewall rules on traffic entering and leaving project
   networks.
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/index.rst` & `neutron-lib-3.6.0/api-ref/source/v2/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/intro.inc` & `neutron-lib-3.6.0/api-ref/source/v2/intro.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/l3-agent-scheduler.inc` & `neutron-lib-3.6.0/api-ref/source/v2/l3-agent-scheduler.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/l3-conntrack-helper.inc` & `neutron-lib-3.6.0/api-ref/source/v2/l3-conntrack-helper.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/local-ips.inc` & `neutron-lib-3.6.0/api-ref/source/v2/local-ips.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/logging.inc` & `neutron-lib-3.6.0/api-ref/source/v2/logging.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/logging_resource.inc` & `neutron-lib-3.6.0/api-ref/source/v2/logging_resource.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/metering.inc` & `neutron-lib-3.6.0/api-ref/source/v2/metering.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/network-ip-availability.inc` & `neutron-lib-3.6.0/api-ref/source/v2/network-ip-availability.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/network_segment_ranges.inc` & `neutron-lib-3.6.0/api-ref/source/v2/network_segment_ranges.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/networks.inc` & `neutron-lib-3.6.0/api-ref/source/v2/networks.inc`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,22 @@
 FloatingIP autodelete internal
 ==============================
 
 The ``floatingip-autodelete-internal`` shim extension signals that the
 update of a network's ``router:external`` attribute from ``true`` to
 ``false`` autodeletes the unused Floating IPs of that network.
 
+HA extension
+============
+
+The ``network-ha`` extension allows to pass a boolean parameter during the
+network creation. If ``true`` is passed, a ``ha_router_networks`` database
+register will be created along with the ``network`` register. This field is
+not visible and, initially, not meant to be supported in the CLI.
+
 L2 adjacency extension
 ======================
 
 The ``l2_adjacency`` extension provides display of L2 Adjacency
 for ``networks`` by adding the read-only ``l2_adjacency`` attribute.
 This is a boolean value where ``true`` means that you can expect
 L2 connectivity throughout the Network and ``false`` means that there
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/parameters.yaml` & `neutron-lib-3.6.0/api-ref/source/v2/parameters.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -4764,14 +4764,20 @@
 network-admin_state_up-request:
   description: |
     The administrative state of the network, which is
     up (``true``) or down (``false``).
   in: body
   required: false
   type: boolean
+network-ha:
+  description: |
+    The high availability input flag when creating a network.
+  in: body
+  required: false
+  type: boolean
 network-id:
   description: |
     The ID of the network.
   in: body
   required: true
   type: string
 network-name:
@@ -5967,14 +5973,30 @@
 router-distributed-request:
   description: |
     ``true`` indicates a distributed router.
     It is available when ``dvr`` extension is enabled.
   in: body
   required: false
   type: boolean
+router-enable_default_route_bfd:
+  description: |
+    ``true`` indicates that Neutron will enable BFD sessions for default routes
+    inferred from the external gateway port subnets.
+    Available when ``external-gateway-multihoming`` extension is enabled.
+  in: body
+  required: false
+  type: boolean
+router-enable_default_route_ecmp:
+  description: |
+    ``true`` indicates that Neutron will add ECMP default routes if multiple
+    are available via different gateway ports.
+    Available when ``external-gateway-multihoming`` extension is enabled.
+  in: body
+  required: false
+  type: boolean
 router-enable_ndp_proxy:
   description: |
     Enable NDP proxy attribute. ``true`` means NDP proxy is enabled for the
     router, the IPv6 address of internal subnets attached to the router can be
     published to external by create ``ndp_proxy``. ``false`` means NDP proxy is
     disabled, the IPv6 address of internal subnets attached to the router can
     not be published to external by ``ndp_proxy``. It is available when
@@ -6028,16 +6050,17 @@
   in: body
   required: false
   type: array
 router-external_gateway_info:
   description: |
     The external gateway information of the router.
     If the router has an external gateway, this would be a dict with
-    ``network_id``, ``enable_snat``, ``external_fixed_ips`` and
-    ``qos_policy_id``.
+    ``network_id``, ``enable_snat``, ``external_fixed_ips``,
+    ``qos_policy_id``, ``enable_default_route_ecmp`` and
+    ``enable_default_route_bfd``.
     Otherwise, this would be ``null``.
   in: body
   required: true
   type: object
 router-external_gateway_info-request:
   description: |
     The external gateway information of the router.
@@ -6050,14 +6073,20 @@
   type: object
 router-external_gateway_ports:
   description: |
     The external gateway ports.
   in: body
   required: true
   type: string
+router-external_gateways:
+  description: |
+    The list of external gateways of the router.
+  in: body
+  required: true
+  type: array
 router-flavor_id:
   description: |
     The ID of the flavor associated with the router.
   in: body
   required: true
   type: string
 router-flavor_id-optional:
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/ports.inc` & `neutron-lib-3.6.0/api-ref/source/v2/ports.inc`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 .. warning::
 
     If a security group with a ``remote_group_id`` rule is used by a port, adding
     an address pair with IP address ``0.0.0.0/0`` (``ANY``) will bypass all rules
     with source IP address restrictions for all ports which use the same security
     group.
 
+Allowed address pairs (atomic) extension
+========================================
+
+The Allowed address pairs (atomic) extension (``allowedaddresspairs-atomic``)
+extends the ``port`` resource by adding two member actions
+(``add_allowed_address_pairs``/ ``remove_allowed_address_pairs``) to edit the set
+of Allowed address pairs atomically on the server side.
+
 Data plane status extension
 ===========================
 
 The data plane port extension (``data-plane-status``) adds a new attribute
 ``data_plane_status`` to represent the status of the underlying data plane.
 This attribute is to be managed by entities outside of the Networking service,
 while the ``status`` attribute is managed by Networking service. Both status
@@ -768,7 +776,161 @@
    - mac_learning_enabled: mac_learning_enabled
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/ports/ports-bulk-create-response.json
    :language: javascript
+
+Add allowed_address_pairs to port
+=================================
+
+.. rest_method::  PUT /v2.0/ports/{port_id}/add_allowed_address_pairs
+
+Atomically adds a set of allowed_address_pairs to the port's already
+existing allowed_address_pairs.
+
+Normal response codes: 200
+
+Error response codes: 400, 401, 404, 412
+
+Request
+-------
+
+.. rest_parameters:: parameters.yaml
+
+   - port_id: port_id-path
+   - port: port
+   - allowed_address_pairs: allowed_address_pairs-request
+
+Request Example
+---------------
+
+.. literalinclude:: samples/ports/port-add-allowed-address-pairs-request.json
+   :language: javascript
+
+Response Parameters
+-------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - port: port
+   - admin_state_up: admin_state_up
+   - allowed_address_pairs: allowed_address_pairs
+   - binding:host_id: binding:host_id
+   - binding:profile: binding:profile
+   - binding:vif_details: binding:vif_details
+   - binding:vif_type: binding:vif_type
+   - binding:vnic_type: binding:vnic_type
+   - created_at: created_at_resource
+   - data_plane_status: data_plane_status
+   - description: description
+   - device_id: device_id
+   - device_owner: device_owner
+   - dns_assignment: dns_assignment
+   - dns_domain: dns_domain
+   - dns_name: dns_name
+   - extra_dhcp_opts: extra_dhcp_opts
+   - fixed_ips: fixed_ips
+   - hints: hints
+   - id: id
+   - ip_allocation: ip_allocation
+   - mac_address: mac_address
+   - name: name
+   - network_id: network_id
+   - numa_affinity_policy: numa_affinity_policy
+   - port_security_enabled: port_security_enabled
+   - project_id: project_id
+   - qos_network_policy_id: qos_network_policy_id-port-response
+   - qos_policy_id: qos_policy_id-port-response
+   - revision_number: revision_number
+   - resource_request: port-resource
+   - security_groups: port-security_groups
+   - status: port-status
+   - tags: tags
+   - tenant_id: project_id
+   - updated_at: updated_at_resource
+   - propagate_uplink_status: propagate_uplink_status
+   - mac_learning_enabled: mac_learning_enabled
+
+Response Example
+----------------
+
+.. literalinclude:: samples/ports/port-add-allowed-address-pairs-response.json
+   :language: javascript
+
+Remove allowed_address_pairs from port
+======================================
+
+.. rest_method::  PUT /v2.0/ports/{port_id}/remove_allowed_address_pairs
+
+Atomically removes a set of allowed_address_pairs from the port's already
+existing allowed_address_pairs.
+
+Normal response codes: 200
+
+Error response codes: 400, 401, 404, 412
+
+Request
+-------
+
+.. rest_parameters:: parameters.yaml
+
+   - port_id: port_id-path
+   - port: port
+   - allowed_address_pairs: allowed_address_pairs-request
+
+Request Example
+---------------
+
+.. literalinclude:: samples/ports/port-remove-allowed-address-pairs-request.json
+   :language: javascript
+
+Response Parameters
+-------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - port: port
+   - admin_state_up: admin_state_up
+   - allowed_address_pairs: allowed_address_pairs
+   - binding:host_id: binding:host_id
+   - binding:profile: binding:profile
+   - binding:vif_details: binding:vif_details
+   - binding:vif_type: binding:vif_type
+   - binding:vnic_type: binding:vnic_type
+   - created_at: created_at_resource
+   - data_plane_status: data_plane_status
+   - description: description
+   - device_id: device_id
+   - device_owner: device_owner
+   - dns_assignment: dns_assignment
+   - dns_domain: dns_domain
+   - dns_name: dns_name
+   - extra_dhcp_opts: extra_dhcp_opts
+   - fixed_ips: fixed_ips
+   - hints: hints
+   - id: id
+   - ip_allocation: ip_allocation
+   - mac_address: mac_address
+   - name: name
+   - network_id: network_id
+   - numa_affinity_policy: numa_affinity_policy
+   - port_security_enabled: port_security_enabled
+   - project_id: project_id
+   - qos_network_policy_id: qos_network_policy_id-port-response
+   - qos_policy_id: qos_policy_id-port-response
+   - revision_number: revision_number
+   - resource_request: port-resource
+   - security_groups: port-security_groups
+   - status: port-status
+   - tags: tags
+   - tenant_id: project_id
+   - updated_at: updated_at_resource
+   - propagate_uplink_status: propagate_uplink_status
+   - mac_learning_enabled: mac_learning_enabled
+
+Response Example
+----------------
+
+.. literalinclude:: samples/ports/port-remove-allowed-address-pairs-response.json
+   :language: javascript
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/qos.inc` & `neutron-lib-3.6.0/api-ref/source/v2/qos.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/quota_details.inc` & `neutron-lib-3.6.0/api-ref/source/v2/quota_details.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/quotas.inc` & `neutron-lib-3.6.0/api-ref/source/v2/quotas.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/rbac-policy.inc` & `neutron-lib-3.6.0/api-ref/source/v2/rbac-policy.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/router-ndp-proxy.inc` & `neutron-lib-3.6.0/api-ref/source/v2/router-ndp-proxy.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/routers.inc` & `neutron-lib-3.6.0/api-ref/source/v2/routers.inc`

 * *Files 24% similar despite different names*

```diff
@@ -64,14 +64,22 @@
 The ``ext-gw-mode`` extension of the router abstraction for specifying whether
 SNAT should occur on the external gateway.
 The ``ext-gw-mode`` extension allows enabling configurable external gateway
 modes, adds the ``external_gateway_info`` attribute to ``routers``
 and allows definitions for ``network_id``, ``enable_snat`` and
 ``external_fixed_ips``.
 
+L3 external gateway multihoming extension (``external-gateway-multihoming``)
+============================================================================
+
+The ``external-gateway-multihoming`` extension allows a router to have
+multiple external gateway ports and to have a policy specified on how
+to handle ECMP and BFD for default routes inferred from the subnets
+associated with gateway ports.
+
 L3 flavors extension (``l3-flavors``)
 =====================================
 
 The router flavor extension (``l3-flavors``) adds the ``flavor_id`` attribute
 to routers, allowing requests to be dispatched to different drivers depending
 on the flavor associated with a given router.
 
@@ -131,14 +139,32 @@
 
 Router gateway IP QoS (qos-gateway-ip)
 ======================================
 
 The ``qos-gateway-ip`` extension adds ``qos_policy_id`` to the
 ``external_gateway_info`` field of routers.
 
+Router enable default route ECMP extension (``enable-default-route-ecmp``)
+==========================================================================
+
+The ``enable-default-route-ecmp`` extension adds a parameter called
+``enable_default_route_ecmp`` to the router resource which can be used to
+enable or disable automatic configuration of ECMP default routes based on the
+default gateways of subnets accessible from a router's gateway ports (see
+the ``external-gateway-multihoming`` extension).
+
+Router enable default route BFD extension (``enable-default-route-bfd``)
+========================================================================
+
+The ``enable-default-route-bfd`` extension adds a parameter called
+``enable_default_route_bfd`` to the router resource which can be used to
+enable or disable automatic configuration of BFD for default routes of a router
+created based on the default gateways of subnets accessible from a router's
+gateway ports (see ``enable-default-route-ecmp`` extension).
+
 List routers
 ============
 
 .. rest_method::  GET /v2.0/routers
 
 Lists logical routers that the project who submits the request can access.
 
@@ -186,14 +212,15 @@
    - tenant_id: project_id
    - project_id: project_id
    - name: name
    - description: description
    - admin_state_up: admin_state_up
    - status: router-status
    - external_gateway_info: router-external_gateway_info
+   - external_gateways: router-external_gateways
    - revision_number: revision_number
    - routes: router-routes
    - destination: router-destination
    - nexthop: router-nexthop
    - distributed: router-distributed
    - ha: router-ha
    - availability_zone_hints: router-availability_zone_hints
@@ -201,14 +228,16 @@
    - service_type_id: router-service_type_id
    - flavor_id: router-flavor_id
    - created_at: created_at_resource
    - updated_at: updated_at_resource
    - tags: tags
    - conntrack_helpers: router-conntrack_helpers
    - enable_ndp_proxy: router-enable_ndp_proxy
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/routers/routers-list-response.json
    :language: javascript
 
@@ -247,14 +276,16 @@
    - external_gateway_info: router-external_gateway_info-request
    - distributed: router-distributed-request
    - ha: router-ha-request
    - availability_zone_hints: router-availability_zone_hints-request
    - service_type_id: router-service_type_id-request
    - flavor_id: router-flavor_id-optional
    - enable_ndp_proxy: router-enable_ndp_proxy-request
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Request Example
 ---------------
 
 .. literalinclude:: samples/routers/router-create-request.json
    :language: javascript
 
@@ -268,14 +299,15 @@
    - tenant_id: project_id
    - project_id: project_id
    - name: name
    - description: description
    - admin_state_up: admin_state_up
    - status: router-status
    - external_gateway_info: router-external_gateway_info
+   - external_gateways: router-external_gateways
    - revision_number: revision_number
    - routes: router-routes
    - destination: router-destination
    - nexthop: router-nexthop
    - distributed: router-distributed
    - ha: router-ha
    - availability_zone_hints: router-availability_zone_hints
@@ -283,14 +315,16 @@
    - service_type_id: router-service_type_id
    - flavor_id: router-flavor_id
    - created_at: created_at_resource
    - updated_at: updated_at_resource
    - tags: tags
    - conntrack_helpers: router-conntrack_helpers
    - enable_ndp_proxy: router-enable_ndp_proxy
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/routers/router-create-response.json
    :language: javascript
 
@@ -329,14 +363,15 @@
    - tenant_id: project_id
    - project_id: project_id
    - name: name
    - description: description
    - admin_state_up: admin_state_up
    - status: router-status
    - external_gateway_info: router-external_gateway_info
+   - external_gateways: router-external_gateways
    - revision_number: revision_number
    - routes: router-routes
    - destination: router-destination
    - nexthop: router-nexthop
    - distributed: router-distributed
    - ha: router-ha
    - availability_zone_hints: router-availability_zone_hints
@@ -344,14 +379,16 @@
    - service_type_id: router-service_type_id
    - flavor_id: router-flavor_id
    - created_at: created_at_resource
    - updated_at: updated_at_resource
    - tags: tags
    - conntrack_helpers: router-conntrack_helpers
    - enable_ndp_proxy: router-enable_ndp_proxy
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/routers/router-show-response.json
    :language: javascript
 
@@ -381,14 +418,16 @@
    - name: name
    - admin_state_up: admin_state_up
    - router_id: router_id
    - description: description-request
    - routes: router-routes-request
    - distributed: router-distributed-request
    - enable_ndp_proxy: router-enable_ndp_proxy-request
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Request Example
 ---------------
 
 .. literalinclude:: samples/routers/router-update-request.json
    :language: javascript
 
@@ -402,14 +441,15 @@
    - tenant_id: project_id
    - project_id: project_id
    - name: name
    - description: description
    - admin_state_up: admin_state_up
    - status: router-status
    - external_gateway_info: router-external_gateway_info
+   - external_gateways: router-external_gateways
    - revision_number: revision_number
    - routes: router-routes
    - destination: router-destination
    - nexthop: router-nexthop
    - distributed: router-distributed
    - ha: router-ha
    - availability_zone_hints: router-availability_zone_hints
@@ -417,14 +457,16 @@
    - service_type_id: router-service_type_id
    - flavor_id: router-flavor_id
    - created_at: created_at_resource
    - updated_at: updated_at_resource
    - tags: tags
    - conntrack_helpers: router-conntrack_helpers
    - enable_ndp_proxy: router-enable_ndp_proxy
+   - enable_default_route_bfd: router-enable_default_route_bfd
+   - enable_default_route_ecmp: router-enable_default_route_ecmp
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/routers/router-update-response.json
    :language: javascript
 
@@ -762,7 +804,243 @@
    - routes: router-routes
 
 Response Example
 ----------------
 
 .. literalinclude:: samples/routers/router-remove-extraroutes-response.json
    :language: javascript
+
+Add external gateways to router
+===============================
+
+.. rest_method::  PUT /v2.0/routers/{router_id}/add_external_gateways
+
+Add external gateways to a router in addition to the ones it already
+has.
+
+Multiple gateways attached to the same network can be added to the
+same router.
+
+The add/update/remove external gateways operations extend the use of
+``router.external_gateway_info`` to manage multiple external gateways.
+The full set of external gateways is exposed in the read-only
+``router.external_gateways`` parameter.  ``router.external_gateways``
+contains a list of ``external_gateway_info`` structures like:
+
+::
+
+    [
+      {"network_id": ...,
+       "external_fixed_ips": [{"ip_address": ..., "subnet_id": ...}, ...],
+       "enable_snat": ...},
+      ...
+    ]
+
+The first item (index 0) of the ``external_gateways`` list is special if a
+router does not have any gateway ports yet:
+
+* It will provide data for the compatibility ``router.external_gateway_info``
+  field of a router;
+
+* This first item sets a router's default route. If ECMP is enabled for
+  default routes inferred from gateway port subnets, then all of those
+  default routes are used for load-sharing;
+
+* The first item is just another extra gateway if the add operation is
+  performed when a router already has one or more gateways.
+
+The order of the the rest of the list (indexes 1, 2, ...) is irrelevant
+and ignored.
+
+The first external gateway can be managed in two
+ways: via ``router.external_gateway_info`` or via
+``add/update/remove_external_gateways``.  The other external gateways
+can only be managed via ``add/update/remove_external_gateways``.
+
+The format of the request body is the same as the format of the read-only
+``router.external_gateways`` parameter, but wrapped as follows:
+
+::
+
+    {"router": {"external_gateways": EXTERNAL-GATEWAY-LIST}}
+
+The response codes and response body are the same as to the update of
+the router.  That is the whole router object is returned including the
+``external_gateway_info`` and ``external_gateways`` parameters which
+represents the result of the operation.
+
+Changes in ``router.external_gateway_info`` are reflected
+in ``router.external_gateways`` and vice versa.  Updating
+``external_gateway_info`` also updates the first element of
+``external_gateways`` and it leaves the rest of ``external_gateways``
+unchanged.  Setting ``external_gateway_info`` to an empty value removes
+a single gateway and one of the extra gateways takes its place instead.
+
+Normal response codes: 200
+
+Error response codes: 400, 401, 404, 412
+
+Request Parameters
+------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - router_id: router_id
+   - external_gateways: router-external_gateways
+
+Request Example
+---------------
+
+.. literalinclude:: samples/routers/router-add-external-gateways-request.json
+   :language: javascript
+
+Response Parameters
+-------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - id: router-id-body
+   - name: router_name
+   - external_gateways: router-external_gateways
+
+Response Example
+----------------
+
+.. literalinclude:: samples/routers/router-add-external-gateways-response.json
+   :language: javascript
+
+Update external gateways of router
+==================================
+
+.. rest_method::  PUT /v2.0/routers/{router_id}/update_external_gateways
+
+Update some external gateways of router.
+
+For general information on the add/update/remove external gateways
+operations see ``add_external_gateways`` above.
+
+The external gateways to be updated are identified by the ``network_ids``
+found in the PUT request.  The ``external_fixed_ips``, ``enable_snat``,
+fields can be updated.  The ``network_id`` field cannot be updated - any
+changes will cause a gateway port to be removed and recreated.
+
+The format of the request body is the same as the format of the read-only
+``router.external_gateways`` parameter, but wrapped as follows:
+
+::
+
+    {"router": {"external_gateways": EXTERNAL-GATEWAY-LIST}}
+
+The ``enable_snat`` field does not have any effect for extra gateways except
+for the first external gateway in the list.
+
+The ``network_id`` field is used to identify a particular gateway port along
+with the ``external_fixed_ips`` field. Specifying just the ``network_id`` field
+is ambiguous: Neutron will attempt to find the matching gateway port but if
+there are multiple matches it will return an error response code.
+
+The ``enable_snat`` field can be omitted from the request. Specifying
+``external_fixed_ips`` will result in matching ports based on those
+fixed IPs. If a gateway port has a subset of the specified fixed IPs,
+then the set of IPs will be updated to match the ones in the request.
+Alternatively, if a gateway port has a superset of fixed IPs from the
+request the IPs will be removed from the gateway port.
+
+The response codes and response body are the same as to the update of
+the router.  That is the whole router object is returned including the
+``external_gateway_info`` and ``external_gateways`` parameters which
+represents the result of the operation.
+
+Please note that updating ``external_gateway_info`` also updates
+the first element of ``external_gateways`` and it leaves the rest of
+``external_gateways`` unchanged.
+
+Normal response codes: 200
+
+Error response codes: 400, 401, 404, 412
+
+Request Parameters
+------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - router_id: router_id
+   - external_gateways: router-external_gateways
+
+Request Example
+---------------
+
+.. literalinclude:: samples/routers/router-update-external-gateways-request.json
+   :language: javascript
+
+Response Parameters
+-------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - id: router-id-body
+   - name: router_name
+   - external_gateways: router-external_gateways
+
+Response Example
+----------------
+
+.. literalinclude:: samples/routers/router-update-external-gateways-response.json
+   :language: javascript
+
+Remove external gateways from router
+====================================
+
+.. rest_method::  PUT /v2.0/routers/{router_id}/remove_external_gateways
+
+Remove some external gateways from router.
+
+For general information on the add/update/remove external gateways
+operations see ``add_external_gateways`` above.
+
+The format of the request body is the same as the format of the read-only
+``router.external_gateways`` parameter, but wrapped as follows:
+
+::
+
+    {"router": {"external_gateways": EXTERNAL-GATEWAY-LIST}}
+
+However the request body can be partial.  Only the ``network_id``
+and ``external_fixed_ips`` fields from the ``external_gateway_info``
+structure is used in order to match the specific gateway ports.
+The ``enable_snat`` key can be present but its value is ignored.
+
+Please note that setting ``external_gateway_info`` to an empty value
+also resets ``external_gateways`` to the empty list.
+
+Normal response codes: 200
+
+Error response codes: 400, 401, 404, 412
+
+Request Parameters
+------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - router_id: router_id
+   - external_gateways: router-external_gateways
+
+Request Example
+---------------
+
+.. literalinclude:: samples/routers/router-remove-external-gateways-request.json
+   :language: javascript
+
+Response Parameters
+-------------------
+
+.. rest_parameters:: parameters.yaml
+
+   - id: router-id-body
+   - name: router_name
+   - external_gateways: router-external_gateways
+
+Response Example
+----------------
+
+.. literalinclude:: samples/routers/router-remove-external-gateways-response.json
+   :language: javascript
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/address-scopes/address-scopes-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/address-scopes/address-scopes-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-dhcp-networks-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-dhcp-networks-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-l3-routers-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-l3-routers-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agent-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agent-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/agents-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/agents-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/network-dhcp-agent-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/network-dhcp-agent-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/agents/router-l3-agent-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/agents/router-l3-agent-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_dragent_host-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/bgp_speaker_list_dragent_host-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgp/dragent_list_agents_hosting_speaker-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgp/dragent_list_agents_hosting_speaker-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpn-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpns-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/bgpvpn/bgpvpns/bgpvpns-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/extensions/extensions-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/extensions/extensions-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-group-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-groups-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-groups-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rule-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall-v2/firewall-rules-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall-v2/firewall-rules-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewall_log/firewall_logs-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewall_log/firewall_logs-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rule-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewall-rules-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewall-rules-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/firewalls/firewalls-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/firewalls/firewalls-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/flavors/service-profiles-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/flavors/service-profiles-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floating-ips-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floating-ips-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-disassociate-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/floatingips/floatingip-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/floatingips/floatingip-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local-ips-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local-ips-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/local_ips/local_ip-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/local_ips/local_ip-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resource-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logging_resource/logging_resources-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logging_resource/logging_resources-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/logs/log-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/logs/log-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-label-rules-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-label-rules-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/metering/metering-labels-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/metering/metering-labels-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxies-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ndp_proxies/ndp-proxies-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-list.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-list.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-show.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network-ip-availability/network-ip-availability-show.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_range-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_ranges-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/network_segment_ranges/network_segment_ranges-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-multi-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-multi-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-provider-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-provider-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/network-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/network-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-bulk-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-bulk-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/networks-provider-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/networks-provider-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/networks/version-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/networks/version-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/port_forwardings/port-fowarding-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-create-request.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-create-request.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-show-response.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8613095238095239%*

 * *Differences: {"'port'": "{'allowed_address_pairs': [], 'binding:host_id': 'devstack', 'binding:profile': "*

 * *           "{replace: OrderedDict()}, 'binding:vif_details': {replace: "*

 * *           "OrderedDict([('ovs_hybrid_plug', True), ('port_filter', True)])}, 'binding:vif_type': "*

 * *           "'ovs', 'binding:vnic_type': 'normal', 'data_plane_status': 'ACTIVE', 'device_id': "*

 * *           "'5e3898d7-11be-483e-9732-b2f5eccd2b2e', 'device_owner': 'network:router_interface', "*

 * *           "'dns_assignment': {0: {'ip_address': '1 […]*

```diff
@@ -1,63 +1,54 @@
 {
     "port": {
         "admin_state_up": true,
-        "allowed_address_pairs": [
-            {
-                "ip_address": "12.12.11.12",
-                "mac_address": "fa:14:2a:b3:cb:f0"
-            }
-        ],
-        "binding:host_id": "4df8d9ff-6f6f-438f-90a1-ef660d4586ad",
-        "binding:profile": {
-            "local_link_information": [
-                {
-                    "port_id": "Ethernet3/1",
-                    "switch_id": "0a:1b:2c:3d:4e:5f",
-                    "switch_info": "switch1"
-                }
-            ]
+        "allowed_address_pairs": [],
+        "binding:host_id": "devstack",
+        "binding:profile": {},
+        "binding:vif_details": {
+            "ovs_hybrid_plug": true,
+            "port_filter": true
         },
-        "binding:vif_details": {},
-        "binding:vif_type": "unbound",
-        "binding:vnic_type": "other",
+        "binding:vif_type": "ovs",
+        "binding:vnic_type": "normal",
         "created_at": "2016-03-08T20:19:41",
-        "data_plane_status": null,
+        "data_plane_status": "ACTIVE",
         "description": "",
-        "device_id": "d90a13da-be41-461f-9f99-1dbcf438fdf2",
-        "device_owner": "baremetal:none",
+        "device_id": "5e3898d7-11be-483e-9732-b2f5eccd2b2e",
+        "device_owner": "network:router_interface",
         "dns_assignment": [
             {
                 "fqdn": "myport.my-domain.org",
                 "hostname": "myport",
-                "ip_address": "10.0.0.2"
+                "ip_address": "10.0.0.1"
             }
         ],
         "dns_domain": "my-domain.org.",
         "dns_name": "myport",
         "extra_dhcp_opts": [
             {
                 "ip_version": 4,
                 "opt_name": "bootfile-name",
                 "opt_value": "pxelinux.0"
             }
         ],
         "fixed_ips": [
             {
-                "ip_address": "10.0.0.2",
+                "ip_address": "10.0.0.1",
                 "subnet_id": "a0304c3a-4f08-4c43-88af-d796509c97d2"
             }
         ],
-        "id": "65c0ee9f-d634-4522-8954-51021b570b0d",
+        "id": "46d4bfb9-b26e-41f3-bd2e-e6dcc1ccedb2",
         "ip_allocation": "immediate",
-        "mac_address": "fa:16:3e:c9:cb:f0",
-        "name": "private-port",
+        "mac_address": "fa:16:3e:23:fd:d7",
+        "mac_learning_enabled": false,
+        "name": "",
         "network_id": "a87cc70a-3e15-4acf-8205-9b711a3531b7",
-        "port_security_enabled": true,
-        "project_id": "d6700c0c9ffa4f1cb322cd4a1f3906fa",
+        "port_security_enabled": false,
+        "project_id": "7e02058126cc4950b75f9970368ba177",
         "propagate_uplink_status": false,
         "qos_network_policy_id": "174dd0c1-a4eb-49d4-a807-ae80246d82f4",
         "qos_policy_id": "29d5e02e-d5ab-4929-bee4-4a9fc12e22ae",
         "resource_request": {
             "request_groups": [
                 {
                     "id": "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
@@ -81,18 +72,16 @@
             ],
             "same_subtree": [
                 "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
                 "b20bb47f-5d6d-45a6-8fe7-2c1b44f0db73"
             ]
         },
         "revision_number": 1,
-        "security_groups": [
-            "f0ac4394-7e4a-4409-9701-ba8be283dbc3"
-        ],
-        "status": "DOWN",
+        "security_groups": [],
+        "status": "ACTIVE",
         "tags": [
             "tag1,tag2"
         ],
-        "tenant_id": "d6700c0c9ffa4f1cb322cd4a1f3906fa",
+        "tenant_id": "7e02058126cc4950b75f9970368ba177",
         "updated_at": "2016-03-08T20:19:41"
     }
 }
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-update-response.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8738095238095238%*

 * *Differences: {"'port'": "{'binding:host_id': 'test_for_port_update_host', 'binding:vif_details': {replace: "*

 * *           "OrderedDict()}, 'binding:vif_type': 'binding_failed', 'data_plane_status': 'DOWN', "*

 * *           "'device_id': 'd90a13da-be41-461f-9f99-1dbcf438fdf2', 'device_owner': 'compute:nova', "*

 * *           "'dns_assignment': {0: {'ip_address': '20.20.0.4'}}, 'fixed_ips': {0: {'ip_address': "*

 * *           "'20.20.0.4', 'subnet_id': '898dec4a-74df-4193-985f-c76721bcc746'}}, 'id': "*

 * *           "'43c831e0-19ce-4a76-9a […]*

```diff
@@ -1,54 +1,50 @@
 {
     "port": {
         "admin_state_up": true,
         "allowed_address_pairs": [],
-        "binding:host_id": "devstack",
+        "binding:host_id": "test_for_port_update_host",
         "binding:profile": {},
-        "binding:vif_details": {
-            "ovs_hybrid_plug": true,
-            "port_filter": true
-        },
-        "binding:vif_type": "ovs",
+        "binding:vif_details": {},
+        "binding:vif_type": "binding_failed",
         "binding:vnic_type": "normal",
         "created_at": "2016-03-08T20:19:41",
-        "data_plane_status": "ACTIVE",
+        "data_plane_status": "DOWN",
         "description": "",
-        "device_id": "5e3898d7-11be-483e-9732-b2f5eccd2b2e",
-        "device_owner": "network:router_interface",
+        "device_id": "d90a13da-be41-461f-9f99-1dbcf438fdf2",
+        "device_owner": "compute:nova",
         "dns_assignment": [
             {
                 "fqdn": "myport.my-domain.org",
                 "hostname": "myport",
-                "ip_address": "10.0.0.1"
+                "ip_address": "20.20.0.4"
             }
         ],
         "dns_domain": "my-domain.org.",
         "dns_name": "myport",
         "extra_dhcp_opts": [
             {
                 "ip_version": 4,
                 "opt_name": "bootfile-name",
                 "opt_value": "pxelinux.0"
             }
         ],
         "fixed_ips": [
             {
-                "ip_address": "10.0.0.1",
-                "subnet_id": "a0304c3a-4f08-4c43-88af-d796509c97d2"
+                "ip_address": "20.20.0.4",
+                "subnet_id": "898dec4a-74df-4193-985f-c76721bcc746"
             }
         ],
-        "id": "46d4bfb9-b26e-41f3-bd2e-e6dcc1ccedb2",
+        "id": "43c831e0-19ce-4a76-9a49-57b57e69428b",
         "ip_allocation": "immediate",
-        "mac_address": "fa:16:3e:23:fd:d7",
-        "mac_learning_enabled": false,
-        "name": "",
-        "network_id": "a87cc70a-3e15-4acf-8205-9b711a3531b7",
+        "mac_address": "fa:16:3e:11:11:5e",
+        "name": "test-for-port-update",
+        "network_id": "883fc383-5ea1-4c8b-8916-e1ddb0a9f365",
         "port_security_enabled": false,
-        "project_id": "7e02058126cc4950b75f9970368ba177",
+        "project_id": "522eda8d23124b25bf03fe44f1986b74",
         "propagate_uplink_status": false,
         "qos_network_policy_id": "174dd0c1-a4eb-49d4-a807-ae80246d82f4",
         "qos_policy_id": "29d5e02e-d5ab-4929-bee4-4a9fc12e22ae",
         "resource_request": {
             "request_groups": [
                 {
                     "id": "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
@@ -71,17 +67,19 @@
                 }
             ],
             "same_subtree": [
                 "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
                 "b20bb47f-5d6d-45a6-8fe7-2c1b44f0db73"
             ]
         },
-        "revision_number": 1,
-        "security_groups": [],
-        "status": "ACTIVE",
+        "revision_number": 2,
+        "security_groups": [
+            "ce0179d6-8a94-4f7c-91c2-f3038e2acbd0"
+        ],
+        "status": "DOWN",
         "tags": [
             "tag1,tag2"
         ],
-        "tenant_id": "7e02058126cc4950b75f9970368ba177",
+        "tenant_id": "522eda8d23124b25bf03fe44f1986b74",
         "updated_at": "2016-03-08T20:19:41"
     }
 }
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-bind-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-bind-create-response.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8666666666666667%*

 * *Differences: {"'port'": "{'allowed_address_pairs': [OrderedDict([('ip_address', '12.12.11.12'), ('mac_address', "*

 * *           "'fa:14:2a:b3:cb:f0')])], 'binding:host_id': '4df8d9ff-6f6f-438f-90a1-ef660d4586ad', "*

 * *           "'binding:profile': {replace: OrderedDict([('local_link_information', "*

 * *           "[OrderedDict([('port_id', 'Ethernet3/1'), ('switch_id', '0a:1b:2c:3d:4e:5f'), "*

 * *           "('switch_info', 'switch1')])])])}, 'binding:vif_type': 'unbound', 'binding:vnic_type': "*

 * *           "'other', 'data_plane_stat […]*

```diff
@@ -1,50 +1,70 @@
 {
     "port": {
         "admin_state_up": true,
-        "allowed_address_pairs": [],
-        "binding:host_id": "test_for_port_update_host",
-        "binding:profile": {},
+        "allowed_address_pairs": [
+            {
+                "ip_address": "12.12.11.12",
+                "mac_address": "fa:14:2a:b3:cb:f0"
+            }
+        ],
+        "binding:host_id": "4df8d9ff-6f6f-438f-90a1-ef660d4586ad",
+        "binding:profile": {
+            "local_link_information": [
+                {
+                    "port_id": "Ethernet3/1",
+                    "switch_id": "0a:1b:2c:3d:4e:5f",
+                    "switch_info": "switch1"
+                }
+            ]
+        },
         "binding:vif_details": {},
-        "binding:vif_type": "binding_failed",
-        "binding:vnic_type": "normal",
+        "binding:vif_type": "unbound",
+        "binding:vnic_type": "other",
         "created_at": "2016-03-08T20:19:41",
-        "data_plane_status": "DOWN",
+        "data_plane_status": null,
         "description": "",
         "device_id": "d90a13da-be41-461f-9f99-1dbcf438fdf2",
-        "device_owner": "compute:nova",
+        "device_owner": "baremetal:none",
         "dns_assignment": [
             {
                 "fqdn": "myport.my-domain.org",
                 "hostname": "myport",
-                "ip_address": "20.20.0.4"
+                "ip_address": "10.0.0.2"
             }
         ],
         "dns_domain": "my-domain.org.",
         "dns_name": "myport",
         "extra_dhcp_opts": [
             {
                 "ip_version": 4,
                 "opt_name": "bootfile-name",
                 "opt_value": "pxelinux.0"
             }
         ],
         "fixed_ips": [
             {
-                "ip_address": "20.20.0.4",
-                "subnet_id": "898dec4a-74df-4193-985f-c76721bcc746"
+                "ip_address": "10.0.0.2",
+                "subnet_id": "a0304c3a-4f08-4c43-88af-d796509c97d2"
             }
         ],
-        "id": "43c831e0-19ce-4a76-9a49-57b57e69428b",
+        "hints": {
+            "openvswitch": {
+                "other_config": {
+                    "tx-steering": "hash"
+                }
+            }
+        },
+        "id": "65c0ee9f-d634-4522-8954-51021b570b0d",
         "ip_allocation": "immediate",
-        "mac_address": "fa:16:3e:11:11:5e",
-        "name": "test-for-port-update",
-        "network_id": "883fc383-5ea1-4c8b-8916-e1ddb0a9f365",
-        "port_security_enabled": false,
-        "project_id": "522eda8d23124b25bf03fe44f1986b74",
+        "mac_address": "fa:16:3e:c9:cb:f0",
+        "name": "private-port",
+        "network_id": "a87cc70a-3e15-4acf-8205-9b711a3531b7",
+        "port_security_enabled": true,
+        "project_id": "d6700c0c9ffa4f1cb322cd4a1f3906fa",
         "propagate_uplink_status": false,
         "qos_network_policy_id": "174dd0c1-a4eb-49d4-a807-ae80246d82f4",
         "qos_policy_id": "29d5e02e-d5ab-4929-bee4-4a9fc12e22ae",
         "resource_request": {
             "request_groups": [
                 {
                     "id": "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
@@ -67,19 +87,19 @@
                 }
             ],
             "same_subtree": [
                 "1e4f3958-c0c9-4dec-82fa-ed2dc1c5cb34",
                 "b20bb47f-5d6d-45a6-8fe7-2c1b44f0db73"
             ]
         },
-        "revision_number": 2,
+        "revision_number": 1,
         "security_groups": [
-            "ce0179d6-8a94-4f7c-91c2-f3038e2acbd0"
+            "f0ac4394-7e4a-4409-9701-ba8be283dbc3"
         ],
         "status": "DOWN",
         "tags": [
             "tag1,tag2"
         ],
-        "tenant_id": "522eda8d23124b25bf03fe44f1986b74",
+        "tenant_id": "d6700c0c9ffa4f1cb322cd4a1f3906fa",
         "updated_at": "2016-03-08T20:19:41"
     }
 }
```

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-create-request.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-create-request.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-resource-request-new-format.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-resource-request-new-format.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/port-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/port-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-bind-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-bind-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-bulk-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-bulk-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/ports/ports-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/ports/ports-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policies-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policies-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/qos/policy-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/qos/policy-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/qos/rule_type-details-bandwidth_limit-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/qos/rule_type-details-bandwidth_limit-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/qos/rule_type-details-dscp_marking-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/qos/rule_type-details-dscp_marking-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/quota_details/quota-details-show-for-project-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/quota_details/quota-details-show-for-project-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-update-request.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-request.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/routers/router-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/routers/router-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/routers/routers-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/routers/routers-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rule-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-rules-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-group-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-group-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/security-groups/security-groups-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/security-groups/security-groups-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/segments/segments-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/segments/segments-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnet-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnet-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpool-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpool-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnetpools-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnetpools-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnets-create-bulk-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/subnets/subnets-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/subnets/subnets-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-add-subports-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-add-subports-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-details-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-details-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunk-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunk-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/trunks/trunks-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/trunks/trunks-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicies-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicies-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ikepolicy-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ikepolicy-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-request.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-request.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connection-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsec-site-connections-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsec-site-connections-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicies-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicies-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/ipsecpolicy-update-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpn-endpoint-groups-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpn-endpoint-groups-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-create-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-create-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservice-show-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservice-show-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/samples/vpn/vpnservices-list-response.json` & `neutron-lib-3.6.0/api-ref/source/v2/samples/vpn/vpnservices-list-response.json`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/security-group-rules.inc` & `neutron-lib-3.6.0/api-ref/source/v2/security-group-rules.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/security-groups.inc` & `neutron-lib-3.6.0/api-ref/source/v2/security-groups.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/segments.inc` & `neutron-lib-3.6.0/api-ref/source/v2/segments.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/service-providers.inc` & `neutron-lib-3.6.0/api-ref/source/v2/service-providers.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/subnetpool_prefix_ops.inc` & `neutron-lib-3.6.0/api-ref/source/v2/subnetpool_prefix_ops.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/subnetpools.inc` & `neutron-lib-3.6.0/api-ref/source/v2/subnetpools.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/subnets.inc` & `neutron-lib-3.6.0/api-ref/source/v2/subnets.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/taas.inc` & `neutron-lib-3.6.0/api-ref/source/v2/taas.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/tags.inc` & `neutron-lib-3.6.0/api-ref/source/v2/tags.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/trunk-details.inc` & `neutron-lib-3.6.0/api-ref/source/v2/trunk-details.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/trunk.inc` & `neutron-lib-3.6.0/api-ref/source/v2/trunk.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/versions.inc` & `neutron-lib-3.6.0/api-ref/source/v2/versions.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/api-ref/source/v2/vpnaas.inc` & `neutron-lib-3.6.0/api-ref/source/v2/vpnaas.inc`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/conf.py` & `neutron-lib-3.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/api_attributes.rst` & `neutron-lib-3.6.0/doc/source/contributor/api_attributes.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/api_converters.rst` & `neutron-lib-3.6.0/doc/source/contributor/api_converters.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/api_extensions.rst` & `neutron-lib-3.6.0/doc/source/contributor/api_extensions.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/api_validators.rst` & `neutron-lib-3.6.0/doc/source/contributor/api_validators.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/callbacks.rst` & `neutron-lib-3.6.0/doc/source/contributor/callbacks.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/consuming.rst` & `neutron-lib-3.6.0/doc/source/contributor/consuming.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/contributing.rst` & `neutron-lib-3.6.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/conventions.rst` & `neutron-lib-3.6.0/doc/source/contributor/conventions.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/db_model_query.rst` & `neutron-lib-3.6.0/doc/source/contributor/db_model_query.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/index.rst` & `neutron-lib-3.6.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/internals.rst` & `neutron-lib-3.6.0/doc/source/contributor/internals.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/releasing.rst` & `neutron-lib-3.6.0/doc/source/contributor/releasing.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/review-guidelines.rst` & `neutron-lib-3.6.0/doc/source/contributor/review-guidelines.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/contributor/rpc_api.rst` & `neutron-lib-3.6.0/doc/source/contributor/rpc_api.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/index.rst` & `neutron-lib-3.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/reference/index.rst` & `neutron-lib-3.6.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/doc/source/user/hacking.rst` & `neutron-lib-3.6.0/doc/source/user/hacking.rst`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/__init__.py` & `neutron-lib-3.6.0/neutron_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/_i18n.py` & `neutron-lib-3.6.0/neutron_lib/_i18n.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/common/constants.py` & `neutron-lib-3.6.0/neutron_lib/agent/common/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/common/utils.py` & `neutron-lib-3.6.0/neutron_lib/agent/common/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/constants.py` & `neutron-lib-3.6.0/neutron_lib/agent/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/extension.py` & `neutron-lib-3.6.0/neutron_lib/agent/extension.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/l2_extension.py` & `neutron-lib-3.6.0/neutron_lib/agent/l2_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/l3_extension.py` & `neutron-lib-3.6.0/neutron_lib/agent/l3_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/linux/interface.py` & `neutron-lib-3.6.0/neutron_lib/agent/linux/interface.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/agent/topics.py` & `neutron-lib-3.6.0/neutron_lib/agent/topics.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/attributes.py` & `neutron-lib-3.6.0/neutron_lib/api/attributes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/converters.py` & `neutron-lib-3.6.0/neutron_lib/api/converters.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/__init__.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from neutron_lib.api.definitions import address_group
 from neutron_lib.api.definitions import address_scope
 from neutron_lib.api.definitions import agent
 from neutron_lib.api.definitions import agent_resources_synced
 from neutron_lib.api.definitions import agent_sort_key
 from neutron_lib.api.definitions import allowedaddresspairs
+from neutron_lib.api.definitions import allowedaddresspairs_atomic
 from neutron_lib.api.definitions import auto_allocated_topology
 from neutron_lib.api.definitions import availability_zone
 from neutron_lib.api.definitions import availability_zone_filter
 from neutron_lib.api.definitions import bgp
 from neutron_lib.api.definitions import bgp_4byte_asn
 from neutron_lib.api.definitions import bgp_dragentscheduler
 from neutron_lib.api.definitions import bgpvpn
@@ -48,39 +49,44 @@
 from neutron_lib.api.definitions import fip64
 from neutron_lib.api.definitions import fip_distributed
 from neutron_lib.api.definitions import fip_pf_description
 from neutron_lib.api.definitions import fip_pf_detail
 from neutron_lib.api.definitions import fip_pf_port_range
 from neutron_lib.api.definitions import fip_port_details
 from neutron_lib.api.definitions import firewall_v2
+from neutron_lib.api.definitions import firewall_v2_stdattrs
 from neutron_lib.api.definitions import flavors
 from neutron_lib.api.definitions import floating_ip_port_forwarding
 from neutron_lib.api.definitions import floatingip_autodelete_internal
 from neutron_lib.api.definitions import floatingip_pools
 from neutron_lib.api.definitions import flowclassifier
 from neutron_lib.api.definitions import ip_allocation
 from neutron_lib.api.definitions import ip_substring_port_filtering
 from neutron_lib.api.definitions import l2_adjacency
 from neutron_lib.api.definitions import l3
 from neutron_lib.api.definitions import l3_conntrack_helper
+from neutron_lib.api.definitions import l3_enable_default_route_bfd
+from neutron_lib.api.definitions import l3_enable_default_route_ecmp
 from neutron_lib.api.definitions import l3_ext_gw_mode
+from neutron_lib.api.definitions import l3_ext_gw_multihoming
 from neutron_lib.api.definitions import l3_ext_ha_mode
 from neutron_lib.api.definitions import l3_ext_ndp_proxy
 from neutron_lib.api.definitions import l3_flavors
 from neutron_lib.api.definitions import l3_ndp_proxy
 from neutron_lib.api.definitions import l3_port_ip_change_not_allowed
 from neutron_lib.api.definitions import local_ip
 from neutron_lib.api.definitions import logging
 from neutron_lib.api.definitions import logging_resource
 from neutron_lib.api.definitions import metering
 from neutron_lib.api.definitions import metering_source_and_destination_filters
 from neutron_lib.api.definitions import multiprovidernet
 from neutron_lib.api.definitions import network
 from neutron_lib.api.definitions import network_availability_zone
 from neutron_lib.api.definitions import network_cascade_delete
+from neutron_lib.api.definitions import network_ha
 from neutron_lib.api.definitions import network_ip_availability
 from neutron_lib.api.definitions import network_mtu
 from neutron_lib.api.definitions import network_mtu_writable
 from neutron_lib.api.definitions import network_segment_range
 from neutron_lib.api.definitions import pagination
 from neutron_lib.api.definitions import port
 from neutron_lib.api.definitions import port_device_profile
@@ -157,14 +163,15 @@
 _ALL_API_DEFINITIONS = {
     address_group,
     address_scope,
     agent,
     agent_resources_synced,
     agent_sort_key,
     allowedaddresspairs,
+    allowedaddresspairs_atomic,
     auto_allocated_topology,
     availability_zone,
     availability_zone_filter,
     bgp,
     bgp_4byte_asn,
     bgp_dragentscheduler,
     bgpvpn,
@@ -188,14 +195,15 @@
     external_net,
     extra_dhcp_opt,
     extraroute,
     extraroute_atomic,
     filter_validation,
     fip64,
     firewall_v2,
+    firewall_v2_stdattrs,
     fip_distributed,
     fip_pf_detail,
     fip_port_details,
     flavors,
     floating_ip_port_forwarding,
     fip_pf_port_range,
     fip_pf_description,
@@ -207,25 +215,29 @@
     flowclassifier,
     l3,
     l3_conntrack_helper,
     l3_ext_gw_mode,
     l3_ext_ha_mode,
     l3_ext_ndp_proxy,
     l3_flavors,
+    l3_ext_gw_multihoming,
+    l3_enable_default_route_bfd,
+    l3_enable_default_route_ecmp,
     l3_ndp_proxy,
     l3_port_ip_change_not_allowed,
     local_ip,
     logging,
     logging_resource,
     metering,
     metering_source_and_destination_filters,
     multiprovidernet,
     network,
     network_availability_zone,
     network_cascade_delete,
+    network_ha,
     network_ip_availability,
     network_mtu,
     network_mtu_writable,
     network_segment_range,
     pagination,
     port,
     port_device_profile,
```

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/_dummy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/_dummy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/address_group.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/address_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/address_scope.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/address_scope.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/agent.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/agent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/agent_resources_synced.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/agent_resources_synced.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/agent_sort_key.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/agent_sort_key.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/allowedaddresspairs.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/allowedaddresspairs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/auto_allocated_topology.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/availability_zone_filter.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/availability_zone_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/base.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     'default_quota',
     'description',
     'device_id',
     'device_owner',
     'dns_nameservers',
     'enable_dhcp',
     'enable_ndp_proxy',
+    'external_gateways',
     'fixed_ips',
     'gateway_ip',
     'host_routes',
     'id',
     'ip_version',
     'ipv6_address_mode',
     'ipv6_ra_mode',
@@ -78,24 +79,27 @@
 )
 
 KNOWN_EXTENSIONS = (
     'address-scope',
     'agent',
     'agent-resources-synced',
     'allowed-address-pairs',
+    'allowed-address-pairs-atomic',
     'auto-allocated-topology',
     'availability_zone',
     'binding',
     'data-plane-status',
     'project-default-networks',
     'default-subnetpools',
     'dhcp_agent_scheduler',
     'dns-domain-ports',
     'dns-integration',
     'dvr',
+    'enable-default-route-ecmp',
+    'enable-default-route-bfd',
     'empty-string-filtering',
     'expose-l3-conntrack-helper',
     'expose-port-forwarding-in-fip',
     'ext-gw-mode',
     'external-net',
     'extra_dhcp_opt',
     'extraroute',
@@ -114,14 +118,15 @@
     'l3-ext-ndp-proxy',
     'l3-ndp-proxy',
     'l3-port-ip-change-not-allowed',
     'logging',
     'metering',
     'metering_source_and_destination_filters',
     'multi-provider',
+    'external-gateway-multihoming',
     'net-mtu',
     'network-ip-availability',
     'network-segment-range',
     'network_availability_zone',
     'pagination',
     'port-mac-address-override',
     'port-resource-request',
@@ -152,14 +157,15 @@
     'router_availability_zone',
     'security-group',
     'segment',
     'service-type',
     'sort-key-validation',
     'sorting',
     'standard-attr-description',
+    'standard-attr-fwaas-v2',
     'standard-attr-revisions',
     'standard-attr-segment',
     'standard-attr-timestamp',
     'subnet',
     'subnet_allocation',
     'subnet_dns_publish_fixed_ip',
     'subnet_onboard',
```

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgp.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgp.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgp_4byte_asn.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgp_4byte_asn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgp_dragentscheduler.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgp_dragentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_routes_control.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_routes_control.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_net_assoc.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_net_assoc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_port_assoc.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_port_assoc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_stdattrs_router_assoc.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_stdattrs_router_assoc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/bgpvpn_vni.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/bgpvpn_vni.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/constants.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/data_plane_status.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/data_plane_status.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/default_subnetpools.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/default_subnetpools.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/dhcpagentscheduler.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/dhcpagentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/dns.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/dns.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/dns_domain_keywords.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/dns_domain_keywords.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/dns_domain_ports.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/dns_domain_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/dvr.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/ecmp_routes.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/ecmp_routes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/empty_string_filtering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/empty_string_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/expose_l3_conntrack_helper.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/expose_l3_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/expose_port_forwarding_in_fip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/expose_port_forwarding_in_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/external_net.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/external_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/extra_dhcp_opt.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/extra_dhcp_opt.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/extraroute.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/extraroute.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/extraroute_atomic.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/extraroute_atomic.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/filter_validation.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/filter_validation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip64.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip64.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip_distributed.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip_distributed.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_description.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_description.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_detail.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_detail.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip_pf_port_range.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip_pf_port_range.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/fip_port_details.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/fip_port_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/firewall_v2.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/firewall_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/flavors.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/floating_ip_port_forwarding.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/floating_ip_port_forwarding.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/floatingip_autodelete_internal.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/floatingip_autodelete_internal.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/floatingip_pools.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/floatingip_pools.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/flowclassifier.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/flowclassifier.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/ip_allocation.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/ip_allocation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/ip_substring_port_filtering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/ip_substring_port_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l2_adjacency.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l2_adjacency.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_conntrack_helper.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_gw_mode.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_gw_mode.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_ha_mode.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_ha_mode.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ext_ndp_proxy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ext_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_flavors.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_ndp_proxy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/l3_port_ip_change_not_allowed.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/l3_port_ip_change_not_allowed.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/local_ip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/logging.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/logging.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/logging_resource.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/logging_resource.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/metering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/metering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/metering_source_and_destination_filters.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/metering_source_and_destination_filters.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/multiprovidernet.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/multiprovidernet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_cascade_delete.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_cascade_delete.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_ip_availability.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_mtu.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_mtu.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_mtu_writable.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_mtu_writable.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/network_segment_range.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/network_segment_range.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/pagination.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/pagination.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_device_profile.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_device_profile.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_hint_ovs_tx_steering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_hint_ovs_tx_steering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_hints.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_hints.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_mac_address_override.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_mac_address_override.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_mac_address_regenerate.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_mac_address_regenerate.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_numa_affinity_policy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_numa_affinity_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_resource_request.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_resource_request.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_resource_request_groups.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_resource_request_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/port_security.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/port_security.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/portbindings.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/portbindings.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/portbindings_extended.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/portbindings_extended.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/project_default_networks.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/project_default_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/project_id.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/project_id.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/provider_net.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/provider_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_bw_limit_direction.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_bw_limit_direction.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_bw_minimum_ingress.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_bw_minimum_ingress.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_default.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_default.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_fip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_fip_network_policy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_fip_network_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_gateway_ip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_bgpvpn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,46 @@
-#
+#    Copyright (c) 2021 Cloudification GmbH.  All rights reserved.
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from neutron_lib.api import converters
-from neutron_lib.api.definitions import l3
-from neutron_lib.api.definitions import l3_ext_gw_mode
-from neutron_lib.api.definitions import qos
-from neutron_lib.services.qos import constants as qos_consts
+from neutron_lib.api.definitions import bgpvpn
+from neutron_lib import constants
 
 
-ALIAS = 'qos-gateway-ip'
+ALIAS = 'rbac-bgpvpn'
 IS_SHIM_EXTENSION = False
 IS_STANDARD_ATTR_EXTENSION = False
-NAME = 'Router gateway IP QoS'
-API_PREFIX = ''
-DESCRIPTION = 'The Router gateway IP Quality of Service extension'
-UPDATED_TIMESTAMP = '2018-02-24T00:00:00-00:00'
-RESOURCE_NAME = l3.ROUTER
-COLLECTION_NAME = l3.ROUTERS
+NAME = 'Add bgpvpn type to RBAC'
+DESCRIPTION = 'Add bgpvpn type to RBAC'
+UPDATED_TIMESTAMP = '2021-06-07T00:00:00-00:00'
+API_PREFIX = bgpvpn.API_PREFIX
+RESOURCE_NAME = bgpvpn.RESOURCE_NAME
+COLLECTION_NAME = bgpvpn.COLLECTION_NAME
 RESOURCE_ATTRIBUTE_MAP = {
     COLLECTION_NAME: {
-        l3.EXTERNAL_GW_INFO: {
-            'allow_post': True,
-            'allow_put': True,
+        constants.SHARED: {
+            'allow_post': False,
+            'allow_put': False,
+            'default': False,
+            'convert_to': converters.convert_to_boolean,
             'is_visible': True,
-            'default': None,
-            'enforce_policy': True,
-            'validate': {
-                'type:dict_or_nodata': {
-                    'network_id': {'type:uuid': None, 'required': True},
-                    'enable_snat': {'type:boolean': None, 'required': False,
-                                    'convert_to':
-                                        converters.convert_to_boolean},
-                    'external_fixed_ips': {
-                        'type:fixed_ips': None,
-                        'required': False
-                    },
-                    qos_consts.QOS_POLICY_ID: {
-                        'type:uuid_or_none': None,
-                        'required': False
-                    }
-                }
-            }
+            'is_filter': True,
+            'is_sort_key': True,
+            'enforce_policy': True
         }
-    }
+    },
 }
 SUB_RESOURCE_ATTRIBUTE_MAP = {}
 ACTION_MAP = {}
-REQUIRED_EXTENSIONS = [l3.ALIAS, qos.ALIAS, l3_ext_gw_mode.ALIAS]
+REQUIRED_EXTENSIONS = ['rbac-policies', bgpvpn.ALIAS]
 OPTIONAL_EXTENSIONS = []
 ACTION_STATUS = {}
```

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_port_network_policy.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_port_network_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_minimum_rule.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_minimum_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_minimum_rule_alias.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_minimum_rule_alias.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_pps_rule.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_pps_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rule_type_details.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rule_type_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rule_type_filter.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rule_type_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/qos_rules_alias.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/qos_rules_alias.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/quota_check_limit.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/quota_check_limit.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_address_groups.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_address_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_address_scope.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_address_scope.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_bgpvpn.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/vpn_flavors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-#    Copyright (c) 2021 Cloudification GmbH.  All rights reserved.
+# Copyright 2017 Eayun, Inc.
+#
 #    Licensed under the Apache License, Version 2.0 (the "License"); you may
 #    not use this file except in compliance with the License. You may obtain
 #    a copy of the License at
 #
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+#
 
-from neutron_lib.api import converters
-from neutron_lib.api.definitions import bgpvpn
-from neutron_lib import constants
+from neutron_lib.api.definitions import flavors
+from neutron_lib.api.definitions import vpn
 
+FLAVOR_ID = 'flavor_id'
 
-ALIAS = 'rbac-bgpvpn'
+ALIAS = 'vpn-flavors'
 IS_SHIM_EXTENSION = False
 IS_STANDARD_ATTR_EXTENSION = False
-NAME = 'Add bgpvpn type to RBAC'
-DESCRIPTION = 'Add bgpvpn type to RBAC'
-UPDATED_TIMESTAMP = '2021-06-07T00:00:00-00:00'
-API_PREFIX = bgpvpn.API_PREFIX
-RESOURCE_NAME = bgpvpn.RESOURCE_NAME
-COLLECTION_NAME = bgpvpn.COLLECTION_NAME
+NAME = 'VPN Service Falvor Extension'
+DESCRIPTION = 'Flavor support for vpnservices.'
+UPDATED_TIMESTAMP = '2017-04-19T00:00:00-00:00'
+API_PREFIX = '/vpn'
+RESOURCE_NAME = vpn.VPNSERVICE
+COLLECTION_NAME = vpn.VPNSERVICES
 RESOURCE_ATTRIBUTE_MAP = {
     COLLECTION_NAME: {
-        constants.SHARED: {
-            'allow_post': False,
-            'allow_put': False,
-            'default': False,
-            'convert_to': converters.convert_to_boolean,
-            'is_visible': True,
-            'is_filter': True,
-            'is_sort_key': True,
-            'enforce_policy': True
-        }
+        FLAVOR_ID: {'allow_post': True, 'allow_put': False,
+                    'validate': {'type:uuid_or_none': None},
+                    'is_visible': True, 'default': None}
     },
 }
 SUB_RESOURCE_ATTRIBUTE_MAP = {}
 ACTION_MAP = {}
-REQUIRED_EXTENSIONS = ['rbac-policies', bgpvpn.ALIAS]
-OPTIONAL_EXTENSIONS = []
+REQUIRED_EXTENSIONS = [vpn.ALIAS]
+OPTIONAL_EXTENSIONS = [flavors.ALIAS]
 ACTION_STATUS = {}
```

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_security_groups.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/rbac_subnetpool.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/rbac_subnetpool.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/revisionifmatch.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/revisionifmatch.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/router_admin_state_down_before_update.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/router_admin_state_down_before_update.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/router_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/router_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/router_interface_fip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/router_interface_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/routerservicetype.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/routerservicetype.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_normalized_cidr.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_normalized_cidr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_port_filtering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_port_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_remote_address_group.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_remote_address_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/security_groups_shared_filtering.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/security_groups_shared_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/segment.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/segment.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/segments_peer_subnet_host_routes.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/segments_peer_subnet_host_routes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/servicetype.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/servicetype.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/sfc.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/sfc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/sort_key_validation.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/sort_key_validation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/sorting.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/sorting.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/standard_attr_segment.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/standard_attr_segment.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/stateful_security_group.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/stateful_security_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_dns_publish_fixed_ip.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_dns_publish_fixed_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_onboard.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_onboard.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_segmentid_enforce.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_segmentid_enforce.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_segmentid_writable.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_segmentid_writable.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnet_service_types.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnet_service_types.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnetpool.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnetpool.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/subnetpool_prefix_ops.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/subnetpool_prefix_ops.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/taas.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/taas.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/tag_ports_during_bulk_creation.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/tag_ports_during_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/trunk.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/trunk_details.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/trunk_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/uplink_status_propagation.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/uplink_status_propagation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/vlan_filter.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/vlan_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/vlantransparent.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/vlantransparent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/vpn.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/vpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/definitions/vpn_endpoint_groups.py` & `neutron-lib-3.6.0/neutron_lib/api/definitions/vpn_endpoint_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/extensions.py` & `neutron-lib-3.6.0/neutron_lib/api/extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/faults.py` & `neutron-lib-3.6.0/neutron_lib/api/faults.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/validators/__init__.py` & `neutron-lib-3.6.0/neutron_lib/api/validators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from oslo_utils import uuidutils
 from webob import exc
 
 from neutron_lib._i18n import _
 from neutron_lib import constants
 from neutron_lib import exceptions as n_exc
 from neutron_lib.plugins import directory
-
+from neutron_lib.services.qos import constants as qos_consts
 
 LOG = logging.getLogger(__name__)
 
 # Used by range check to indicate no limit for a bound.
 UNLIMITED = None
 
 # Note: In order to ensure that the MAC address is unicast the first byte
@@ -1211,14 +1211,50 @@
         msg_data = {'ethertype': ethertype, 'valid_ethertypes': valids}
         msg = ("Ethertype %(ethertype)s is not a valid ethertype, must be "
                "one of %(valid_ethertypes)s.")
         LOG.debug(msg, msg_data)
         return _(msg) % msg_data
 
 
+def validate_external_gw_info(data, valid_values=None):
+    """Validate data is an external_gateway_info.
+
+    :param data: The data to validate.
+    :param valid_values: Not used!
+    :returns: None if valid, error string otherwise.
+    """
+    # See https://github.com/PyCQA/pylint/issues/850
+    # pylint: disable=import-outside-toplevel,cyclic-import
+    from neutron_lib.api import converters
+    return validate_dict_or_nodata(
+        data,
+        key_specs={
+            'network_id': {'type:uuid': None, 'required': True},
+            'external_fixed_ips': {'type:fixed_ips': None, 'required': False},
+            'enable_snat': {'type:boolean': None, 'required': False,
+                            'convert_to': converters.convert_to_boolean},
+            qos_consts.QOS_POLICY_ID: {
+                'type:uuid_or_none': None,
+                'required': False
+            }
+        }
+    )
+
+
+def validate_external_gw_info_list(data, valid_values=None):
+    """Validate data is a list of external_gateway_info.
+
+    :param data: The data to validate.
+    :param valid_values: Not used!
+    :returns: None if valid, error string otherwise.
+    """
+    if data is not None:
+        return _validate_list_of_items(validate_external_gw_info, data)
+
+
 # Dictionary that maintains a list of validation functions
 validators = {'type:dict': validate_dict,
               'type:dict_or_none': validate_dict_or_none,
               'type:dict_or_empty': validate_dict_or_empty,
               'type:dict_or_nodata': validate_dict_or_nodata,
               'type:ethertype': validate_ethertype,
               'type:fixed_ips': validate_fixed_ips,
@@ -1261,15 +1297,17 @@
               'type:integer': validate_integer,
               'type:list_of_unique_strings': validate_list_of_unique_strings,
               'type:list_of_any_key_specs_or_none':
                   validate_any_key_specs_or_none,
               'type:service_plugin_type': validate_service_plugin_type,
               'type:list_of_subnets_or_none': validate_subnet_list_or_none,
               'type:list_of_subnet_service_types':
-                  validate_subnet_service_types
+                  validate_subnet_service_types,
+              'type:external_gw_info': validate_external_gw_info,
+              'type:external_gw_info_list': validate_external_gw_info_list,
               }
 
 
 class UndefinedValidator(Exception):
 
     def __init__(self, validator_name):
         self.validator_name = validator_name
```

### Comparing `neutron-lib-3.5.0/neutron_lib/api/validators/allowedaddresspairs.py` & `neutron-lib-3.6.0/neutron_lib/api/validators/allowedaddresspairs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/validators/availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/api/validators/availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/validators/dns.py` & `neutron-lib-3.6.0/neutron_lib/api/validators/dns.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/api/validators/multiprovidernet.py` & `neutron-lib-3.6.0/neutron_lib/api/validators/multiprovidernet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/events.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/events.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/exceptions.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/manager.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/priority_group.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/priority_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/registry.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/registry.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/callbacks/resources.py` & `neutron-lib-3.6.0/neutron_lib/callbacks/resources.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/constants.py` & `neutron-lib-3.6.0/neutron_lib/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,16 @@
 
 DVR_SNAT_BOUND = 'dvr_snat_bound'
 PORT_BINDING_EXT_ALIAS = 'binding'
 L3_AGENT_SCHEDULER_EXT_ALIAS = 'l3_agent_scheduler'
 DHCP_AGENT_SCHEDULER_EXT_ALIAS = 'dhcp_agent_scheduler'
 L3_DISTRIBUTED_EXT_ALIAS = 'dvr'
 L3_HA_MODE_EXT_ALIAS = 'l3-ha'
+L3_ENABLE_DEFAULT_ROUTE_ECMP_ALIAS = 'enable-default-route-ecmp'
+L3_ENABLE_DEFAULT_ROUTE_BFD_ALIAS = 'enable-default-route-bfd'
 SUBNET_ALLOCATION_EXT_ALIAS = 'subnet_allocation'
 
 # Protocol names and numbers for Security Groups/Firewalls
 PROTO_NAME_AH = 'ah'
 PROTO_NAME_DCCP = 'dccp'
 PROTO_NAME_EGP = 'egp'
 PROTO_NAME_ESP = 'esp'
@@ -621,15 +623,15 @@
 # When configuring an address on an interface.
 # When adding a route.
 METADATA_V4_CIDR = '169.254.169.254/32'
 # When checking if a metadata subnet is present.
 METADATA_V4_SUBNET = '169.254.0.0/16'
 
 METADATA_V6_IP = 'fe80::a9fe:a9fe'
-METADATA_V6_CIDR = 'fe80::a9fe:a9fe/64'
+METADATA_V6_CIDR = 'fe80::a9fe:a9fe/128'
 
 METADATA_PORT = 80
 
 # For backwards compatibility, prefer METADATA_V4_CIDR instead.
 METADATA_CIDR = METADATA_V4_CIDR
 
 # The only defined IpamAllocation status at this stage is 'ALLOCATED'.
```

### Comparing `neutron-lib-3.5.0/neutron_lib/context.py` & `neutron-lib-3.6.0/neutron_lib/context.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/api.py` & `neutron-lib-3.6.0/neutron_lib/db/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,15 @@
 
 
 @_synchronized("context-manager")
 def _create_context_manager():
     global _CTX_MANAGER
     if _CTX_MANAGER is None:
         _CTX_MANAGER = enginefacade.transaction_context()
-        # TODO(stephenfin): Drop "__autocommit=False" when oslo.db changes its
-        # default (https://review.opendev.org/c/openstack/oslo.db/+/804775)
-        _CTX_MANAGER.configure(sqlite_fk=True, flush_on_subtransaction=True,
-                               __autocommit=False)
+        _CTX_MANAGER.configure(sqlite_fk=True, flush_on_subtransaction=True)
 
     return _CTX_MANAGER
 
 
 def get_context_manager():
     """Transaction Context Manager accessor.
```

### Comparing `neutron-lib-3.5.0/neutron_lib/db/constants.py` & `neutron-lib-3.6.0/neutron_lib/db/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/model_base.py` & `neutron-lib-3.6.0/neutron_lib/db/model_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,22 @@
     """Project mixin, add to subclasses that have a user."""
 
     # NOTE: project_id is just a free form string
     project_id = sa.Column(sa.String(db_const.PROJECT_ID_FIELD_SIZE),
                            nullable=False, primary_key=True)
 
 
+class HasProjectPrimaryUniqueKey(HasProject):
+    """Project mixin, add to subclasses that have a user."""
+
+    # NOTE: project_id is just a free form string
+    project_id = sa.Column(sa.String(db_const.PROJECT_ID_FIELD_SIZE),
+                           nullable=False, primary_key=True, unique=True)
+
+
 class HasId(object):
     """id mixin, add to subclasses that have an id."""
 
     id = sa.Column(sa.String(db_const.UUID_FIELD_SIZE),
                    primary_key=True,
                    default=uuidutils.generate_uuid)
```

### Comparing `neutron-lib-3.5.0/neutron_lib/db/model_query.py` & `neutron-lib-3.6.0/neutron_lib/db/model_query.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/quota_api.py` & `neutron-lib-3.6.0/neutron_lib/db/quota_api.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/resource_extend.py` & `neutron-lib-3.6.0/neutron_lib/db/resource_extend.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/sqlalchemytypes.py` & `neutron-lib-3.6.0/neutron_lib/db/sqlalchemytypes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/standard_attr.py` & `neutron-lib-3.6.0/neutron_lib/db/standard_attr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/db/utils.py` & `neutron-lib-3.6.0/neutron_lib/db/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/__init__.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/address_group.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/address_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/address_scope.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/address_scope.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/agent.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/agent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/allowedaddresspairs.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/allowedaddresspairs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/dhcpagentscheduler.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/dhcpagentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/dns.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/dns.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/dvr.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/external_net.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/external_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/extraroute.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/extraroute.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/firewall_v2.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/firewall_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/flavors.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/l3.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/l3.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/l3_ext_ha_mode.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/l3_ext_ha_mode.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/local_ip.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/metering.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/metering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/multiprovidernet.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/multiprovidernet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/network_segment_range.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/network_segment_range.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/placement.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/placement.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/port_security.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/port_security.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/qos.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/qos.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/taas.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/taas.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/vlantransparent.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/vlantransparent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/exceptions/vpn.py` & `neutron-lib-3.6.0/neutron_lib/exceptions/vpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/fixture.py` & `neutron-lib-3.6.0/neutron_lib/fixture.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/hacking/checks.py` & `neutron-lib-3.6.0/neutron_lib/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/hacking/translation_checks.py` & `neutron-lib-3.6.0/neutron_lib/hacking/translation_checks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/locale/zh_CN/LC_MESSAGES/neutron_lib.po` & `neutron-lib-3.6.0/neutron_lib/locale/zh_CN/LC_MESSAGES/neutron_lib.po`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/common_types.py` & `neutron-lib-3.6.0/neutron_lib/objects/common_types.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/exceptions.py` & `neutron-lib-3.6.0/neutron_lib/objects/exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/extensions/standardattributes.py` & `neutron-lib-3.6.0/neutron_lib/objects/extensions/standardattributes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/logapi/event_types.py` & `neutron-lib-3.6.0/neutron_lib/objects/logapi/event_types.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/registry.py` & `neutron-lib-3.6.0/neutron_lib/objects/registry.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/objects/utils.py` & `neutron-lib-3.6.0/neutron_lib/objects/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/placement/client.py` & `neutron-lib-3.6.0/neutron_lib/placement/client.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/placement/constants.py` & `neutron-lib-3.6.0/neutron_lib/placement/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/placement/utils.py` & `neutron-lib-3.6.0/neutron_lib/placement/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/plugins/constants.py` & `neutron-lib-3.6.0/neutron_lib/plugins/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/plugins/directory.py` & `neutron-lib-3.6.0/neutron_lib/plugins/directory.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/plugins/ml2/api.py` & `neutron-lib-3.6.0/neutron_lib/plugins/ml2/api.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/plugins/ml2/ovs_constants.py` & `neutron-lib-3.6.0/neutron_lib/plugins/ml2/ovs_constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,16 +210,20 @@
 EXTENSION_DRIVER_TYPE = 'ovs'
 
 # ovs datapath types
 OVS_DATAPATH_SYSTEM = 'system'
 OVS_DATAPATH_NETDEV = 'netdev'
 OVS_DPDK_VHOST_USER = 'dpdkvhostuser'
 OVS_DPDK_VHOST_USER_CLIENT = 'dpdkvhostuserclient'
+OVS_DPDK = 'dpdk'
 
-OVS_DPDK_PORT_TYPES = [OVS_DPDK_VHOST_USER, OVS_DPDK_VHOST_USER_CLIENT]
+OVS_DPDK_PORT_TYPES = [OVS_DPDK_VHOST_USER,
+                       OVS_DPDK_VHOST_USER_CLIENT,
+                       OVS_DPDK,
+                       ]
 
 # default ovs vhost-user socket location
 VHOST_USER_SOCKET_DIR = '/var/run/openvswitch'
 
 MAX_DEVICE_RETRIES = 5
 
 # OpenFlow version constants
```

### Comparing `neutron-lib-3.5.0/neutron_lib/plugins/utils.py` & `neutron-lib-3.6.0/neutron_lib/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/policy/__init__.py` & `neutron-lib-3.6.0/neutron_lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/policy/_engine.py` & `neutron-lib-3.6.0/neutron_lib/policy/_engine.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/rpc.py` & `neutron-lib-3.6.0/neutron_lib/rpc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/base.py` & `neutron-lib-3.6.0/neutron_lib/services/base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/constants.py` & `neutron-lib-3.6.0/neutron_lib/services/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/logapi/constants.py` & `neutron-lib-3.6.0/neutron_lib/services/logapi/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/qos/base.py` & `neutron-lib-3.6.0/neutron_lib/services/qos/base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/qos/constants.py` & `neutron-lib-3.6.0/neutron_lib/services/qos/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/services/trunk/constants.py` & `neutron-lib-3.6.0/neutron_lib/services/trunk/constants.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/_base.py` & `neutron-lib-3.6.0/neutron_lib/tests/_base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/_post_mortem_debug.py` & `neutron-lib-3.6.0/neutron_lib/tests/_post_mortem_debug.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/tools.py` & `neutron-lib-3.6.0/neutron_lib/tests/tools.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/agent/common/test_utils.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/agent/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/base.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/ip_allocation.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/ip_allocation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test__dummy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test__dummy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_address_group.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_address_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_address_scope.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_address_scope.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_admin_state_down_before_update.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_admin_state_down_before_update.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent_resources_synced.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent_resources_synced.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_agent_sort_key.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_agent_sort_key.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_auto_allocated_topology.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_auto_allocated_topology.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_availability_zone_filter.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_availability_zone_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp_4byte_asn.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp_4byte_asn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgp_dragentscheduler.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgp_dragentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_net_assoc_stdattrs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_net_assoc_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_port_assoc_stdattrs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_port_assoc_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_router_assoc_stdattrs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_router_assoc_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_routes_control.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_routes_control.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_stdattrs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_stdattrs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_vni.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_bgpvpn_vni.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_data_plane_status.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_data_plane_status.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_default_subnetpools.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_default_subnetpools.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dhcpagentscheduler.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dhcpagentscheduler.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dns.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dns.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dns_domain_ports.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dns_domain_ports.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_dvr.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_dvr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_empty_string_filtering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_empty_string_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_expose_l3_conntrack_helper.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_expose_l3_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_expose_port_forwarding_in_fip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_expose_port_forwarding_in_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_external_net.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_external_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extra_dhcp_opt.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extra_dhcp_opt.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extraroute.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extraroute.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_extraroute_atomic.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_extraroute_atomic.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_filter_validation.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_filter_validation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip64.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip64.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip_distributed.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip_distributed.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_fip_port_details.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_fip_port_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_firewall_v2.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_firewall_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_flavors.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_extension.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_extension.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_port_range.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_port_range.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floatingip_autodelete_internal.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floatingip_autodelete_internal.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_floatingip_pools.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_floatingip_pools.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_flowclassifier.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_flowclassifier.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_ip_substring_port_filtering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_ip_substring_port_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l2_adjancency.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l2_adjancency.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_conntrack_helper.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_conntrack_helper.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_gw_mode.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_gw_mode.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ha_mode.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ha_mode.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ndp_proxy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ext_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_flavors.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_ndp_proxy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_ndp_proxy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_l3_port_ip_change_not_allowed.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_l3_port_ip_change_not_allowed.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_local_ip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_local_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_logging.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_logging.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_logging_resource.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_logging_resource.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_metering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_metering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_metering_source_and_destination_filters.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_metering_source_and_destination_filters.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_multiprovidernet.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_multiprovidernet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_cascade_delete.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_cascade_delete.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_ip_availability.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_ip_availability.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_mtu.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_mtu.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_mtu_writable.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_mtu_writable.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_network_segment_range.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_network_segment_range.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_pagination.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_pagination.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_device_profile.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_device_profile.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_hint_ovs_tx_steering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_hint_ovs_tx_steering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_hints.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_hints.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_mac_address_regenerate.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_mac_address_regenerate.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_numa_affinity_policy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_numa_affinity_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request_groups.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_resource_request_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_port_security.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_port_security.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_portbindings.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_portbindings.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_portbindings_extended.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_portbindings_extended.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_project_default_networks.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_project_default_networks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_project_id.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_project_id.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_provider_net.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_provider_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_limit_direction.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_limit_direction.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_minimum_ingress.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_bw_minimum_ingress.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_default.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_default.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_fip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_fip_network_policy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_fip_network_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_gateway_ip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_gateway_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_port_network_policy.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_port_network_policy.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule_alias.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_minimum_rule_alias.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_rule.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_pps_rule.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_details.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_filter.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rule_type_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_qos_rules_alias.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_qos_rules_alias.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_quota_check_limit.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_quota_check_limit.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_groups.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_scope.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_address_scope.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_bgpvpn.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_bgpvpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_security_groups.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_security_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_rbac_subnetpool.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_rbac_subnetpool.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_revisionifmatch.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_revisionifmatch.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_router_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_router_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_router_interface_fip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_router_interface_fip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_routerservicetype.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_routerservicetype.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_normalized_cidr.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_normalized_cidr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_port_filtering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_port_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_remote_address_group.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_remote_address_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_security_groups_shared_filtering.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_security_groups_shared_filtering.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_segment.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_segment.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_segment_peer_subnet_host_routes.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_segment_peer_subnet_host_routes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_servicetype.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_servicetype.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sfc.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sfc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sort_key_validation.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sort_key_validation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_sorting.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_sorting.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_standard_attr_segment.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_standard_attr_segment.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_stateful_security_group.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_stateful_security_group.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_dns_publish_fixed_ip.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_dns_publish_fixed_ip.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_onboard.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_onboard.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_enforce.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_enforce.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_writable.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_segmentid_writable.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnet_service_types.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnet_service_types.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnetpool.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnetpool.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_subnetpool_prefix_ops.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_subnetpool_prefix_ops.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_taas.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_taas.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_tag_ports_during_bulk_creation.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_tag_ports_during_bulk_creation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_trunk.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_trunk.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_trunk_details.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_trunk_details.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_uplink_status_propagation.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_uplink_status_propagation.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vlan_filter.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vlan_filter.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vlantransparent.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vlantransparent.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn_endpoint_groups.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn_endpoint_groups.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/definitions/test_vpn_flavors.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/definitions/test_vpn_flavors.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_attributes.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_attributes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_conversions.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_conversions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_extensions.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_extensions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/test_faults.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/test_faults.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_allowedaddresspairs.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_allowedaddresspairs.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_availability_zone.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_dns.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_dns.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_multiprovidernet.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_multiprovidernet.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/api/validators/test_validators.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/api/validators/test_validators.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_callback_exceptions.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_callback_exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_events.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_events.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_manager.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_manager.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/callbacks/test_registry.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/callbacks/test_registry.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/_base.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/_base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_api.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_api.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_model_base.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_model_base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_model_query.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_model_query.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_resource_extend.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_resource_extend.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_sqlalchemytypes.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_sqlalchemytypes.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_standard_attr.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_standard_attr.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/db/test_utils.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/db/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/exceptions/test_exceptions.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/exceptions/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/fake_notifier.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/fake_notifier.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/hacking/test_checks.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/hacking/test_checks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/objects/test_common_types.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/objects/test_common_types.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/objects/test_utils.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/objects/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/placement/test_client.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/placement/test_client.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/placement/test_utils.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/placement/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/ml2/test_api.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/ml2/test_api.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/test_directory.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/test_directory.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/plugins/test_utils.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/plugins/test_utils.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/policy/test__engine.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/policy/test__engine.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/services/qos/test_base.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/services/qos/test_base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/services/test_base.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/services/test_base.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/test_context.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/test_fixture.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/test_fixture.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/test_neutron_lib.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/test_neutron_lib.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/test_rpc.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/test_rpc.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/test_worker.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/test_worker.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_file.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_helpers.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_host.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_host.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_net.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_runtime.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_runtime.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/tests/unit/utils/test_test.py` & `neutron-lib-3.6.0/neutron_lib/tests/unit/utils/test_test.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/file.py` & `neutron-lib-3.6.0/neutron_lib/utils/file.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/helpers.py` & `neutron-lib-3.6.0/neutron_lib/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/host.py` & `neutron-lib-3.6.0/neutron_lib/utils/host.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/net.py` & `neutron-lib-3.6.0/neutron_lib/utils/net.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/runtime.py` & `neutron-lib-3.6.0/neutron_lib/utils/runtime.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/test.py` & `neutron-lib-3.6.0/neutron_lib/utils/test.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/utils/upgrade_checks.py` & `neutron-lib-3.6.0/neutron_lib/utils/upgrade_checks.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/version.py` & `neutron-lib-3.6.0/neutron_lib/version.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib/worker.py` & `neutron-lib-3.6.0/neutron_lib/worker.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/neutron_lib.egg-info/PKG-INFO` & `neutron-lib-3.6.0/neutron_lib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-lib
-Version: 3.5.0
+Version: 3.6.0
 Summary: Neutron shared routines and utilities
 Home-page: https://docs.openstack.org/neutron-lib/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `neutron-lib-3.5.0/neutron_lib.egg-info/SOURCES.txt` & `neutron-lib-3.6.0/neutron_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -297,21 +297,25 @@
 api-ref/source/v2/samples/networks/versions-list-response.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-create-request.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-create-response.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-list-response.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-show-response.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-update-request.json
 api-ref/source/v2/samples/port_forwardings/port-fowarding-update-response.json
+api-ref/source/v2/samples/ports/port-add-allowed-address-pairs-request.json
+api-ref/source/v2/samples/ports/port-add-allowed-address-pairs-response.json
 api-ref/source/v2/samples/ports/port-bind-create-request.json
 api-ref/source/v2/samples/ports/port-bind-create-response.json
 api-ref/source/v2/samples/ports/port-bind-show-response.json
 api-ref/source/v2/samples/ports/port-bind-update-request.json
 api-ref/source/v2/samples/ports/port-bind-update-response.json
 api-ref/source/v2/samples/ports/port-create-request.json
 api-ref/source/v2/samples/ports/port-create-response.json
+api-ref/source/v2/samples/ports/port-remove-allowed-address-pairs-request.json
+api-ref/source/v2/samples/ports/port-remove-allowed-address-pairs-response.json
 api-ref/source/v2/samples/ports/port-resource-request-new-format.json
 api-ref/source/v2/samples/ports/port-show-response.json
 api-ref/source/v2/samples/ports/port-update-request.json
 api-ref/source/v2/samples/ports/port-update-response.json
 api-ref/source/v2/samples/ports/ports-bind-list-response.json
 api-ref/source/v2/samples/ports/ports-bulk-create-request.json
 api-ref/source/v2/samples/ports/ports-bulk-create-response.json
@@ -362,27 +366,33 @@
 api-ref/source/v2/samples/quotas/quotas-update-response.json
 api-ref/source/v2/samples/rbac_policy/rbac-policies-list-response.json
 api-ref/source/v2/samples/rbac_policy/rbac-policy-create-request.json
 api-ref/source/v2/samples/rbac_policy/rbac-policy-create-response.json
 api-ref/source/v2/samples/rbac_policy/rbac-policy-show-response.json
 api-ref/source/v2/samples/rbac_policy/rbac-policy-update-request.json
 api-ref/source/v2/samples/rbac_policy/rbac-policy-update-response.json
+api-ref/source/v2/samples/routers/router-add-external-gateways-request.json
+api-ref/source/v2/samples/routers/router-add-external-gateways-response.json
 api-ref/source/v2/samples/routers/router-add-extraroutes-request.json
 api-ref/source/v2/samples/routers/router-add-extraroutes-response.json
 api-ref/source/v2/samples/routers/router-add-interface-request-with-port.json
 api-ref/source/v2/samples/routers/router-add-interface-request.json
 api-ref/source/v2/samples/routers/router-add-interface-response.json
 api-ref/source/v2/samples/routers/router-create-request.json
 api-ref/source/v2/samples/routers/router-create-response.json
+api-ref/source/v2/samples/routers/router-remove-external-gateways-request.json
+api-ref/source/v2/samples/routers/router-remove-external-gateways-response.json
 api-ref/source/v2/samples/routers/router-remove-extraroutes-request.json
 api-ref/source/v2/samples/routers/router-remove-extraroutes-response.json
 api-ref/source/v2/samples/routers/router-remove-interface-request-with-port.json
 api-ref/source/v2/samples/routers/router-remove-interface-request.json
 api-ref/source/v2/samples/routers/router-remove-interface-response.json
 api-ref/source/v2/samples/routers/router-show-response.json
+api-ref/source/v2/samples/routers/router-update-external-gateways-request.json
+api-ref/source/v2/samples/routers/router-update-external-gateways-response.json
 api-ref/source/v2/samples/routers/router-update-request.json
 api-ref/source/v2/samples/routers/router-update-response.json
 api-ref/source/v2/samples/routers/routers-list-response.json
 api-ref/source/v2/samples/security-groups/security-group-create-request.json
 api-ref/source/v2/samples/security-groups/security-group-create-response.json
 api-ref/source/v2/samples/security-groups/security-group-delete-request-json-http.txt
 api-ref/source/v2/samples/security-groups/security-group-delete-response-json-http.txt
@@ -538,14 +548,15 @@
 neutron_lib/api/definitions/_dummy.py
 neutron_lib/api/definitions/address_group.py
 neutron_lib/api/definitions/address_scope.py
 neutron_lib/api/definitions/agent.py
 neutron_lib/api/definitions/agent_resources_synced.py
 neutron_lib/api/definitions/agent_sort_key.py
 neutron_lib/api/definitions/allowedaddresspairs.py
+neutron_lib/api/definitions/allowedaddresspairs_atomic.py
 neutron_lib/api/definitions/auto_allocated_topology.py
 neutron_lib/api/definitions/availability_zone.py
 neutron_lib/api/definitions/availability_zone_filter.py
 neutron_lib/api/definitions/base.py
 neutron_lib/api/definitions/bgp.py
 neutron_lib/api/definitions/bgp_4byte_asn.py
 neutron_lib/api/definitions/bgp_dragentscheduler.py
@@ -576,39 +587,44 @@
 neutron_lib/api/definitions/fip64.py
 neutron_lib/api/definitions/fip_distributed.py
 neutron_lib/api/definitions/fip_pf_description.py
 neutron_lib/api/definitions/fip_pf_detail.py
 neutron_lib/api/definitions/fip_pf_port_range.py
 neutron_lib/api/definitions/fip_port_details.py
 neutron_lib/api/definitions/firewall_v2.py
+neutron_lib/api/definitions/firewall_v2_stdattrs.py
 neutron_lib/api/definitions/flavors.py
 neutron_lib/api/definitions/floating_ip_port_forwarding.py
 neutron_lib/api/definitions/floatingip_autodelete_internal.py
 neutron_lib/api/definitions/floatingip_pools.py
 neutron_lib/api/definitions/flowclassifier.py
 neutron_lib/api/definitions/ip_allocation.py
 neutron_lib/api/definitions/ip_substring_port_filtering.py
 neutron_lib/api/definitions/l2_adjacency.py
 neutron_lib/api/definitions/l3.py
 neutron_lib/api/definitions/l3_conntrack_helper.py
+neutron_lib/api/definitions/l3_enable_default_route_bfd.py
+neutron_lib/api/definitions/l3_enable_default_route_ecmp.py
 neutron_lib/api/definitions/l3_ext_gw_mode.py
+neutron_lib/api/definitions/l3_ext_gw_multihoming.py
 neutron_lib/api/definitions/l3_ext_ha_mode.py
 neutron_lib/api/definitions/l3_ext_ndp_proxy.py
 neutron_lib/api/definitions/l3_flavors.py
 neutron_lib/api/definitions/l3_ndp_proxy.py
 neutron_lib/api/definitions/l3_port_ip_change_not_allowed.py
 neutron_lib/api/definitions/local_ip.py
 neutron_lib/api/definitions/logging.py
 neutron_lib/api/definitions/logging_resource.py
 neutron_lib/api/definitions/metering.py
 neutron_lib/api/definitions/metering_source_and_destination_filters.py
 neutron_lib/api/definitions/multiprovidernet.py
 neutron_lib/api/definitions/network.py
 neutron_lib/api/definitions/network_availability_zone.py
 neutron_lib/api/definitions/network_cascade_delete.py
+neutron_lib/api/definitions/network_ha.py
 neutron_lib/api/definitions/network_ip_availability.py
 neutron_lib/api/definitions/network_mtu.py
 neutron_lib/api/definitions/network_mtu_writable.py
 neutron_lib/api/definitions/network_segment_range.py
 neutron_lib/api/definitions/pagination.py
 neutron_lib/api/definitions/port.py
 neutron_lib/api/definitions/port_device_profile.py
@@ -712,14 +728,15 @@
 neutron_lib/exceptions/dns.py
 neutron_lib/exceptions/dvr.py
 neutron_lib/exceptions/external_net.py
 neutron_lib/exceptions/extraroute.py
 neutron_lib/exceptions/firewall_v2.py
 neutron_lib/exceptions/flavors.py
 neutron_lib/exceptions/l3.py
+neutron_lib/exceptions/l3_ext_gw_multihoming.py
 neutron_lib/exceptions/l3_ext_ha_mode.py
 neutron_lib/exceptions/local_ip.py
 neutron_lib/exceptions/metering.py
 neutron_lib/exceptions/multiprovidernet.py
 neutron_lib/exceptions/network_segment_range.py
 neutron_lib/exceptions/placement.py
 neutron_lib/exceptions/port_security.py
@@ -794,14 +811,15 @@
 neutron_lib/tests/unit/api/definitions/test_address_group.py
 neutron_lib/tests/unit/api/definitions/test_address_scope.py
 neutron_lib/tests/unit/api/definitions/test_admin_state_down_before_update.py
 neutron_lib/tests/unit/api/definitions/test_agent.py
 neutron_lib/tests/unit/api/definitions/test_agent_resources_synced.py
 neutron_lib/tests/unit/api/definitions/test_agent_sort_key.py
 neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs.py
+neutron_lib/tests/unit/api/definitions/test_allowedaddresspairs_atomic.py
 neutron_lib/tests/unit/api/definitions/test_auto_allocated_topology.py
 neutron_lib/tests/unit/api/definitions/test_availability_zone.py
 neutron_lib/tests/unit/api/definitions/test_availability_zone_filter.py
 neutron_lib/tests/unit/api/definitions/test_bgp.py
 neutron_lib/tests/unit/api/definitions/test_bgp_4byte_asn.py
 neutron_lib/tests/unit/api/definitions/test_bgp_dragentscheduler.py
 neutron_lib/tests/unit/api/definitions/test_bgpvpn.py
@@ -825,29 +843,33 @@
 neutron_lib/tests/unit/api/definitions/test_extraroute.py
 neutron_lib/tests/unit/api/definitions/test_extraroute_atomic.py
 neutron_lib/tests/unit/api/definitions/test_filter_validation.py
 neutron_lib/tests/unit/api/definitions/test_fip64.py
 neutron_lib/tests/unit/api/definitions/test_fip_distributed.py
 neutron_lib/tests/unit/api/definitions/test_fip_port_details.py
 neutron_lib/tests/unit/api/definitions/test_firewall_v2.py
+neutron_lib/tests/unit/api/definitions/test_firewall_v2_stdattrs.py
 neutron_lib/tests/unit/api/definitions/test_flavors.py
 neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding.py
 neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_extension.py
 neutron_lib/tests/unit/api/definitions/test_floating_ip_port_forwarding_port_range.py
 neutron_lib/tests/unit/api/definitions/test_floatingip_autodelete_internal.py
 neutron_lib/tests/unit/api/definitions/test_floatingip_pools.py
 neutron_lib/tests/unit/api/definitions/test_flowclassifier.py
 neutron_lib/tests/unit/api/definitions/test_ip_substring_port_filtering.py
 neutron_lib/tests/unit/api/definitions/test_l2_adjancency.py
 neutron_lib/tests/unit/api/definitions/test_l3.py
 neutron_lib/tests/unit/api/definitions/test_l3_conntrack_helper.py
+neutron_lib/tests/unit/api/definitions/test_l3_enable_default_route_bfd.py
+neutron_lib/tests/unit/api/definitions/test_l3_enable_default_route_ecmp.py
 neutron_lib/tests/unit/api/definitions/test_l3_ext_gw_mode.py
 neutron_lib/tests/unit/api/definitions/test_l3_ext_ha_mode.py
 neutron_lib/tests/unit/api/definitions/test_l3_ext_ndp_proxy.py
 neutron_lib/tests/unit/api/definitions/test_l3_flavors.py
+neutron_lib/tests/unit/api/definitions/test_l3_multi_ext_gw.py
 neutron_lib/tests/unit/api/definitions/test_l3_ndp_proxy.py
 neutron_lib/tests/unit/api/definitions/test_l3_port_ip_change_not_allowed.py
 neutron_lib/tests/unit/api/definitions/test_local_ip.py
 neutron_lib/tests/unit/api/definitions/test_logging.py
 neutron_lib/tests/unit/api/definitions/test_logging_resource.py
 neutron_lib/tests/unit/api/definitions/test_metering.py
 neutron_lib/tests/unit/api/definitions/test_metering_source_and_destination_filters.py
@@ -1004,14 +1026,15 @@
 releasenotes/notes/add-description-field-in-port-forwarding-9da781b1e38ca858.yaml
 releasenotes/notes/add-directory-is-loaded-e9da5b65824dddad.yaml
 releasenotes/notes/add-empty-string-filtering-api-extension-44cb392025dc359c.yaml
 releasenotes/notes/add-exception-pkg-5a14389891abf358.yaml
 releasenotes/notes/add-extension-address-group-5e306d90666982aa.yaml
 releasenotes/notes/add-extension-security-groups-normalized-cidr-ef7521b226090d7e.yaml
 releasenotes/notes/add-extension-security-groups-remote-address-group-c71dbb57b61a1dba.yaml
+releasenotes/notes/add-extension-standard-attr-fwaasv2-7e9250015afbe112.yaml
 releasenotes/notes/add-extension-standard-attr-segment-8c721741589bf10b.yaml
 releasenotes/notes/add-extension-supported-be6f7069856d2891.yaml
 releasenotes/notes/add-extension-uplink-status-propagation-6b6050d6609c19c8.yaml
 releasenotes/notes/add-filter-validation-api-extension-15cc667d5498f163.yaml
 releasenotes/notes/add-fip-distributed-extension-ce44e8df264d44b6.yaml
 releasenotes/notes/add-fip-pf-detail-extension-fa8cd3b3857901d7.yaml
 releasenotes/notes/add-floatingip-pools-extension-17a1ee5c7eafc989.yaml
@@ -1023,14 +1046,15 @@
 releasenotes/notes/add-is_sort_key-keyword-to-attribute-map-75342446d99f4490.yaml
 releasenotes/notes/add-local-ip-extension-fb4a18f5a6525f1f.yaml
 releasenotes/notes/add-network-address-scope-affinity-error-8f6b4493a92142d4.yaml
 releasenotes/notes/add-network-cascade-delete-api-extension-f418e44b37c2b2ed.yaml
 releasenotes/notes/add-network-segment-range-overlap-exception-e8b4b2b425c51c80.yaml
 releasenotes/notes/add-network-segment-range-plugin-constant-9e80453919162c89.yaml
 releasenotes/notes/add-ovo-registry-27cb7d4ac76d4dc8.yaml
+releasenotes/notes/add-ovs-port-type-dpdk-b00f5bda3161773f.yaml
 releasenotes/notes/add-placement-report-plugin-constant-a6a4146c2e39cba3.yaml
 releasenotes/notes/add-port-binding-resource-73f9800dbda121ca.yaml
 releasenotes/notes/add-port-bindings-resource-messages-rpc-1382ba9842561cdb.yaml
 releasenotes/notes/add-port-mac-address-override-shim-extension-fb11c4f40c12a99b.yaml
 releasenotes/notes/add-port-ranges-support-in-port-forwarding-417da8ef7e2ec140.yaml
 releasenotes/notes/add-port_details-to-floatingip-a2a3c95cc54737ac.yaml
 releasenotes/notes/add-quota-check-limit-api-extension-8e39299644d41f74.yaml
@@ -1056,14 +1080,15 @@
 releasenotes/notes/add_qos_pps_rule_api_def-dae7c6e67904781b.yaml
 releasenotes/notes/admin-state-down-before-update-c06fb3a551fe499f.yaml
 releasenotes/notes/advsvc-role-support-d4f1c532264b729a.yaml
 releasenotes/notes/agent-resources-synced-e70828841faf7acd.yaml
 releasenotes/notes/agent_extensions-2b497ff33c6dc3e8.yaml
 releasenotes/notes/alembic-branches-6d5947d141efd26e.yaml
 releasenotes/notes/allocations_api-1ae5fd78c83353df.yaml
+releasenotes/notes/allowedaddresspairs-atomic-apidef-6f9d6865854vwfrs
 releasenotes/notes/api-definition-base-d2e9514c5ee2ef5b.yaml
 releasenotes/notes/bgpvpn-api-def-22c7072575316ddd.yaml
 releasenotes/notes/bgpvpn-api-ref-f0294d9ddec726a0.yaml
 releasenotes/notes/bgpvpn-routes-control-51cd95d6ab265cb1.yaml
 releasenotes/notes/bgpvpn_rt_fix-6d02db6a1c22f002.yaml
 releasenotes/notes/boilerplate-ext-descriptor-a5cec8b9b900cbfd.yaml
 releasenotes/notes/bug-1877254-2b997b3911e98079.yaml
@@ -1120,27 +1145,29 @@
 releasenotes/notes/ipv6-canonical-address-13900a784f847ce3.yaml
 releasenotes/notes/ipv6_address_usage-ef3d65ad5aa5798b.yaml
 releasenotes/notes/l3-agent-extensions-ha-state-change-837140efe4187a99.yaml
 releasenotes/notes/l3-agent-extensions-update-network-e4887f7f258e40f0.yaml
 releasenotes/notes/l3-apidef-exceptions-ee57b9df1c7443d4.yaml
 releasenotes/notes/l3-apidefs-d028c708c22ef2a0.yaml
 releasenotes/notes/l3-conntrack-helper-validator-654ccafb296e5f21.yaml
+releasenotes/notes/l3-ext-gw-multihoming-1a7b556c541923cf.yaml
 releasenotes/notes/l3-ndp-proxy-71eee0cba8565dad.yaml
 releasenotes/notes/l3-port-ip-change-not-allow-2c98e13c08b5ee85.yaml
 releasenotes/notes/l3-support-ecmp-91a8aa61e3a73037.yaml
 releasenotes/notes/l3_conntrack_helper-f186bcdcc31bcaf2.yaml
 releasenotes/notes/logging-api-ref-fafb884367ca60a2.yaml
 releasenotes/notes/logging-resource-api-cecf33e3be468eb2.yaml
 releasenotes/notes/mac-generator-f927df2fe57300c0.yaml
 releasenotes/notes/mechanism_driver_supported_extensions-67e1b0b763571ae9.yaml
 releasenotes/notes/mechanismdriver-connectivity-00dc679a3f307345.yaml
 releasenotes/notes/migrate-public-to-shared-0c67b32f9c37c751.yaml
 releasenotes/notes/move-get-random-mac-98f47d81cb34483d.yaml
 releasenotes/notes/move-segment-range-types-to-lib-constants-d45c6959607e9136.yaml
 releasenotes/notes/moved-netmtu-extension-5999348000adcfaf.yaml
+releasenotes/notes/network-ha-e6e0c3202b084762.yaml
 releasenotes/notes/network-ip-availability-pagging-support-cc01592cd477fd02.yaml
 releasenotes/notes/network-segment-range-ext-2b93b7fa42310c25.yaml
 releasenotes/notes/new-hacking-check-no-log-translations-4a430a38aeb06452.yaml
 releasenotes/notes/new-policy-module-f5638e23fe91a287.yaml
 releasenotes/notes/new-validator-range-or-none-dc8d557ec1f2622a.yaml
 releasenotes/notes/new-vif-details-parameters-71e70ab5e7c26c45.yaml
 releasenotes/notes/one-hacking-factory-01053e8e3d88c3d5.yaml
```

### Comparing `neutron-lib-3.5.0/releasenotes/notes/add-ovo-registry-27cb7d4ac76d4dc8.yaml` & `neutron-lib-3.6.0/releasenotes/notes/add-ovo-registry-27cb7d4ac76d4dc8.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/bug-1921150-a38bef3c1be69650.yaml` & `neutron-lib-3.6.0/releasenotes/notes/bug-1921150-a38bef3c1be69650.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/change_placement_client_method_names_b26bb71425f42db3.yaml` & `neutron-lib-3.6.0/releasenotes/notes/change_placement_client_method_names_b26bb71425f42db3.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/core-attributes-43e6969f1b187e5c.yaml` & `neutron-lib-3.6.0/releasenotes/notes/core-attributes-43e6969f1b187e5c.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/directory-fixture-083c5c5f365670d6.yaml` & `neutron-lib-3.6.0/releasenotes/notes/directory-fixture-083c5c5f365670d6.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/expose-and-enhance-callback-api-714cce65a3c44fe7.yaml` & `neutron-lib-3.6.0/releasenotes/notes/expose-and-enhance-callback-api-714cce65a3c44fe7.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/extension-fixture-b7fd61384f1a4d1d.yaml` & `neutron-lib-3.6.0/releasenotes/notes/extension-fixture-b7fd61384f1a4d1d.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/new-hacking-check-no-log-translations-4a430a38aeb06452.yaml` & `neutron-lib-3.6.0/releasenotes/notes/new-hacking-check-no-log-translations-4a430a38aeb06452.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/placement-client-optional-rp-generations-44d1f1055d5496be.yaml` & `neutron-lib-3.6.0/releasenotes/notes/placement-client-optional-rp-generations-44d1f1055d5496be.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/placement-resource-provider-functions-17ec45f714ea2b23.yaml` & `neutron-lib-3.6.0/releasenotes/notes/placement-resource-provider-functions-17ec45f714ea2b23.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/port-hints-8273fa5b7454a8ef.yaml` & `neutron-lib-3.6.0/releasenotes/notes/port-hints-8273fa5b7454a8ef.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/qos-rules-alias-ext-fix-3f3f7dd21837cfec.yaml` & `neutron-lib-3.6.0/releasenotes/notes/qos-rules-alias-ext-fix-3f3f7dd21837cfec.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/rehome-common-rpc-5d84a9fe0faa71b7.yaml` & `neutron-lib-3.6.0/releasenotes/notes/rehome-common-rpc-5d84a9fe0faa71b7.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/rehome-db-api-63300ddab6a41e28.yaml` & `neutron-lib-3.6.0/releasenotes/notes/rehome-db-api-63300ddab6a41e28.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/rehome-db-model-query-234b1559f3728a5e.yaml` & `neutron-lib-3.6.0/releasenotes/notes/rehome-db-model-query-234b1559f3728a5e.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/rehome-flavors-apidef-ef84b2c1c7eaeed7.yaml` & `neutron-lib-3.6.0/releasenotes/notes/rehome-flavors-apidef-ef84b2c1c7eaeed7.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/resource-provider-uuid5-namespace-f7276ba1945ce82f.yaml` & `neutron-lib-3.6.0/releasenotes/notes/resource-provider-uuid5-namespace-f7276ba1945ce82f.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/setproctitle_for_workers-e8805fcaf34026ab.yaml` & `neutron-lib-3.6.0/releasenotes/notes/setproctitle_for_workers-e8805fcaf34026ab.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/sfc-api-def-4f46632eadfe895a.yaml` & `neutron-lib-3.6.0/releasenotes/notes/sfc-api-def-4f46632eadfe895a.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/sqlalchemy-2.0-c794885886a62fa6.yaml` & `neutron-lib-3.6.0/releasenotes/notes/sqlalchemy-2.0-c794885886a62fa6.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/subresource-update-attrmap-and-classmethods-76accdd5c56a3bd4.yaml` & `neutron-lib-3.6.0/releasenotes/notes/subresource-update-attrmap-and-classmethods-76accdd5c56a3bd4.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/notes/vhost-vdpa-cc35f8d0ff9b3c4a.yaml` & `neutron-lib-3.6.0/releasenotes/notes/vhost-vdpa-cc35f8d0ff9b3c4a.yaml`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/source/conf.py` & `neutron-lib-3.6.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `neutron-lib-3.6.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/requirements.txt` & `neutron-lib-3.6.0/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 keystoneauth1>=3.14.0 # Apache-2.0
 netaddr>=0.7.18 # BSD
 stevedore>=1.20.0 # Apache-2.0
 os-ken >= 0.3.0 # Apache-2.0
 oslo.concurrency>=3.26.0 # Apache-2.0
 oslo.config>=8.0.0 # Apache-2.0
 oslo.context>=2.22.0 # Apache-2.0
-oslo.db>=4.44.0 # Apache-2.0
+oslo.db>=12.1.0 # Apache-2.0
 oslo.i18n>=3.20.0 # Apache-2.0
 oslo.log>=4.3.0 # Apache-2.0
 oslo.messaging>=14.2.0 # Apache-2.0
 oslo.policy>=3.6.2 # Apache-2.0
 oslo.serialization>=2.25.0 # Apache-2.0
 oslo.service!=1.28.1,>=1.24.0 # Apache-2.0
 oslo.utils>=4.5.0 # Apache-2.0
```

### Comparing `neutron-lib-3.5.0/setup.cfg` & `neutron-lib-3.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/setup.py` & `neutron-lib-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/test-requirements.txt` & `neutron-lib-3.6.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tools/api_report.sh` & `neutron-lib-3.6.0/tools/api_report.sh`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tools/check_samples.sh` & `neutron-lib-3.6.0/tools/check_samples.sh`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tools/coding-checks.sh` & `neutron-lib-3.6.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tools/migration_report.sh` & `neutron-lib-3.6.0/tools/migration_report.sh`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tools/pyir.py` & `neutron-lib-3.6.0/tools/pyir.py`

 * *Files identical despite different names*

### Comparing `neutron-lib-3.5.0/tox.ini` & `neutron-lib-3.6.0/tox.ini`

 * *Files identical despite different names*

