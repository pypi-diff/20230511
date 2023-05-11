# Comparing `tmp/sushy-4.4.2.tar.gz` & `tmp/sushy-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sushy-4.4.2.tar", last modified: Fri Feb 10 16:08:00 2023, max compression
+gzip compressed data, was "sushy-4.5.0.tar", last modified: Thu May 11 09:12:15 2023, max compression
```

## Comparing `sushy-4.4.2.tar` & `sushy-4.5.0.tar`

### file list

```diff
@@ -1,464 +1,474 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.087798 sushy-4.4.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:07:32.000000 sushy-4.4.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-10 16:07:32.000000 sushy-4.4.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2023-02-10 16:07:32.000000 sushy-4.4.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2739 2023-02-10 16:07:59.000000 sushy-4.4.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-02-10 16:07:32.000000 sushy-4.4.2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16744 2023-02-10 16:07:59.000000 sushy-4.4.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-02-10 16:07:32.000000 sushy-4.4.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:07:32.000000 sushy-4.4.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-02-10 16:08:00.087798 sushy-4.4.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2023-02-10 16:07:32.000000 sushy-4.4.2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-02-10 16:07:32.000000 sushy-4.4.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.003780 sushy-4.4.2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.003780 sushy-4.4.2/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.003780 sushy-4.4.2/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.003780 sushy-4.4.2/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.003780 sushy-4.4.2/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2023-02-10 16:07:32.000000 sushy-4.4.2/doc/source/reference/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:59.995778 sushy-4.4.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.027785 sushy-4.4.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/enums-3aff03d940012f33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/event-service-d6607420effc3df8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/sessions.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.027785 sushy-4.4.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.027785 sushy-4.4.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.027785 sushy-4.4.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-10 16:07:32.000000 sushy-4.4.2/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2023-02-10 16:07:32.000000 sushy-4.4.2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-02-10 16:08:00.087798 sushy-4.4.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-10 16:07:32.000000 sushy-4.4.2/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.031786 sushy-4.4.2/sushy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11603 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21152 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25604 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.035787 sushy-4.4.2/sushy/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30891 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.035787 sushy-4.4.2/sushy/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/certificateservice/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/certificateservice/certificateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/certificateservice/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.035787 sushy-4.4.2/sushy/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12123 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.035787 sushy-4.4.2/sushy/resources/chassis/power/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/power/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/power/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/power/power.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.039788 sushy-4.4.2/sushy/resources/chassis/thermal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/thermal/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/thermal/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/chassis/thermal/thermal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.039788 sushy-4.4.2/sushy/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/compositionservice/compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/compositionservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/compositionservice/resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/compositionservice/resourcezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.039788 sushy-4.4.2/sushy/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/eventservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/eventservice/eventdestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/eventservice/eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.039788 sushy-4.4.2/sushy/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/fabric/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/fabric/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/fabric/fabric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/ipaddresses.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.039788 sushy-4.4.2/sushy/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/manager/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/manager/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10100 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/manager/virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.043789 sushy-4.4.2/sushy/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/oem/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/oem/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/oem/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.043789 sushy-4.4.2/sushy/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/registry/attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/registry/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/registry/message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7199 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/registry/message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.043789 sushy-4.4.2/sushy/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/sessionservice/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/sessionservice/sessionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6563 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.043789 sushy-4.4.2/sushy/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9322 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12820 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/ethernet_interface.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.047789 sushy-4.4.2/sushy/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/network/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/network/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/network/device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/network/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5482 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/simple_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.047789 sushy-4.4.2/sushy/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/storage/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20500 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/system/system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.047789 sushy-4.4.2/sushy/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/taskservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/taskservice/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/taskservice/taskservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.047789 sushy-4.4.2/sushy/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/updateservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/updateservice/softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/resources/updateservice/updateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.051790 sushy-4.4.2/sushy/standard_registries/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26501 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/standard_registries/Base.1.0.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/standard_registries/Base.1.2.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/standard_registries/Base.1.3.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/standard_registries/Base.1.3.1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/standard_registries/Base.1.4.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/taskmonitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.051790 sushy-4.4.2/sushy/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.051790 sushy-4.4.2/sushy/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.075796 sushy-4.4.2/sushy/tests/unit/json_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/TestRegistry.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/bare_minimum_root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/bios.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/bios_attribute_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/bios_settings.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/certificate.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/certificate_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/certificate_locations.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/certificateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/chassis.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/chassis_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/compositionservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/drive2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/drive3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/endpoint.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/endpoint_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/error_single_ext_info.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/ethernet_interfaces.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/eventdestination1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/eventdestination2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/eventdestination3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/eventdestination_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/eventservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/fabric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/fabric_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/firmwareinventory_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/manager.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/manager_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/message_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/message_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/message_registry_file_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_adapter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_adapter_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_device_function.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_device_function_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/network_port_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/power.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/processor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/processor2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/processor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/resourceblock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/resourceblock_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/resourcezone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/resourcezone_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot_database.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot_database_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session_creation_headers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/session_service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings-body-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/simple_storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/simple_storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/softwareinventory.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/storage_controller.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/storage_controller_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/storage_controller_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/subprocessor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/subprocessor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/system_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/task.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/task2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/task_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/task_monitor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/taskservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/thermal.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/transfer_proto_required_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/updateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/updateservice_no_inv.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/virtual_media.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/virtual_media_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/volume2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/volume3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/volume4.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/json_samples/volume_collection.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.075796 sushy-4.4.2/sushy/tests/unit/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.075796 sushy-4.4.2/sushy/tests/unit/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/certificateservice/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.075796 sushy-4.4.2/sushy/tests/unit/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12064 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/chassis/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/chassis/test_power.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/chassis/test_thermal.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.075796 sushy-4.4.2/sushy/tests/unit/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/eventservice/test_evendestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/eventservice/test_eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/fabric/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/fabric/test_fabric.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13706 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/manager/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14758 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/manager/test_virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/oem/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/oem/test_fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3121 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/registry/test_attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/registry/test_message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/registry/test_message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.079796 sushy-4.4.2/sushy/tests/unit/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/sessionservice/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.083797 sushy-4.4.2/sushy/tests/unit/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.083797 sushy-4.4.2/sushy/tests/unit/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/network/test_adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/network/test_device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/network/test_port.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.083797 sushy-4.4.2/sushy/tests/unit/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6245 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15644 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_simple_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38692 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/system/test_system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.083797 sushy-4.4.2/sushy/tests/unit/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/taskservice/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/taskservice/test_taskservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4897 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/test_settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.087798 sushy-4.4.2/sushy/tests/unit/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/resources/updateservice/test_updateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37140 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27368 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/test_taskmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2023-02-10 16:07:32.000000 sushy-4.4.2/sushy/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.031786 sushy-4.4.2/sushy.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20679 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2023-02-10 16:07:59.000000 sushy-4.4.2/sushy.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-10 16:07:32.000000 sushy-4.4.2/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.087798 sushy-4.4.2/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2023-02-10 16:07:32.000000 sushy-4.4.2/tools/generate-enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2023-02-10 16:07:32.000000 sushy-4.4.2/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:08:00.087798 sushy-4.4.2/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-02-10 16:07:32.000000 sushy-4.4.2/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-02-10 16:07:32.000000 sushy-4.4.2/zuul.d/sushy-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.658070 sushy-4.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:11:46.000000 sushy-4.5.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-11 09:11:46.000000 sushy-4.5.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2023-05-11 09:11:46.000000 sushy-4.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2799 2023-05-11 09:12:15.000000 sushy-4.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-05-11 09:11:46.000000 sushy-4.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17068 2023-05-11 09:12:15.000000 sushy-4.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 09:11:46.000000 sushy-4.5.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 09:11:46.000000 sushy-4.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-05-11 09:12:15.658070 sushy-4.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2023-05-11 09:11:46.000000 sushy-4.5.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-05-11 09:11:46.000000 sushy-4.5.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.570059 sushy-4.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.570059 sushy-4.5.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.570059 sushy-4.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.570059 sushy-4.5.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.570059 sushy-4.5.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2023-05-11 09:11:46.000000 sushy-4.5.0/doc/source/reference/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.562058 sushy-4.5.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.602063 sushy-4.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/enums-3aff03d940012f33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/event-service-d6607420effc3df8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/sessions.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.606063 sushy-4.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.610064 sushy-4.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.610064 sushy-4.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:11:46.000000 sushy-4.5.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2023-05-11 09:11:46.000000 sushy-4.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2023-05-11 09:12:15.658070 sushy-4.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:11:46.000000 sushy-4.5.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.610064 sushy-4.5.0/sushy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11603 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22399 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25604 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.614065 sushy-4.5.0/sushy/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31250 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.614065 sushy-4.5.0/sushy/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/certificateservice/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/certificateservice/certificateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/certificateservice/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.614065 sushy-4.5.0/sushy/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12123 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.614065 sushy-4.5.0/sushy/resources/chassis/power/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/power/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/power/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/power/power.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.614065 sushy-4.5.0/sushy/resources/chassis/thermal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/thermal/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/thermal/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/chassis/thermal/thermal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/compositionservice/compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/compositionservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/compositionservice/resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/compositionservice/resourcezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/eventservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/eventservice/eventdestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/eventservice/eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/fabric/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/fabric/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/fabric/fabric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/ipaddresses.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/manager/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/manager/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11088 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/manager/virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/oem/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/oem/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/oem/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.618065 sushy-4.5.0/sushy/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/registry/attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/registry/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/registry/message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/registry/message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.622065 sushy-4.5.0/sushy/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/sessionservice/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/sessionservice/sessionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6563 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.622065 sushy-4.5.0/sushy/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9322 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12820 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/ethernet_interface.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.622065 sushy-4.5.0/sushy/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/network/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/network/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/network/device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/network/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5482 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/simple_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.626066 sushy-4.5.0/sushy/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/storage/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20500 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/system/system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.626066 sushy-4.5.0/sushy/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/taskservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/taskservice/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/taskservice/taskservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.626066 sushy-4.5.0/sushy/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/updateservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/updateservice/softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/resources/updateservice/updateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.626066 sushy-4.5.0/sushy/standard_registries/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26501 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/standard_registries/Base.1.0.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/standard_registries/Base.1.2.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/standard_registries/Base.1.3.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/standard_registries/Base.1.3.1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/standard_registries/Base.1.4.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/taskmonitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.626066 sushy-4.5.0/sushy/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.630066 sushy-4.5.0/sushy/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.646068 sushy-4.5.0/sushy/tests/unit/json_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/TestRegistry.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bare_minimum_root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11114 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/bios_zt.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/certificate.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/certificate_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/certificate_locations.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/certificateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/chassis.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/chassis_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/compositionservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/drive2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/drive3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/endpoint.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/endpoint_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/error_single_ext_info.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/ethernet_interfaces.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/eventdestination1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/eventdestination2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/eventdestination3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/eventdestination_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/eventservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/fabric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/fabric_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/manager.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/manager_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/message_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/message_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/message_registry_file_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_adapter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_adapter_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_device_function.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_device_function_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/network_port_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/power.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/processor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/processor2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/processor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/resourceblock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/resourceblock_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/resourcezone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/resourcezone_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot_database.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session_creation_headers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/session_service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings-body-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/simple_storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/simple_storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/softwareinventory.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/storage_controller.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/storage_controller_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/storage_controller_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/subprocessor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/subprocessor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/system_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/task.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/task2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/task_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/task_monitor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/taskservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/thermal.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/transfer_method_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/transfer_proto_required_error2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/updateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/updateservice_no_inv.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/virtual_media.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/virtual_media_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/volume2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/volume3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/volume4.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/json_samples/volume_collection.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.646068 sushy-4.5.0/sushy/tests/unit/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.646068 sushy-4.5.0/sushy/tests/unit/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/certificateservice/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12064 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/chassis/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/chassis/test_power.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/chassis/test_thermal.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/eventservice/test_evendestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/eventservice/test_eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/fabric/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/fabric/test_fabric.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13706 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/manager/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15741 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/manager/test_virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/oem/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/oem/test_fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.650069 sushy-4.5.0/sushy/tests/unit/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/registry/test_attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/registry/test_message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/registry/test_message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.654070 sushy-4.5.0/sushy/tests/unit/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/sessionservice/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.654070 sushy-4.5.0/sushy/tests/unit/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.654070 sushy-4.5.0/sushy/tests/unit/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/network/test_adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/network/test_device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/network/test_port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.654070 sushy-4.5.0/sushy/tests/unit/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6245 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4279 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19610 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5058 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_simple_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38692 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/system/test_system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.658070 sushy-4.5.0/sushy/tests/unit/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/taskservice/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/taskservice/test_taskservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4897 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/test_settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.658070 sushy-4.5.0/sushy/tests/unit/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/resources/updateservice/test_updateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38922 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27368 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/test_taskmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2023-05-11 09:11:46.000000 sushy-4.5.0/sushy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.610064 sushy-4.5.0/sushy.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21301 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2023-05-11 09:12:15.000000 sushy-4.5.0/sushy.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-05-11 09:11:46.000000 sushy-4.5.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.658070 sushy-4.5.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2023-05-11 09:11:46.000000 sushy-4.5.0/tools/generate-enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2023-05-11 09:11:46.000000 sushy-4.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:12:15.658070 sushy-4.5.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-05-11 09:11:46.000000 sushy-4.5.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-05-11 09:11:46.000000 sushy-4.5.0/zuul.d/sushy-jobs.yaml
```

### Comparing `sushy-4.4.2/AUTHORS` & `sushy-4.5.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 Anshul Jain <theanshuljain@gmail.com>
 Arne Wiebalck <Arne.Wiebalck@cern.ch>
 Arundhati Surpur <arundhati@nectechnologies.in>
 Bill Dodd <billdodd@gmail.com>
 Bob Fournier <bfournie@redhat.com>
 Christopher Dearborn <Christopher.Dearborn@dell.com>
 Debayan Ray <debayan.ray@gmail.com>
+Derek Higgins <derekh@redhat.com>
 Dmitry Tantsur <divius.inside@gmail.com>
 Dmitry Tantsur <dtantsur@protonmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Gabriela Soria <soria.gaby@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Ha Manh Dong <donghm@vn.fujitsu.com>
 Hervé Beraud <hberaud@redhat.com>
 Ilya Etingof <etingof@gmail.com>
 Iury Gregory Melo Ferreira <imelofer@redhat.com>
 Iury Gregory Melo Ferreira <iurygregory@gmail.com>
 Jacob Anders <janders@redhat.com>
 James E. Blair <jeblair@redhat.com>
 Javier Pena <jpena@redhat.com>
+Jay Faulkner <jay@jvf.cc>
 John L. Villalovos <john.l.villalovos@intel.com>
 Julia Kreger <juliaashleykreger@gmail.com>
 Kafilat Adeleke <adelekekafilatadenike@gmail.com>
 Kaifeng Wang <kaifeng.w@gmail.com>
 Kamlesh Chauvhan <kamlesh.chauvhan@gmail.com>
 LiZekun <2954674728@qq.com>
 Lin Yang <lin.a.yang@intel.com>
```

### Comparing `sushy-4.4.2/CONTRIBUTING.rst` & `sushy-4.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/ChangeLog` & `sushy-4.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+4.5.0
+-----
+
+* Retry on ilo state error
+* Update pep8 dep hacking to latest: v6
+* Handle TransferMethod in vmedia insertion
+* Add TransferProtocolType for any general error that mentions it
+* Exclude all files starting with . from flake8 tests
+* Update master for stable/2023.1
+* Handle non-default language for registries
+
 4.4.2
 -----
 
 * workaround: requests verify handling if env is set
 * Remove setuptools workaround
 * Fix tox4 and setuptools errors
 * Fix exceeding retries
```

### Comparing `sushy-4.4.2/LICENSE` & `sushy-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/PKG-INFO` & `sushy-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 4.4.2
+Version: 4.5.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
```

### Comparing `sushy-4.4.2/README.rst` & `sushy-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/doc/source/conf.py` & `sushy-4.5.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/doc/source/contributor/index.rst` & `sushy-4.5.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/doc/source/index.rst` & `sushy-4.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/doc/source/reference/usage.rst` & `sushy-4.5.0/doc/source/reference/usage.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml` & `sushy-4.5.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml` & `sushy-4.5.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml` & `sushy-4.5.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml` & `sushy-4.5.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/enums-3aff03d940012f33.yaml` & `sushy-4.5.0/releasenotes/notes/enums-3aff03d940012f33.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml` & `sushy-4.5.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml` & `sushy-4.5.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml` & `sushy-4.5.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/releasenote-d7138d1e1d414632.yaml` & `sushy-4.5.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml` & `sushy-4.5.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/releasenotes/source/conf.py` & `sushy-4.5.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/requirements.txt` & `sushy-4.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/setup.cfg` & `sushy-4.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/setup.py` & `sushy-4.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/__init__.py` & `sushy-4.5.0/sushy/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/auth.py` & `sushy-4.5.0/sushy/auth.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/connector.py` & `sushy-4.5.0/sushy/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,20 +90,25 @@
 
     def close(self):
         """Close this connector and the associated HTTP session."""
         self._session.close()
 
     def check_retry_on_exception(self, exception_msg):
         """Checks whether retry on exception is required."""
-        if ('SYS518' in str(exception_msg)):
+        retry = False
+        exc_str = str(exception_msg)
+        if 'SYS518' in exc_str:
             LOG.debug('iDRAC is not yet ready after previous operation. '
-                      'Error: %(err)s', {'err': str(exception_msg)})
-            return True
-        else:
-            return False
+                      'Error: %(err)s', {'err': exc_str})
+            retry = True
+        elif 'iLO.2.15.InvalidOperationForSystemState' in exc_str:
+            LOG.debug('iLO is not ready after previous operation. '
+                      'Error: %(error)s', {'err': exc_str})
+            retry = True
+        return retry
 
     def _op(self, method, path='', data=None, headers=None, blocking=False,
             timeout=60, server_side_retries_left=None,
             **extra_session_req_kwargs):
         """Generic RESTful request handler.
 
         :param method: The HTTP method to be used, e.g: GET, POST,
@@ -222,28 +227,46 @@
                               "%s", e.message)
                 raise
         except exceptions.ServerSideError as e:
             if ((method.lower() == 'get'
                 or self.check_retry_on_exception(e.message))
                     and server_side_retries_left > 0):
                 LOG.warning('Got server side error %s in response to a '
-                            'GET request, retrying after %d seconds. Retries '
+                            'request, retrying after %d seconds. Retries '
                             'left %d.',
                             e, self._server_side_retries_delay,
                             server_side_retries_left)
                 time.sleep(self._server_side_retries_delay)
                 server_side_retries_left -= 1
                 return self._op(
                     method, path, data=data, headers=headers,
                     blocking=blocking, timeout=timeout,
                     server_side_retries_left=server_side_retries_left,
                     **extra_session_req_kwargs)
             else:
                 raise
-
+        except exceptions.BadRequestError as e:
+            if (method.lower() != 'get'
+                    and self.check_retry_on_exception(e.message)
+                    and server_side_retries_left > 0):
+                LOG.warning('Server has indicated a BadRequest for %s but '
+                            'the response payload is a known retriable '
+                            'condition and we will retry in %d seconds. '
+                            'Retries left  %d.',
+                            e, self._server_side_retries_delay,
+                            server_side_retries_left)
+                time.sleep(self._server_side_retries_delay)
+                server_side_retries_left -= 1
+                return self._op(
+                    method, path, data=data, headers=headers,
+                    blocking=blocking, timeout=timeout,
+                    server_side_retries_left=server_side_retries_left,
+                    **extra_session_req_kwargs)
+            else:
+                raise
         if blocking and response.status_code == 202:
             if not response.headers.get('Location'):
                 m = ('HTTP response for %(method)s request to %(url)s '
                      'returned status 202, but no Location header'
                      % {'method': method, 'url': url})
                 raise exceptions.ConnectionError(url=url, error=m)
```

### Comparing `sushy-4.4.2/sushy/exceptions.py` & `sushy-4.5.0/sushy/exceptions.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/main.py` & `sushy-4.5.0/sushy/main.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/base.py` & `sushy-4.5.0/sushy/resources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,15 +590,20 @@
         if not registries:
             LOG.info('No %s is available', description)
             return None
 
         for key, registry in registries.items():
             if (registry
                     and self._attribute_registry in (key, registry.identity)):
-                if language != registry.language:
+                # NOTE(iurygregory): some registries may have "en-US"
+                # as their language, in this case we can check if the
+                # registry language starts with the requested language.
+                registry_language = registry.language.lower().split('-', 1)[0]
+                if (language != registry.language
+                        and language.lower() != registry_language):
                     LOG.debug('Found %(descr)s but its language %(reg_lang)s '
                               'does not match the requested %(lang)s',
                               {'descr': description,
                                'lang': language,
                                'reg_lang': registry.language})
                     continue
```

### Comparing `sushy-4.4.2/sushy/resources/certificateservice/certificate.py` & `sushy-4.5.0/sushy/resources/certificateservice/certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/certificateservice/certificateservice.py` & `sushy-4.5.0/sushy/resources/certificateservice/certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/certificateservice/constants.py` & `sushy-4.5.0/sushy/resources/certificateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/chassis.py` & `sushy-4.5.0/sushy/resources/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/constants.py` & `sushy-4.5.0/sushy/resources/chassis/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/power/constants.py` & `sushy-4.5.0/sushy/resources/chassis/power/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/power/power.py` & `sushy-4.5.0/sushy/resources/chassis/power/power.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/thermal/constants.py` & `sushy-4.5.0/sushy/resources/chassis/thermal/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/chassis/thermal/thermal.py` & `sushy-4.5.0/sushy/resources/chassis/thermal/thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/common.py` & `sushy-4.5.0/sushy/resources/common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/compositionservice/compositionservice.py` & `sushy-4.5.0/sushy/resources/compositionservice/compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/compositionservice/constants.py` & `sushy-4.5.0/sushy/resources/compositionservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/compositionservice/resourceblock.py` & `sushy-4.5.0/sushy/resources/compositionservice/resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/compositionservice/resourcezone.py` & `sushy-4.5.0/sushy/resources/compositionservice/resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/constants.py` & `sushy-4.5.0/sushy/resources/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/eventservice/constants.py` & `sushy-4.5.0/sushy/resources/eventservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/eventservice/eventdestination.py` & `sushy-4.5.0/sushy/resources/eventservice/eventdestination.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/eventservice/eventservice.py` & `sushy-4.5.0/sushy/resources/eventservice/eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/fabric/constants.py` & `sushy-4.5.0/sushy/resources/fabric/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/fabric/endpoint.py` & `sushy-4.5.0/sushy/resources/fabric/endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/fabric/fabric.py` & `sushy-4.5.0/sushy/resources/fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/ipaddresses.py` & `sushy-4.5.0/sushy/resources/ipaddresses.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/manager/constants.py` & `sushy-4.5.0/sushy/resources/manager/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/manager/manager.py` & `sushy-4.5.0/sushy/resources/manager/manager.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/manager/virtual_media.py` & `sushy-4.5.0/sushy/resources/manager/virtual_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,20 +107,34 @@
         return eject_uri, use_patch
 
     def is_transfer_protocol_required(self, error=None):
         """Check the response code and body and in case of failure
 
         Try to determine if it happened due to missing TransferProtocolType.
         """
+        if (error.code.endswith('GeneralError')
+           and 'TransferProtocolType' in error.detail):
+            return True
+
         return (
             (error.code.endswith(".ActionParameterMissing")
              or error.code.endswith(".PropertyMissing"))
             and "#/TransferProtocolType" in error.related_properties
         )
 
+    def is_transfer_method_required(self, error=None):
+        """Check the response code and body and in case of failure
+
+        Try to determine if it happened due to missing TransferMethod
+        """
+        if (error.code.endswith('GeneralError')
+                and 'TransferMethod' in error.detail):
+            return True
+        return False
+
     def insert_media(self, image, inserted=True, write_protected=True,
                      username=None, password=None, transfer_method=None):
         """Attach remote media to virtual media
 
         :param image: a URI providing the location of the selected image
         :param inserted: specify if the image is to be treated as inserted upon
             completion of the action.
@@ -178,15 +192,26 @@
                 self._conn.post(target_uri, data=payload)
             except exceptions.HTTPError as error:
                 if self.is_transfer_protocol_required(error):
                     if payload['Image'].startswith('https://'):
                         payload['TransferProtocolType'] = "HTTPS"
                     elif payload['Image'].startswith('http://'):
                         payload['TransferProtocolType'] = "HTTP"
-                    self._conn.post(target_uri, data=payload)
+
+                    # NOTE (iurygregory) we try to handle the case where a
+                    # a TransferMethod is also required in the payload.
+                    try:
+                        self._conn.post(target_uri, data=payload)
+                    except exceptions.HTTPError as error2:
+                        if self.is_transfer_method_required(error2):
+                            payload['TransferMethod'] = "Stream"
+                            self._conn.post(target_uri, data=payload)
+                        else:
+                            raise
+
                 else:
                     raise
         self.invalidate()
 
     def eject_media(self):
         """Detach remote media from virtual media
```

### Comparing `sushy-4.4.2/sushy/resources/oem/__init__.py` & `sushy-4.5.0/sushy/resources/oem/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/oem/base.py` & `sushy-4.5.0/sushy/resources/oem/base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/oem/common.py` & `sushy-4.5.0/sushy/resources/oem/common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/oem/fake.py` & `sushy-4.5.0/sushy/resources/oem/fake.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/registry/attribute_registry.py` & `sushy-4.5.0/sushy/resources/registry/attribute_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/registry/constants.py` & `sushy-4.5.0/sushy/resources/registry/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/registry/message_registry.py` & `sushy-4.5.0/sushy/resources/registry/message_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/registry/message_registry_file.py` & `sushy-4.5.0/sushy/resources/registry/message_registry_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,22 @@
         :param registry_class: registry class
         :returns: registry or None if not found
         """
 
         # NOTE (etingof): as per RFC5646, languages are case-insensitive
         language = language.lower()
 
+        # NOTE(iurygregory): some registries may have "en-US" as their
+        # language, in this case we can check if the registry language
+        # starts with the requested language.
         locations = [
-            l for l in self.location if l.language.lower() == language]
+            l for l in self.location
+            if l.language.lower().split('-', 1)[0] == language
+            or l.language == language
+        ]
 
         locations += [
             l for l in self.location if l.language.lower() == 'default']
 
         for location in locations:
             if location.uri:
                 args = self._conn,
```

### Comparing `sushy-4.4.2/sushy/resources/sessionservice/session.py` & `sushy-4.5.0/sushy/resources/sessionservice/session.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/sessionservice/sessionservice.py` & `sushy-4.5.0/sushy/resources/sessionservice/sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/settings.py` & `sushy-4.5.0/sushy/resources/settings.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/bios.py` & `sushy-4.5.0/sushy/resources/system/bios.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/constants.py` & `sushy-4.5.0/sushy/resources/system/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/ethernet_interface.py` & `sushy-4.5.0/sushy/resources/system/ethernet_interface.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/network/adapter.py` & `sushy-4.5.0/sushy/resources/system/network/adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/network/constants.py` & `sushy-4.5.0/sushy/resources/system/network/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/network/device_function.py` & `sushy-4.5.0/sushy/resources/system/network/device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/network/port.py` & `sushy-4.5.0/sushy/resources/system/network/port.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/processor.py` & `sushy-4.5.0/sushy/resources/system/processor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/secure_boot.py` & `sushy-4.5.0/sushy/resources/system/secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/secure_boot_database.py` & `sushy-4.5.0/sushy/resources/system/secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/simple_storage.py` & `sushy-4.5.0/sushy/resources/system/simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/storage/constants.py` & `sushy-4.5.0/sushy/resources/system/storage/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/storage/controller.py` & `sushy-4.5.0/sushy/resources/system/storage/controller.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/storage/drive.py` & `sushy-4.5.0/sushy/resources/system/storage/drive.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/storage/storage.py` & `sushy-4.5.0/sushy/resources/system/storage/storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/storage/volume.py` & `sushy-4.5.0/sushy/resources/system/storage/volume.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/system/system.py` & `sushy-4.5.0/sushy/resources/system/system.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/taskservice/constants.py` & `sushy-4.5.0/sushy/resources/taskservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/taskservice/task.py` & `sushy-4.5.0/sushy/resources/taskservice/task.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/taskservice/taskservice.py` & `sushy-4.5.0/sushy/resources/taskservice/taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/updateservice/constants.py` & `sushy-4.5.0/sushy/resources/updateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/updateservice/softwareinventory.py` & `sushy-4.5.0/sushy/resources/updateservice/softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/resources/updateservice/updateservice.py` & `sushy-4.5.0/sushy/resources/updateservice/updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/standard_registries/Base.1.0.0.json` & `sushy-4.5.0/sushy/standard_registries/Base.1.0.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/standard_registries/Base.1.2.0.json` & `sushy-4.5.0/sushy/standard_registries/Base.1.2.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/standard_registries/Base.1.3.0.json` & `sushy-4.5.0/sushy/standard_registries/Base.1.3.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/standard_registries/Base.1.3.1.json` & `sushy-4.5.0/sushy/standard_registries/Base.1.3.1.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/standard_registries/Base.1.4.0.json` & `sushy-4.5.0/sushy/standard_registries/Base.1.4.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/taskmonitor.py` & `sushy-4.5.0/sushy/taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/base.py` & `sushy-4.5.0/sushy/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/TestRegistry.zip` & `sushy-4.5.0/sushy/tests/unit/json_samples/TestRegistry.zip`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/bios.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/bios.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/bios_attribute_registry.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/bios_attribute_registry_file.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/bios_settings.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/bios_settings.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/certificate.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/certificate.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/certificate_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/certificate_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/certificate_locations.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/certificate_locations.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/certificateservice.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/certificateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/chassis.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/chassis.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/chassis_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/chassis_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/compositionservice.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/compositionservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/drive.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/drive.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/drive2.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/drive2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/drive3.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/drive3.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/endpoint.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/endpoint.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/error.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/error_single_ext_info.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/error_single_ext_info.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/ethernet_interfaces.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/ethernet_interfaces.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/eventservice.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/eventservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/fabric.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/fabric.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/fabric_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/fabric_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/firmwareinventory_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/manager.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/manager.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/manager_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/manager_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/message_registry.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/message_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/message_registry_file.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/message_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/network_adapter.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/network_adapter.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/network_device_function.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/network_device_function.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/network_device_function_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/network_device_function_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/network_port.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/network_port.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/network_port_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/network_port_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/power.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/power.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/processor.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/processor.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/processor2.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/processor2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/processor_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/processor_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/resourceblock.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/resourceblock.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/resourcezone.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/resourcezone.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/root.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/root.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot_database.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot_database.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/secure_boot_database_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/session.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/session.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/session_creation_headers.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/session_creation_headers.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/session_creation_headers_no_location.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/session_error.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/session_error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/session_service.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/session_service.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/settings-body-nokia.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/settings-body-nokia.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/settings.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/settings.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/simple_storage.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/simple_storage.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/simple_storage_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/simple_storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/softwareinventory.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/softwareinventory.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/storage.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/storage.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/storage_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/storage_controller.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/storage_controller.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/storage_controller_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/storage_controller_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/system.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/system.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/system_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/system_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/task.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/task.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/task_monitor.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/task_monitor.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/taskservice.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/taskservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/thermal.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/thermal.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/transfer_proto_required_error.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/updateservice.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/updateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/updateservice_no_inv.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/updateservice_no_inv.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/virtual_media.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/virtual_media.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/virtual_media_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/virtual_media_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/volume.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/volume.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/volume2.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/volume2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/volume3.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/volume3.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/volume4.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/volume4.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/json_samples/volume_collection.json` & `sushy-4.5.0/sushy/tests/unit/json_samples/volume_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/certificateservice/test_certificate.py` & `sushy-4.5.0/sushy/tests/unit/resources/certificateservice/test_certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/certificateservice/test_certificateservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/chassis/test_chassis.py` & `sushy-4.5.0/sushy/tests/unit/resources/chassis/test_chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/chassis/test_power.py` & `sushy-4.5.0/sushy/tests/unit/resources/chassis/test_power.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/chassis/test_thermal.py` & `sushy-4.5.0/sushy/tests/unit/resources/chassis/test_thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_compositionservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_resourceblock.py` & `sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/compositionservice/test_resourcezone.py` & `sushy-4.5.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/eventservice/test_evendestination.py` & `sushy-4.5.0/sushy/tests/unit/resources/eventservice/test_evendestination.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/eventservice/test_eventservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/eventservice/test_eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/fabric/test_endpoint.py` & `sushy-4.5.0/sushy/tests/unit/resources/fabric/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/fabric/test_fabric.py` & `sushy-4.5.0/sushy/tests/unit/resources/fabric/test_fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/manager/test_manager.py` & `sushy-4.5.0/sushy/tests/unit/resources/manager/test_manager.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/manager/test_virtual_media.py` & `sushy-4.5.0/sushy/tests/unit/resources/manager/test_virtual_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,25 +182,45 @@
             response_obj = json.load(f)
         response = mock.Mock(spec=['json', 'status_code'])
         response.json.return_value = response_obj
         error = exceptions.HTTPError('GET', 'VirtualMedia', response)
         retval = self.sys_virtual_media.is_transfer_protocol_required(error)
         self.assertTrue(retval)
 
-    def test_is_transfer_protocol_required_alt_code(self):
+    def test_is_transfer_protocol_required_alt(self):
         with open('sushy/tests/unit/json_samples/'
                   'transfer_proto_required_error.json') as f:
             response_obj = json.load(f)
         response_obj['error']['code'] = 'Base.1.5.PropertyMissing'
         response = mock.Mock(spec=['json', 'status_code'])
         response.json.return_value = response_obj
         error = exceptions.HTTPError('GET', 'VirtualMedia', response)
         retval = self.sys_virtual_media.is_transfer_protocol_required(error)
         self.assertTrue(retval)
 
+    def test_is_transfer_protocol_required_alt2(self):
+        with open('sushy/tests/unit/json_samples/'
+                  'transfer_proto_required_error2.json') as f:
+            response_obj = json.load(f)
+        response = mock.Mock(spec=['json', 'status_code'])
+        response.json.return_value = response_obj
+        error = exceptions.HTTPError('GET', 'VirtualMedia', response)
+        retval = self.sys_virtual_media.is_transfer_protocol_required(error)
+        self.assertTrue(retval)
+
+    def test_is_transfer_method_required(self):
+        with open('sushy/tests/unit/json_samples/'
+                  'transfer_method_required_error.json') as f:
+            response_obj = json.load(f)
+        response = mock.Mock(spec=['json', 'status_code'])
+        response.json.return_value = response_obj
+        error = exceptions.HTTPError('POST', 'VirtualMedia', response)
+        retval = self.sys_virtual_media.is_transfer_method_required(error)
+        self.assertTrue(retval)
+
     def test_eject_media_none(self):
         self.sys_virtual_media._actions.eject_media = None
         self.assertRaisesRegex(
             exceptions.MissingActionError, 'action #VirtualMedia.EjectMedia',
             self.sys_virtual_media.eject_media)
 
         self.sys_virtual_media._actions = None
```

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/oem/test_common.py` & `sushy-4.5.0/sushy/tests/unit/resources/oem/test_common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/oem/test_fake.py` & `sushy-4.5.0/sushy/tests/unit/resources/oem/test_fake.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/registry/test_message_registry.py` & `sushy-4.5.0/sushy/tests/unit/resources/registry/test_message_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/registry/test_message_registry_file.py` & `sushy-4.5.0/sushy/tests/unit/resources/registry/test_message_registry_file.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/sessionservice/test_session.py` & `sushy-4.5.0/sushy/tests/unit/resources/sessionservice/test_session.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/sessionservice/test_sessionservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/network/test_adapter.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/network/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/network/test_device_function.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/network/test_device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/network/test_port.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/network/test_port.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_controller.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_controller.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_drive.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_drive.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_storage.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/storage/test_volume.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/storage/test_volume.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_bios.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_bios.py`

 * *Files 22% similar despite different names*

```diff
@@ -337,7 +337,93 @@
         self.assertIsNone(registry)
 
     def test_get_attribute_registry_not_found(self):
 
         self.sys_bios._attribute_registry = "Unknown"
         registry = self.sys_bios.get_attribute_registry()
         self.assertIsNone(registry)
+
+
+class BiosZTTestCase(base.TestCase):
+
+    def setUp(self):
+        super(BiosZTTestCase, self).setUp()
+        self.conn = mock.Mock()
+        with open('sushy/tests/unit/json_samples/bios_zt.json') as f:
+            self.bios_json = json.load(f)
+        # NOTE(iurygregory): ZT Hardware doesn't have Settings for Bios.
+
+        self.conn.get.return_value.json.side_effect = [self.bios_json]
+
+        registries = {}
+        conn = mock.Mock()
+        # Note(iurygregory): re-use message registry for now.
+        with open('sushy/tests/unit/json_samples/message_registry.json') as f:
+            conn.get.return_value.json.return_value = json.load(f)
+            msg_reg = message_registry.MessageRegistry(
+                conn, '/redfish/v1/Registries/Test',
+                redfish_version='1.0.2')
+
+            registries['Test.1.0'] = msg_reg
+
+        with open('sushy/tests/unit/json_samples/'
+                  'bios_attribute_registry_zthardware.json') as f:
+            conn.get.return_value.json.return_value = json.load(f)
+            self.bios_reg = attribute_registry.AttributeRegistry(
+                conn,
+                '/redfish/v1/Registries/BiosAttributeRegistryProt0.208.208.0',
+                redfish_version='1.3.1')
+
+            registries['BiosAttributeRegistryProt0.208.208.0'] = self.bios_reg
+
+        self.sys_bios = bios.Bios(
+            self.conn, '/redfish/v1/Systems/Self/Bios',
+            registries=registries,
+            redfish_version='1.0.2')
+
+    def test__parse_attributes(self):
+        self.sys_bios._parse_attributes(self.bios_json)
+        self.assertEqual('1.0.2', self.sys_bios.redfish_version)
+        self.assertEqual('Bios', self.sys_bios.identity)
+        self.assertEqual('Current BIOS Settings',
+                         self.sys_bios.name)
+        self.assertEqual(self.sys_bios.description,
+                         'Current BIOS Settings')
+        self.assertEqual('BiosAttributeRegistryProt0.208.208.0',
+                         self.sys_bios._attribute_registry)
+
+    def test_get_attribute_registry_no_lang(self):
+
+        registry = self.sys_bios.get_attribute_registry(language='zh')
+        self.assertIsNone(registry)
+
+    def test_get_attribute_registry(self):
+
+        registry = self.sys_bios.get_attribute_registry(language="en")
+        registry2 = self.sys_bios.get_attribute_registry(language="en-US")
+
+        self.assertEqual(registry.name, 'Prot0 BIOS Attribute Registry')
+        self.assertEqual(registry.description, 'This registry defines a '
+                         'representation of BIOS Attribute instances')
+        self.assertEqual(registry.language, 'en-US')
+        self.assertEqual(registry.registry_entries.attributes[0].name,
+                         'TCG003')
+        self.assertEqual(registry.registry_entries.attributes[0].display_name,
+                         'TPM SUPPORT')
+        self.assertEqual(registry.registry_entries.attributes[0].read_only,
+                         False)
+        self.assertEqual(registry.registry_entries.attributes[0].
+                         attribute_type, 'Enumeration')
+
+        self.assertEqual(registry.name, registry2.name)
+        self.assertEqual(registry.description, registry2.description)
+        self.assertEqual(registry.language, registry2.language)
+        self.assertEqual(registry.registry_entries.attributes[0].name,
+                         registry2.registry_entries.attributes[0].name)
+        self.assertEqual(registry.registry_entries.attributes[0].display_name,
+                         registry2.registry_entries.attributes[0].display_name)
+        self.assertEqual(registry.registry_entries.attributes[0].read_only,
+                         registry2.registry_entries.attributes[0].read_only)
+        self.assertEqual(registry.registry_entries.attributes[0].
+                         attribute_type,
+                         registry2.registry_entries.attributes[0].
+                         attribute_type)
```

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_ethernet_interfaces.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_processor.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_processor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_secure_boot.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_secure_boot_database.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_simple_storage.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/system/test_system.py` & `sushy-4.5.0/sushy/tests/unit/resources/system/test_system.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/taskservice/test_task.py` & `sushy-4.5.0/sushy/tests/unit/resources/taskservice/test_task.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/taskservice/test_taskservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/taskservice/test_taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/test_base.py` & `sushy-4.5.0/sushy/tests/unit/resources/test_base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/test_settings.py` & `sushy-4.5.0/sushy/tests/unit/resources/test_settings.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/updateservice/test_softwareinventory.py` & `sushy-4.5.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/resources/updateservice/test_updateservice.py` & `sushy-4.5.0/sushy/tests/unit/resources/updateservice/test_updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/test_auth.py` & `sushy-4.5.0/sushy/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/test_connector.py` & `sushy-4.5.0/sushy/tests/unit/test_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,14 +441,51 @@
                 method='DELETE', url='http://foo.bar', response=mock_error)
 
         self.assertRaises(exceptions.ServerSideError, self.conn._op, 'DELETE',
                           'http://foo.bar')
         self.assertEqual(0, mock_sleep.call_count)
         self.assertEqual(1, self.request.call_count)
 
+    @mock.patch('time.sleep', autospec=True)
+    def test_op_retry_on_server_400_ilo_not_ready(self, mock_sleep):
+        response_info = {"error": {"@Message.ExtendedInfo": [
+            {'MessageId': 'iLO.2.15.InvalidOperationForSystemState'}]}}
+        mock_error = mock.Mock()
+        mock_error.status_code = 400
+        mock_error.json.return_value = response_info
+        self.request.return_value.status_code = (
+            http_client.INTERNAL_SERVER_ERROR)
+        self.request.return_value.json.side_effect =\
+            exceptions.ServerSideError(
+                method='DELETE', url='http://foo.bar', response=mock_error)
+
+        self.assertRaises(exceptions.ServerSideError, self.conn._op, 'DELETE',
+                          'http://foo.bar')
+        self.assertEqual(10, mock_sleep.call_count)
+        self.assertEqual(11, self.request.call_count)
+
+    @mock.patch('time.sleep', autospec=True)
+    def test_op_retry_on_server_400_ilo_not_ready_other_error(self,
+                                                              mock_sleep):
+        response_info = {"error": {"@Message.ExtendedInfo": [
+            {'MessageId': 'iLO.Invalid'}]}}
+        mock_error = mock.Mock()
+        mock_error.status_code = 400
+        mock_error.json.return_value = response_info
+        self.request.return_value.status_code = (
+            http_client.INTERNAL_SERVER_ERROR)
+        self.request.return_value.json.side_effect =\
+            exceptions.ServerSideError(
+                method='DELETE', url='http://foo.bar', response=mock_error)
+
+        self.assertRaises(exceptions.ServerSideError, self.conn._op, 'DELETE',
+                          'http://foo.bar')
+        self.assertEqual(0, mock_sleep.call_count)
+        self.assertEqual(1, self.request.call_count)
+
     def test_access_error(self):
         self.conn._auth = None
 
         self.request.return_value.status_code = http_client.FORBIDDEN
         self.request.return_value.json.side_effect = ValueError('no json')
 
         with self.assertRaisesRegex(exceptions.AccessError,
```

### Comparing `sushy-4.4.2/sushy/tests/unit/test_main.py` & `sushy-4.5.0/sushy/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/test_taskmonitor.py` & `sushy-4.5.0/sushy/tests/unit/test_taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/tests/unit/test_utils.py` & `sushy-4.5.0/sushy/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy/utils.py` & `sushy-4.5.0/sushy/utils.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/sushy.egg-info/PKG-INFO` & `sushy-4.5.0/sushy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 4.4.2
+Version: 4.5.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
```

### Comparing `sushy-4.4.2/sushy.egg-info/SOURCES.txt` & `sushy-4.5.0/sushy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -101,32 +101,36 @@
 releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
 releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
 releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
 releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
 releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
 releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
 releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
+releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
 releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
 releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
 releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
 releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
 releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
 releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
 releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
 releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
 releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
+releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
 releasenotes/notes/no-passwords-295207ac891d27ab.yaml
+releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
 releasenotes/notes/property-missing-7602c421ec177e9a.yaml
 releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
 releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
 releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
 releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
 releasenotes/notes/releasenote-d7138d1e1d414632.yaml
 releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
 releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
+releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
 releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
 releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
 releasenotes/notes/sessions.yml
 releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
 releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
 releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
 releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
@@ -134,14 +138,15 @@
 releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
 releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
 releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
 releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
 releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
 releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
 releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
@@ -259,15 +264,18 @@
 sushy/tests/unit/test_taskmonitor.py
 sushy/tests/unit/test_utils.py
 sushy/tests/unit/json_samples/TestRegistry.zip
 sushy/tests/unit/json_samples/bare_minimum_root.json
 sushy/tests/unit/json_samples/bios.json
 sushy/tests/unit/json_samples/bios_attribute_registry.json
 sushy/tests/unit/json_samples/bios_attribute_registry_file.json
+sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
+sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
 sushy/tests/unit/json_samples/bios_settings.json
+sushy/tests/unit/json_samples/bios_zt.json
 sushy/tests/unit/json_samples/certificate.json
 sushy/tests/unit/json_samples/certificate_collection.json
 sushy/tests/unit/json_samples/certificate_locations.json
 sushy/tests/unit/json_samples/certificateservice.json
 sushy/tests/unit/json_samples/chassis.json
 sushy/tests/unit/json_samples/chassis_collection.json
 sushy/tests/unit/json_samples/compositionservice.json
@@ -337,15 +345,17 @@
 sushy/tests/unit/json_samples/system_collection.json
 sushy/tests/unit/json_samples/task.json
 sushy/tests/unit/json_samples/task2.json
 sushy/tests/unit/json_samples/task_collection.json
 sushy/tests/unit/json_samples/task_monitor.json
 sushy/tests/unit/json_samples/taskservice.json
 sushy/tests/unit/json_samples/thermal.json
+sushy/tests/unit/json_samples/transfer_method_required_error.json
 sushy/tests/unit/json_samples/transfer_proto_required_error.json
+sushy/tests/unit/json_samples/transfer_proto_required_error2.json
 sushy/tests/unit/json_samples/updateservice.json
 sushy/tests/unit/json_samples/updateservice_no_inv.json
 sushy/tests/unit/json_samples/virtual_media.json
 sushy/tests/unit/json_samples/virtual_media_collection.json
 sushy/tests/unit/json_samples/volume.json
 sushy/tests/unit/json_samples/volume2.json
 sushy/tests/unit/json_samples/volume3.json
```

### Comparing `sushy-4.4.2/tools/generate-enum.py` & `sushy-4.5.0/tools/generate-enum.py`

 * *Files identical despite different names*

### Comparing `sushy-4.4.2/tox.ini` & `sushy-4.5.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
   -r{toxinidir}/requirements.txt
 commands = stestr run --slowest {posargs}
 
 [testenv:pep8]
 deps=
-    hacking>=4.1.0,<5.0.0 # Apache-2.0
+    hacking~=6.0.0 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
     pycodestyle>=2.0.0,<3.0.0 # MIT
 commands = flake8 {posargs}
 
 [testenv:venv]
 setenv = PYTHONHASHSEED=0
 deps =
@@ -79,11 +79,11 @@
 # [H203] Use assertIs(Not)None to check for None.
 # [H204] Use assert(Not)Equal to check for equality.
 # [H205] Use assert(Greater|Less)(Equal) for comparison.
 # [H210] Require 'autospec', 'spec', or 'spec_set' in mock.patch/mock.patch.object calls
 # [H904] Delay string interpolations at logging calls.
 enable-extensions=H106,H203,H204,H205,H210,H904
 builtins = _
-exclude=.venv,.git,.tox,dist,doc,*lib/python*,*egg,build
+exclude=.*,dist,doc,*lib/python*,*egg,build
 import-order-style = pep8
 application-import-names = sushy
 filename = *.py
```

### Comparing `sushy-4.4.2/zuul.d/sushy-jobs.yaml` & `sushy-4.5.0/zuul.d/sushy-jobs.yaml`

 * *Files identical despite different names*

