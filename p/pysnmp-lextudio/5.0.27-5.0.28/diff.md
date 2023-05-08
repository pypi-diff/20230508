# Comparing `tmp/pysnmp_lextudio-5.0.27.tar.gz` & `tmp/pysnmp_lextudio-5.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnmp_lextudio-5.0.27.tar", max compression
+gzip compressed data, was "pysnmp_lextudio-5.0.28.tar", max compression
```

## Comparing `pysnmp_lextudio-5.0.27.tar` & `pysnmp_lextudio-5.0.28.tar`

### file list

```diff
@@ -1,326 +1,326 @@
--rw-r--r--   0        0        0     1386 2023-01-21 20:50:50.830634 pysnmp_lextudio-5.0.27/LICENSE.rst
--rw-r--r--   0        0        0     6528 2023-04-28 19:33:54.577293 pysnmp_lextudio-5.0.27/README.md
--rw-r--r--   0        0        0     7418 2022-11-10 07:54:24.451176 pysnmp_lextudio-5.0.27/docs/Makefile
--rw-r--r--   0        0        0      226 2022-11-10 07:54:24.451245 pysnmp_lextudio-5.0.27/docs/README.txt
--rw-r--r--   0        0        0     1670 2023-01-21 20:50:50.833766 pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-MIB.txt
--rw-r--r--   0        0        0     2774 2023-01-21 20:50:50.834272 pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-SOURCE-MIB.txt
--rw-r--r--   0        0        0     7084 2023-02-26 23:53:14.445656 pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-USM-MIB.txt
--rw-r--r--   0        0        0     1738 2022-11-10 07:54:24.451628 pysnmp_lextudio-5.0.27/docs/net-snmpd.conf
--rw-r--r--   0        0        0     2141 2022-11-10 07:54:24.451741 pysnmp_lextudio-5.0.27/docs/net-snmptrapd.conf
--rw-r--r--   0        0        0      232 2022-11-10 07:54:24.451936 pysnmp_lextudio-5.0.27/docs/source/.static/css/rtdimproved.css
--rw-r--r--   0        0        0     4030 2022-11-10 07:54:24.452014 pysnmp_lextudio-5.0.27/docs/source/.static/favicon.ico
--rw-r--r--   0        0        0      143 2023-01-29 09:26:05.471724 pysnmp_lextudio-5.0.27/docs/source/.static/google_analytics_tracker.js
--rw-r--r--   0        0        0    13811 2022-11-10 07:54:24.452123 pysnmp_lextudio-5.0.27/docs/source/.static/logo.svg
--rw-r--r--   0        0        0      557 2023-01-21 20:50:50.835204 pysnmp_lextudio-5.0.27/docs/source/.templates/layout.html
--rw-r--r--   0        0        0      558 2023-01-29 09:29:30.479143 pysnmp_lextudio-5.0.27/docs/source/.templates/sourcelink.html
--rw-r--r--   0        0        0       54 2022-11-10 07:54:24.452185 pysnmp_lextudio-5.0.27/docs/source/changelog.rst
--rw-r--r--   0        0        0    10773 2023-04-29 01:45:28.989268 pysnmp_lextudio-5.0.27/docs/source/conf.py
--rw-r--r--   0        0        0     5167 2023-01-21 20:50:50.836511 pysnmp_lextudio-5.0.27/docs/source/development.rst
--rw-r--r--   0        0        0     9568 2023-01-28 08:01:44.614630 pysnmp_lextudio-5.0.27/docs/source/docs/api-reference.rst
--rw-r--r--   0        0        0      138 2022-11-10 08:01:10.001761 pysnmp_lextudio-5.0.27/docs/source/docs/hlapi/asyncio/agent/ntforg/notification.rst
--rw-r--r--   0        0        0      111 2022-11-10 08:01:10.001888 pysnmp_lextudio-5.0.27/docs/source/docs/hlapi/asyncio/manager/cmdgen/bulkcmd.rst
--rw-r--r--   0        0        0      102 2022-11-10 08:01:10.001957 pysnmp_lextudio-5.0.27/docs/source/docs/hlapi/asyncio/manager/cmdgen/getcmd.rst
--rw-r--r--   0        0        0      111 2022-11-10 08:01:10.002015 pysnmp_lextudio-5.0.27/docs/source/docs/hlapi/asyncio/manager/cmdgen/nextcmd.rst
--rw-r--r--   0        0        0      102 2022-11-10 08:01:10.002070 pysnmp_lextudio-5.0.27/docs/source/docs/hlapi/asyncio/manager/cmdgen/setcmd.rst
--rw-r--r--   0        0        0    28148 2022-11-10 07:54:24.456435 pysnmp_lextudio-5.0.27/docs/source/docs/mib-object-instances.svg
--rw-r--r--   0        0        0   134409 2022-11-10 07:54:24.457060 pysnmp_lextudio-5.0.27/docs/source/docs/nms-components.svg
--rw-r--r--   0        0        0    25840 2022-11-10 07:54:24.457265 pysnmp_lextudio-5.0.27/docs/source/docs/oid-tree-mibs.svg
--rw-r--r--   0        0        0    17023 2022-11-10 07:54:24.457488 pysnmp_lextudio-5.0.27/docs/source/docs/oid-tree.svg
--rw-r--r--   0        0        0     4769 2023-04-28 19:25:50.731506 pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-architecture.rst
--rw-r--r--   0        0        0    35260 2023-01-21 20:50:50.837684 pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-design.svg
--rw-r--r--   0        0        0    22937 2023-04-21 00:52:22.286522 pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-hlapi-tutorial.rst
--rw-r--r--   0        0        0    11023 2022-11-10 07:54:24.458530 pysnmp_lextudio-5.0.27/docs/source/docs/snmp-apps.svg
--rw-r--r--   0        0        0    10594 2023-01-21 20:50:50.840073 pysnmp_lextudio-5.0.27/docs/source/docs/snmp-design.rst
--rw-r--r--   0        0        0    19939 2022-11-10 07:54:24.458826 pysnmp_lextudio-5.0.27/docs/source/docs/snmp-engine.svg
--rw-r--r--   0        0        0     4748 2022-11-10 07:54:24.458954 pysnmp_lextudio-5.0.27/docs/source/docs/snmp-history.rst
--rw-r--r--   0        0        0      164 2022-11-10 08:01:10.003361 pysnmp_lextudio-5.0.27/docs/source/docs/tutorial.rst
--rw-r--r--   0        0        0      960 2023-04-29 01:49:59.423191 pysnmp_lextudio-5.0.27/docs/source/download.rst
--rw-r--r--   0        0        0      537 2022-11-10 08:01:10.003968 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst
--rw-r--r--   0        0        0      468 2022-11-10 08:01:10.004053 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/agent/ntforg/common-notifications.rst
--rw-r--r--   0        0        0     2423 2023-04-21 00:52:22.286962 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/index.rst
--rw-r--r--   0        0        0      960 2022-11-10 08:01:10.004282 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst
--rw-r--r--   0        0        0      792 2022-11-10 08:01:10.004363 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst
--rw-r--r--   0        0        0      467 2022-11-10 08:01:10.004435 pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/manager/cmdgen/walking-operations.rst
--rw-r--r--   0        0        0     4719 2023-04-21 00:52:22.288740 pysnmp_lextudio-5.0.27/docs/source/examples/index.rst
--rw-r--r--   0        0        0      745 2022-11-10 07:54:24.466971 pysnmp_lextudio-5.0.27/docs/source/examples/smi/agent/implementing-mib-objects.rst
--rw-r--r--   0        0        0     1184 2022-11-10 07:54:24.467088 pysnmp_lextudio-5.0.27/docs/source/examples/smi/manager/browsing-mib-tree.rst
--rw-r--r--   0        0        0      600 2023-04-21 00:52:22.289077 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst
--rw-r--r--   0        0        0      895 2023-04-21 00:52:22.289192 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst
--rw-r--r--   0        0        0      486 2023-04-21 00:52:22.289317 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/fetching-variables.rst
--rw-r--r--   0        0        0      455 2023-04-21 00:52:22.289376 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/modifying-variables.rst
--rw-r--r--   0        0        0      868 2023-04-21 00:52:22.289431 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst
--rw-r--r--   0        0        0      877 2023-04-21 00:52:22.289507 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst
--rw-r--r--   0        0        0      530 2023-04-21 00:52:22.289594 pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst
--rw-r--r--   0        0        0      483 2022-11-10 07:54:24.468931 pysnmp_lextudio-5.0.27/docs/source/examples/v3arch/asyncio/agent/cmdrsp/snmp-versions.rst
--rw-r--r--   0        0        0     1531 2023-01-21 20:50:50.841628 pysnmp_lextudio-5.0.27/docs/source/examples/v3arch/asyncio/index.rst
--rw-r--r--   0        0        0      482 2022-11-10 07:54:24.469199 pysnmp_lextudio-5.0.27/docs/source/examples/v3arch/asyncio/manager/ntfrcv/transport-tweaks.rst
--rw-r--r--   0        0        0     1410 2022-11-10 07:54:24.472768 pysnmp_lextudio-5.0.27/docs/source/faq/getting-peer-information.rst
--rw-r--r--   0        0        0     3823 2022-11-10 07:54:24.472856 pysnmp_lextudio-5.0.27/docs/source/faq/how-to-implement-agent-mib.rst
--rw-r--r--   0        0        0     3139 2023-01-23 07:07:30.039469 pysnmp_lextudio-5.0.27/docs/source/faq/ignored-snmp-packets.rst
--rw-r--r--   0        0        0     1224 2022-11-10 07:54:24.473003 pysnmp_lextudio-5.0.27/docs/source/faq/listening-on-multiple-interfaces.rst
--rw-r--r--   0        0        0     1016 2023-01-21 20:50:50.843902 pysnmp_lextudio-5.0.27/docs/source/faq/non-printable-snmp-values-apps.rst
--rw-r--r--   0        0        0     1538 2022-11-10 07:54:24.473152 pysnmp_lextudio-5.0.27/docs/source/faq/non-printable-snmp-values-tools.rst
--rw-r--r--   0        0        0     2004 2023-01-21 20:50:50.844674 pysnmp_lextudio-5.0.27/docs/source/faq/oids-not-increasing.rst
--rw-r--r--   0        0        0     1983 2023-01-21 20:50:50.845230 pysnmp_lextudio-5.0.27/docs/source/faq/pass-custom-mib-to-manager.rst
--rw-r--r--   0        0        0     1237 2022-11-10 07:54:24.473460 pysnmp_lextudio-5.0.27/docs/source/faq/py2exe-throws-error.rst
--rw-r--r--   0        0        0     1726 2022-11-10 07:54:24.473561 pysnmp_lextudio-5.0.27/docs/source/faq/response-values-mib-resolution.rst
--rw-r--r--   0        0        0     1596 2022-11-10 07:54:24.473654 pysnmp_lextudio-5.0.27/docs/source/faq/snmp-data-constraints-verification-failure.rst
--rw-r--r--   0        0        0      839 2022-11-10 07:54:24.473727 pysnmp_lextudio-5.0.27/docs/source/faq/walk-whole-mib.rst
--rw-r--r--   0        0        0      389 2023-01-21 20:50:50.843361 pysnmp_lextudio-5.0.27/docs/source/faq.rst
--rw-r--r--   0        0        0     3207 2023-01-21 20:50:50.849633 pysnmp_lextudio-5.0.27/docs/source/index.rst
--rw-r--r--   0        0        0       49 2022-11-10 07:54:24.473797 pysnmp_lextudio-5.0.27/docs/source/license.rst
--rw-r--r--   0        0        0      330 2023-01-21 20:50:50.850267 pysnmp_lextudio-5.0.27/docs/source/oldsite.rst
--rw-r--r--   0        0        0     1871 2023-01-28 05:36:25.676602 pysnmp_lextudio-5.0.27/docs/source/quick-start.rst
--rw-r--r--   0        0        0      363 2023-01-21 20:50:50.852549 pysnmp_lextudio-5.0.27/examples/README.md
--rw-r--r--   0        0        0     1336 2023-01-28 02:10:04.207146 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py
--rw-r--r--   0        0        0     1941 2023-01-28 02:10:04.207497 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py
--rw-r--r--   0        0        0     1581 2023-01-28 08:09:49.565481 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/v3-inform.py
--rw-r--r--   0        0        0     1304 2023-01-21 20:50:50.858767 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py
--rw-r--r--   0        0        0     1648 2023-01-28 02:10:04.207259 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py
--rw-r--r--   0        0        0     1556 2023-01-28 02:10:04.207201 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     1559 2023-01-28 02:10:04.207244 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py
--rw-r--r--   0        0        0     1728 2023-04-21 00:52:22.290304 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py
--rw-r--r--   0        0        0     1120 2023-01-28 02:10:04.207716 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-get.py
--rw-r--r--   0        0        0     1125 2023-01-28 02:10:04.207214 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-next.py
--rw-r--r--   0        0        0     1134 2023-01-28 02:10:04.207668 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-set.py
--rw-r--r--   0        0        0     1148 2023-01-28 02:10:04.207230 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py
--rw-r--r--   0        0        0     1120 2023-04-21 00:52:22.290743 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py
--rw-r--r--   0        0        0     1119 2023-01-28 20:02:25.533801 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py
--rw-r--r--   0        0        0     1133 2023-01-28 02:10:04.207177 pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py
--rw-r--r--   0        0        0     1601 2023-01-28 02:10:04.201800 pysnmp_lextudio-5.0.27/examples/smi/agent/custom-managed-object.py
--rw-r--r--   0        0        0     1745 2023-01-28 02:10:04.093856 pysnmp_lextudio-5.0.27/examples/smi/agent/operations-on-managed-objects.py
--rw-r--r--   0        0        0    17033 2023-01-21 20:50:50.867580 pysnmp_lextudio-5.0.27/examples/smi/manager/builder.py
--rw-r--r--   0        0        0     1338 2023-04-21 00:52:22.291317 pysnmp_lextudio-5.0.27/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py
--rw-r--r--   0        0        0     3809 2023-01-28 02:10:04.201814 pysnmp_lextudio-5.0.27/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py
--rw-r--r--   0        0        0     2617 2023-01-28 02:10:04.111797 pysnmp_lextudio-5.0.27/examples/smi/manager/mib-tree-inspection.py
--rw-r--r--   0        0        0     1045 2023-04-21 00:52:22.291835 pysnmp_lextudio-5.0.27/examples/smi/manager/print-oid-description.py
--rw-r--r--   0        0        0     5169 2023-04-21 00:52:22.292532 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2849 2023-04-21 00:52:22.292945 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2406 2023-04-21 00:52:22.293292 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3235 2023-04-21 00:52:22.295613 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py
--rw-r--r--   0        0        0     3226 2023-04-21 00:52:22.295979 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py
--rw-r--r--   0        0        0     3919 2023-04-21 00:52:22.296288 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py
--rw-r--r--   0        0        0     3471 2023-04-21 00:52:22.296592 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py
--rw-r--r--   0        0        0     3901 2023-04-21 00:52:22.296931 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py
--rw-r--r--   0        0        0     2764 2023-04-21 00:52:22.297258 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py
--rw-r--r--   0        0        0     3468 2023-04-21 00:52:22.297618 pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py
--rw-r--r--   0        0        0     2677 2023-01-28 02:10:04.337349 pysnmp_lextudio-5.0.27/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py
--rw-r--r--   0        0        0     2155 2023-01-28 02:10:04.345263 pysnmp_lextudio-5.0.27/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py
--rw-r--r--   0        0        0     2519 2023-04-21 00:52:22.298051 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py
--rw-r--r--   0        0        0     2464 2023-04-21 00:52:22.298392 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py
--rw-r--r--   0        0        0     1995 2023-04-21 00:52:22.300650 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py
--rw-r--r--   0        0        0     3603 2023-04-21 00:52:22.301465 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py
--rw-r--r--   0        0        0     2458 2023-04-21 00:52:22.301890 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py
--rw-r--r--   0        0        0     4319 2023-04-21 00:52:22.302623 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py
--rw-r--r--   0        0        0     2065 2023-04-21 00:52:22.303159 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py
--rw-r--r--   0        0        0     2090 2023-04-21 00:52:22.303511 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py
--rw-r--r--   0        0        0     3167 2023-04-21 00:52:22.304156 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py
--rw-r--r--   0        0        0     2199 2023-04-21 00:52:22.304446 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py
--rw-r--r--   0        0        0     3352 2023-04-21 00:52:22.304775 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py
--rw-r--r--   0        0        0     2714 2023-04-21 00:52:22.305142 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py
--rw-r--r--   0        0        0     3314 2023-04-21 00:52:22.305471 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py
--rw-r--r--   0        0        0     3883 2023-04-21 00:52:22.305829 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py
--rw-r--r--   0        0        0     2616 2023-04-21 00:52:22.306131 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py
--rw-r--r--   0        0        0     3567 2023-04-21 00:52:22.306448 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py
--rw-r--r--   0        0        0     3393 2023-04-21 00:52:22.308732 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     2652 2023-04-21 00:52:22.309070 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py
--rw-r--r--   0        0        0     3523 2023-04-21 00:52:22.309442 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py
--rw-r--r--   0        0        0     3028 2023-04-21 00:52:22.309745 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py
--rw-r--r--   0        0        0     3333 2023-04-21 00:52:22.310190 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v1-trap.py
--rw-r--r--   0        0        0     3315 2023-04-21 00:52:22.310647 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py
--rw-r--r--   0        0        0     3360 2023-04-21 00:52:22.310987 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py
--rw-r--r--   0        0        0     3223 2023-04-21 00:52:22.311434 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py
--rw-r--r--   0        0        0     2961 2023-04-21 00:52:22.313615 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v3-trap.py
--rw-r--r--   0        0        0     2508 2023-04-21 00:52:22.314329 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py
--rw-r--r--   0        0        0     2162 2023-04-21 00:52:22.314850 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py
--rw-r--r--   0        0        0     2298 2023-04-21 00:52:22.315285 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py
--rw-r--r--   0        0        0     2572 2023-04-21 00:52:22.315750 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py
--rw-r--r--   0        0        0     2368 2023-04-21 00:52:22.316195 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py
--rw-r--r--   0        0        0     3224 2023-04-21 00:52:22.316656 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py
--rw-r--r--   0        0        0     2421 2023-04-21 00:52:22.317102 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py
--rw-r--r--   0        0        0     3631 2023-04-21 00:52:22.317652 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py
--rw-r--r--   0        0        0     2441 2023-04-21 00:52:22.318154 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py
--rw-r--r--   0        0        0     2437 2023-04-21 00:52:22.320606 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py
--rw-r--r--   0        0        0     2436 2023-04-21 00:52:22.320980 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py
--rw-r--r--   0        0        0     3102 2023-04-21 00:52:22.321321 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py
--rw-r--r--   0        0        0     2230 2023-04-21 00:52:22.321632 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py
--rw-r--r--   0        0        0     2191 2023-04-21 00:52:22.321947 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py
--rw-r--r--   0        0        0     2087 2023-04-21 00:52:22.322265 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/v1-get.py
--rw-r--r--   0        0        0     2106 2023-04-21 00:52:22.322723 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py
--rw-r--r--   0        0        0     2215 2023-04-21 00:52:22.325388 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py
--rw-r--r--   0        0        0     2131 2023-04-21 00:52:22.326374 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py
--rw-r--r--   0        0        0     2129 2023-04-21 00:52:22.326737 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3728 2023-04-21 00:52:22.327858 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py
--rw-r--r--   0        0        0     3313 2023-04-21 00:52:22.328342 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py
--rw-r--r--   0        0        0     3291 2023-04-21 00:52:22.328688 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py
--rw-r--r--   0        0        0     4028 2023-04-21 00:52:22.329088 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py
--rw-r--r--   0        0        0     3997 2023-04-21 00:52:22.330152 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py
--rw-r--r--   0        0        0     3980 2023-04-21 00:52:22.330836 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py
--rw-r--r--   0        0        0     4121 2023-04-21 00:52:22.331364 pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py
--rw-r--r--   0        0        0     1320 2023-04-29 01:45:28.978504 pysnmp_lextudio-5.0.27/pyproject.toml
--rw-r--r--   0        0        0      471 2023-04-29 01:45:28.988252 pysnmp_lextudio-5.0.27/pysnmp/__init__.py
--rw-r--r--   0        0        0     1252 2023-01-21 20:50:50.911870 pysnmp_lextudio-5.0.27/pysnmp/cache.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.495155 pysnmp_lextudio-5.0.27/pysnmp/carrier/__init__.py
--rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495252 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/__init__.py
--rw-r--r--   0        0        0     1857 2023-01-21 20:50:50.912293 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/base.py
--rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495435 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/__init__.py
--rw-r--r--   0        0        0     5316 2023-04-21 00:52:22.331968 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/base.py
--rw-r--r--   0        0        0     1994 2023-01-21 20:50:50.914278 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/udp.py
--rw-r--r--   0        0        0     1101 2023-01-21 20:50:50.914731 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/udp6.py
--rw-r--r--   0        0        0     3443 2023-01-21 20:50:50.916499 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dispatch.py
--rw-r--r--   0        0        0       59 2023-04-21 00:52:22.332205 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/__init__.py
--rw-r--r--   0        0        0     3335 2023-04-21 00:52:22.333698 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/base.py
--rw-r--r--   0        0        0       59 2023-04-21 00:52:22.333778 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/__init__.py
--rw-r--r--   0        0        0     7379 2023-04-21 00:52:22.334421 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/base.py
--rw-r--r--   0        0        0      584 2023-04-21 00:52:22.335041 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/udp.py
--rw-r--r--   0        0        0     1389 2023-04-21 00:52:22.335816 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/udp6.py
--rw-r--r--   0        0        0     1621 2023-04-21 00:52:22.336644 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/unix.py
--rw-r--r--   0        0        0     1734 2023-04-21 00:52:22.337494 pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dispatch.py
--rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337591 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/__init__.py
--rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337679 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/dgram/__init__.py
--rw-r--r--   0        0        0      208 2023-04-21 00:52:22.346381 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/dgram/udp.py
--rw-r--r--   0        0        0      209 2023-04-21 00:52:22.346875 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/dgram/udp6.py
--rw-r--r--   0        0        0      209 2023-04-21 00:52:22.347793 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/dgram/unix.py
--rw-r--r--   0        0        0      248 2023-04-21 00:52:22.348394 pysnmp_lextudio-5.0.27/pysnmp/carrier/asynsock/dispatch.py
--rw-r--r--   0        0        0     8140 2023-04-21 00:52:22.349103 pysnmp_lextudio-5.0.27/pysnmp/carrier/base.py
--rw-r--r--   0        0        0      235 2023-01-21 20:50:50.922097 pysnmp_lextudio-5.0.27/pysnmp/carrier/error.py
--rw-r--r--   0        0        0      676 2023-01-21 20:50:50.922367 pysnmp_lextudio-5.0.27/pysnmp/carrier/sockfix.py
--rw-r--r--   0        0        0     3558 2023-01-21 20:50:50.922632 pysnmp_lextudio-5.0.27/pysnmp/carrier/sockmsg.py
--rw-r--r--   0        0        0     3501 2023-01-21 20:50:50.922909 pysnmp_lextudio-5.0.27/pysnmp/debug.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.497717 pysnmp_lextudio-5.0.27/pysnmp/entity/__init__.py
--rw-r--r--   0        0        0    34968 2023-04-21 00:52:22.353135 pysnmp_lextudio-5.0.27/pysnmp/entity/config.py
--rw-r--r--   0        0        0     8176 2023-01-21 20:50:50.925875 pysnmp_lextudio-5.0.27/pysnmp/entity/engine.py
--rw-r--r--   0        0        0     2561 2023-01-21 20:50:50.927273 pysnmp_lextudio-5.0.27/pysnmp/entity/observer.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.498303 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/__init__.py
--rw-r--r--   0        0        0    18591 2023-01-21 20:50:50.927634 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/cmdgen.py
--rw-r--r--   0        0        0    14980 2023-01-21 20:50:50.927946 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/cmdrsp.py
--rw-r--r--   0        0        0    10212 2023-01-21 20:50:50.930359 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/config.py
--rw-r--r--   0        0        0     2623 2023-01-21 20:50:50.930748 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/context.py
--rw-r--r--   0        0        0     2855 2023-01-21 20:50:50.931078 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/mibvar.py
--rw-r--r--   0        0        0    17749 2023-01-21 20:50:50.931536 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/ntforg.py
--rw-r--r--   0        0        0     4532 2023-01-21 20:50:50.931830 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/ntfrcv.py
--rw-r--r--   0        0        0       59 2022-11-10 08:01:10.022472 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/oneliner/__init__.py
--rw-r--r--   0        0        0    10016 2023-04-21 00:52:22.354201 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/oneliner/cmdgen.py
--rw-r--r--   0        0        0     6644 2023-04-21 00:52:22.356701 pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/oneliner/ntforg.py
--rw-r--r--   0        0        0      501 2023-01-21 20:50:50.932669 pysnmp_lextudio-5.0.27/pysnmp/error.py
--rw-r--r--   0        0        0     3321 2023-04-21 00:52:22.357264 pysnmp_lextudio-5.0.27/pysnmp/hlapi/__init__.py
--rw-r--r--   0        0        0      459 2023-01-21 20:50:50.933233 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/__init__.py
--rw-r--r--   0        0        0    19830 2023-01-31 07:58:06.498827 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/cmdgen.py
--rw-r--r--   0        0        0     5525 2023-01-23 06:09:50.177751 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/ntforg.py
--rw-r--r--   0        0        0    13211 2023-01-25 01:36:58.327193 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/slim.py
--rw-r--r--   0        0        0     4976 2023-01-23 20:11:38.568253 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/transport.py
--rw-r--r--   0        0        0      462 2023-04-21 00:52:22.358928 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/__init__.py
--rw-r--r--   0        0        0    20298 2023-04-21 00:52:22.362071 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/cmdgen.py
--rw-r--r--   0        0        0     5202 2023-04-21 00:52:22.363199 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/ntforg.py
--rw-r--r--   0        0        0      624 2023-04-21 00:52:22.363767 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/__init__.py
--rw-r--r--   0        0        0    24567 2023-04-21 00:52:22.364659 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/cmdgen.py
--rw-r--r--   0        0        0       59 2023-04-21 00:52:22.364765 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/compat/__init__.py
--rw-r--r--   0        0        0     9212 2023-04-21 00:52:22.365599 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
--rw-r--r--   0        0        0     1572 2023-04-21 00:52:22.365784 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
--rw-r--r--   0        0        0     4573 2023-04-21 00:52:22.366001 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/ntforg.py
--rw-r--r--   0        0        0     5124 2023-04-21 00:52:22.366195 pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/transport.py
--rw-r--r--   0        0        0    18218 2023-04-21 00:52:22.366583 pysnmp_lextudio-5.0.27/pysnmp/hlapi/auth.py
--rw-r--r--   0        0        0     2050 2023-04-21 00:52:22.366871 pysnmp_lextudio-5.0.27/pysnmp/hlapi/context.py
--rw-r--r--   0        0        0    11790 2023-01-21 20:50:50.938949 pysnmp_lextudio-5.0.27/pysnmp/hlapi/lcd.py
--rw-r--r--   0        0        0     1922 2023-04-21 00:52:22.367114 pysnmp_lextudio-5.0.27/pysnmp/hlapi/transport.py
--rw-r--r--   0        0        0     2920 2023-01-21 20:50:50.939457 pysnmp_lextudio-5.0.27/pysnmp/hlapi/varbinds.py
--rw-r--r--   0        0        0     1197 2023-01-21 20:50:50.939677 pysnmp_lextudio-5.0.27/pysnmp/nextid.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504675 pysnmp_lextudio-5.0.27/pysnmp/proto/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504925 pysnmp_lextudio-5.0.27/pysnmp/proto/acmod/__init__.py
--rw-r--r--   0        0        0    12323 2023-01-21 20:50:50.939958 pysnmp_lextudio-5.0.27/pysnmp/proto/acmod/rfc3415.py
--rw-r--r--   0        0        0      889 2023-01-21 20:50:50.940198 pysnmp_lextudio-5.0.27/pysnmp/proto/acmod/void.py
--rw-r--r--   0        0        0      371 2023-01-21 20:50:50.940472 pysnmp_lextudio-5.0.27/pysnmp/proto/api/__init__.py
--rw-r--r--   0        0        0     9391 2023-01-21 20:50:50.940745 pysnmp_lextudio-5.0.27/pysnmp/proto/api/v1.py
--rw-r--r--   0        0        0     5599 2023-01-21 20:50:50.940989 pysnmp_lextudio-5.0.27/pysnmp/proto/api/v2c.py
--rw-r--r--   0        0        0      926 2023-04-22 01:36:13.197204 pysnmp_lextudio-5.0.27/pysnmp/proto/api/verdec.py
--rw-r--r--   0        0        0     1151 2023-04-21 00:52:22.367350 pysnmp_lextudio-5.0.27/pysnmp/proto/cache.py
--rw-r--r--   0        0        0     5977 2023-04-28 19:25:50.733203 pysnmp_lextudio-5.0.27/pysnmp/proto/errind.py
--rw-r--r--   0        0        0     1191 2023-01-21 20:50:50.941881 pysnmp_lextudio-5.0.27/pysnmp/proto/error.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.507349 pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/__init__.py
--rw-r--r--   0        0        0     1754 2023-01-21 20:50:50.942134 pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/base.py
--rw-r--r--   0        0        0     3910 2023-01-21 20:50:50.942358 pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/cache.py
--rw-r--r--   0        0        0    20350 2023-01-21 20:50:50.942628 pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/rfc2576.py
--rw-r--r--   0        0        0    35109 2023-01-22 07:40:10.590039 pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/rfc3412.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.508803 pysnmp_lextudio-5.0.27/pysnmp/proto/proxy/__init__.py
--rw-r--r--   0        0        0     9874 2023-01-21 20:50:50.943242 pysnmp_lextudio-5.0.27/pysnmp/proto/proxy/rfc2576.py
--rw-r--r--   0        0        0     6085 2023-04-21 00:52:22.367846 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1155.py
--rw-r--r--   0        0        0     3323 2023-01-21 20:50:50.943726 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1157.py
--rw-r--r--   0        0        0      563 2023-01-21 20:50:50.943981 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1901.py
--rw-r--r--   0        0        0    21296 2023-04-21 00:52:22.368250 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1902.py
--rw-r--r--   0        0        0     5671 2023-01-21 20:50:50.944541 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1905.py
--rw-r--r--   0        0        0     1374 2023-01-21 20:50:50.944781 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc3411.py
--rw-r--r--   0        0        0    21759 2023-01-21 20:50:50.945141 pysnmp_lextudio-5.0.27/pysnmp/proto/rfc3412.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510738 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/__init__.py
--rw-r--r--   0        0        0     1485 2023-01-21 20:50:50.945499 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/base.py
--rw-r--r--   0        0        0      881 2023-01-21 20:50:50.945778 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/cache.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510991 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511096 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/__init__.py
--rw-r--r--   0        0        0     1030 2023-01-21 20:50:50.946099 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aes192.py
--rw-r--r--   0        0        0      999 2023-01-21 20:50:50.946416 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aes256.py
--rw-r--r--   0        0        0     3203 2023-01-21 20:50:50.946711 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aesbase.py
--rw-r--r--   0        0        0     5517 2023-04-29 01:41:10.500798 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/des3.py
--rw-r--r--   0        0        0    21657 2023-04-21 00:52:22.368591 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc2576.py
--rw-r--r--   0        0        0      261 2023-01-21 20:50:50.947549 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511982 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/__init__.py
--rw-r--r--   0        0        0      850 2023-01-21 20:50:50.947795 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/base.py
--rw-r--r--   0        0        0     3709 2023-01-21 20:50:50.948046 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
--rw-r--r--   0        0        0     3468 2023-01-21 20:50:50.948325 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
--rw-r--r--   0        0        0      733 2023-01-22 19:49:47.441260 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/noauth.py
--rw-r--r--   0        0        0     2098 2023-01-21 20:50:50.949099 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/localkey.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.512518 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/__init__.py
--rw-r--r--   0        0        0      728 2023-01-21 20:50:50.951254 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/base.py
--rw-r--r--   0        0        0     5060 2023-04-29 01:41:47.475223 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/des.py
--rw-r--r--   0        0        0      807 2023-01-21 20:50:50.951774 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
--rw-r--r--   0        0        0    56002 2023-01-22 20:02:41.908685 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/service.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513200 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3826/__init__.py
--rw-r--r--   0        0        0       59 2022-12-02 02:52:14.601095 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3826/priv/__init__.py
--rw-r--r--   0        0        0     5041 2023-04-29 01:40:11.337560 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3826/priv/aes.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513516 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc7860/__init__.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513622 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc7860/auth/__init__.py
--rw-r--r--   0        0        0     4037 2023-01-21 20:50:50.953621 pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513825 pysnmp_lextudio-5.0.27/pysnmp/smi/__init__.py
--rw-r--r--   0        0        0    16487 2023-01-21 20:50:50.953912 pysnmp_lextudio-5.0.27/pysnmp/smi/builder.py
--rw-r--r--   0        0        0     2326 2023-04-04 18:56:40.326682 pysnmp_lextudio-5.0.27/pysnmp/smi/compiler.py
--rw-r--r--   0        0        0     2351 2023-01-21 20:50:50.954423 pysnmp_lextudio-5.0.27/pysnmp/smi/error.py
--rw-r--r--   0        0        0      317 2023-01-21 20:50:50.954638 pysnmp_lextudio-5.0.27/pysnmp/smi/exval.py
--rw-r--r--   0        0        0     3084 2023-01-21 20:50:50.954871 pysnmp_lextudio-5.0.27/pysnmp/smi/indices.py
--rw-r--r--   0        0        0     9227 2023-01-21 20:50:50.955119 pysnmp_lextudio-5.0.27/pysnmp/smi/instrum.py
--rw-r--r--   0        0        0      283 2023-01-21 20:50:50.955343 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/ASN1-ENUMERATION.py
--rw-r--r--   0        0        0      534 2023-01-21 20:50:50.955553 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/ASN1-REFINEMENT.py
--rw-r--r--   0        0        0      505 2023-01-21 20:50:50.955778 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/ASN1.py
--rw-r--r--   0        0        0    17614 2023-01-21 20:50:50.957301 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/INET-ADDRESS-MIB.py
--rw-r--r--   0        0        0     3591 2023-01-21 20:50:50.957643 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-MIB.py
--rw-r--r--   0        0        0     4620 2023-01-21 20:50:50.957971 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
--rw-r--r--   0        0        0     9922 2023-01-21 20:50:50.958209 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
--rw-r--r--   0        0        0     1318 2023-01-21 20:50:50.958608 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/RFC1158-MIB.py
--rw-r--r--   0        0        0    56809 2023-01-21 20:50:50.959093 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/RFC1213-MIB.py
--rw-r--r--   0        0        0    17437 2023-01-21 20:50:50.959514 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
--rw-r--r--   0        0        0    18836 2023-01-21 20:50:50.961309 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
--rw-r--r--   0        0        0     5882 2023-01-21 20:50:50.961679 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-MPD-MIB.py
--rw-r--r--   0        0        0    19031 2023-01-21 20:50:50.962008 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
--rw-r--r--   0        0        0    10138 2023-01-21 20:50:50.962396 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
--rw-r--r--   0        0        0    24833 2023-01-21 20:50:50.962836 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
--rw-r--r--   0        0        0     3913 2023-01-21 20:50:50.963197 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
--rw-r--r--   0        0        0    33731 2023-01-21 20:50:50.963774 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
--rw-r--r--   0        0        0     3572 2023-01-21 20:50:50.964077 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
--rw-r--r--   0        0        0     5841 2023-01-21 20:50:50.964367 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py
--rw-r--r--   0        0        0    30173 2023-01-21 20:50:50.964903 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
--rw-r--r--   0        0        0     4096 2023-01-21 20:50:50.965255 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-CONF.py
--rw-r--r--   0        0        0    31135 2023-01-21 20:50:50.965742 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-MIB.py
--rw-r--r--   0        0        0    46776 2023-01-21 20:50:50.966284 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-SMI.py
--rw-r--r--   0        0        0    28986 2023-01-21 20:50:50.966685 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-TC.py
--rw-r--r--   0        0        0     6921 2023-01-21 20:50:50.967022 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-TM.py
--rw-r--r--   0        0        0    24370 2023-01-21 20:50:50.967422 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.522800 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/__init__.py
--rw-r--r--   0        0        0      926 2023-01-21 20:50:50.967752 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
--rw-r--r--   0        0        0     1174 2023-01-21 20:50:50.968042 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
--rw-r--r--   0        0        0     1047 2023-01-21 20:50:50.968298 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
--rw-r--r--   0        0        0     1046 2023-01-21 20:50:50.968546 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
--rw-r--r--   0        0        0     2232 2023-01-21 20:50:50.968782 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
--rw-r--r--   0        0        0      530 2023-01-21 20:50:50.969033 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
--rw-r--r--   0        0        0     7605 2023-01-21 20:50:50.969323 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
--rw-r--r--   0        0        0       59 2022-11-10 07:54:24.523596 pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__init__.py
--rw-r--r--   0        0        0    44735 2023-04-21 00:52:22.370798 pysnmp_lextudio-5.0.27/pysnmp/smi/rfc1902.py
--rw-r--r--   0        0        0    12218 2023-01-21 20:50:50.971883 pysnmp_lextudio-5.0.27/pysnmp/smi/view.py
--rw-r--r--   0        0        0     8299 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.27/setup.py
--rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.27/PKG-INFO
+-rw-r--r--   0        0        0     1386 2023-01-21 20:50:50.830634 pysnmp_lextudio-5.0.28/LICENSE.rst
+-rw-r--r--   0        0        0     6528 2023-04-28 19:33:54.577293 pysnmp_lextudio-5.0.28/README.md
+-rw-r--r--   0        0        0     7418 2022-11-10 07:54:24.451176 pysnmp_lextudio-5.0.28/docs/Makefile
+-rw-r--r--   0        0        0      226 2022-11-10 07:54:24.451245 pysnmp_lextudio-5.0.28/docs/README.txt
+-rw-r--r--   0        0        0     1670 2023-01-21 20:50:50.833766 pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-MIB.txt
+-rw-r--r--   0        0        0     2774 2023-01-21 20:50:50.834272 pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-SOURCE-MIB.txt
+-rw-r--r--   0        0        0     7084 2023-02-26 23:53:14.445656 pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-USM-MIB.txt
+-rw-r--r--   0        0        0     1738 2022-11-10 07:54:24.451628 pysnmp_lextudio-5.0.28/docs/net-snmpd.conf
+-rw-r--r--   0        0        0     2141 2022-11-10 07:54:24.451741 pysnmp_lextudio-5.0.28/docs/net-snmptrapd.conf
+-rw-r--r--   0        0        0      232 2022-11-10 07:54:24.451936 pysnmp_lextudio-5.0.28/docs/source/.static/css/rtdimproved.css
+-rw-r--r--   0        0        0     4030 2022-11-10 07:54:24.452014 pysnmp_lextudio-5.0.28/docs/source/.static/favicon.ico
+-rw-r--r--   0        0        0      143 2023-01-29 09:26:05.471724 pysnmp_lextudio-5.0.28/docs/source/.static/google_analytics_tracker.js
+-rw-r--r--   0        0        0    13811 2022-11-10 07:54:24.452123 pysnmp_lextudio-5.0.28/docs/source/.static/logo.svg
+-rw-r--r--   0        0        0      557 2023-01-21 20:50:50.835204 pysnmp_lextudio-5.0.28/docs/source/.templates/layout.html
+-rw-r--r--   0        0        0      558 2023-01-29 09:29:30.479143 pysnmp_lextudio-5.0.28/docs/source/.templates/sourcelink.html
+-rw-r--r--   0        0        0       54 2022-11-10 07:54:24.452185 pysnmp_lextudio-5.0.28/docs/source/changelog.rst
+-rw-r--r--   0        0        0    10773 2023-05-08 04:13:48.520870 pysnmp_lextudio-5.0.28/docs/source/conf.py
+-rw-r--r--   0        0        0     5167 2023-01-21 20:50:50.836511 pysnmp_lextudio-5.0.28/docs/source/development.rst
+-rw-r--r--   0        0        0     9568 2023-01-28 08:01:44.614630 pysnmp_lextudio-5.0.28/docs/source/docs/api-reference.rst
+-rw-r--r--   0        0        0      138 2022-11-10 08:01:10.001761 pysnmp_lextudio-5.0.28/docs/source/docs/hlapi/asyncio/agent/ntforg/notification.rst
+-rw-r--r--   0        0        0      111 2022-11-10 08:01:10.001888 pysnmp_lextudio-5.0.28/docs/source/docs/hlapi/asyncio/manager/cmdgen/bulkcmd.rst
+-rw-r--r--   0        0        0      102 2022-11-10 08:01:10.001957 pysnmp_lextudio-5.0.28/docs/source/docs/hlapi/asyncio/manager/cmdgen/getcmd.rst
+-rw-r--r--   0        0        0      111 2022-11-10 08:01:10.002015 pysnmp_lextudio-5.0.28/docs/source/docs/hlapi/asyncio/manager/cmdgen/nextcmd.rst
+-rw-r--r--   0        0        0      102 2022-11-10 08:01:10.002070 pysnmp_lextudio-5.0.28/docs/source/docs/hlapi/asyncio/manager/cmdgen/setcmd.rst
+-rw-r--r--   0        0        0    28148 2022-11-10 07:54:24.456435 pysnmp_lextudio-5.0.28/docs/source/docs/mib-object-instances.svg
+-rw-r--r--   0        0        0   134409 2022-11-10 07:54:24.457060 pysnmp_lextudio-5.0.28/docs/source/docs/nms-components.svg
+-rw-r--r--   0        0        0    25840 2022-11-10 07:54:24.457265 pysnmp_lextudio-5.0.28/docs/source/docs/oid-tree-mibs.svg
+-rw-r--r--   0        0        0    17023 2022-11-10 07:54:24.457488 pysnmp_lextudio-5.0.28/docs/source/docs/oid-tree.svg
+-rw-r--r--   0        0        0     4769 2023-04-28 19:25:50.731506 pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-architecture.rst
+-rw-r--r--   0        0        0    35260 2023-01-21 20:50:50.837684 pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-design.svg
+-rw-r--r--   0        0        0    22937 2023-04-21 00:52:22.286522 pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-hlapi-tutorial.rst
+-rw-r--r--   0        0        0    11023 2022-11-10 07:54:24.458530 pysnmp_lextudio-5.0.28/docs/source/docs/snmp-apps.svg
+-rw-r--r--   0        0        0    10594 2023-01-21 20:50:50.840073 pysnmp_lextudio-5.0.28/docs/source/docs/snmp-design.rst
+-rw-r--r--   0        0        0    19939 2022-11-10 07:54:24.458826 pysnmp_lextudio-5.0.28/docs/source/docs/snmp-engine.svg
+-rw-r--r--   0        0        0     4748 2022-11-10 07:54:24.458954 pysnmp_lextudio-5.0.28/docs/source/docs/snmp-history.rst
+-rw-r--r--   0        0        0      164 2022-11-10 08:01:10.003361 pysnmp_lextudio-5.0.28/docs/source/docs/tutorial.rst
+-rw-r--r--   0        0        0      960 2023-04-29 01:49:59.423191 pysnmp_lextudio-5.0.28/docs/source/download.rst
+-rw-r--r--   0        0        0      537 2022-11-10 08:01:10.003968 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst
+-rw-r--r--   0        0        0      468 2022-11-10 08:01:10.004053 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/agent/ntforg/common-notifications.rst
+-rw-r--r--   0        0        0     2423 2023-04-21 00:52:22.286962 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/index.rst
+-rw-r--r--   0        0        0      960 2022-11-10 08:01:10.004282 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst
+-rw-r--r--   0        0        0      792 2022-11-10 08:01:10.004363 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst
+-rw-r--r--   0        0        0      467 2022-11-10 08:01:10.004435 pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/manager/cmdgen/walking-operations.rst
+-rw-r--r--   0        0        0     4719 2023-04-21 00:52:22.288740 pysnmp_lextudio-5.0.28/docs/source/examples/index.rst
+-rw-r--r--   0        0        0      745 2022-11-10 07:54:24.466971 pysnmp_lextudio-5.0.28/docs/source/examples/smi/agent/implementing-mib-objects.rst
+-rw-r--r--   0        0        0     1184 2022-11-10 07:54:24.467088 pysnmp_lextudio-5.0.28/docs/source/examples/smi/manager/browsing-mib-tree.rst
+-rw-r--r--   0        0        0      600 2023-04-21 00:52:22.289077 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst
+-rw-r--r--   0        0        0      895 2023-04-21 00:52:22.289192 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst
+-rw-r--r--   0        0        0      486 2023-04-21 00:52:22.289317 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/fetching-variables.rst
+-rw-r--r--   0        0        0      455 2023-04-21 00:52:22.289376 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/modifying-variables.rst
+-rw-r--r--   0        0        0      868 2023-04-21 00:52:22.289431 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst
+-rw-r--r--   0        0        0      877 2023-04-21 00:52:22.289507 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst
+-rw-r--r--   0        0        0      530 2023-04-21 00:52:22.289594 pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst
+-rw-r--r--   0        0        0      483 2022-11-10 07:54:24.468931 pysnmp_lextudio-5.0.28/docs/source/examples/v3arch/asyncio/agent/cmdrsp/snmp-versions.rst
+-rw-r--r--   0        0        0     1531 2023-01-21 20:50:50.841628 pysnmp_lextudio-5.0.28/docs/source/examples/v3arch/asyncio/index.rst
+-rw-r--r--   0        0        0      482 2022-11-10 07:54:24.469199 pysnmp_lextudio-5.0.28/docs/source/examples/v3arch/asyncio/manager/ntfrcv/transport-tweaks.rst
+-rw-r--r--   0        0        0     1410 2022-11-10 07:54:24.472768 pysnmp_lextudio-5.0.28/docs/source/faq/getting-peer-information.rst
+-rw-r--r--   0        0        0     3823 2022-11-10 07:54:24.472856 pysnmp_lextudio-5.0.28/docs/source/faq/how-to-implement-agent-mib.rst
+-rw-r--r--   0        0        0     3139 2023-01-23 07:07:30.039469 pysnmp_lextudio-5.0.28/docs/source/faq/ignored-snmp-packets.rst
+-rw-r--r--   0        0        0     1224 2022-11-10 07:54:24.473003 pysnmp_lextudio-5.0.28/docs/source/faq/listening-on-multiple-interfaces.rst
+-rw-r--r--   0        0        0     1016 2023-01-21 20:50:50.843902 pysnmp_lextudio-5.0.28/docs/source/faq/non-printable-snmp-values-apps.rst
+-rw-r--r--   0        0        0     1538 2022-11-10 07:54:24.473152 pysnmp_lextudio-5.0.28/docs/source/faq/non-printable-snmp-values-tools.rst
+-rw-r--r--   0        0        0     2004 2023-01-21 20:50:50.844674 pysnmp_lextudio-5.0.28/docs/source/faq/oids-not-increasing.rst
+-rw-r--r--   0        0        0     1983 2023-01-21 20:50:50.845230 pysnmp_lextudio-5.0.28/docs/source/faq/pass-custom-mib-to-manager.rst
+-rw-r--r--   0        0        0     1237 2022-11-10 07:54:24.473460 pysnmp_lextudio-5.0.28/docs/source/faq/py2exe-throws-error.rst
+-rw-r--r--   0        0        0     1726 2022-11-10 07:54:24.473561 pysnmp_lextudio-5.0.28/docs/source/faq/response-values-mib-resolution.rst
+-rw-r--r--   0        0        0     1596 2022-11-10 07:54:24.473654 pysnmp_lextudio-5.0.28/docs/source/faq/snmp-data-constraints-verification-failure.rst
+-rw-r--r--   0        0        0      839 2022-11-10 07:54:24.473727 pysnmp_lextudio-5.0.28/docs/source/faq/walk-whole-mib.rst
+-rw-r--r--   0        0        0      389 2023-01-21 20:50:50.843361 pysnmp_lextudio-5.0.28/docs/source/faq.rst
+-rw-r--r--   0        0        0     3207 2023-01-21 20:50:50.849633 pysnmp_lextudio-5.0.28/docs/source/index.rst
+-rw-r--r--   0        0        0       49 2022-11-10 07:54:24.473797 pysnmp_lextudio-5.0.28/docs/source/license.rst
+-rw-r--r--   0        0        0      330 2023-01-21 20:50:50.850267 pysnmp_lextudio-5.0.28/docs/source/oldsite.rst
+-rw-r--r--   0        0        0     1871 2023-01-28 05:36:25.676602 pysnmp_lextudio-5.0.28/docs/source/quick-start.rst
+-rw-r--r--   0        0        0      363 2023-01-21 20:50:50.852549 pysnmp_lextudio-5.0.28/examples/README.md
+-rw-r--r--   0        0        0     1336 2023-01-28 02:10:04.207146 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py
+-rw-r--r--   0        0        0     1941 2023-01-28 02:10:04.207497 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py
+-rw-r--r--   0        0        0     1581 2023-01-28 08:09:49.565481 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/v3-inform.py
+-rw-r--r--   0        0        0     1304 2023-01-21 20:50:50.858767 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py
+-rw-r--r--   0        0        0     1648 2023-01-28 02:10:04.207259 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py
+-rw-r--r--   0        0        0     1556 2023-01-28 02:10:04.207201 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     1559 2023-01-28 02:10:04.207244 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py
+-rw-r--r--   0        0        0     1728 2023-05-08 04:15:54.256116 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py
+-rw-r--r--   0        0        0     1120 2023-01-28 02:10:04.207716 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-get.py
+-rw-r--r--   0        0        0     1125 2023-01-28 02:10:04.207214 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-next.py
+-rw-r--r--   0        0        0     1134 2023-01-28 02:10:04.207668 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-set.py
+-rw-r--r--   0        0        0     1148 2023-01-28 02:10:04.207230 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py
+-rw-r--r--   0        0        0     1120 2023-04-21 00:52:22.290743 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py
+-rw-r--r--   0        0        0     1119 2023-01-28 20:02:25.533801 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py
+-rw-r--r--   0        0        0     1133 2023-01-28 02:10:04.207177 pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     1601 2023-01-28 02:10:04.201800 pysnmp_lextudio-5.0.28/examples/smi/agent/custom-managed-object.py
+-rw-r--r--   0        0        0     1745 2023-01-28 02:10:04.093856 pysnmp_lextudio-5.0.28/examples/smi/agent/operations-on-managed-objects.py
+-rw-r--r--   0        0        0    17033 2023-01-21 20:50:50.867580 pysnmp_lextudio-5.0.28/examples/smi/manager/builder.py
+-rw-r--r--   0        0        0     1338 2023-04-21 00:52:22.291317 pysnmp_lextudio-5.0.28/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py
+-rw-r--r--   0        0        0     3809 2023-01-28 02:10:04.201814 pysnmp_lextudio-5.0.28/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py
+-rw-r--r--   0        0        0     2617 2023-01-28 02:10:04.111797 pysnmp_lextudio-5.0.28/examples/smi/manager/mib-tree-inspection.py
+-rw-r--r--   0        0        0     1045 2023-04-21 00:52:22.291835 pysnmp_lextudio-5.0.28/examples/smi/manager/print-oid-description.py
+-rw-r--r--   0        0        0     5169 2023-04-21 00:52:22.292532 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2849 2023-04-21 00:52:22.292945 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2406 2023-04-21 00:52:22.293292 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3235 2023-04-21 00:52:22.295613 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py
+-rw-r--r--   0        0        0     3226 2023-04-21 00:52:22.295979 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py
+-rw-r--r--   0        0        0     3919 2023-04-21 00:52:22.296288 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py
+-rw-r--r--   0        0        0     3471 2023-04-21 00:52:22.296592 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py
+-rw-r--r--   0        0        0     3901 2023-04-21 00:52:22.296931 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py
+-rw-r--r--   0        0        0     2764 2023-04-21 00:52:22.297258 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     3468 2023-04-21 00:52:22.297618 pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py
+-rw-r--r--   0        0        0     2677 2023-01-28 02:10:04.337349 pysnmp_lextudio-5.0.28/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py
+-rw-r--r--   0        0        0     2155 2023-01-28 02:10:04.345263 pysnmp_lextudio-5.0.28/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py
+-rw-r--r--   0        0        0     2519 2023-04-21 00:52:22.298051 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py
+-rw-r--r--   0        0        0     2464 2023-04-21 00:52:22.298392 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py
+-rw-r--r--   0        0        0     1995 2023-04-21 00:52:22.300650 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py
+-rw-r--r--   0        0        0     3603 2023-04-21 00:52:22.301465 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py
+-rw-r--r--   0        0        0     2458 2023-04-21 00:52:22.301890 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py
+-rw-r--r--   0        0        0     4319 2023-04-21 00:52:22.302623 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py
+-rw-r--r--   0        0        0     2065 2023-04-21 00:52:22.303159 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py
+-rw-r--r--   0        0        0     2090 2023-04-21 00:52:22.303511 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py
+-rw-r--r--   0        0        0     3167 2023-04-21 00:52:22.304156 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py
+-rw-r--r--   0        0        0     2199 2023-04-21 00:52:22.304446 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py
+-rw-r--r--   0        0        0     3352 2023-04-21 00:52:22.304775 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py
+-rw-r--r--   0        0        0     2714 2023-04-21 00:52:22.305142 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py
+-rw-r--r--   0        0        0     3314 2023-04-21 00:52:22.305471 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py
+-rw-r--r--   0        0        0     3883 2023-04-21 00:52:22.305829 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py
+-rw-r--r--   0        0        0     2616 2023-04-21 00:52:22.306131 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py
+-rw-r--r--   0        0        0     3567 2023-04-21 00:52:22.306448 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py
+-rw-r--r--   0        0        0     3393 2023-04-21 00:52:22.308732 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     2652 2023-04-21 00:52:22.309070 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py
+-rw-r--r--   0        0        0     3523 2023-04-21 00:52:22.309442 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py
+-rw-r--r--   0        0        0     3028 2023-04-21 00:52:22.309745 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py
+-rw-r--r--   0        0        0     3333 2023-04-21 00:52:22.310190 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v1-trap.py
+-rw-r--r--   0        0        0     3315 2023-04-21 00:52:22.310647 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py
+-rw-r--r--   0        0        0     3360 2023-04-21 00:52:22.310987 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py
+-rw-r--r--   0        0        0     3223 2023-04-21 00:52:22.311434 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py
+-rw-r--r--   0        0        0     2961 2023-04-21 00:52:22.313615 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v3-trap.py
+-rw-r--r--   0        0        0     2508 2023-04-21 00:52:22.314329 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py
+-rw-r--r--   0        0        0     2162 2023-04-21 00:52:22.314850 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py
+-rw-r--r--   0        0        0     2298 2023-04-21 00:52:22.315285 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py
+-rw-r--r--   0        0        0     2572 2023-04-21 00:52:22.315750 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py
+-rw-r--r--   0        0        0     2368 2023-04-21 00:52:22.316195 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py
+-rw-r--r--   0        0        0     3224 2023-04-21 00:52:22.316656 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py
+-rw-r--r--   0        0        0     2421 2023-04-21 00:52:22.317102 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py
+-rw-r--r--   0        0        0     3631 2023-04-21 00:52:22.317652 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py
+-rw-r--r--   0        0        0     2441 2023-04-21 00:52:22.318154 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py
+-rw-r--r--   0        0        0     2437 2023-04-21 00:52:22.320606 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py
+-rw-r--r--   0        0        0     2436 2023-04-21 00:52:22.320980 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py
+-rw-r--r--   0        0        0     3102 2023-04-21 00:52:22.321321 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py
+-rw-r--r--   0        0        0     2230 2023-04-21 00:52:22.321632 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py
+-rw-r--r--   0        0        0     2191 2023-04-21 00:52:22.321947 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py
+-rw-r--r--   0        0        0     2087 2023-04-21 00:52:22.322265 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/v1-get.py
+-rw-r--r--   0        0        0     2106 2023-04-21 00:52:22.322723 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py
+-rw-r--r--   0        0        0     2215 2023-04-21 00:52:22.325388 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py
+-rw-r--r--   0        0        0     2131 2023-04-21 00:52:22.326374 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py
+-rw-r--r--   0        0        0     2129 2023-04-21 00:52:22.326737 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3728 2023-04-21 00:52:22.327858 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py
+-rw-r--r--   0        0        0     3313 2023-04-21 00:52:22.328342 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py
+-rw-r--r--   0        0        0     3291 2023-04-21 00:52:22.328688 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py
+-rw-r--r--   0        0        0     4028 2023-04-21 00:52:22.329088 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py
+-rw-r--r--   0        0        0     3997 2023-04-21 00:52:22.330152 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py
+-rw-r--r--   0        0        0     3980 2023-04-21 00:52:22.330836 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py
+-rw-r--r--   0        0        0     4121 2023-04-21 00:52:22.331364 pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py
+-rw-r--r--   0        0        0     1320 2023-05-08 04:13:48.509091 pysnmp_lextudio-5.0.28/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-05-08 04:13:48.519493 pysnmp_lextudio-5.0.28/pysnmp/__init__.py
+-rw-r--r--   0        0        0     1252 2023-01-21 20:50:50.911870 pysnmp_lextudio-5.0.28/pysnmp/cache.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.495155 pysnmp_lextudio-5.0.28/pysnmp/carrier/__init__.py
+-rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495252 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/__init__.py
+-rw-r--r--   0        0        0     1857 2023-01-21 20:50:50.912293 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/base.py
+-rw-r--r--   0        0        0       60 2022-11-10 07:54:24.495435 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/__init__.py
+-rw-r--r--   0        0        0     5316 2023-04-21 00:52:22.331968 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/base.py
+-rw-r--r--   0        0        0     1994 2023-01-21 20:50:50.914278 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/udp.py
+-rw-r--r--   0        0        0     1101 2023-01-21 20:50:50.914731 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/udp6.py
+-rw-r--r--   0        0        0     3443 2023-01-21 20:50:50.916499 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dispatch.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.332205 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/__init__.py
+-rw-r--r--   0        0        0     3335 2023-04-21 00:52:22.333698 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/base.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.333778 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/__init__.py
+-rw-r--r--   0        0        0     7379 2023-04-21 00:52:22.334421 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/base.py
+-rw-r--r--   0        0        0      584 2023-04-21 00:52:22.335041 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/udp.py
+-rw-r--r--   0        0        0     1389 2023-04-21 00:52:22.335816 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/udp6.py
+-rw-r--r--   0        0        0     1621 2023-04-21 00:52:22.336644 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/unix.py
+-rw-r--r--   0        0        0     1734 2023-04-21 00:52:22.337494 pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dispatch.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337591 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.337679 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/dgram/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-21 00:52:22.346381 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/dgram/udp.py
+-rw-r--r--   0        0        0      209 2023-04-21 00:52:22.346875 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/dgram/udp6.py
+-rw-r--r--   0        0        0      209 2023-04-21 00:52:22.347793 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/dgram/unix.py
+-rw-r--r--   0        0        0      248 2023-04-21 00:52:22.348394 pysnmp_lextudio-5.0.28/pysnmp/carrier/asynsock/dispatch.py
+-rw-r--r--   0        0        0     8140 2023-04-21 00:52:22.349103 pysnmp_lextudio-5.0.28/pysnmp/carrier/base.py
+-rw-r--r--   0        0        0      235 2023-01-21 20:50:50.922097 pysnmp_lextudio-5.0.28/pysnmp/carrier/error.py
+-rw-r--r--   0        0        0      676 2023-01-21 20:50:50.922367 pysnmp_lextudio-5.0.28/pysnmp/carrier/sockfix.py
+-rw-r--r--   0        0        0     3558 2023-01-21 20:50:50.922632 pysnmp_lextudio-5.0.28/pysnmp/carrier/sockmsg.py
+-rw-r--r--   0        0        0     3501 2023-01-21 20:50:50.922909 pysnmp_lextudio-5.0.28/pysnmp/debug.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.497717 pysnmp_lextudio-5.0.28/pysnmp/entity/__init__.py
+-rw-r--r--   0        0        0    34968 2023-04-21 00:52:22.353135 pysnmp_lextudio-5.0.28/pysnmp/entity/config.py
+-rw-r--r--   0        0        0     8176 2023-01-21 20:50:50.925875 pysnmp_lextudio-5.0.28/pysnmp/entity/engine.py
+-rw-r--r--   0        0        0     2561 2023-01-21 20:50:50.927273 pysnmp_lextudio-5.0.28/pysnmp/entity/observer.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.498303 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/__init__.py
+-rw-r--r--   0        0        0    18591 2023-01-21 20:50:50.927634 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/cmdgen.py
+-rw-r--r--   0        0        0    14980 2023-01-21 20:50:50.927946 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/cmdrsp.py
+-rw-r--r--   0        0        0    10212 2023-01-21 20:50:50.930359 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/config.py
+-rw-r--r--   0        0        0     2623 2023-01-21 20:50:50.930748 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/context.py
+-rw-r--r--   0        0        0     2855 2023-01-21 20:50:50.931078 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/mibvar.py
+-rw-r--r--   0        0        0    17749 2023-01-21 20:50:50.931536 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/ntforg.py
+-rw-r--r--   0        0        0     4532 2023-01-21 20:50:50.931830 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/ntfrcv.py
+-rw-r--r--   0        0        0       59 2022-11-10 08:01:10.022472 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/oneliner/__init__.py
+-rw-r--r--   0        0        0    10016 2023-04-21 00:52:22.354201 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/oneliner/cmdgen.py
+-rw-r--r--   0        0        0     6644 2023-04-21 00:52:22.356701 pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/oneliner/ntforg.py
+-rw-r--r--   0        0        0      501 2023-01-21 20:50:50.932669 pysnmp_lextudio-5.0.28/pysnmp/error.py
+-rw-r--r--   0        0        0     3321 2023-04-21 00:52:22.357264 pysnmp_lextudio-5.0.28/pysnmp/hlapi/__init__.py
+-rw-r--r--   0        0        0      459 2023-01-21 20:50:50.933233 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/__init__.py
+-rw-r--r--   0        0        0    19830 2023-01-31 07:58:06.498827 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/cmdgen.py
+-rw-r--r--   0        0        0     5525 2023-01-23 06:09:50.177751 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/ntforg.py
+-rw-r--r--   0        0        0    13211 2023-01-25 01:36:58.327193 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/slim.py
+-rw-r--r--   0        0        0     4976 2023-01-23 20:11:38.568253 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/transport.py
+-rw-r--r--   0        0        0      462 2023-04-21 00:52:22.358928 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/__init__.py
+-rw-r--r--   0        0        0    20298 2023-04-21 00:52:22.362071 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/cmdgen.py
+-rw-r--r--   0        0        0     5202 2023-04-21 00:52:22.363199 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/ntforg.py
+-rw-r--r--   0        0        0      624 2023-04-21 00:52:22.363767 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/__init__.py
+-rw-r--r--   0        0        0    24567 2023-04-21 00:52:22.364659 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/cmdgen.py
+-rw-r--r--   0        0        0       59 2023-04-21 00:52:22.364765 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/compat/__init__.py
+-rw-r--r--   0        0        0     9212 2023-04-21 00:52:22.365599 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py
+-rw-r--r--   0        0        0     1572 2023-04-21 00:52:22.365784 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/compat/ntforg.py
+-rw-r--r--   0        0        0     4573 2023-04-21 00:52:22.366001 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/ntforg.py
+-rw-r--r--   0        0        0     5124 2023-04-21 00:52:22.366195 pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/transport.py
+-rw-r--r--   0        0        0    18218 2023-04-21 00:52:22.366583 pysnmp_lextudio-5.0.28/pysnmp/hlapi/auth.py
+-rw-r--r--   0        0        0     2050 2023-04-21 00:52:22.366871 pysnmp_lextudio-5.0.28/pysnmp/hlapi/context.py
+-rw-r--r--   0        0        0    11790 2023-01-21 20:50:50.938949 pysnmp_lextudio-5.0.28/pysnmp/hlapi/lcd.py
+-rw-r--r--   0        0        0     1922 2023-04-21 00:52:22.367114 pysnmp_lextudio-5.0.28/pysnmp/hlapi/transport.py
+-rw-r--r--   0        0        0     2920 2023-01-21 20:50:50.939457 pysnmp_lextudio-5.0.28/pysnmp/hlapi/varbinds.py
+-rw-r--r--   0        0        0     1197 2023-01-21 20:50:50.939677 pysnmp_lextudio-5.0.28/pysnmp/nextid.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504675 pysnmp_lextudio-5.0.28/pysnmp/proto/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.504925 pysnmp_lextudio-5.0.28/pysnmp/proto/acmod/__init__.py
+-rw-r--r--   0        0        0    12323 2023-01-21 20:50:50.939958 pysnmp_lextudio-5.0.28/pysnmp/proto/acmod/rfc3415.py
+-rw-r--r--   0        0        0      889 2023-01-21 20:50:50.940198 pysnmp_lextudio-5.0.28/pysnmp/proto/acmod/void.py
+-rw-r--r--   0        0        0      371 2023-01-21 20:50:50.940472 pysnmp_lextudio-5.0.28/pysnmp/proto/api/__init__.py
+-rw-r--r--   0        0        0     9391 2023-01-21 20:50:50.940745 pysnmp_lextudio-5.0.28/pysnmp/proto/api/v1.py
+-rw-r--r--   0        0        0     5599 2023-01-21 20:50:50.940989 pysnmp_lextudio-5.0.28/pysnmp/proto/api/v2c.py
+-rw-r--r--   0        0        0      926 2023-04-22 01:36:13.197204 pysnmp_lextudio-5.0.28/pysnmp/proto/api/verdec.py
+-rw-r--r--   0        0        0     1151 2023-04-21 00:52:22.367350 pysnmp_lextudio-5.0.28/pysnmp/proto/cache.py
+-rw-r--r--   0        0        0     5977 2023-04-28 19:25:50.733203 pysnmp_lextudio-5.0.28/pysnmp/proto/errind.py
+-rw-r--r--   0        0        0     1191 2023-01-21 20:50:50.941881 pysnmp_lextudio-5.0.28/pysnmp/proto/error.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.507349 pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/__init__.py
+-rw-r--r--   0        0        0     1754 2023-01-21 20:50:50.942134 pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/base.py
+-rw-r--r--   0        0        0     3910 2023-01-21 20:50:50.942358 pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/cache.py
+-rw-r--r--   0        0        0    20350 2023-01-21 20:50:50.942628 pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/rfc2576.py
+-rw-r--r--   0        0        0    35109 2023-01-22 07:40:10.590039 pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/rfc3412.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.508803 pysnmp_lextudio-5.0.28/pysnmp/proto/proxy/__init__.py
+-rw-r--r--   0        0        0     9874 2023-01-21 20:50:50.943242 pysnmp_lextudio-5.0.28/pysnmp/proto/proxy/rfc2576.py
+-rw-r--r--   0        0        0     6085 2023-04-21 00:52:22.367846 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1155.py
+-rw-r--r--   0        0        0     3323 2023-01-21 20:50:50.943726 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1157.py
+-rw-r--r--   0        0        0      563 2023-01-21 20:50:50.943981 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1901.py
+-rw-r--r--   0        0        0    21296 2023-04-21 00:52:22.368250 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1902.py
+-rw-r--r--   0        0        0     5671 2023-01-21 20:50:50.944541 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1905.py
+-rw-r--r--   0        0        0     1374 2023-01-21 20:50:50.944781 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc3411.py
+-rw-r--r--   0        0        0    21759 2023-01-21 20:50:50.945141 pysnmp_lextudio-5.0.28/pysnmp/proto/rfc3412.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510738 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/__init__.py
+-rw-r--r--   0        0        0     1485 2023-01-21 20:50:50.945499 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/base.py
+-rw-r--r--   0        0        0      881 2023-01-21 20:50:50.945778 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/cache.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.510991 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511096 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/__init__.py
+-rw-r--r--   0        0        0     1030 2023-01-21 20:50:50.946099 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aes192.py
+-rw-r--r--   0        0        0      999 2023-01-21 20:50:50.946416 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aes256.py
+-rw-r--r--   0        0        0     3203 2023-01-21 20:50:50.946711 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aesbase.py
+-rw-r--r--   0        0        0     5517 2023-04-29 01:41:10.500798 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/des3.py
+-rw-r--r--   0        0        0    21657 2023-04-21 00:52:22.368591 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc2576.py
+-rw-r--r--   0        0        0      261 2023-01-21 20:50:50.947549 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.511982 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/__init__.py
+-rw-r--r--   0        0        0      850 2023-01-21 20:50:50.947795 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/base.py
+-rw-r--r--   0        0        0     3709 2023-01-21 20:50:50.948046 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py
+-rw-r--r--   0        0        0     3468 2023-01-21 20:50:50.948325 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py
+-rw-r--r--   0        0        0      733 2023-01-22 19:49:47.441260 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/noauth.py
+-rw-r--r--   0        0        0     2098 2023-01-21 20:50:50.949099 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/localkey.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.512518 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/__init__.py
+-rw-r--r--   0        0        0      728 2023-01-21 20:50:50.951254 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/base.py
+-rw-r--r--   0        0        0     5060 2023-04-29 01:41:47.475223 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/des.py
+-rw-r--r--   0        0        0      807 2023-01-21 20:50:50.951774 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/nopriv.py
+-rw-r--r--   0        0        0    56002 2023-01-22 20:02:41.908685 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/service.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513200 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3826/__init__.py
+-rw-r--r--   0        0        0       59 2022-12-02 02:52:14.601095 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3826/priv/__init__.py
+-rw-r--r--   0        0        0     5041 2023-04-29 01:40:11.337560 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3826/priv/aes.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513516 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc7860/__init__.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513622 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc7860/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2023-01-21 20:50:50.953621 pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.513825 pysnmp_lextudio-5.0.28/pysnmp/smi/__init__.py
+-rw-r--r--   0        0        0    16487 2023-01-21 20:50:50.953912 pysnmp_lextudio-5.0.28/pysnmp/smi/builder.py
+-rw-r--r--   0        0        0     2326 2023-04-04 18:56:40.326682 pysnmp_lextudio-5.0.28/pysnmp/smi/compiler.py
+-rw-r--r--   0        0        0     2351 2023-01-21 20:50:50.954423 pysnmp_lextudio-5.0.28/pysnmp/smi/error.py
+-rw-r--r--   0        0        0      317 2023-01-21 20:50:50.954638 pysnmp_lextudio-5.0.28/pysnmp/smi/exval.py
+-rw-r--r--   0        0        0     3084 2023-01-21 20:50:50.954871 pysnmp_lextudio-5.0.28/pysnmp/smi/indices.py
+-rw-r--r--   0        0        0     9227 2023-01-21 20:50:50.955119 pysnmp_lextudio-5.0.28/pysnmp/smi/instrum.py
+-rw-r--r--   0        0        0      283 2023-01-21 20:50:50.955343 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/ASN1-ENUMERATION.py
+-rw-r--r--   0        0        0      534 2023-01-21 20:50:50.955553 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/ASN1-REFINEMENT.py
+-rw-r--r--   0        0        0      505 2023-01-21 20:50:50.955778 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/ASN1.py
+-rw-r--r--   0        0        0    17614 2023-01-21 20:50:50.957301 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/INET-ADDRESS-MIB.py
+-rw-r--r--   0        0        0     3591 2023-01-21 20:50:50.957643 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-MIB.py
+-rw-r--r--   0        0        0     4620 2023-01-21 20:50:50.957971 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py
+-rw-r--r--   0        0        0     9922 2023-01-21 20:50:50.958209 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-USM-MIB.py
+-rw-r--r--   0        0        0     1318 2023-01-21 20:50:50.958608 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/RFC1158-MIB.py
+-rw-r--r--   0        0        0    56809 2023-01-21 20:50:50.959093 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/RFC1213-MIB.py
+-rw-r--r--   0        0        0    17437 2023-01-21 20:50:50.959514 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py
+-rw-r--r--   0        0        0    18854 2023-05-08 04:12:20.147320 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py
+-rw-r--r--   0        0        0     5882 2023-01-21 20:50:50.961679 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-MPD-MIB.py
+-rw-r--r--   0        0        0    19031 2023-01-21 20:50:50.962008 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py
+-rw-r--r--   0        0        0    10138 2023-01-21 20:50:50.962396 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-PROXY-MIB.py
+-rw-r--r--   0        0        0    24833 2023-01-21 20:50:50.962836 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-TARGET-MIB.py
+-rw-r--r--   0        0        0     3913 2023-01-21 20:50:50.963197 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py
+-rw-r--r--   0        0        0    33731 2023-01-21 20:50:50.963774 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py
+-rw-r--r--   0        0        0     3572 2023-01-21 20:50:50.964077 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py
+-rw-r--r--   0        0        0     5841 2023-01-21 20:50:50.964367 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py
+-rw-r--r--   0        0        0    30173 2023-01-21 20:50:50.964903 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py
+-rw-r--r--   0        0        0     4096 2023-01-21 20:50:50.965255 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-CONF.py
+-rw-r--r--   0        0        0    31135 2023-01-21 20:50:50.965742 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-MIB.py
+-rw-r--r--   0        0        0    46776 2023-01-21 20:50:50.966284 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-SMI.py
+-rw-r--r--   0        0        0    28986 2023-01-21 20:50:50.966685 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-TC.py
+-rw-r--r--   0        0        0     6921 2023-01-21 20:50:50.967022 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-TM.py
+-rw-r--r--   0        0        0    24370 2023-01-21 20:50:50.967422 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.522800 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/__init__.py
+-rw-r--r--   0        0        0      926 2023-01-21 20:50:50.967752 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py
+-rw-r--r--   0        0        0     1174 2023-01-21 20:50:50.968042 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py
+-rw-r--r--   0        0        0     1047 2023-01-21 20:50:50.968298 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py
+-rw-r--r--   0        0        0     1046 2023-01-21 20:50:50.968546 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py
+-rw-r--r--   0        0        0     2232 2023-01-21 20:50:50.968782 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py
+-rw-r--r--   0        0        0      530 2023-01-21 20:50:50.969033 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py
+-rw-r--r--   0        0        0     7605 2023-01-21 20:50:50.969323 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py
+-rw-r--r--   0        0        0       59 2022-11-10 07:54:24.523596 pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__init__.py
+-rw-r--r--   0        0        0    44735 2023-04-21 00:52:22.370798 pysnmp_lextudio-5.0.28/pysnmp/smi/rfc1902.py
+-rw-r--r--   0        0        0    12218 2023-01-21 20:50:50.971883 pysnmp_lextudio-5.0.28/pysnmp/smi/view.py
+-rw-r--r--   0        0        0     8299 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.28/setup.py
+-rw-r--r--   0        0        0     7834 1970-01-01 00:00:00.000000 pysnmp_lextudio-5.0.28/PKG-INFO
```

### Comparing `pysnmp_lextudio-5.0.27/LICENSE.rst` & `pysnmp_lextudio-5.0.28/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/README.md` & `pysnmp_lextudio-5.0.28/README.md`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/Makefile` & `pysnmp_lextudio-5.0.28/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-MIB.txt` & `pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-SOURCE-MIB.txt` & `pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-SOURCE-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/mibs/PYSNMP-USM-MIB.txt` & `pysnmp_lextudio-5.0.28/docs/mibs/PYSNMP-USM-MIB.txt`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/net-snmpd.conf` & `pysnmp_lextudio-5.0.28/docs/net-snmpd.conf`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/net-snmptrapd.conf` & `pysnmp_lextudio-5.0.28/docs/net-snmptrapd.conf`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/.static/favicon.ico` & `pysnmp_lextudio-5.0.28/docs/source/.static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/.static/logo.svg` & `pysnmp_lextudio-5.0.28/docs/source/.static/logo.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/.templates/layout.html` & `pysnmp_lextudio-5.0.28/docs/source/.templates/layout.html`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/.templates/sourcelink.html` & `pysnmp_lextudio-5.0.28/docs/source/.templates/sourcelink.html`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/conf.py` & `pysnmp_lextudio-5.0.28/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '5.0'
 # The full version, including alpha/beta/rc tags.
-release = '5.0.27'
+release = '5.0.28'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
```

### Comparing `pysnmp_lextudio-5.0.27/docs/source/development.rst` & `pysnmp_lextudio-5.0.28/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/api-reference.rst` & `pysnmp_lextudio-5.0.28/docs/source/docs/api-reference.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/mib-object-instances.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/mib-object-instances.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/nms-components.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/nms-components.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/oid-tree-mibs.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/oid-tree-mibs.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/oid-tree.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/oid-tree.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-architecture.rst` & `pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-architecture.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-design.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-design.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/pysnmp-hlapi-tutorial.rst` & `pysnmp_lextudio-5.0.28/docs/source/docs/pysnmp-hlapi-tutorial.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/snmp-apps.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/snmp-apps.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/snmp-design.rst` & `pysnmp_lextudio-5.0.28/docs/source/docs/snmp-design.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/snmp-engine.svg` & `pysnmp_lextudio-5.0.28/docs/source/docs/snmp-engine.svg`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/docs/snmp-history.rst` & `pysnmp_lextudio-5.0.28/docs/source/docs/snmp-history.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/download.rst` & `pysnmp_lextudio-5.0.28/docs/source/download.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/agent/ntforg/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/index.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/manager/cmdgen/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/hlapi/asyncio/manager/cmdgen/snmp-versions.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/index.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/smi/agent/implementing-mib-objects.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/smi/agent/implementing-mib-objects.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/smi/manager/browsing-mib-tree.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/smi/manager/browsing-mib-tree.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/agent/cmdrsp/agent-side-mib-implementations.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/agent/ntforg/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/cmdgen/walking-operations.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v1arch/asyncore/manager/ntfrcv/transport-tweaks.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/examples/v3arch/asyncio/index.rst` & `pysnmp_lextudio-5.0.28/docs/source/examples/v3arch/asyncio/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/getting-peer-information.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/getting-peer-information.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/how-to-implement-agent-mib.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/how-to-implement-agent-mib.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/ignored-snmp-packets.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/ignored-snmp-packets.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/listening-on-multiple-interfaces.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/listening-on-multiple-interfaces.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/non-printable-snmp-values-apps.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/non-printable-snmp-values-apps.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/non-printable-snmp-values-tools.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/non-printable-snmp-values-tools.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/oids-not-increasing.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/oids-not-increasing.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/pass-custom-mib-to-manager.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/pass-custom-mib-to-manager.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/py2exe-throws-error.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/py2exe-throws-error.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/response-values-mib-resolution.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/response-values-mib-resolution.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/snmp-data-constraints-verification-failure.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/snmp-data-constraints-verification-failure.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/faq/walk-whole-mib.rst` & `pysnmp_lextudio-5.0.28/docs/source/faq/walk-whole-mib.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/index.rst` & `pysnmp_lextudio-5.0.28/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/docs/source/quick-start.rst` & `pysnmp_lextudio-5.0.28/docs/source/quick-start.rst`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/default-v1-trap.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/multiple-notifications-at-once.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/agent/ntforg/v3-inform.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/agent/ntforg/v3-inform.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/custom-asn1-mib-search-path.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/getbulk-to-eom.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/multiple-concurrent-queries-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/multiple-sequential-queries.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/usm-sha-aes128.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-get.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-get.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-next.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-next.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v1-set.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v1-set.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-bulk.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-get.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-next.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py` & `pysnmp_lextudio-5.0.28/examples/hlapi/asyncio/manager/cmdgen/v2c-set.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/agent/custom-managed-object.py` & `pysnmp_lextudio-5.0.28/examples/smi/agent/custom-managed-object.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/agent/operations-on-managed-objects.py` & `pysnmp_lextudio-5.0.28/examples/smi/agent/operations-on-managed-objects.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/manager/builder.py` & `pysnmp_lextudio-5.0.28/examples/smi/manager/builder.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py` & `pysnmp_lextudio-5.0.28/examples/smi/manager/configure-mib-viewer-and-resolve-pdu-varbinds.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py` & `pysnmp_lextudio-5.0.28/examples/smi/manager/convert-between-pdu-varbinds-and-mib-objects.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/manager/mib-tree-inspection.py` & `pysnmp_lextudio-5.0.28/examples/smi/manager/mib-tree-inspection.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/smi/manager/print-oid-description.py` & `pysnmp_lextudio-5.0.28/examples/smi/manager/print-oid-description.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/ntforg/send-inform-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/agent/ntforg/send-trap-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/broadcast-agent-discovery.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/fetch-scalar-value.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/getbulk-pull-whole-mib.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/getnext-pull-whole-mib.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/spoof-source-address.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/cmdgen/v2c-set.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py` & `pysnmp_lextudio-5.0.28/examples/v1arch/asyncore/manager/ntfrcv/listen-on-ipv4-and-ipv6-interfaces.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncio/agent/cmdrsp/multiple-usm-users.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncio/manager/ntfrcv/multiple-interfaces.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/alternative-mib-tree.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/custom-mib-controller.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/custom-snmp-engine-id.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/detailed-vacm-configuration.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/implementing-scalar-mib-objects.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/implementing-snmp-table.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listen-on-ipv4-and-ipv6-interfaces.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listen-on-multiple-interfaces.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/listening-on-virtual-network-interface.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-communities.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-snmp-engines.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/multiple-usm-users.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/cmdrsp/observe-request-processing.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/multiple-different-notifications-at-once.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-custom-pdu.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-inform-to-multiple-managers.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-notification-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-packet-from-specific-address.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/send-trap-to-multiple-managers.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/usm-md5-none.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v1-trap.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v1-trap.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-inform.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-trap-with-notification-objects.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v2c-trap.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/agent/ntforg/v3-trap.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/agent/ntforg/v3-trap.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/custom-contextengineid-and-contextname.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/custom-timeout-and-retries.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/fetch-variables-over-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getbulk-fetch-scalar-and-table-variables.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getbulk-multiple-oids-to-eom.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-and-resolve-with-mib.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/getnext-multiple-oids-to-eom.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/observe-request-processing.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/pull-subtree.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/send-packets-from-specific-interface.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/set-multiple-scalar-values.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/spoof-source-address.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/usm-sha-aes128.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/usm-sha-none.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/v1-get.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/v1-get.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/cmdgen/v2c-set.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/determine-peer-network-address.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-interfaces.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-network-transports-incl-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/multiple-usm-users.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/observe-request-processing-over-ipv4-and-ipv6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/manager/ntfrcv/regexp-community-name.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/ipv6-to-ipv4-conversion.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v2c-to-v1-conversion.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v2c-to-v3-conversion.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py` & `pysnmp_lextudio-5.0.28/examples/v3arch/asyncore/proxy/command/v3-to-v2c-conversion.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pyproject.toml` & `pysnmp_lextudio-5.0.28/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnmp-lextudio"
-version = "5.0.27"
+version = "5.0.28"
 description = ""
 authors = ["Ilya Etingof <etingof@gmail.com>", "Lex Li <support@lextudio.com>"]
 license = "BSD-2-Clause"
 repository = "https://github.com/lextudio/pysnmp"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -29,15 +29,15 @@
 python = "^3.7"
 pyasn1 = ">=0.4.8, <0.5.0"
 pysnmpcrypto = "^0.0.4"
 pysmi-lextudio = "^1.0.4"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.3.0"
-pytest = "^6.2.5"
+pytest = "^7.2.0"
 codecov = "^2.1.12"
 pytest-codecov = "^0.4.0"
 
 [tool.poetry_bumpversion.file."pysnmp/__init__.py"]
 
 [tool.poetry_bumpversion.file."docs/source/conf.py"]
 search = "release = '{current_version}'"
```

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/cache.py` & `pysnmp_lextudio-5.0.28/pysnmp/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/udp.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dgram/udp6.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncio/dispatch.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncio/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/udp.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/udp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/udp6.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/udp6.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dgram/unix.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dgram/unix.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/asyncore/dispatch.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/asyncore/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/sockfix.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/sockfix.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/carrier/sockmsg.py` & `pysnmp_lextudio-5.0.28/pysnmp/carrier/sockmsg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/debug.py` & `pysnmp_lextudio-5.0.28/pysnmp/debug.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/config.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/config.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/engine.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/engine.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/observer.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/observer.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/cmdrsp.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/cmdrsp.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/config.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/config.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/context.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/context.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/mibvar.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/mibvar.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/ntfrcv.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/ntfrcv.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/oneliner/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/oneliner/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/entity/rfc3413/oneliner/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/entity/rfc3413/oneliner/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/__init__.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/slim.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/slim.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncio/transport.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncio/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/__init__.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/compat/cmdgen.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/compat/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/compat/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/sync/ntforg.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/sync/ntforg.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/asyncore/transport.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/asyncore/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/auth.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/auth.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/context.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/context.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/lcd.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/lcd.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/transport.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/transport.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/hlapi/varbinds.py` & `pysnmp_lextudio-5.0.28/pysnmp/hlapi/varbinds.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/nextid.py` & `pysnmp_lextudio-5.0.28/pysnmp/nextid.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/acmod/rfc3415.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/acmod/rfc3415.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/acmod/void.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/acmod/void.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/api/v1.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/api/v1.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/api/v2c.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/api/v2c.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/api/verdec.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/api/verdec.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/cache.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/errind.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/errind.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/error.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/error.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/cache.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/rfc2576.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/mpmod/rfc3412.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/mpmod/rfc3412.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/proxy/rfc2576.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/proxy/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1155.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1155.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1157.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1157.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1901.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1901.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1902.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1902.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc1905.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc1905.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc3411.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc3411.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/rfc3412.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/rfc3412.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/cache.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/cache.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aes192.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aes192.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aes256.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aes256.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/aesbase.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/aesbase.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/eso/priv/des3.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/eso/priv/des3.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc2576.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc2576.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/hmacmd5.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/hmacsha.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/auth/noauth.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/auth/noauth.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/localkey.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/localkey.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/base.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/des.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/des.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/priv/nopriv.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/priv/nopriv.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3414/service.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3414/service.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc3826/priv/aes.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc3826/priv/aes.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py` & `pysnmp_lextudio-5.0.28/pysnmp/proto/secmod/rfc7860/auth/hmacsha2.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/builder.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/builder.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/compiler.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/compiler.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/error.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/error.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/indices.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/indices.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/instrum.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/instrum.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/ASN1-REFINEMENT.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/ASN1-REFINEMENT.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/INET-ADDRESS-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/INET-ADDRESS-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-SOURCE-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/PYSNMP-USM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/RFC1158-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/RFC1158-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/RFC1213-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/RFC1213-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-COMMUNITY-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-FRAMEWORK-MIB.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 # PySNMP MIB module SNMP-FRAMEWORK-MIB (https://www.pysnmp.com/pysnmp)
 # ASN.1 source http://mibs.pysnmp.com:80/asn1/SNMP-FRAMEWORK-MIB
 # Produced by pysmi-0.1.3 at Mon Apr 17 13:59:41 2017
 # On host grommit.local platform Darwin version 16.4.0 by user ilya
 # Using Python version 3.4.2 (v3.4.2:ab2c023a9432, Oct  5 2014, 20:42:22)
 #
+import platform
 import time
 try:
     import os
 except ImportError:
     pass
 
 OctetString, ObjectIdentifier, Integer = mibBuilder.importSymbols("ASN1", "OctetString", "ObjectIdentifier", "Integer")
@@ -44,15 +45,15 @@
 class SnmpEngineID(TextualConvention, OctetString):
     description = "An SNMP engine's administratively-unique identifier. Objects of this type are for identification, not for addressing, even though it is possible that an address may have been used in the generation of a specific value. The value for this object may not be all zeros or all 'ff'H or the empty (zero length) string. The initial value for this object may be configured via an operator console entry or via an algorithmic function. In the latter case, the following example algorithm is recommended. In cases where there are multiple engines on the same system, the use of this algorithm is NOT appropriate, as it would result in all of those engines ending up with the same ID value. 1) The very first bit is used to indicate how the rest of the data is composed. 0 - as defined by enterprise using former methods that existed before SNMPv3. See item 2 below. 1 - as defined by this architecture, see item 3 below. Note that this allows existing uses of the engineID (also known as AgentID [RFC1910]) to co-exist with any new uses. 2) The snmpEngineID has a length of 12 octets. The first four octets are set to the binary equivalent of the agent's SNMP management private enterprise number as assigned by the Internet Assigned Numbers Authority (IANA). For example, if Acme Networks has been assigned { enterprises 696 }, the first four octets would be assigned '000002b8'H. The remaining eight octets are determined via one or more enterprise-specific methods. Such methods must be designed so as to maximize the possibility that the value of this object will be unique in the agent's administrative domain. For example, it may be the IP address of the SNMP entity, or the MAC address of one of the interfaces, with each address suitably padded with random octets. If multiple methods are defined, then it is recommended that the first octet indicate the method being used and the remaining octets be a function of the method. 3) The length of the octet string varies. The first four octets are set to the binary equivalent of the agent's SNMP management private enterprise number as assigned by the Internet Assigned Numbers Authority (IANA). For example, if Acme Networks has been assigned { enterprises 696 }, the first four octets would be assigned '000002b8'H. The very first bit is set to 1. For example, the above value for Acme Networks now changes to be '800002b8'H. The fifth octet indicates how the rest (6th and following octets) are formatted. The values for the fifth octet are: 0 - reserved, unused. 1 - IPv4 address (4 octets) lowest non-special IP address 2 - IPv6 address (16 octets) lowest non-special IP address 3 - MAC address (6 octets) lowest IEEE MAC address, canonical order 4 - Text, administratively assigned Maximum remaining length 27 5 - Octets, administratively assigned Maximum remaining length 27 6-127 - reserved, unused 128-255 - as defined by the enterprise Maximum remaining length 27 "
     status = 'current'
     subtypeSpec = OctetString.subtypeSpec + ValueSizeConstraint(5, 32)
     defaultValue = [128, 0, 79, 184, 5]
     try:
         # Attempt to base engine ID on local system name and properties
-        defaultValue += [ord(x) for x in os.uname()[1][:16]]
+        defaultValue += [ord(x) for x in platform.node()[:16]]
     except Exception:
         pass
     try:
         # Attempt to base engine ID on PID
         defaultValue += [os.getpid() >> 8 & 0xff, os.getpid() & 0xff]
     except Exception:
         pass
```

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-MPD-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-NOTIFICATION-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-PROXY-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-PROXY-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-TARGET-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USER-BASED-SM-3DES-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USM-AES-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-USM-HMAC-SHA2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMP-VIEW-BASED-ACM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-CONF.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-CONF.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-SMI.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-SMI.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-TC.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-TC.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/SNMPv2-TM.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/SNMPv2-TM.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/TRANSPORT-ADDRESS-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-FRAMEWORK-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-MPD-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-TARGET-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-USER-BASED-SM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMP-VIEW-BASED-ACM-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/mibs/instances/__SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/rfc1902.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/rfc1902.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/pysnmp/smi/view.py` & `pysnmp_lextudio-5.0.28/pysnmp/smi/view.py`

 * *Files identical despite different names*

### Comparing `pysnmp_lextudio-5.0.27/setup.py` & `pysnmp_lextudio-5.0.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 install_requires = \
 ['pyasn1>=0.4.8,<0.5.0',
  'pysmi-lextudio>=1.0.4,<2.0.0',
  'pysnmpcrypto>=0.0.4,<0.0.5']
 
 setup_kwargs = {
     'name': 'pysnmp-lextudio',
-    'version': '5.0.27',
+    'version': '5.0.28',
     'description': '',
     'long_description': "\nSNMP Library for Python\n-----------------------\n\n[![PyPI](https://img.shields.io/pypi/v/pysnmp-lextudio.svg)](https://pypi.python.org/pypi/pysnmp-lextudio)\n[![PyPI Downloads](https://img.shields.io/pypi/dd/pysnmp-lextudio)](https://pypi.python.org/pypi/pysnmp-lextudio/)\n[![Python Versions](https://img.shields.io/pypi/pyversions/pysnmp-lextudio.svg)](https://pypi.python.org/pypi/pysnmp-lextudio/)\n[![GitHub license](https://img.shields.io/badge/license-BSD-blue.svg)](https://raw.githubusercontent.com/lextudio/pysnmp/master/LICENSE.rst)\n\nThis is a pure-Python, open source and free implementation of v1/v2c/v3\nSNMP engine distributed under 2-clause [BSD license](https://www.pysnmp.com/pysnmp/license.html).\n\nThe PySNMP project was initially sponsored by a [PSF](http://www.python.org/psf/) grant.\nThank you!\n\nThis version is a fork of Ilya Etingof's project [etingof/pysnmp](https://github.com/etingof/pysnmp). Ilya sadly passed away on 10-Aug-2022. Announcement [here](https://lists.openstack.org/pipermail/openstack-discuss/2022-August/030062.html).  His work is still of great use to the Python community and he will be missed.\n\nFeatures\n--------\n\n* Complete SNMPv1/v2c and SNMPv3 support\n* SMI framework for resolving MIB information and implementing SMI\n  Managed Objects\n* Complete SNMP entity implementation\n* USM Extended Security Options support (3DES, 192/256-bit AES encryption)\n* Extensible network transports framework (UDP/IPv4, UDP/IPv6)\n* Asynchronous socket-based IO API support\n* [Asyncio](https://docs.python.org/3/library/asyncio.html) integration\n* [PySMI](https://www.pysnmp.com/pysmi/) integration for dynamic MIB compilation\n* Built-in instrumentation exposing protocol engine operations\n* Python eggs and py2exe friendly\n* 100% Python, works with Python 3.7+\n* MT-safe (if SnmpEngine is thread-local)\n\nFeatures, specific to SNMPv3 model include:\n\n* USM authentication (MD5/SHA-1/SHA-2) and privacy (DES/AES) protocols (RFC3414, RFC7860)\n* View-based access control to use with any SNMP model (RFC3415)\n* Built-in SNMP proxy PDU converter for building multi-lingual\n  SNMP entities (RFC2576)\n* Remote SNMP engine configuration\n* Optional SNMP engine discovery\n* Shipped with standard SNMP applications (RC3413)\n\n\nDownload & Install\n------------------\n\nThe PySNMP software is freely available for download from [PyPI](https://pypi.python.org/pypi/pysnmp-lextudio)\nand [GitHub](https://github.com/lextudio/pysnmp.git).\n\nJust run:\n\n```bash\n$ pip install pysnmp-lextudio\n```\n\nTo download and install PySNMP along with its dependencies:\n\n<!-- Need to find an alternate location for the links to pysnmp.com -->\n* [PyASN1](https://pyasn1.readthedocs.io)\n* [PySMI](https://www.pysnmp.com/pysmi/) (required for MIB services only)\n* Optional [pysnmpcrypto](https://github.com/etingof/pysnmpcrypto) package\n  whenever strong SNMPv3 encryption is desired\n\nBesides the library, command-line [SNMP utilities](https://github.com/lextudio/snmpclitools)\nwritten in pure-Python could be installed via:\n\n```bash\n$ pip install snmpclitools-lextudio\n```\n\nand used in the very similar manner as conventional Net-SNMP tools:\n\n```bash\n$ snmpget.py -v3 -l authPriv -u usr-md5-des -A authkey1 -X privkey1 demo.pysnmp.com sysDescr.0\nSNMPv2-MIB::sysDescr.0 = STRING: Linux zeus 4.8.6.5-smp #2 SMP Sun Nov 13 14:58:11 CDT 2016 i686\n```\n\nExamples\n--------\n\nPySNMP is designed in a layered fashion. Top-level and easiest to use API is known as\n*hlapi*. Here's a quick example on how to SNMP GET:\n\n```python\nfrom pysnmp.hlapi import *\n\niterator = getCmd(SnmpEngine(),\n                  CommunityData('public'),\n                  UdpTransportTarget(('demo.pysnmp.com', 161)),\n                  ContextData(),\n                  ObjectType(ObjectIdentity('SNMPv2-MIB', 'sysDescr', 0)))\n\nerrorIndication, errorStatus, errorIndex, varBinds = next(iterator)\n\nif errorIndication:  # SNMP engine errors\n    print(errorIndication)\nelse:\n    if errorStatus:  # SNMP agent errors\n        print('%s at %s' % (errorStatus.prettyPrint(), varBinds[int(errorIndex)-1] if errorIndex else '?'))\n    else:\n        for varBind in varBinds:  # SNMP response contents\n            print(' = '.join([x.prettyPrint() for x in varBind]))\n```\n\nThis is how to send SNMP TRAP:\n\n```python\nfrom pysnmp.hlapi import *\n\nerrorIndication, errorStatus, errorIndex, varBinds = next(\n    sendNotification(\n        SnmpEngine(OctetString(hexValue='8000000001020304')),\n        UsmUserData('usr-sha-aes128', 'authkey1', 'privkey1',\n                    authProtocol=usmHMACSHAAuthProtocol,\n                    privProtocol=usmAesCfb128Protocol),\n        UdpTransportTarget(('demo.pysnmp.com', 162)),\n        ContextData(),\n        'trap',\n        NotificationType(ObjectIdentity('SNMPv2-MIB', 'authenticationFailure'))\n    )\n)\n\nif errorIndication:\n    print(errorIndication)\n```\n\n> We maintain publicly available SNMP Agent and TRAP sink at\n> [demo.pysnmp.com](https://www.pysnmp.com/snmpsim/public-snmp-agent-simulator.html). You are\n> welcome to use it while experimenting with whatever SNMP software you deal with.\n\n```bash\n$ python3 examples/hlapi/asyncore/sync/manager/cmdgen/usm-sha-aes128.py\nSNMPv2-MIB::sysDescr.0 = SunOS zeus.pysnmp.com 4.1.3_U1 1 sun4m\n$\n$ python3 examples//hlapi/asyncore/sync/agent/ntforg/v3-inform.py\nSNMPv2-MIB::sysUpTime.0 = 0\nSNMPv2-MIB::snmpTrapOID.0 = SNMPv2-MIB::warmStart\nSNMPv2-MIB::sysName.0 = system name\n```\n\nOther than that, PySNMP is capable to automatically fetch and use required MIBs from HTTP, FTP sites\nor local directories. You could configure any MIB source available to you (including\n[this one](https://github.com/lextudio/mibs.snmplabs.com/tree/master/asn1)) for that purpose.\n\nFor more example scripts please refer to [examples section](https://www.pysnmp.com/pysnmp/examples/index.html#high-level-snmp)\nat pysnmp web site.\n\nDocumentation\n-------------\n\nLibrary documentation and examples can be found at the [pysnmp project site](https://www.pysnmp.com/pysnmp/).\n\nIf something does not work as expected, please\n[open an issue](https://github.com/lextudio/pysnmp/issues) at GitHub or\npost your question [on Stack Overflow](http://stackoverflow.com/questions/ask) or try browsing pysnmp\n[mailing list archives](https://sourceforge.net/p/pysnmp/mailman/pysnmp-users/).\n\nBug reports and PRs are appreciated! ;-)\n\nCopyright (c) 2005-2019, [Ilya Etingof](https://lists.openstack.org/pipermail/openstack-discuss/2022-August/030062.html).\nCopyright (c) 2022, [LeXtudio Inc](mailto:support@lextudio.com).\nAll rights reserved.\n",
     'author': 'Ilya Etingof',
     'author_email': 'etingof@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/lextudio/pysnmp',
```

### Comparing `pysnmp_lextudio-5.0.27/PKG-INFO` & `pysnmp_lextudio-5.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnmp-lextudio
-Version: 5.0.27
+Version: 5.0.28
 Summary: 
 Home-page: https://github.com/lextudio/pysnmp
 License: BSD-2-Clause
 Author: Ilya Etingof
 Author-email: etingof@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

