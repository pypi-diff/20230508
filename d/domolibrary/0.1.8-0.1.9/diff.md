# Comparing `tmp/domolibrary-0.1.8.tar.gz` & `tmp/domolibrary-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.8.tar", last modified: Wed Apr 26 19:37:21 2023, max compression
+gzip compressed data, was "domolibrary-0.1.9.tar", last modified: Thu Apr 27 13:57:59 2023, max compression
```

## Comparing `domolibrary-0.1.8.tar` & `domolibrary-0.1.9.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.128456 domolibrary-0.1.8/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.004458 domolibrary-0.1.8/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.8/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.016457 domolibrary-0.1.8/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.060457 domolibrary-0.1.8/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.8/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.8/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.8/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.8/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.8/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.8/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.8/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.8/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.8/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.8/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.8/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 19:37:21.128456 domolibrary-0.1.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.076457 domolibrary-0.1.8/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148101 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.088456 domolibrary-0.1.8/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18323 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.088456 domolibrary-0.1.8/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 19:35:46.000000 domolibrary-0.1.8/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.092456 domolibrary-0.1.8/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.100456 domolibrary-0.1.8/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8346 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.100456 domolibrary-0.1.8/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 19:35:47.000000 domolibrary-0.1.8/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.080457 domolibrary-0.1.8/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.8/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 19:37:20.000000 domolibrary-0.1.8/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 19:37:15.000000 domolibrary-0.1.8/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 19:37:21.128456 domolibrary-0.1.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.8/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 19:37:21.124456 domolibrary-0.1.8/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.8/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.8/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.8/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.8/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.375308 domolibrary-0.1.9/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.179308 domolibrary-0.1.9/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.9/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.187308 domolibrary-0.1.9/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.223308 domolibrary-0.1.9/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.9/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.9/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.9/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.243308 domolibrary-0.1.9/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.9/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.9/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.9/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.9/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.9/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.243308 domolibrary-0.1.9/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.9/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.9/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-27 13:57:59.371308 domolibrary-0.1.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.247308 domolibrary-0.1.9/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   151032 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.259308 domolibrary-0.1.9/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18323 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2076 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25143 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7045 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5045 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6984 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15704 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14378 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.263308 domolibrary-0.1.9/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12088 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.267308 domolibrary-0.1.9/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.303308 domolibrary-0.1.9/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8346 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4533 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3859 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.307308 domolibrary-0.1.9/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-27 13:55:56.000000 domolibrary-0.1.9/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.251308 domolibrary-0.1.9/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3874 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.9/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-27 13:57:58.000000 domolibrary-0.1.9/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-27 13:57:47.000000 domolibrary-0.1.9/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-27 13:57:59.375308 domolibrary-0.1.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-27 13:57:59.367308 domolibrary-0.1.9/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.9/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.9/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.9/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.9/utils/upload_data.py
```

### Comparing `domolibrary-0.1.8/Automation/automation.py` & `domolibrary-0.1.9/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DataOcean/Transport.py` & `domolibrary-0.1.9/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.9/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.9/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DataOcean/cnfg_s3.py` & `domolibrary-0.1.9/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.9/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoAccount.py` & `domolibrary-0.1.9/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.9/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.9/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoApplication.py` & `domolibrary-0.1.9/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoAuth.py` & `domolibrary-0.1.9/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.9/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoCard.py` & `domolibrary-0.1.9/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoCertification.py` & `domolibrary-0.1.9/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.9/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.9/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoDataset.py` & `domolibrary-0.1.9/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoGrant.py` & `domolibrary-0.1.9/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoGroup.py` & `domolibrary-0.1.9/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.9/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoJob.py` & `domolibrary-0.1.9/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoLineage.py` & `domolibrary-0.1.9/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoPDP.py` & `domolibrary-0.1.9/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoPage.py` & `domolibrary-0.1.9/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoPublish.py` & `domolibrary-0.1.9/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoRole.py` & `domolibrary-0.1.9/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.9/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoStream.py` & `domolibrary-0.1.9/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoTag.py` & `domolibrary-0.1.9/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/DomoUser.py` & `domolibrary-0.1.9/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/get_data.py` & `domolibrary-0.1.9/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.9/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/LICENSE` & `domolibrary-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/PKG-INFO` & `domolibrary-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.8/README.md` & `domolibrary-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/_modidx.py` & `domolibrary-0.1.9/domolibrary/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,22 @@
                                                                                                                      'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap.get_pages': ( 'classes/domobootstrap.html#domobootstrap.get_pages',
                                                                                                                   'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature': ( 'classes/domobootstrap.html#domobootstrap_feature',
                                                                                                                 'domolibrary/classes/DomoBootstrap.py'),
                                                    'domolibrary.classes.DomoBootstrap.DomoBootstrap_Feature._from_json_bootstrap': ( 'classes/domobootstrap.html#domobootstrap_feature._from_json_bootstrap',
                                                                                                                                      'domolibrary/classes/DomoBootstrap.py')},
+            'domolibrary.classes.DomoCard': { 'domolibrary.classes.DomoCard.DomoCard': ( 'classes/domocard.html#domocard',
+                                                                                         'domolibrary/classes/DomoCard.py'),
+                                              'domolibrary.classes.DomoCard.DomoCard.__post_init__': ( 'classes/domocard.html#domocard.__post_init__',
+                                                                                                       'domolibrary/classes/DomoCard.py'),
+                                              'domolibrary.classes.DomoCard.DomoCard._from_json': ( 'classes/domocard.html#domocard._from_json',
+                                                                                                    'domolibrary/classes/DomoCard.py'),
+                                              'domolibrary.classes.DomoCard.DomoCard.display_url': ( 'classes/domocard.html#domocard.display_url',
+                                                                                                     'domolibrary/classes/DomoCard.py')},
             'domolibrary.classes.DomoDatacenter': { 'domolibrary.classes.DomoDatacenter.DomoDatacenter': ( 'classes/domodatacenter.html#domodatacenter',
                                                                                                            'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.get_accounts': ( 'classes/domodatacenter.html#domodatacenter.get_accounts',
                                                                                                                         'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datacenter': ( 'classes/domodatacenter.html#domodatacenter.search_datacenter',
                                                                                                                              'domolibrary/classes/DomoDatacenter.py'),
                                                     'domolibrary.classes.DomoDatacenter.DomoDatacenter.search_datasets': ( 'classes/domodatacenter.html#domodatacenter.search_datasets',
@@ -281,14 +289,16 @@
                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_allowlist',
                                                                                                                                      'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_authorized_domains': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_authorized_domains',
                                                                                                                                               'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_grants': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_grants',
                                                                                                                                   'domolibrary/classes/DomoInstanceConfig.py'),
+                                                        'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_publications': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_publications',
+                                                                                                                                        'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.get_roles': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.get_roles',
                                                                                                                                  'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.set_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.set_allowlist',
                                                                                                                                      'domolibrary/classes/DomoInstanceConfig.py'),
                                                         'domolibrary.classes.DomoInstanceConfig.DomoInstanceConfig.upsert_allowlist': ( 'classes/domoinstanceconfig.html#domoinstanceconfig.upsert_allowlist',
                                                                                                                                         'domolibrary/classes/DomoInstanceConfig.py')},
             'domolibrary.classes.DomoPDP': { 'domolibrary.classes.DomoPDP.Dataset_PDP_Policies': ( 'classes/domopdp.html#dataset_pdp_policies',
@@ -317,14 +327,16 @@
                                                                                                        'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.SearchPDP_NotFound': ( 'classes/domopdp.html#searchpdp_notfound',
                                                                                                  'domolibrary/classes/DomoPDP.py'),
                                              'domolibrary.classes.DomoPDP.SearchPDP_NotFound.__init__': ( 'classes/domopdp.html#searchpdp_notfound.__init__',
                                                                                                           'domolibrary/classes/DomoPDP.py')},
             'domolibrary.classes.DomoPage': { 'domolibrary.classes.DomoPage.DomoPage': ( 'classes/domopage.html#domopage',
                                                                                          'domolibrary/classes/DomoPage.py'),
+                                              'domolibrary.classes.DomoPage.DomoPage._from_adminsummary': ( 'classes/domopage.html#domopage._from_adminsummary',
+                                                                                                            'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_bootstrap': ( 'classes/domopage.html#domopage._from_bootstrap',
                                                                                                          'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage._from_content_stacks_v3': ( 'classes/domopage.html#domopage._from_content_stacks_v3',
                                                                                                                  'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.display_url': ( 'classes/domopage.html#domopage.display_url',
                                                                                                      'domolibrary/classes/DomoPage.py'),
                                               'domolibrary.classes.DomoPage.DomoPage.get_accesslist': ( 'classes/domopage.html#domopage.get_accesslist',
@@ -427,14 +439,16 @@
                                                                                                             'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.get_by_id': ( 'classes/domouser.html#domouser.get_by_id',
                                                                                                    'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.request_password_reset': ( 'classes/domouser.html#domouser.request_password_reset',
                                                                                                                 'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.reset_password': ( 'classes/domouser.html#domouser.reset_password',
                                                                                                         'domolibrary/classes/DomoUser.py'),
+                                              'domolibrary.classes.DomoUser.DomoUser.set_user_landing_page': ( 'classes/domouser.html#domouser.set_user_landing_page',
+                                                                                                               'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUser.update_properties': ( 'classes/domouser.html#domouser.update_properties',
                                                                                                            'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers': ( 'classes/domouser.html#domousers',
                                                                                           'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers._generate_logger': ( 'classes/domouser.html#domousers._generate_logger',
                                                                                                            'domolibrary/classes/DomoUser.py'),
                                               'domolibrary.classes.DomoUser.DomoUsers._users_to_domo_user': ( 'classes/domouser.html#domousers._users_to_domo_user',
@@ -707,15 +721,19 @@
                                                                                                           'domolibrary/routes/activity_log.py')},
             'domolibrary.routes.bootstrap': { 'domolibrary.routes.bootstrap.get_bootstrap': ( 'routes/bootstrap.html#get_bootstrap',
                                                                                               'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_features': ( 'routes/bootstrap.html#get_bootstrap_features',
                                                                                                        'domolibrary/routes/bootstrap.py'),
                                               'domolibrary.routes.bootstrap.get_bootstrap_pages': ( 'routes/bootstrap.html#get_bootstrap_pages',
                                                                                                     'domolibrary/routes/bootstrap.py')},
-            'domolibrary.routes.card': { 'domolibrary.routes.card.generate_body_search_cards_admin_summary': ( 'routes/card.html#generate_body_search_cards_admin_summary',
+            'domolibrary.routes.card': { 'domolibrary.routes.card.CardSearch_NotFoundError': ( 'routes/card.html#cardsearch_notfounderror',
+                                                                                               'domolibrary/routes/card.py'),
+                                         'domolibrary.routes.card.CardSearch_NotFoundError.__init__': ( 'routes/card.html#cardsearch_notfounderror.__init__',
+                                                                                                        'domolibrary/routes/card.py'),
+                                         'domolibrary.routes.card.generate_body_search_cards_admin_summary': ( 'routes/card.html#generate_body_search_cards_admin_summary',
                                                                                                                'domolibrary/routes/card.py'),
                                          'domolibrary.routes.card.get_card_metadata': ( 'routes/card.html#get_card_metadata',
                                                                                         'domolibrary/routes/card.py'),
                                          'domolibrary.routes.card.get_kpi_definition': ( 'routes/card.html#get_kpi_definition',
                                                                                          'domolibrary/routes/card.py'),
                                          'domolibrary.routes.card.search_cards_admin_summary': ( 'routes/card.html#search_cards_admin_summary',
                                                                                                  'domolibrary/routes/card.py')},
@@ -842,15 +860,17 @@
                                                     'domolibrary.routes.instance_config.set_authorized_domains': ( 'routes/instance_config.html#set_authorized_domains',
                                                                                                                    'domolibrary/routes/instance_config.py')},
             'domolibrary.routes.page': { 'domolibrary.routes.page.get_page_access_list': ( 'routes/page.html#get_page_access_list',
                                                                                            'domolibrary/routes/page.py'),
                                          'domolibrary.routes.page.get_page_by_id': ( 'routes/page.html#get_page_by_id',
                                                                                      'domolibrary/routes/page.py'),
                                          'domolibrary.routes.page.get_page_definition': ( 'routes/page.html#get_page_definition',
-                                                                                          'domolibrary/routes/page.py')},
+                                                                                          'domolibrary/routes/page.py'),
+                                         'domolibrary.routes.page.get_pages_adminsummary': ( 'routes/page.html#get_pages_adminsummary',
+                                                                                             'domolibrary/routes/page.py')},
             'domolibrary.routes.pdp': { 'domolibrary.routes.pdp.CreatePolicy_Error': ( 'routes/pdp.html#createpolicy_error',
                                                                                        'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.CreatePolicy_Error.__init__': ( 'routes/pdp.html#createpolicy_error.__init__',
                                                                                                 'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.PDP_NotRetrieved': ( 'routes/pdp.html#pdp_notretrieved',
                                                                                      'domolibrary/routes/pdp.py'),
                                         'domolibrary.routes.pdp.PDP_NotRetrieved.__init__': ( 'routes/pdp.html#pdp_notretrieved.__init__',
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.9/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.9/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.9/domolibrary/classes/DomoBootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoBootstrap.ipynb.
 
 # %% auto 0
 __all__ = ['DomoBootstrap_Feature', 'DomoBootstrap']
 
 # %% ../../nbs/classes/50_DomoBootstrap.ipynb 2
 from dataclasses import dataclass, field
-
+from fastcore.basics import patch_to
 import httpx
 
 import domolibrary.classes.DomoPage as dmpg
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.Logger as lc
 import domolibrary.routes.bootstrap as bootstrap_routes
 
 
 # %% ../../nbs/classes/50_DomoBootstrap.ipynb 3
-from fastcore.basics import patch_to
-
-
-
-# %% ../../nbs/classes/50_DomoBootstrap.ipynb 4
 @dataclass
 class DomoBootstrap_Feature:
     id: int
     name: str
     label: str
     type: str
     purchased: bool
@@ -41,35 +36,35 @@
             label=dd.label,
             type=dd.type,
             purchased=dd.purchased,
             enabled=dd.enabled
         )
         return bsf
 
-# %% ../../nbs/classes/50_DomoBootstrap.ipynb 5
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 4
 @dataclass
 class DomoBootstrap:
     auth : dmda.DomoAuth = field(repr = False)
     page_ls : list[dmpg.DomoPage] = field(default = None)
     feature_ls : list[DomoBootstrap_Feature] = field(default = None)
     
 
-# %% ../../nbs/classes/50_DomoBootstrap.ipynb 6
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 5
 @patch_to(DomoBootstrap)
 async def get_all(self: DomoBootstrap,
                   auth: dmda.DomoAuth = None, debug_api: bool = False):
     
     auth = auth or self.auth
 
     res =  await bootstrap_routes.get_bootstrap(auth=auth, debug_api=debug_api)
 
     return res.response
 
 
-# %% ../../nbs/classes/50_DomoBootstrap.ipynb 9
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 8
 @patch_to(DomoBootstrap)
 async def get_pages(self: DomoBootstrap,
                     auth: dmda.DomoAuth = None, return_raw : bool = False, debug_api: bool = False) -> list[dmpg.DomoPage]:
 
     auth = auth or self.auth
 
     res = await bootstrap_routes.get_bootstrap_pages(auth=auth,
@@ -84,15 +79,15 @@
     page_ls = res.response
 
     self.page_ls =  [dmpg.DomoPage._from_bootstrap(page_obj, auth = auth) for page_obj in page_ls]
 
     return self.page_ls
 
 
-# %% ../../nbs/classes/50_DomoBootstrap.ipynb 12
+# %% ../../nbs/classes/50_DomoBootstrap.ipynb 11
 @patch_to(DomoBootstrap)
 async def get_features(self : DomoBootstrap,
                         auth: dmda.DomoAuth = None,
                         debug_api: bool = False,
                         return_raw:bool = False,
                         session: httpx.AsyncClient = None, 
                         ):
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.9/domolibrary/classes/DomoDataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 # from . import DomoTag as dmtg
 
 
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.DomoError as de
 import domolibrary.routes.dataset as dataset_routes
+import domolibrary.classes.DomoPDP as dmpdp
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 7
 async def _have_prereqs(self, auth, dataset_id, function_name):
     """tests if have a parent dataset or prerequsite dataset_id and auth object"""
 
     auth_from_self_dataset = getattr(self.dataset, 'auth', None) if getattr(self, 'dataset', None) else None
     auth_from_self = getattr(self , 'auth', None)
@@ -274,21 +275,21 @@
     owner: dict = field(default_factory=dict)
     formula: dict = field(default_factory=dict)
 
     schema: DomoDataset_Schema = field(default=None)
     tags: DomoDataset_Tags = field(default=None)
 
     # certification: dmdc.DomoCertification = None
-    # PDPPolicies: dmpdp.Dataset_PDP_Policies = None
+    PDPPolicies: dmpdp.Dataset_PDP_Policies = None
 
     def __post_init__(self):
         self.schema = DomoDataset_Schema(dataset=self)
         self.tags = DomoDataset_Tags(dataset=self)
 
-        # self.PDPPolicies = dmpdp.Dataset_PDP_Policies(dataset=self)
+        self.PDPPolicies = dmpdp.Dataset_PDP_Policies(dataset=self)
 
     def display_url(self):
         return f"https://{self.auth.domo_instance }.domo.com/datasources/{self.id}/details/overview"
 
 # %% ../../nbs/classes/50_DomoDataset.ipynb 26
 @patch_to(DomoDataset, cls_method=True)
 async def get_from_id(
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.9/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.9/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.9/domolibrary/classes/DomoInstanceConfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,35 +17,52 @@
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoError as de
 import domolibrary.routes.instance_config as instance_config_routes
 import domolibrary.routes.grant as grant_routes
 import domolibrary.classes.DomoGrant as dmdg
 import domolibrary.classes.DomoRole as dmr
 import domolibrary.routes.role as role_routes
+import domolibrary.routes.publish as publish_routes
+import domolibrary.classes.DomoPublish as dmpb
 
 # import Library.utils.convert as cd
-# from .DomoAuth import DomoAuth
 # from .DomoApplication import DomoApplication
-# import Library.DomoClasses.DomoPublish as dmpb
-
 
 # import domolibrary.utils.convert as cd
 # import domolibrary.utils.DictDot as util_dd
 # import domolibrary.client.DomoError as de
 
 
 # %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 4
 @dataclass
 class DomoInstanceConfig:
     """utility class that absorbs many of the domo instance configuration methods"""
     
     auth: dmda.DomoAuth
     allowlist : list[str] = field(default_factory = list)
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 5
+    @classmethod
+    async def get_publications(cls,
+                            auth: dmda.DomoFullAuth,
+                            debug_api: bool = False, session: httpx.AsyncClient = None, return_raw: bool = False):
+        
+        res = await publish_routes.search_publications(auth=auth,
+                                                       debug_api=debug_api,
+                                                       session=session)
+        if debug_api:
+            print('Getting Publish jobs')
+
+        if res.status == 200 and not return_raw:
+            return await asyncio.gather(*[dmpb.DomoPublication.get_from_id(publication_id=job.get('id'),
+                                                                           auth=auth) for job in res.response])
+
+        if res.status == 200 and return_raw:
+            return res.response
+
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 7
 @patch_to(DomoInstanceConfig)
 async def get_allowlist(self: DomoInstanceConfig, 
                         auth: dmda.DomoFullAuth = None, # get_allowlist requires full authentication
                         session: httpx.AsyncClient = None, 
                         return_raw : bool = False,
                         debug_api: bool = False) -> list[str]:
     """retrieves the allowlist for an instance"""
@@ -72,15 +89,15 @@
     allowlist = res.response.get('addresses')
 
     self.allowlist = allowlist
 
     return allowlist
 
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 9
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 11
 @patch_to(DomoInstanceConfig)
 async def set_allowlist(self : DomoInstanceConfig,
                         ip_address_ls: list[str],
                         debug_api: bool = False,
                         auth: dmda.DomoFullAuth = None,
                         session: httpx.AsyncClient = None
                         ):
@@ -106,15 +123,15 @@
     ip_address_ls += exist_ip_address_ls
 
     return await self.set_allowlist(auth=auth,
                                    ip_address_ls=list(set(ip_address_ls)),
                                    debug_api=debug_api, session=session)
 
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 14
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 16
 @patch_to(DomoInstanceConfig)
 async def get_grants(self: DomoInstanceConfig,
                      auth: dmda.DomoAuth = None,
                      debug_prn:bool = False,
                      debug_api: bool = False,
                      session: httpx.AsyncClient = None,
                      return_raw: bool = False):
@@ -135,15 +152,15 @@
         return res
 
     if res.status == 200:
         json_list = res.response
         return [dmdg.DomoGrant._from_json(obj) for obj in json_list]
 
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 17
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 19
 @patch_to(DomoInstanceConfig)
 async def get_roles(self, auth: dmda.DomoAuth = None,
                     debug_api: bool = False,
                     return_raw: bool = False,
                     session: httpx.AsyncClient = None):
 
     auth = auth or self.auth
@@ -156,15 +173,15 @@
 
     if res.status == 200:
         json_list = res.response
         return [dmr.DomoRole._from_json(obj = obj, auth = auth
                                    ) for obj in json_list]
 
 
-# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 21
+# %% ../../nbs/classes/50_DomoInstanceConfig.ipynb 23
 @patch_to(DomoInstanceConfig)
 async def get_authorized_domains(self: DomoInstanceConfig,
                                  auth: dmda.DomoAuth = None, 
                                  debug_api: bool = False,
                                  session: httpx.AsyncClient = None,
                                  return_raw :bool = False
                                  ):
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.9/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.9/domolibrary/classes/DomoPage.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,14 +108,40 @@
     pg = await cls._from_content_stacks_v3(page_obj=res.response, auth=auth)
 
     return pg
 
 
 # %% ../../nbs/classes/50_DomoPage.ipynb 10
 @patch_to(DomoPage)
+async def _from_adminsummary():
+
+    import domolibrary.classes.DomoCard as dmc
+
+    dd = page_obj
+    if isinstance(page_obj, dict):
+        dd = util_dd.DictDot(page_obj)
+
+    pg = cls(
+        id=dd.id,
+        title=dd.title,
+        parent_page_id=dd.page.parentPageId,
+        owners=dd.page.owners,
+        collections=dd.collections,
+        auth=auth
+    )
+
+    if dd.cards and len(dd.cards) > 0:
+        pg.cards = await asyncio.gather(
+            *[dmc.DomoCard.get_from_id(id=card.id, auth=auth) for card in dd.cards])
+
+    return pg
+
+
+# %% ../../nbs/classes/50_DomoPage.ipynb 11
+@patch_to(DomoPage)
 async def get_accesslist(self,
                          auth: dmda.DomoAuth = None,
                          is_expand_users: bool = False,
                          return_raw: bool = False,
                          debug_api: bool = False):
 
     auth = auth or self.auth
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.9/domolibrary/classes/DomoPublish.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 __all__ = ['DomoPublication_Subscription', 'DomoPublication_Content', 'DomoPublication_UnexpectedContentType', 'DomoPublication',
            'DomoPublications']
 
 # %% ../../nbs/classes/50_DomoPublish.ipynb 2
 from dataclasses import dataclass, field
 
 from typing import Optional
-
 import datetime as dt
 import asyncio
 import httpx
 
 from fastcore.basics import patch_to
 
 # import importlib
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.9/domolibrary/classes/DomoRole.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 # %% ../../nbs/classes/50_DomoRole.ipynb 8
 class SetRoleGrants_MissingGrants(de.DomoError):
     def __init__(self, role_id, missing_grants: [str], domo_instance):
         super().__init__(domo_instance=domo_instance, entity_id=role_id,
                          message=f"failed to add grants: {', '.join(missing_grants)}")
 
 
+# %% ../../nbs/classes/50_DomoRole.ipynb 9
 @patch_to(DomoRole)
 async def set_grants(self: DomoRole,
                      grant_ls: list[dmg.DomoGrant],
                      role_id: str = None,
                      auth: dmda.DomoAuth = None,
                      debug_api: bool = False):
 
@@ -155,15 +156,15 @@
     if missing_grants:
         raise SetRoleGrants_MissingGrants(
             role_id=role_id, missing_grants=missing_grants, domo_instance=auth.domo_instance)
 
     return domo_grants
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 12
+# %% ../../nbs/classes/50_DomoRole.ipynb 13
 @patch_to(DomoRole)
 async def get_membership(self,
                          role_id=None,
                          auth: dmda.DomoAuth = None,
                          return_raw:bool = False,
                          debug_api: bool = False, session: httpx.AsyncClient = None):
 
@@ -181,21 +182,21 @@
     membership_ls = [dmu.DomoUser._from_search_json(user_obj = obj, auth = auth)for obj in res.response]
 
     self.membership_ls = membership_ls
 
     return membership_ls
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 15
+# %% ../../nbs/classes/50_DomoRole.ipynb 16
 class AddUser_Error(de.DomoError):
     def __init__(self, role_id, domo_instance, user_id, user_name = None):
         user_str = f"{user_id} - {user_name}" if user_name else user_id
         super().__init__(domo_instance = domo_instance, message = f"unable to add {user_str} to role {role_id}")
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 16
+# %% ../../nbs/classes/50_DomoRole.ipynb 17
 @patch_to(DomoRole)
 async def add_user(self,
                    user: dmu.DomoUser,
                    role_id: str = None,
                    auth: dmda.DomoAuth = None, debug_api: bool = False,
                    session : httpx.AsyncClient = None
                    ):
@@ -218,15 +219,15 @@
     if user not in domo_members:
         raise AddUser_Error(role_id=role_id, domo_instance=auth.domo_instance,
                             user_id=user.id, user_name=user.display_name)
 
     return domo_members
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 20
+# %% ../../nbs/classes/50_DomoRole.ipynb 21
 @patch_to(DomoRole)
 async def update_role_metadata(self : DomoRole,
                                auth: dmda.DomoAuth = None,
                                role_name=None,
                                role_description: str = None,
                                debug_api: bool = False,
                                session: httpx.AsyncClient = None,
@@ -254,23 +255,24 @@
         (DomoRole._from_json(role, auth = auth) for role in role_ls.response if role.get('name') == role_name), None)
     
     return domo_role
 
 
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 24
+# %% ../../nbs/classes/50_DomoRole.ipynb 25
 class DeleteRole_Error(de.DomoError):
     def __init__(self,
                  role_id,
                  domo_instance):
         super().__init__(
             message=f'role: {role_id} not found', domo_instance=domo_instance)
 
 
+# %% ../../nbs/classes/50_DomoRole.ipynb 26
 @patch_to(DomoRole, cls_method=True)
 async def delete_role(cls: DomoRole,
                       role_id: int,
                       auth: dmda.DomoAuth = None,
                       debug_api: bool = False,
                       session: httpx.AsyncClient = None,
                       ):
@@ -287,21 +289,21 @@
         role_id= role_id,
         auth=auth,
         debug_api=debug_api,
         session=session
     )
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 28
+# %% ../../nbs/classes/50_DomoRole.ipynb 30
 @dataclass
 class DomoRoles:
     auth: dmda.DomoAuth
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 29
+# %% ../../nbs/classes/50_DomoRole.ipynb 31
 @patch_to(DomoRoles, cls_method=True)
 async def get_roles(cls: DomoRoles,
                     auth: dmda.DomoAuth,
                     debug_api: bool = False,
                     session: httpx.AsyncClient = None,
                     return_raw: bool = False
                     ):
@@ -316,24 +318,26 @@
     default_role_res = await role_routes.get_default_role(auth=auth, session=session, debug_api=debug_api)
 
     return [DomoRole._from_json(role,
                                 auth, 
                                 is_default_role=str(default_role_res.response) == str(role.get('id'))) for role in res.response]
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 32
+# %% ../../nbs/classes/50_DomoRole.ipynb 34
 class SearchRole_NotFound(de.DomoError):
     def __init__(self, domo_instance,
                  role_id,
                  message='not found',
                  function_name='search_role'):
 
         super().__init__(domo_instance=domo_instance, message=message,
                          entity_id=role_id, function_name=function_name)
 
+
+# %% ../../nbs/classes/50_DomoRole.ipynb 35
 @patch_to(DomoRoles, cls_method=True)
 async def search_role(cls: DomoRoles,
                     auth: dmda.DomoAuth,
                     role_name: str = None,
                     role_id : str = None,
                     debug_api: bool = False,
                     session: httpx.AsyncClient = None,
@@ -351,29 +355,29 @@
             (role for role in all_roles if str(role.id) == str(role_id)), None)
 
     if not domo_role:
         raise SearchRole_NotFound(domo_instance=auth.domo_instance, role_id=role_name)
 
     return domo_role
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 36
+# %% ../../nbs/classes/50_DomoRole.ipynb 39
 class CreateRole_Error(de.DomoError):
     def __init__(self, domo_instance,
                  role_id,
                  message,
                  status,
                  function_name='create_role'):
 
         super().__init__(domo_instance=domo_instance,
                          message=message, status=status,
                          entity_id=role_id,
                          function_name=function_name)
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 37
+# %% ../../nbs/classes/50_DomoRole.ipynb 40
 @patch_to(DomoRoles, cls_method=True)
 async def create_role(cls: DomoRoles,
                       auth: dmda.DomoAuth,
                       name: str,
                       description: str = None,
                       debug_api: bool = False,
                       session : httpx.AsyncClient = None
@@ -405,15 +409,15 @@
             message = res.response,
             status = res.status,
         )
     
     return await DomoRoles.search_role(auth = auth, role_name= name)
     
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 40
+# %% ../../nbs/classes/50_DomoRole.ipynb 43
 @patch_to(DomoRoles, cls_method=True)
 async def upsert_role(cls: DomoRoles,
                       auth: dmda.DomoAuth,
                       name: str,
                       description: str = None,
                       grant_ls : [dmg.DomoGrant] = None,
                       debug_api: bool = False,
@@ -450,15 +454,15 @@
             grant_ls = domo_role._valid_grant_ls(grant_ls)
             await domo_role.set_grants(grant_ls= grant_ls)
             
 
         return domo_role
 
 
-# %% ../../nbs/classes/50_DomoRole.ipynb 44
+# %% ../../nbs/classes/50_DomoRole.ipynb 47
 @patch_to(DomoRole)
 async def set_as_default_role(self: DomoRole, debug_api: bool = False, session : httpx.AsyncClient = None):
     return await role_routes.set_default_role(auth=self.auth,
                                                 role_id=self.id,
                                                 debug_api=debug_api, session = session
                                                 )
```

### Comparing `domolibrary-0.1.8/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.9/domolibrary/classes/DomoUser.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,36 @@
         domo_instance=domo_instance,
         email=email,
         locale=locale,
         debug_api=debug_api,
         session=session,
     )
 
+# %% ../../nbs/classes/50_DomoUser.ipynb 12
+@patch_to(DomoUser)
+async def set_user_landing_page(
+    self: DomoUser,
+    page_id: str,
+    user_id: str = None,
+    auth: dmda.DomoAuth = None,
+    debug_api: bool = False,
+):
+
+    res = await user_routes.set_user_landing_page(
+        auth=auth or self.auth,
+        page_id=page_id,
+        user_id=self.id or user_id,
+        debug_api=debug_api,
+    )
+
+    if res.status != 200:
+        return False
+
+    return True
+
 # %% ../../nbs/classes/50_DomoUser.ipynb 13
 @patch_to(DomoUser)
 async def update_properties(
     self: DomoUser,
     property_ls: [UserProperty],
     return_raw: bool = False,
     auth: dmda.DomoAuth = None,
```

### Comparing `domolibrary-0.1.8/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.9/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/client/DomoError.py` & `domolibrary-0.1.9/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/client/Logger.py` & `domolibrary-0.1.9/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.9/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/client/get_data.py` & `domolibrary-0.1.9/domolibrary/client/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 # %% ../../nbs/client/10_get_data.ipynb 11
 async def looper(
     auth: dmda.DomoAuth,
     session: httpx.AsyncClient,
     url,
     offset_params,
     arr_fn: callable,
-    loop_until_end: bool = False,
+    loop_until_end: bool = False, # usually you'll set this to true.  it will override maximum
     method="POST",
     body: dict = None,
     fixed_params: dict = None,
     offset_params_in_body: bool = False,
     body_fn=None,
     limit=1000,
     skip=0,
```

### Comparing `domolibrary-0.1.8/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.9/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.9/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/account.py` & `domolibrary-0.1.9/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/activity_log.py` & `domolibrary-0.1.9/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.9/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/card.py` & `domolibrary-0.1.9/domolibrary/routes/card.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,109 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/card.ipynb.
 
 # %% auto 0
-__all__ = ['get_kpi_definition', 'get_card_metadata', 'generate_body_search_cards_admin_summary', 'search_cards_admin_summary']
+__all__ = ['CardSearch_NotFoundError', 'get_kpi_definition', 'get_card_metadata', 'generate_body_search_cards_admin_summary',
+           'search_cards_admin_summary']
 
 # %% ../../nbs/routes/card.ipynb 2
 from typing import Optional
 
 import io
 import pandas as pd
 
 import httpx
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
+import domolibrary.client.DomoError as de
 
 
 # %% ../../nbs/routes/card.ipynb 3
+class CardSearch_NotFoundError(de.DomoError):
+    def __init__(self, card_id,
+                 domo_instance, 
+                 function_name,status,
+                  message = None,
+                 ):
+        super().__init__(status=status,
+                         message=f"card {card_id} not found", domo_instance=domo_instance, function_name=function_name)
+
+
+# %% ../../nbs/routes/card.ipynb 4
 async def get_kpi_definition(auth: dmda.DomoAuth, card_id: str, debug_api: bool = False) -> rgd.ResponseGetData:
-    
+
     url = f"https://{auth.domo_instance}.domo.com/api/content/v3/cards/kpi/definition"
 
     body = {"urn": card_id}
 
     res = await gd.get_data(
         auth=auth,
         url=url,
         method='PUT',
         body=body,
         debug_api=False
     )
 
+    if not res.is_success and res.response == 'Not Found':
+        raise CardSearch_NotFoundError(card_id=card_id,
+                                       status=res.status,
+                                       domo_instance=auth.domo_instance, 
+                                       function_name='get_kpi_definition')
+
     return res
 
-# %% ../../nbs/routes/card.ipynb 6
+
+# %% ../../nbs/routes/card.ipynb 7
 async def get_card_metadata(auth: dmda.DomoAuth, card_id: str, debug_api: bool = False) -> rgd.ResponseGetData:
     optional_params = "metadata,certification,datasources,owners,problems"
     url = f"https://{auth.domo_instance}.domo.com/api/content/v1/cards?urns={card_id}&parts={optional_params}"
 
     res = await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
         debug_api=debug_api
     )
 
+    if res.is_success and len( res.response) == 0:
+        raise CardSearch_NotFoundError(card_id=card_id,
+                                       status=res.status,
+                                       domo_instance=auth.domo_instance,
+                                       function_name='get_kpi_definition')
+
+    res.response = res.response[0]
+
     return res
 
-# %% ../../nbs/routes/card.ipynb 9
+# %% ../../nbs/routes/card.ipynb 10
 def generate_body_search_cards_admin_summary(page_ids: [str] = None,
                                              searchPages: bool = True,
                                              cardSearchText: str = '',
                                              pageSearchText: str = '') -> dict:
     body = {
         "ascending": True,
         "orderBy": "cardTitle"
     }
 
-    
-
     if cardSearchText:
         body.update({'cardTitleSearchText': cardSearchText, "includeCardTitleClause": True })
 
     if pageSearchText:
         body.update({'pageTitleSearchText': pageSearchText, "includePageTitleClause": True, "notOnPage": False})
 
     if page_ids:
         body.update({'pageIds': page_ids})
 
     return body
 
-# %% ../../nbs/routes/card.ipynb 10
+# %% ../../nbs/routes/card.ipynb 11
 async def search_cards_admin_summary(auth: dmda.DomoAuth,
                                      body: dict,
-
                                      maximum :int = None,
-                                     
                                      debug_api: bool = False,
                                      debug_loop: bool = False,
                                      session : httpx.AsyncClient  = None,
                                      wait_sleep: int = 3
 
                                      ) -> rgd.ResponseGetData:
```

### Comparing `domolibrary-0.1.8/domolibrary/routes/datacenter.py` & `domolibrary-0.1.9/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/dataflow.py` & `domolibrary-0.1.9/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/dataset.py` & `domolibrary-0.1.9/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/grant.py` & `domolibrary-0.1.9/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/group.py` & `domolibrary-0.1.9/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/instance_config.py` & `domolibrary-0.1.9/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/page.py` & `domolibrary-0.1.9/domolibrary/routes/page.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/page.ipynb.
 
 # %% auto 0
-__all__ = ['get_page_by_id', 'get_page_definition', 'get_page_access_list']
+__all__ = ['get_page_by_id', 'get_page_definition', 'get_page_access_list', 'get_pages_adminsummary']
 
 # %% ../../nbs/routes/page.ipynb 2
 import httpx
 import pandas as pd
 
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 
 
 # %% ../../nbs/routes/page.ipynb 3
 async def get_page_by_id(auth: dmda.DomoAuth, page_id: str,
                          debug_api: bool = False, 
                          session: httpx.AsyncClient = None,
+                         include_layout: bool = False
                          ) -> rgd.ResponseGetData:
     url = f'https://{auth.domo_instance}.domo.com/api/content/v3/stacks/{page_id}/cards'
-
+    
+    if include_layout:
+        url+='?includeV4PageLayouts=true'
+    
     res = await gd.get_data(
         auth=auth,
         url=url,
         method='GET',
         debug_api=debug_api,
         session = session,
     )
@@ -68,7 +72,40 @@
         group_users = [user for group in res.response.get(
             'groups') for user in group.get('users')]
         users = res.response.get('users') + group_users
         res.response.update({'users': users})
 
     return res
 
+
+# %% ../../nbs/routes/page.ipynb 12
+async def get_pages_adminsummary(auth: dmda.DomoAuth,
+                                 debug_loop: bool = False,
+                                 debug_api : bool = False,
+                                 limit = 35,
+                                 session: httpx.AsyncClient = None):
+    """retrieves all pages in instance user is able to see (but may not have been explicitly shared)"""
+
+    url = f'https://{auth.domo_instance}.domo.com/api/content/v1/pages/adminsummary'
+
+    offset_params = {
+        'offset': 'skip',
+        'limit': 'limit',
+    }
+
+    body = {"orderBy": "pageTitle", "ascending": True}
+
+    def arr_fn(res) -> list[dict]:
+        return res.response.get('pageAdminSummaries')
+
+    res = await gd.looper(auth=auth,
+                          method='POST',
+                          url=url,
+                          arr_fn=arr_fn,
+                          offset_params=offset_params,
+                          session=session,
+                          loop_until_end=True,
+                          body = body,
+                          limit = limit, 
+                          debug_loop=debug_loop, debug_api= debug_api)
+    return res.response
+
```

### Comparing `domolibrary-0.1.8/domolibrary/routes/pdp.py` & `domolibrary-0.1.9/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/publish.py` & `domolibrary-0.1.9/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/role.py` & `domolibrary-0.1.9/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/routes/user.py` & `domolibrary-0.1.9/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/utils/DictDot.py` & `domolibrary-0.1.9/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.9/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/utils/convert.py` & `domolibrary-0.1.9/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.9/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary/utils/upload_data.py` & `domolibrary-0.1.9/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.9/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.8/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.9/domolibrary.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 domolibrary.egg-info/entry_points.txt
 domolibrary.egg-info/not-zip-safe
 domolibrary.egg-info/requires.txt
 domolibrary.egg-info/top_level.txt
 domolibrary/classes/DomoAccount.py
 domolibrary/classes/DomoActivityLog.py
 domolibrary/classes/DomoBootstrap.py
+domolibrary/classes/DomoCard.py
 domolibrary/classes/DomoDatacenter.py
 domolibrary/classes/DomoDataflow.py
 domolibrary/classes/DomoDataset.py
 domolibrary/classes/DomoGrant.py
 domolibrary/classes/DomoGroup.py
 domolibrary/classes/DomoInstanceConfig.py
 domolibrary/classes/DomoPDP.py
```

### Comparing `domolibrary-0.1.8/settings.ini` & `domolibrary-0.1.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.08
+version = 0.1.09
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.8/setup.py` & `domolibrary-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/Base.py` & `domolibrary-0.1.9/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/DictDot.py` & `domolibrary-0.1.9/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/Exceptions.py` & `domolibrary-0.1.9/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/LoggerClass.py` & `domolibrary-0.1.9/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/chunk_execution.py` & `domolibrary-0.1.9/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/consol_get_creds.py` & `domolibrary-0.1.9/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/convert.py` & `domolibrary-0.1.9/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.9/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.8/utils/upload_data.py` & `domolibrary-0.1.9/utils/upload_data.py`

 * *Files identical despite different names*

