# Comparing `tmp/assemblyline-4.4.1.dev8.tar.gz` & `tmp/assemblyline-4.4.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-4.4.1.dev8.tar", last modified: Fri Mar 24 14:59:37 2023, max compression
+gzip compressed data, was "assemblyline-4.4.1.dev9.tar", last modified: Fri Mar 24 16:14:12 2023, max compression
```

## Comparing `assemblyline-4.4.1.dev8.tar` & `assemblyline-4.4.1.dev9.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (122)       47 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1558 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.041979 assemblyline-4.4.1.dev8/assemblyline/
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-03-24 14:59:34.000000 assemblyline-4.4.1.dev8/assemblyline/VERSION
--rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.045979 assemblyline-4.4.1.dev8/assemblyline/cachestore/
--rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/cachestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.073980 assemblyline-4.4.1.dev8/assemblyline/common/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4138 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/archiving.py
--rw-r--r--   0 vsts      (1001) docker     (122)  2243670 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/attack_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13368 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/backupmanager.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/banner.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15837 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/bundling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5646 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/caching.py
--rw-r--r--   0 vsts      (1001) docker     (122)      903 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/chunk.py
--rw-r--r--   0 vsts      (1001) docker     (122)    38686 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4532 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/classification.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     5811 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/cleanup_filestore.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1789 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/codec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5031 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/comms.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2512 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5147 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/custom.magic
--rw-r--r--   0 vsts      (1001) docker     (122)    23191 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/custom.yara
--rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/dict_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2091 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/digests.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2041 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/entropy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1903 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8326 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/forge.py
--rw-r--r--   0 vsts      (1001) docker     (122)   168009 2023-03-24 14:59:36.000000 assemblyline-4.4.1.dev8/assemblyline/common/frequency.c
--rw-r--r--   0 vsts      (1001) docker     (122)      709 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/frequency.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6402 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/heuristics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1398 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/hexdump.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19731 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/identify.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17758 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/identify_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/importing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/iprange.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3610 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/isotime.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4310 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/log.py
--rw-r--r--   0 vsts      (1001) docker     (122)      909 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/logformat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1564 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/lucene.lark
--rw-r--r--   0 vsts      (1001) docker     (122)     1105 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/memory_zip.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4815 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/net.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21606 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/net_static.py
--rw-r--r--   0 vsts      (1001) docker     (122)      231 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/null.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/path.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28059 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/postprocess.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4971 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/random_user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/security.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/signaturing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7002 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/str_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7665 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/common/tag_safelist.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3715 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/uid.py
--rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/common/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.073980 assemblyline-4.4.1.dev8/assemblyline/datasource/
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/datasource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2183 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/datasource/al.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1462 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/datasource/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/datasource/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.077980 assemblyline-4.4.1.dev8/assemblyline/datastore/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2950 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/bulk.py
--rw-r--r--   0 vsts      (1001) docker     (122)    86851 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/collection.py
--rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    52444 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10135 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.077980 assemblyline-4.4.1.dev8/assemblyline/datastore/support/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/support/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9259 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/support/build.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4531 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/datastore/support/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.081981 assemblyline-4.4.1.dev8/assemblyline/filestore/
--rw-r--r--   0 vsts      (1001) docker     (122)    10145 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.081981 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7663 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/azure.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2720 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9405 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/http.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5353 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/local.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6956 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/s3.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/filestore/transport/sftp.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.081981 assemblyline-4.4.1.dev8/assemblyline/odm/
--rw-r--r--   0 vsts      (1001) docker     (122)     1637 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48035 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)      323 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/common.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.089981 assemblyline-4.4.1.dev8/assemblyline/odm/messages/
--rw-r--r--   0 vsts      (1001) docker     (122)       75 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      596 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1532 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/archive_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      940 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/changes.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/dispatching.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1546 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3372 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1787 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/service_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2190 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/submission.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/task.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1116 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/odm/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/actions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6894 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/alert.py
--rw-r--r--   0 vsts      (1001) docker     (122)      281 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/cached_file.py
--rw-r--r--   0 vsts      (1001) docker     (122)    55609 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)      322 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/emptyresult.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2072 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/error.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2007 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/file.py
--rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/filescore.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1331 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/heuristic.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/filetypes/
--rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/filetypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24751 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5726 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/ontology.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/
--rw-r--r--   0 vsts      (1001) docker     (122)      445 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9834 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/network.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/process.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2507 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2886 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/signature.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3231 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/result.py
--rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/retrohunt.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3000 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10153 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/service.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/service_delta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/signature.py
--rw-r--r--   0 vsts      (1001) docker     (122)      695 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/statistics.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8663 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/submission.py
--rw-r--r--   0 vsts      (1001) docker     (122)      843 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/submission_summary.py
--rw-r--r--   0 vsts      (1001) docker     (122)      638 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/submission_tree.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35620 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/tagging.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9742 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/user.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1255 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/user_favorites.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2317 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/user_settings.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/models/workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/odm/random_data/
--rw-r--r--   0 vsts      (1001) docker     (122)    15957 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/random_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/random_data/create_test_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25241 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/random_data/sample_rules.yar
--rw-r--r--   0 vsts      (1001) docker     (122)     9244 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/odm/random_data/sample_suricata.rules
--rw-r--r--   0 vsts      (1001) docker     (122)    14680 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/odm/randomizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.101981 assemblyline-4.4.1.dev8/assemblyline/remote/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/
--rw-r--r--   0 vsts      (1001) docker     (122)     3448 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1984 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/counters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/events.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7000 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/exporting_counter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6018 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/hash.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1442 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/lock.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/comms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/multi.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/named.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7394 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/priority.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2902 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/set.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1926 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/assemblyline/run/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/run/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    53134 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/assemblyline/run/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/run/pubsub_reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3760 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/run/suricata_importer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4791 2023-03-24 14:59:18.000000 assemblyline-4.4.1.dev8/assemblyline/run/yara_importer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 14:59:37.045979 assemblyline-4.4.1.dev8/assemblyline.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 14:59:36.000000 assemblyline-4.4.1.dev8/assemblyline.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     6041 2023-03-24 14:59:37.000000 assemblyline-4.4.1.dev8/assemblyline.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-24 14:59:36.000000 assemblyline-4.4.1.dev8/assemblyline.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      506 2023-03-24 14:59:36.000000 assemblyline-4.4.1.dev8/assemblyline.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-03-24 14:59:36.000000 assemblyline-4.4.1.dev8/assemblyline.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-03-24 14:59:37.105982 assemblyline-4.4.1.dev8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3681 2023-03-24 14:59:20.000000 assemblyline-4.4.1.dev8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       47 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1558 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.138347 assemblyline-4.4.1.dev9/assemblyline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-03-24 16:14:10.000000 assemblyline-4.4.1.dev9/assemblyline/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.142347 assemblyline-4.4.1.dev9/assemblyline/cachestore/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3463 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/cachestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.150347 assemblyline-4.4.1.dev9/assemblyline/common/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4138 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/archiving.py
+-rw-r--r--   0 vsts      (1001) docker     (122)  2243670 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/attack_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13368 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/backupmanager.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2369 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/banner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15837 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/bundling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5646 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/caching.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      903 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/chunk.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    38686 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4532 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/classification.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     5811 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/cleanup_filestore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1789 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/codec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5031 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2512 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5147 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/custom.magic
+-rw-r--r--   0 vsts      (1001) docker     (122)    23191 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/custom.yara
+-rw-r--r--   0 vsts      (1001) docker     (122)     2903 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/dict_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2091 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/digests.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2041 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/entropy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1903 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8326 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/forge.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   168009 2023-03-24 16:14:11.000000 assemblyline-4.4.1.dev9/assemblyline/common/frequency.c
+-rw-r--r--   0 vsts      (1001) docker     (122)      709 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/frequency.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6402 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/heuristics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1398 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/hexdump.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19731 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/identify.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17758 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/identify_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      413 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/importing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4229 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/iprange.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3610 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/isotime.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4310 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/log.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      909 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/logformat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1564 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/lucene.lark
+-rw-r--r--   0 vsts      (1001) docker     (122)     1105 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/memory_zip.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4815 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/net.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21606 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/net_static.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      231 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/null.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/path.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28059 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/postprocess.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4971 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/random_user.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/security.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/signaturing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7002 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/str_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7665 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/common/tag_safelist.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3715 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/uid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/common/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.150347 assemblyline-4.4.1.dev9/assemblyline/datasource/
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2183 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/al.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1462 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datasource/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/datastore/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2950 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/bulk.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    86851 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    52444 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10135 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/datastore/support/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9259 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/build.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4531 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/datastore/support/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/filestore/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10145 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7663 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/azure.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2720 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9405 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3650 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/http.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5353 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/local.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6956 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/s3.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/filestore/transport/sftp.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.154347 assemblyline-4.4.1.dev9/assemblyline/odm/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1637 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48035 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      323 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/common.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.158347 assemblyline-4.4.1.dev9/assemblyline/odm/messages/
+-rw-r--r--   0 vsts      (1001) docker     (122)       75 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      596 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/alerter_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1532 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/archive_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      940 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/changes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatcher_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatching.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1546 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/expiry_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3372 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/ingest_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_status_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1787 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_timing_heartbeat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2190 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3788 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/task.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1116 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/messages/vacuum_heartbeat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3072 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/actions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6894 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/alert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      281 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/cached_file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    55609 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      322 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/emptyresult.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2072 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/error.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2007 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/file.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/filescore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1331 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/heuristic.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/
+-rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24751 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/pe.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5726 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/ontology.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.162347 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/
+-rw-r--r--   0 vsts      (1001) docker     (122)      445 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1843 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/antivirus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9834 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/malware_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/network.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2765 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/process.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2507 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/sandbox.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2886 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3231 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/result.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/retrohunt.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3000 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10153 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/service.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7749 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/service_delta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/signature.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      695 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/statistics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8663 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      843 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_summary.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      638 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_tree.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35620 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/tagging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9742 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1255 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user_favorites.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2317 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/user_settings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/models/workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15957 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/create_test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25241 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_rules.yar
+-rw-r--r--   0 vsts      (1001) docker     (122)     9244 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_suricata.rules
+-rw-r--r--   0 vsts      (1001) docker     (122)    14680 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/odm/randomizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3448 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1984 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/counters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/events.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7000 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/exporting_counter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6018 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/hash.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1442 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/lock.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1793 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/comms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      870 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/named.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7394 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/priority.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2902 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/set.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1926 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/user_quota_tracker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/assemblyline/run/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53134 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/assemblyline/run/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/pubsub_reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3760 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/suricata_importer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4791 2023-03-24 16:13:56.000000 assemblyline-4.4.1.dev9/assemblyline/run/yara_importer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:12.138347 assemblyline-4.4.1.dev9/assemblyline.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2393 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     6041 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      506 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       13 2023-03-24 16:14:12.000000 assemblyline-4.4.1.dev9/assemblyline.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-03-24 16:14:12.166347 assemblyline-4.4.1.dev9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3681 2023-03-24 16:13:58.000000 assemblyline-4.4.1.dev9/setup.py
```

### Comparing `assemblyline-4.4.1.dev8/LICENCE.md` & `assemblyline-4.4.1.dev9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/PKG-INFO` & `assemblyline-4.4.1.dev9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.4.1.dev8
+Version: 4.4.1.dev9
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-4.4.1.dev8/README.md` & `assemblyline-4.4.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/cachestore/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/archiving.py` & `assemblyline-4.4.1.dev9/assemblyline/common/archiving.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/attack_map.py` & `assemblyline-4.4.1.dev9/assemblyline/common/attack_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/backupmanager.py` & `assemblyline-4.4.1.dev9/assemblyline/common/backupmanager.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/banner.py` & `assemblyline-4.4.1.dev9/assemblyline/common/banner.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/bundling.py` & `assemblyline-4.4.1.dev9/assemblyline/common/bundling.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/caching.py` & `assemblyline-4.4.1.dev9/assemblyline/common/caching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/chunk.py` & `assemblyline-4.4.1.dev9/assemblyline/common/chunk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/classification.py` & `assemblyline-4.4.1.dev9/assemblyline/common/classification.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/classification.yml` & `assemblyline-4.4.1.dev9/assemblyline/common/classification.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/cleanup_filestore.py` & `assemblyline-4.4.1.dev9/assemblyline/common/cleanup_filestore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/codec.py` & `assemblyline-4.4.1.dev9/assemblyline/common/codec.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/comms.py` & `assemblyline-4.4.1.dev9/assemblyline/common/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/constants.py` & `assemblyline-4.4.1.dev9/assemblyline/common/constants.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/custom.magic` & `assemblyline-4.4.1.dev9/assemblyline/common/custom.magic`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/custom.yara` & `assemblyline-4.4.1.dev9/assemblyline/common/custom.yara`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/dict_utils.py` & `assemblyline-4.4.1.dev9/assemblyline/common/dict_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/digests.py` & `assemblyline-4.4.1.dev9/assemblyline/common/digests.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/entropy.py` & `assemblyline-4.4.1.dev9/assemblyline/common/entropy.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/exceptions.py` & `assemblyline-4.4.1.dev9/assemblyline/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/forge.py` & `assemblyline-4.4.1.dev9/assemblyline/common/forge.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/frequency.c` & `assemblyline-4.4.1.dev9/assemblyline/common/frequency.c`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/frequency.pyx` & `assemblyline-4.4.1.dev9/assemblyline/common/frequency.pyx`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/heuristics.py` & `assemblyline-4.4.1.dev9/assemblyline/common/heuristics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/hexdump.py` & `assemblyline-4.4.1.dev9/assemblyline/common/hexdump.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/identify.py` & `assemblyline-4.4.1.dev9/assemblyline/common/identify.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/identify_defaults.py` & `assemblyline-4.4.1.dev9/assemblyline/common/identify_defaults.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/iprange.py` & `assemblyline-4.4.1.dev9/assemblyline/common/iprange.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/isotime.py` & `assemblyline-4.4.1.dev9/assemblyline/common/isotime.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/log.py` & `assemblyline-4.4.1.dev9/assemblyline/common/log.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/logformat.py` & `assemblyline-4.4.1.dev9/assemblyline/common/logformat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/lucene.lark` & `assemblyline-4.4.1.dev9/assemblyline/common/lucene.lark`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/memory_zip.py` & `assemblyline-4.4.1.dev9/assemblyline/common/memory_zip.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/metrics.py` & `assemblyline-4.4.1.dev9/assemblyline/common/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/net.py` & `assemblyline-4.4.1.dev9/assemblyline/common/net.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/net_static.py` & `assemblyline-4.4.1.dev9/assemblyline/common/net_static.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/path.py` & `assemblyline-4.4.1.dev9/assemblyline/common/path.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/postprocess.py` & `assemblyline-4.4.1.dev9/assemblyline/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/random_user.py` & `assemblyline-4.4.1.dev9/assemblyline/common/random_user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/security.py` & `assemblyline-4.4.1.dev9/assemblyline/common/security.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/signaturing.py` & `assemblyline-4.4.1.dev9/assemblyline/common/signaturing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/str_utils.py` & `assemblyline-4.4.1.dev9/assemblyline/common/str_utils.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/tag_safelist.yml` & `assemblyline-4.4.1.dev9/assemblyline/common/tag_safelist.yml`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/tagging.py` & `assemblyline-4.4.1.dev9/assemblyline/common/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/common/uid.py` & `assemblyline-4.4.1.dev9/assemblyline/common/uid.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datasource/al.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/al.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datasource/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datasource/common.py` & `assemblyline-4.4.1.dev9/assemblyline/datasource/common.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/bulk.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/bulk.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/collection.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/exceptions.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/helper.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/store.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/store.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/support/build.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/support/build.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/datastore/support/schemas.py` & `assemblyline-4.4.1.dev9/assemblyline/datastore/support/schemas.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/azure.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/azure.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/base.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/ftp.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/ftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/http.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/http.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/local.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/local.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/s3.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/s3.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/filestore/transport/sftp.py` & `assemblyline-4.4.1.dev9/assemblyline/filestore/transport/sftp.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/base.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/alerter_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/alerter_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/archive_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/archive_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/changes.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/changes.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/dispatcher_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatcher_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/dispatching.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/dispatching.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/expiry_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/expiry_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/ingest_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/ingest_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/metrics.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/scaler_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/scaler_status_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/scaler_status_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/service_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/service_timing_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/service_timing_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/submission.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/task.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/task.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/messages/vacuum_heartbeat.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/messages/vacuum_heartbeat.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/actions.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/actions.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/alert.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/alert.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/config.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/error.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/error.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/file.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/file.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/filescore.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/filescore.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/heuristic.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/filetypes/pe.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/filetypes/pe.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/ontology.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/antivirus.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/antivirus.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/malware_config.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/malware_config.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/network.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/network.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/process.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/process.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/sandbox.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/sandbox.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/ontology/results/signature.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/ontology/results/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/replay.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/result.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/result.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/retrohunt.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/retrohunt.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/safelist.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/service.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/service.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/service_delta.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/service_delta.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/signature.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/signature.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/statistics.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/statistics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/submission.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/submission_summary.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_summary.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/submission_tree.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/submission_tree.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/tagging.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/tagging.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/user.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/user_favorites.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user_favorites.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/user_settings.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/user_settings.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/models/workflow.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/models/workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/random_data/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/random_data/create_test_data.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/create_test_data.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/random_data/sample_rules.yar` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_rules.yar`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/random_data/sample_suricata.rules` & `assemblyline-4.4.1.dev9/assemblyline/odm/random_data/sample_suricata.rules`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/odm/randomizer.py` & `assemblyline-4.4.1.dev9/assemblyline/odm/randomizer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/__init__.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/counters.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/counters.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/events.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/events.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/exporting_counter.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/exporting_counter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/hash.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/hash.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/lock.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/lock.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/comms.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/comms.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/multi.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/multi.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/named.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/named.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/queues/priority.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/queues/priority.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/set.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/set.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/remote/datatypes/user_quota_tracker.py` & `assemblyline-4.4.1.dev9/assemblyline/remote/datatypes/user_quota_tracker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/run/cli.py` & `assemblyline-4.4.1.dev9/assemblyline/run/cli.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/run/pubsub_reader.py` & `assemblyline-4.4.1.dev9/assemblyline/run/pubsub_reader.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/run/suricata_importer.py` & `assemblyline-4.4.1.dev9/assemblyline/run/suricata_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline/run/yara_importer.py` & `assemblyline-4.4.1.dev9/assemblyline/run/yara_importer.py`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/assemblyline.egg-info/PKG-INFO` & `assemblyline-4.4.1.dev9/assemblyline.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline
-Version: 4.4.1.dev8
+Version: 4.4.1.dev9
 Summary: Assemblyline 4 - Automated malware analysis framework
 Home-page: https://github.com/CybercentreCanada/assemblyline-base
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-4.4.1.dev8/assemblyline.egg-info/SOURCES.txt` & `assemblyline-4.4.1.dev9/assemblyline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-4.4.1.dev8/setup.py` & `assemblyline-4.4.1.dev9/setup.py`

 * *Files identical despite different names*

