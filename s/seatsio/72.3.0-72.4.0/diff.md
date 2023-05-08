# Comparing `tmp/seatsio-72.3.0.tar.gz` & `tmp/seatsio-72.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatsio-72.3.0.tar", last modified: Mon Mar 20 08:35:01 2023, max compression
+gzip compressed data, was "seatsio-72.4.0.tar", last modified: Mon May  8 11:12:59 2023, max compression
```

## Comparing `seatsio-72.3.0.tar` & `seatsio-72.4.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-20 08:34:47.000000 seatsio-72.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 08:34:47.000000 seatsio-72.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-03-20 08:35:01.568930 seatsio-72.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-03-20 08:34:47.000000 seatsio-72.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.564930 seatsio-72.3.0/seatsio/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.564930 seatsio-72.3.0/seatsio/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/charts/chartsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/charts/chartsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/charts/socialDistancingRulesetsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/changeObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/channelProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/channelsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/channelsRequests.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/createMultipleEventsRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/createSingleEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/eventProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/eventsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/extraDataRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/forSaleRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/objectProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/events/statusChangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/holdtokens/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/holdtokens/HoldTokenClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/holdtokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/httpClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/listableObjectsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/lister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/pageFetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/pagination/pagedIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/charts/chartReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/reports/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/events/eventReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/reports/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/reports/usage/usageReports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/seasons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/seasons/seasonsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/subaccounts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/subaccounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/subaccounts/subaccountsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.568930 seatsio-72.3.0/seatsio/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/workspaces/UpdateWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/workspaces/createWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-20 08:34:47.000000 seatsio-72.3.0/seatsio/workspaces/workspacesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 08:35:01.564930 seatsio-72.3.0/seatsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-03-20 08:35:01.000000 seatsio-72.3.0/seatsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-20 08:35:01.000000 seatsio-72.3.0/seatsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 08:35:01.000000 seatsio-72.3.0/seatsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-20 08:35:01.000000 seatsio-72.3.0/seatsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-20 08:35:01.000000 seatsio-72.3.0/seatsio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 08:35:01.568930 seatsio-72.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-20 08:34:57.000000 seatsio-72.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 11:12:52.000000 seatsio-72.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 11:12:52.000000 seatsio-72.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-08 11:12:59.033161 seatsio-72.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-08 11:12:52.000000 seatsio-72.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/chartsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/chartsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/charts/socialDistancingRulesetsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/changeObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/channelsRequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/createMultipleEventsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/createSingleEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/eventProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/eventsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/extraDataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/forSaleRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/objectProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/events/statusChangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/holdtokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/holdtokens/HoldTokenClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/holdtokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/httpClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/listableObjectsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/lister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/pageFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/pagination/pagedIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/charts/chartReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/events/eventReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/reports/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/reports/usage/usageReports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/seasons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/seasons/seasonsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/subaccounts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/subaccounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/subaccounts/subaccountsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.033161 seatsio-72.4.0/seatsio/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/UpdateWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/createWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 11:12:52.000000 seatsio-72.4.0/seatsio/workspaces/workspacesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:12:59.029161 seatsio-72.4.0/seatsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-08 11:12:59.000000 seatsio-72.4.0/seatsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 11:12:58.000000 seatsio-72.4.0/seatsio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:12:59.033161 seatsio-72.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-08 11:12:55.000000 seatsio-72.4.0/setup.py
```

### Comparing `seatsio-72.3.0/LICENSE` & `seatsio-72.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/PKG-INFO` & `seatsio-72.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 72.3.0
+Version: 72.4.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-72.3.0/README.md` & `seatsio-72.4.0/README.md`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/charts/chartsClient.py` & `seatsio-72.4.0/seatsio/charts/chartsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/charts/socialDistancingRulesetsRequest.py` & `seatsio-72.4.0/seatsio/charts/socialDistancingRulesetsRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/client.py` & `seatsio-72.4.0/seatsio/client.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/domain.py` & `seatsio-72.4.0/seatsio/domain.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/changeBestAvailableObjectStatusRequest.py` & `seatsio-72.4.0/seatsio/events/changeBestAvailableObjectStatusRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 class ChangeBestAvailableObjectStatusRequest:
-    def __init__(self, number, categories, extra_data, ticket_types, status, hold_token, order_id, keep_extra_data, ignore_channels, channel_keys):
+    def __init__(self, number, categories, extra_data, ticket_types, status, hold_token, order_id, keep_extra_data, ignore_channels, channel_keys, try_to_prevent_orphan_seats):
         best_available = {"number": number}
         if categories:
             best_available["categories"] = categories
         if extra_data:
             best_available["extraData"] = extra_data
         if ticket_types:
             best_available["ticketTypes"] = ticket_types
+        if try_to_prevent_orphan_seats is not None:
+            best_available["tryToPreventOrphanSeats"] = try_to_prevent_orphan_seats
         self.bestAvailable = best_available
         self.status = status
         if hold_token:
             self.holdToken = hold_token
         if order_id:
             self.orderId = order_id
         if keep_extra_data is not None:
```

### Comparing `seatsio-72.3.0/seatsio/events/changeObjectStatusRequest.py` & `seatsio-72.4.0/seatsio/events/changeObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/channelsClient.py` & `seatsio-72.4.0/seatsio/events/channelsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/channelsRequests.py` & `seatsio-72.4.0/seatsio/events/channelsRequests.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/createSingleEventRequest.py` & `seatsio-72.4.0/seatsio/events/createSingleEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/eventProperties.py` & `seatsio-72.4.0/seatsio/events/eventProperties.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/events/eventsClient.py` & `seatsio-72.4.0/seatsio/events/eventsClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
              ignore_channels=None, channel_keys=None, ignore_social_distancing=None):
         return self.change_object_status(event_key_or_keys, object_or_objects, EventObjectInfo.BOOKED, hold_token,
                                          order_id, keep_extra_data, ignore_channels, channel_keys,
                                          ignore_social_distancing)
 
     def book_best_available(self, event_key, number, categories=None, hold_token=None, extra_data=None,
                             ticket_types=None, order_id=None, keep_extra_data=None, ignore_channels=None,
-                            channel_keys=None):
+                            channel_keys=None, try_to_prevent_orphan_seats=None):
         return self.change_best_available_object_status(
             event_key,
             number,
             EventObjectInfo.BOOKED,
             categories,
             hold_token,
             extra_data,
@@ -97,35 +97,36 @@
             keep_extra_data,
             ignore_channels,
             channel_keys
         )
 
     def hold_best_available(self, event_key, number, categories=None, hold_token=None, extra_data=None,
                             ticket_types=None, order_id=None, keep_extra_data=None, ignore_channels=None,
-                            channel_keys=None):
+                            channel_keys=None, try_to_prevent_orphan_seats=None):
         return self.change_best_available_object_status(
             event_key,
             number,
             EventObjectInfo.HELD,
             categories,
             hold_token,
             extra_data,
             ticket_types,
             order_id,
             keep_extra_data,
             ignore_channels,
-            channel_keys
+            channel_keys,
+            try_to_prevent_orphan_seats
         )
 
     def change_best_available_object_status(self, event_key, number, status, categories=None, hold_token=None,
                                             extra_data=None, ticket_types=None, order_id=None, keep_extra_data=None,
-                                            ignore_channels=None, channel_keys=None):
+                                            ignore_channels=None, channel_keys=None, try_to_prevent_orphan_seats=None):
         response = self.http_client.url("/events/{key}/actions/change-object-status", key=event_key).post(
             ChangeBestAvailableObjectStatusRequest(number, categories, extra_data, ticket_types, status, hold_token,
-                                                   order_id, keep_extra_data, ignore_channels, channel_keys))
+                                                   order_id, keep_extra_data, ignore_channels, channel_keys, try_to_prevent_orphan_seats))
         return BestAvailableObjects(response.json())
 
     def release(self, event_key_or_keys, object_or_objects, hold_token=None, order_id=None, keep_extra_data=None,
                 ignore_channels=None, channel_keys=None):
         return self.change_object_status(event_key_or_keys, object_or_objects, EventObjectInfo.FREE, hold_token,
                                          order_id, keep_extra_data, ignore_channels, channel_keys)
```

### Comparing `seatsio-72.3.0/seatsio/events/statusChangeRequest.py` & `seatsio-72.4.0/seatsio/events/statusChangeRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/exceptions.py` & `seatsio-72.4.0/seatsio/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/holdtokens/HoldTokenClient.py` & `seatsio-72.4.0/seatsio/holdtokens/HoldTokenClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/httpClient.py` & `seatsio-72.4.0/seatsio/httpClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/pagination/listableObjectsClient.py` & `seatsio-72.4.0/seatsio/pagination/listableObjectsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/pagination/lister.py` & `seatsio-72.4.0/seatsio/pagination/lister.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/pagination/page.py` & `seatsio-72.4.0/seatsio/pagination/page.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/pagination/pageFetcher.py` & `seatsio-72.4.0/seatsio/pagination/pageFetcher.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/pagination/pagedIterator.py` & `seatsio-72.4.0/seatsio/pagination/pagedIterator.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/reports/charts/chartReports.py` & `seatsio-72.4.0/seatsio/reports/charts/chartReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/reports/events/eventReports.py` & `seatsio-72.4.0/seatsio/reports/events/eventReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/reports/usage/usageReports.py` & `seatsio-72.4.0/seatsio/reports/usage/usageReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/seasons/seasonsClient.py` & `seatsio-72.4.0/seatsio/seasons/seasonsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/subaccounts/subaccountsClient.py` & `seatsio-72.4.0/seatsio/subaccounts/subaccountsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio/workspaces/workspacesClient.py` & `seatsio-72.4.0/seatsio/workspaces/workspacesClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/seatsio.egg-info/PKG-INFO` & `seatsio-72.4.0/seatsio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 72.3.0
+Version: 72.4.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-72.3.0/seatsio.egg-info/SOURCES.txt` & `seatsio-72.4.0/seatsio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatsio-72.3.0/setup.py` & `seatsio-72.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='seatsio',
-    version='v72.3.0',
+    version='v72.4.0',
     description='The official Seats.io Python client library',
     author='The seats.io dev team',
     author_email='hello@seats.io',
     url='https://github.com/seatsio/seatsio-python',
     license="MIT",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

