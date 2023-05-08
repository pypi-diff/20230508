# Comparing `tmp/mojo_xmodules-0.0.8.tar.gz` & `tmp/mojo_xmodules-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_xmodules-0.0.8.tar", max compression
+gzip compressed data, was "mojo_xmodules-0.0.9.tar", max compression
```

## Comparing `mojo_xmodules-0.0.8.tar` & `mojo_xmodules-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1083 2023-03-16 20:43:00.880170 mojo_xmodules-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      135 2023-03-16 20:53:43.045371 mojo_xmodules-0.0.8/README.md
--rw-r--r--   0        0        0      725 2023-03-20 22:39:57.200465 mojo_xmodules-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-16 20:45:05.093185 mojo_xmodules-0.0.8/source/packages/mojo/xmods/__init__.py
--rw-r--r--   0        0        0     6162 2023-03-18 15:00:54.909241 mojo_xmodules-0.0.8/source/packages/mojo/xmods/aspects.py
--rw-r--r--   0        0        0        0 2023-03-18 20:58:12.680802 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/__init__.py
--rw-r--r--   0        0        0     1503 2023-03-19 22:38:23.146480 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/basecredential.py
--rw-r--r--   0        0        0     2832 2023-03-20 16:21:16.300965 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/basiccredential.py
--rw-r--r--   0        0        0     7798 2023-03-20 16:21:16.300965 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/credentialmanager.py
--rw-r--r--   0        0        0     4828 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/sshcredential.py
--rw-r--r--   0        0        0     2970 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/wifichoicecredential.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/__init__.py
--rw-r--r--   0        0        0      697 2023-03-20 17:24:31.549872 mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/enumerations.py
--rw-r--r--   0        0        0    11832 2023-03-17 22:42:20.249616 mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/eventedvariable.py
--rw-r--r--   0        0        0     8064 2023-03-20 20:02:21.844837 mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/eventedvariablesink.py
--rw-r--r--   0        0        0     7829 2023-03-20 22:39:03.060006 mojo_xmodules-0.0.8/source/packages/mojo/xmods/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-20 19:58:20.119208 mojo_xmodules-0.0.8/source/packages/mojo/xmods/extension/__init__.py
--rw-r--r--   0        0        0     5090 2023-03-20 22:13:52.339596 mojo_xmodules-0.0.8/source/packages/mojo/xmods/extension/configured.py
--rw-r--r--   0        0        0     5304 2023-03-20 20:01:40.496550 mojo_xmodules-0.0.8/source/packages/mojo/xmods/extension/dynamic.py
--rw-r--r--   0        0        0     4468 2023-03-20 22:24:29.116702 mojo_xmodules-0.0.8/source/packages/mojo/xmods/fspath.py
--rw-r--r--   0        0        0     2571 2023-03-19 21:11:58.020431 mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/icommandcontext.py
--rw-r--r--   0        0        0     1551 2023-03-18 15:00:54.917241 mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/iexcludefilter.py
--rw-r--r--   0        0        0     1544 2023-03-18 15:00:54.917241 mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/iincludefilter.py
--rw-r--r--   0        0        0        0 2023-03-18 15:50:52.156409 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/__init__.py
--rw-r--r--   0        0        0     7261 2023-03-20 20:03:03.445129 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coordinatorbase.py
--rw-r--r--   0        0        0        0 2023-03-18 15:51:11.564572 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/__init__.py
--rw-r--r--   0        0        0      770 2023-03-18 21:13:32.688424 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/basecoupling.py
--rw-r--r--   0        0        0     1494 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/coordinatorcoupling.py
--rw-r--r--   0        0        0     7519 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/integrationcoupling.py
--rw-r--r--   0        0        0     8144 2023-03-19 21:38:15.981754 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/scopecoupling.py
--rw-r--r--   0        0        0     1425 2023-03-20 22:13:21.763357 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/extensionpoints.py
--rw-r--r--   0        0        0     3345 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/friendlyidentifier.py
--rw-r--r--   0        0        0    14151 2023-03-20 19:25:02.203011 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscape.py
--rw-r--r--   0        0        0    11427 2023-03-20 22:11:06.874318 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscapedevice.py
--rw-r--r--   0        0        0     3567 2023-03-20 18:10:24.231781 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscapedeviceextension.py
--rw-r--r--   0        0        0      295 2023-03-20 19:21:05.317585 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscapeparameters.py
--rw-r--r--   0        0        0    11652 2023-03-20 21:54:55.871237 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeconfigurationlayer.py
--rw-r--r--   0        0        0     1601 2023-03-20 21:55:40.399635 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeinstallationlayer.py
--rw-r--r--   0        0        0      348 2023-03-20 18:12:27.367940 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeintegrationlayer.py
--rw-r--r--   0        0        0      412 2023-03-20 19:10:07.793241 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapelayerbase.py
--rw-r--r--   0        0        0      290 2023-03-20 18:12:36.927970 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeoperationallayer.py
--rw-r--r--   0        0        0       85 2023-03-20 18:24:47.698887 mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/topologyconfigurationlayer.py
--rw-r--r--   0        0        0     1930 2023-03-20 20:08:26.339472 mojo_xmodules-0.0.8/source/packages/mojo/xmods/wellknown/singletons.py
--rw-r--r--   0        0        0        0 2023-03-17 05:37:59.626173 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/__init__.py
--rw-r--r--   0        0        0     5971 2023-03-20 22:17:26.293286 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/caseinsensitivebytesdict.py
--rw-r--r--   0        0        0     5980 2023-03-20 22:17:32.737337 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/caseinsensitivestringdict.py
--rw-r--r--   0        0        0    15733 2023-03-19 23:37:46.320624 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/context.py
--rw-r--r--   0        0        0     1126 2023-03-17 05:31:09.177401 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/helpers.py
--rw-r--r--   0        0        0     4668 2023-03-20 22:19:33.314304 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/mergemap.py
--rw-r--r--   0        0        0     1239 2023-03-20 22:39:06.740037 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xconvert.py
--rwxr-xr-x   0        0        0     2157 2023-03-20 22:24:51.764886 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xdatetime.py
--rw-r--r--   0        0        0     5018 2023-03-20 22:27:30.618186 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xdebugger.py
--rw-r--r--   0        0        0     6559 2023-03-20 22:28:45.698802 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xfeature.py
--rw-r--r--   0        0        0     4655 2023-03-17 07:22:53.076604 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xformatting.py
--rw-r--r--   0        0        0     2220 2023-03-20 22:29:42.983273 mojo_xmodules-0.0.8/source/packages/mojo/xmods/ximport.py
--rw-r--r--   0        0        0     1986 2023-03-17 07:22:53.068604 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xinspect.py
--rw-r--r--   0        0        0        0 2023-03-17 05:04:01.183401 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/__init__.py
--rw-r--r--   0        0        0    23265 2023-03-17 22:42:42.417801 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/foundations.py
--rw-r--r--   0        0        0      955 2023-03-17 05:04:16.663773 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/levels.py
--rw-r--r--   0        0        0    10508 2023-03-19 21:35:49.832165 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/scopemonitoring.py
--rw-r--r--   0        0        0      544 2023-03-17 07:22:53.076604 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/__init__.py
--rw-r--r--   0        0        0     1632 2023-03-20 22:22:15.683616 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/lockscopes.py
--rw-r--r--   0        0        0     3274 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looper.py
--rw-r--r--   0        0        0     4913 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looperpool.py
--rw-r--r--   0        0        0     3549 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looperqueue.py
--rw-r--r--   0        0        0     5779 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/readwritelock.py
--rw-r--r--   0        0        0     1255 2023-03-20 22:31:33.404181 mojo_xmodules-0.0.8/source/packages/mojo/xmods/xyaml.py
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 mojo_xmodules-0.0.8/setup.py
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 mojo_xmodules-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-16 20:43:00.880170 mojo_xmodules-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      135 2023-03-16 20:53:43.045371 mojo_xmodules-0.0.9/README.md
+-rw-r--r--   0        0        0      664 2023-03-20 22:47:05.872078 mojo_xmodules-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-16 20:45:05.093185 mojo_xmodules-0.0.9/source/packages/mojo/xmods/__init__.py
+-rw-r--r--   0        0        0     6162 2023-03-18 15:00:54.909241 mojo_xmodules-0.0.9/source/packages/mojo/xmods/aspects.py
+-rw-r--r--   0        0        0        0 2023-03-18 20:58:12.680802 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/__init__.py
+-rw-r--r--   0        0        0     1503 2023-03-19 22:38:23.146480 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/basecredential.py
+-rw-r--r--   0        0        0     2832 2023-03-20 16:21:16.300965 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/basiccredential.py
+-rw-r--r--   0        0        0     7798 2023-03-20 16:21:16.300965 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/credentialmanager.py
+-rw-r--r--   0        0        0     4828 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/sshcredential.py
+-rw-r--r--   0        0        0     2970 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/wifichoicecredential.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.276698 mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/__init__.py
+-rw-r--r--   0        0        0      697 2023-03-20 17:24:31.549872 mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/enumerations.py
+-rw-r--r--   0        0        0    11832 2023-03-17 22:42:20.249616 mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/eventedvariable.py
+-rw-r--r--   0        0        0     8064 2023-03-20 20:02:21.844837 mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/eventedvariablesink.py
+-rw-r--r--   0        0        0     7829 2023-03-20 22:39:03.060006 mojo_xmodules-0.0.9/source/packages/mojo/xmods/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-20 19:58:20.119208 mojo_xmodules-0.0.9/source/packages/mojo/xmods/extension/__init__.py
+-rw-r--r--   0        0        0     5090 2023-03-20 22:13:52.339596 mojo_xmodules-0.0.9/source/packages/mojo/xmods/extension/configured.py
+-rw-r--r--   0        0        0     5304 2023-03-20 20:01:40.496550 mojo_xmodules-0.0.9/source/packages/mojo/xmods/extension/dynamic.py
+-rw-r--r--   0        0        0     4468 2023-03-20 22:24:29.116702 mojo_xmodules-0.0.9/source/packages/mojo/xmods/fspath.py
+-rw-r--r--   0        0        0     2571 2023-03-19 21:11:58.020431 mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/icommandcontext.py
+-rw-r--r--   0        0        0     1551 2023-03-18 15:00:54.917241 mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/iexcludefilter.py
+-rw-r--r--   0        0        0     1544 2023-03-18 15:00:54.917241 mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/iincludefilter.py
+-rw-r--r--   0        0        0        0 2023-03-18 15:50:52.156409 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/__init__.py
+-rw-r--r--   0        0        0     7261 2023-03-20 20:03:03.445129 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coordinatorbase.py
+-rw-r--r--   0        0        0        0 2023-03-18 15:51:11.564572 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/__init__.py
+-rw-r--r--   0        0        0      770 2023-03-18 21:13:32.688424 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/basecoupling.py
+-rw-r--r--   0        0        0     1494 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/coordinatorcoupling.py
+-rw-r--r--   0        0        0     7519 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/integrationcoupling.py
+-rw-r--r--   0        0        0     8144 2023-03-19 21:38:15.981754 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/scopecoupling.py
+-rw-r--r--   0        0        0     1425 2023-03-20 22:13:21.763357 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/extensionpoints.py
+-rw-r--r--   0        0        0     3345 2023-03-20 16:21:16.292966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/friendlyidentifier.py
+-rw-r--r--   0        0        0    14151 2023-03-20 19:25:02.203011 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscape.py
+-rw-r--r--   0        0        0    11427 2023-03-20 22:11:06.874318 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscapedevice.py
+-rw-r--r--   0        0        0     3567 2023-03-20 18:10:24.231781 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscapedeviceextension.py
+-rw-r--r--   0        0        0      295 2023-03-20 19:21:05.317585 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscapeparameters.py
+-rw-r--r--   0        0        0    11652 2023-03-20 21:54:55.871237 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeconfigurationlayer.py
+-rw-r--r--   0        0        0     1601 2023-03-20 21:55:40.399635 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeinstallationlayer.py
+-rw-r--r--   0        0        0      348 2023-03-20 18:12:27.367940 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeintegrationlayer.py
+-rw-r--r--   0        0        0      412 2023-03-20 19:10:07.793241 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapelayerbase.py
+-rw-r--r--   0        0        0      290 2023-03-20 18:12:36.927970 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeoperationallayer.py
+-rw-r--r--   0        0        0       85 2023-03-20 18:24:47.698887 mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/topologyconfigurationlayer.py
+-rw-r--r--   0        0        0     1930 2023-03-20 20:08:26.339472 mojo_xmodules-0.0.9/source/packages/mojo/xmods/wellknown/singletons.py
+-rw-r--r--   0        0        0        0 2023-03-17 05:37:59.626173 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/__init__.py
+-rw-r--r--   0        0        0     5971 2023-03-20 22:17:26.293286 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/caseinsensitivebytesdict.py
+-rw-r--r--   0        0        0     5980 2023-03-20 22:17:32.737337 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/caseinsensitivestringdict.py
+-rw-r--r--   0        0        0    15733 2023-03-19 23:37:46.320624 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/context.py
+-rw-r--r--   0        0        0     1126 2023-03-17 05:31:09.177401 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/helpers.py
+-rw-r--r--   0        0        0     4668 2023-03-20 22:19:33.314304 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/mergemap.py
+-rw-r--r--   0        0        0     1239 2023-03-20 22:39:06.740037 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xconvert.py
+-rwxr-xr-x   0        0        0     2157 2023-03-20 22:24:51.764886 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xdatetime.py
+-rw-r--r--   0        0        0     5018 2023-03-20 22:27:30.618186 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xdebugger.py
+-rw-r--r--   0        0        0     6559 2023-03-20 22:28:45.698802 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xfeature.py
+-rw-r--r--   0        0        0     4655 2023-03-17 07:22:53.076604 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xformatting.py
+-rw-r--r--   0        0        0     2220 2023-03-20 22:29:42.983273 mojo_xmodules-0.0.9/source/packages/mojo/xmods/ximport.py
+-rw-r--r--   0        0        0     1986 2023-03-17 07:22:53.068604 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xinspect.py
+-rw-r--r--   0        0        0        0 2023-03-17 05:04:01.183401 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/__init__.py
+-rw-r--r--   0        0        0    23265 2023-03-17 22:42:42.417801 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/foundations.py
+-rw-r--r--   0        0        0      955 2023-03-17 05:04:16.663773 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/levels.py
+-rw-r--r--   0        0        0    10508 2023-03-19 21:35:49.832165 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/scopemonitoring.py
+-rw-r--r--   0        0        0      544 2023-03-17 07:22:53.076604 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/__init__.py
+-rw-r--r--   0        0        0     1632 2023-03-20 22:22:15.683616 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/lockscopes.py
+-rw-r--r--   0        0        0     3274 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looper.py
+-rw-r--r--   0        0        0     4913 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looperpool.py
+-rw-r--r--   0        0        0     3549 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looperqueue.py
+-rw-r--r--   0        0        0     5779 2023-03-20 16:21:16.288966 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/readwritelock.py
+-rw-r--r--   0        0        0     1255 2023-03-20 22:31:33.404181 mojo_xmodules-0.0.9/source/packages/mojo/xmods/xyaml.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 mojo_xmodules-0.0.9/setup.py
+-rw-r--r--   0        0        0      856 1970-01-01 00:00:00.000000 mojo_xmodules-0.0.9/PKG-INFO
```

### Comparing `mojo_xmodules-0.0.8/LICENSE.txt` & `mojo_xmodules-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/pyproject.toml` & `mojo_xmodules-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-xmodules"
 description = "Automation Mojo X-Modules"
-version = "0.0.8"
+version = "0.0.9"
 authors = []
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
@@ -15,19 +15,16 @@
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 mojo-waiting = "^1.0.0"
 debugpy = "^1.6.6"
-netifaces = "^0.11.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
-[tool.poetry.group.dbio.dependencies]
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/aspects.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/aspects.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/basecredential.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/basecredential.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/basiccredential.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/basiccredential.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/credentialmanager.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/credentialmanager.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/sshcredential.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/sshcredential.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/credentials/wifichoicecredential.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/credentials/wifichoicecredential.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/enumerations.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/enumerations.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/eventedvariable.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/eventedvariable.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/eventing/eventedvariablesink.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/eventing/eventedvariablesink.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/exceptions.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/extension/configured.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/extension/configured.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/extension/dynamic.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/extension/dynamic.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/fspath.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/fspath.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/icommandcontext.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/icommandcontext.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/iexcludefilter.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/iexcludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/interfaces/iincludefilter.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/interfaces/iincludefilter.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coordinatorbase.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coordinatorbase.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/basecoupling.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/basecoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/coordinatorcoupling.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/coordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/integrationcoupling.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/integrationcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/coupling/scopecoupling.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/coupling/scopecoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/extensionpoints.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/extensionpoints.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/friendlyidentifier.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/friendlyidentifier.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscape.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscape.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscapedevice.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscapedevice.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/landscapedeviceextension.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/landscapedeviceextension.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeconfigurationlayer.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeconfigurationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/landscaping/layers/landscapeinstallationlayer.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/landscaping/layers/landscapeinstallationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/wellknown/singletons.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/wellknown/singletons.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/caseinsensitivebytesdict.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/caseinsensitivebytesdict.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/caseinsensitivestringdict.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/caseinsensitivestringdict.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/context.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/context.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/helpers.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/helpers.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xcollections/mergemap.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xcollections/mergemap.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xconvert.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xconvert.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xdatetime.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xdatetime.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xdebugger.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xdebugger.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xfeature.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xfeature.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xformatting.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xformatting.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/ximport.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/ximport.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xinspect.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xinspect.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/foundations.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/foundations.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/levels.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/levels.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xlogging/scopemonitoring.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xlogging/scopemonitoring.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/__init__.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/lockscopes.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/lockscopes.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looper.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looper.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looperpool.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looperpool.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/looperqueue.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/looperqueue.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xthreading/readwritelock.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xthreading/readwritelock.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/source/packages/mojo/xmods/xyaml.py` & `mojo_xmodules-0.0.9/source/packages/mojo/xmods/xyaml.py`

 * *Files identical despite different names*

### Comparing `mojo_xmodules-0.0.8/setup.py` & `mojo_xmodules-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,21 +19,19 @@
  'mojo.xmods.xlogging',
  'mojo.xmods.xthreading']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['debugpy>=1.6.6,<2.0.0',
- 'mojo-waiting>=1.0.0,<2.0.0',
- 'netifaces>=0.11.0,<0.12.0']
+['debugpy>=1.6.6,<2.0.0', 'mojo-waiting>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'mojo-xmodules',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Automation Mojo X-Modules',
     'long_description': '# Automation Mojo X-Modules (mojo-xmodules)\nThis package contains helper modules that extend the function of standard python modules.\n\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_xmodules-0.0.8/PKG-INFO` & `mojo_xmodules-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-xmodules
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation Mojo X-Modules
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
@@ -12,14 +12,13 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: debugpy (>=1.6.6,<2.0.0)
 Requires-Dist: mojo-waiting (>=1.0.0,<2.0.0)
-Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Automation Mojo X-Modules (mojo-xmodules)
 This package contains helper modules that extend the function of standard python modules.
```

