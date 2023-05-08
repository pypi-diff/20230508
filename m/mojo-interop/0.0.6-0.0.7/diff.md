# Comparing `tmp/mojo_interop-0.0.6.tar.gz` & `tmp/mojo_interop-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_interop-0.0.6.tar", max compression
+gzip compressed data, was "mojo_interop-0.0.7.tar", max compression
```

## Comparing `mojo_interop-0.0.6.tar` & `mojo_interop-0.0.7.tar`

### file list

```diff
@@ -1,284 +1,284 @@
--rw-r--r--   0        0        0     1083 2023-04-30 20:18:46.226836 mojo_interop-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      434 2023-04-30 21:10:35.023558 mojo_interop-0.0.6/README.rst
--rw-r--r--   0        0        0      738 2023-05-07 10:50:37.794700 mojo_interop-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1630 2023-04-30 20:54:05.542332 mojo_interop-0.0.6/source/packages/mojo/factories/xmodsfactory.py
--rw-r--r--   0        0        0      180 2023-04-23 00:21:47.238814 mojo_interop-0.0.6/source/packages/mojo/interop/clients/constants.py
--rw-r--r--   0        0        0        0 2023-04-26 04:50:59.262714 mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/__init__.py
--rw-r--r--   0        0        0      634 2023-05-06 19:38:19.555362 mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclient.py
--rw-r--r--   0        0        0     1412 2023-05-06 19:38:34.671483 mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
--rw-r--r--   0        0        0     1289 2023-05-06 19:53:48.915347 mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-04-21 02:40:59.664563 mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/__init__.py
--rw-r--r--   0        0        0      633 2023-05-06 19:40:03.716205 mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclient.py
--rw-r--r--   0        0        0     1388 2023-05-06 19:41:35.468963 mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
--rw-r--r--   0        0        0     1271 2023-05-06 19:53:59.927446 mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-04-26 04:43:08.306443 mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/__init__.py
--rw-r--r--   0        0        0      637 2023-05-06 19:40:17.036314 mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclient.py
--rw-r--r--   0        0        0     1436 2023-05-06 19:41:59.749166 mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
--rw-r--r--   0        0        0     1307 2023-05-06 19:54:10.971544 mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
--rw-r--r--   0        0        0        0 2023-05-06 19:44:21.610368 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/__init__.py
--rw-r--r--   0        0        0       69 2023-05-06 21:03:43.255179 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/constants.py
--rw-r--r--   0        0        0      510 2023-05-07 00:29:56.495970 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/picluster.py
--rw-r--r--   0        0        0      624 2023-05-06 19:48:13.812380 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinode.py
--rw-r--r--   0        0        0     1529 2023-05-06 21:01:52.014567 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py
--rw-r--r--   0        0        0     1314 2023-05-07 00:29:20.295618 mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py
--rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-30 21:03:13.691162 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsaddress.py
--rw-r--r--   0        0        0      639 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsapi.py
--rw-r--r--   0        0        0     9720 2023-03-17 03:47:56.259994 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsconst.py
--rw-r--r--   0        0        0     2121 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
--rw-r--r--   0        0        0     9274 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
--rw-r--r--   0        0        0    15537 2023-04-30 21:03:11.223140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
--rw-r--r--   0        0        0     1862 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnspointer.py
--rw-r--r--   0        0        0     2250 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsquestion.py
--rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
--rw-r--r--   0        0        0     6850 2023-04-30 21:03:11.223140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsrecord.py
--rw-r--r--   0        0        0     3606 2023-04-30 21:03:11.223140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsserver.py
--rw-r--r--   0        0        0     2719 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsservice.py
--rw-r--r--   0        0        0     2004 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnstext.py
--rw-r--r--   0        0        0     3750 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsutil.py
--rw-r--r--   0        0        0     2807 2023-04-30 21:03:11.207140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
--rw-r--r--   0        0        0     1052 2023-03-17 15:51:43.102472 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/exceptions.py
--rw-r--r--   0        0        0     2615 2023-04-30 21:03:11.223140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsagent.py
--rw-r--r--   0        0        0     6279 2023-04-30 21:03:11.223140 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
--rw-r--r--   0        0        0     2505 2023-03-17 06:36:21.314128 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
--rw-r--r--   0        0        0     1294 2023-03-16 22:12:31.133035 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/testmessages.py
--rw-r--r--   0        0        0        0 2023-03-25 19:42:09.132533 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
--rw-r--r--   0        0        0      894 2023-03-28 16:14:15.598469 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
--rw-r--r--   0        0        0     3767 2023-03-28 16:14:15.598469 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
--rw-r--r--   0        0        0     6138 2023-04-29 04:47:55.337890 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
--rw-r--r--   0        0        0     7794 2023-03-25 18:55:12.050499 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
--rw-r--r--   0        0        0     4913 2023-04-29 04:47:55.329891 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
--rw-r--r--   0        0        0     6059 2023-04-29 04:47:55.333891 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
--rw-r--r--   0        0        0     1398 2023-04-29 04:47:55.321890 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
--rw-r--r--   0        0        0        0 2023-03-24 06:52:51.435618 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/__init__.py
--rw-r--r--   0        0        0    70641 2023-03-28 16:14:15.598469 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshagent.py
--rw-r--r--   0        0        0    12109 2023-04-29 04:47:55.353891 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
--rw-r--r--   0        0        0     7541 2023-04-29 04:47:55.349891 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
--rw-r--r--   0        0        0     1255 2023-04-29 04:47:55.353891 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshdevice.py
--rw-r--r--   0        0        0      540 2023-03-20 16:55:58.998382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/__init__.py
--rw-r--r--   0        0        0      319 2023-03-20 16:55:58.990382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/aliases.py
--rw-r--r--   0        0        0     2431 2023-03-21 07:47:58.411623 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/content/__init__.py
--rw-r--r--   0        0        0    15564 2023-03-21 07:49:16.837478 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/content/didllite.py
--rw-r--r--   0        0        0      557 2023-03-20 16:55:59.002382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
--rw-r--r--   0        0        0    14091 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
--rw-r--r--   0        0        0     1761 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
--rw-r--r--   0        0        0    44978 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
--rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
--rw-r--r--   0        0        0     3512 2023-04-30 20:52:11.401306 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
--rw-r--r--   0        0        0     6222 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    11201 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
--rw-r--r--   0        0        0    11596 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
--rw-r--r--   0        0        0    14933 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
--rw-r--r--   0        0        0    20201 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
--rw-r--r--   0        0        0    13583 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
--rw-r--r--   0        0        0    16776 2023-04-30 20:52:11.589308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
--rw-r--r--   0        0        0     6120 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
--rw-r--r--   0        0        0    12568 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
--rw-r--r--   0        0        0    17020 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4574 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
--rw-r--r--   0        0        0      630 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
--rw-r--r--   0        0        0     4109 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
--rw-r--r--   0        0        0    11330 2023-04-30 20:52:11.049303 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
--rw-r--r--   0        0        0    12948 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
--rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
--rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.589308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
--rw-r--r--   0        0        0     5719 2023-04-30 20:52:11.513307 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
--rw-r--r--   0        0        0     9453 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
--rw-r--r--   0        0        0    11449 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
--rw-r--r--   0        0        0    13534 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
--rw-r--r--   0        0        0    23744 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
--rw-r--r--   0        0        0     4429 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
--rw-r--r--   0        0        0     7462 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
--rw-r--r--   0        0        0    10870 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
--rw-r--r--   0        0        0     7731 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
--rw-r--r--   0        0        0     8828 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
--rw-r--r--   0        0        0    10006 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
--rw-r--r--   0        0        0     2043 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
--rw-r--r--   0        0        0     3992 2023-04-30 20:52:10.993303 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
--rw-r--r--   0        0        0     4959 2023-04-30 20:52:11.573308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
--rw-r--r--   0        0        0     3828 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
--rw-r--r--   0        0        0     3166 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     2039 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
--rw-r--r--   0        0        0     3577 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
--rw-r--r--   0        0        0     3071 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
--rw-r--r--   0        0        0     4686 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
--rw-r--r--   0        0        0     9951 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
--rw-r--r--   0        0        0     1782 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
--rw-r--r--   0        0        0     8071 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
--rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
--rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
--rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
--rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
--rw-r--r--   0        0        0     4675 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
--rw-r--r--   0        0        0     5801 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
--rw-r--r--   0        0        0    11116 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
--rw-r--r--   0        0        0     1691 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
--rw-r--r--   0        0        0     3288 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
--rw-r--r--   0        0        0     2107 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
--rw-r--r--   0        0        0     2712 2023-04-30 20:52:11.189304 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
--rw-r--r--   0        0        0     4718 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
--rw-r--r--   0        0        0     5214 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
--rw-r--r--   0        0        0     5733 2023-04-30 20:52:11.321306 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
--rw-r--r--   0        0        0     1751 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
--rw-r--r--   0        0        0    20947 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
--rw-r--r--   0        0        0    22560 2023-04-30 20:52:11.293305 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
--rw-r--r--   0        0        0    26952 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
--rw-r--r--   0        0        0     7336 2023-04-30 20:52:11.261305 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
--rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
--rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
--rw-r--r--   0        0        0     9804 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
--rw-r--r--   0        0        0    10325 2023-04-30 20:52:11.629308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
--rw-r--r--   0        0        0     2199 2023-04-30 20:52:11.157304 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
--rw-r--r--   0        0        0     3257 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
--rw-r--r--   0        0        0     4234 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
--rw-r--r--   0        0        0     7786 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     8132 2023-04-30 20:52:11.597308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
--rw-r--r--   0        0        0     6178 2023-04-30 20:52:11.081303 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
--rw-r--r--   0        0        0     1351 2023-04-30 20:52:11.217305 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    12414 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
--rw-r--r--   0        0        0    15214 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
--rw-r--r--   0        0        0     5133 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
--rw-r--r--   0        0        0     6600 2023-04-30 20:52:11.657309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
--rw-r--r--   0        0        0    17131 2023-04-30 20:52:11.601308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
--rw-r--r--   0        0        0    30991 2023-04-30 20:52:11.633308 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
--rw-r--r--   0        0        0      479 2023-03-20 16:55:59.002382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
--rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
--rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
--rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
--rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
--rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
--rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
--rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
--rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
--rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
--rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
--rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
--rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
--rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
--rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
--rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
--rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
--rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
--rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
--rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
--rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
--rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
--rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
--rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
--rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
--rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
--rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
--rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
--rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
--rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
--rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
--rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
--rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
--rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
--rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
--rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
--rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
--rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
--rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
--rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
--rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
--rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
--rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
--rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
--rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
--rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
--rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
--rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
--rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
--rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
--rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
--rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
--rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
--rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
--rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
--rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
--rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
--rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
--rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
--rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
--rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
--rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
--rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
--rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
--rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
--rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
--rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
--rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
--rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
--rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
--rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
--rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
--rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
--rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
--rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
--rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
--rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
--rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
--rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
--rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
--rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
--rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
--rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
--rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
--rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
--rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
--rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
--rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
--rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
--rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
--rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
--rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
--rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
--rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
--rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
--rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
--rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
--rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
--rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
--rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
--rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
--rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
--rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
--rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
--rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
--rw-r--r--   0        0        0    16858 2023-04-30 20:52:10.965302 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
--rw-r--r--   0        0        0     2631 2023-03-20 16:55:58.994382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/paths.py
--rw-r--r--   0        0        0      481 2023-03-20 16:55:59.002382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/services/__init__.py
--rw-r--r--   0        0        0     5518 2023-03-21 07:56:39.142504 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
--rw-r--r--   0        0        0    26076 2023-04-30 20:52:11.669309 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
--rw-r--r--   0        0        0    11691 2023-04-30 20:52:10.937302 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/soap.py
--rw-r--r--   0        0        0      943 2023-04-30 20:52:10.853301 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
--rw-r--r--   0        0        0    55895 2023-04-30 20:52:13.489325 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
--rw-r--r--   0        0        0     7480 2023-04-30 21:01:15.502130 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
--rw-r--r--   0        0        0     2628 2023-03-21 08:17:25.473613 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnperrors.py
--rw-r--r--   0        0        0    11109 2023-04-30 20:52:10.881301 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
--rw-r--r--   0        0        0    21613 2023-03-21 08:16:35.890071 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
--rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
--rw-r--r--   0        0        0    20710 2023-03-21 08:11:33.022274 mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
--rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 mojo_interop-0.0.6/setup.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 mojo_interop-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-30 20:18:46.226836 mojo_interop-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      434 2023-04-30 21:10:35.023558 mojo_interop-0.0.7/README.rst
+-rw-r--r--   0        0        0      738 2023-05-08 14:26:12.912076 mojo_interop-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1630 2023-04-30 20:54:05.542332 mojo_interop-0.0.7/source/packages/mojo/factories/xmodsfactory.py
+-rw-r--r--   0        0        0      180 2023-04-23 00:21:47.238814 mojo_interop-0.0.7/source/packages/mojo/interop/clients/constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 04:50:59.262714 mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-06 19:38:19.555362 mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclient.py
+-rw-r--r--   0        0        0     1412 2023-05-06 19:38:34.671483 mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py
+-rw-r--r--   0        0        0     1289 2023-05-06 19:53:48.915347 mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-04-21 02:40:59.664563 mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-06 19:40:03.716205 mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclient.py
+-rw-r--r--   0        0        0     1388 2023-05-06 19:41:35.468963 mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py
+-rw-r--r--   0        0        0     1271 2023-05-06 19:53:59.927446 mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-04-26 04:43:08.306443 mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-06 19:40:17.036314 mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclient.py
+-rw-r--r--   0        0        0     1436 2023-05-06 19:41:59.749166 mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py
+-rw-r--r--   0        0        0     1307 2023-05-06 19:54:10.971544 mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:44:21.610368 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-06 21:03:43.255179 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/constants.py
+-rw-r--r--   0        0        0      510 2023-05-07 00:29:56.495970 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/picluster.py
+-rw-r--r--   0        0        0      624 2023-05-06 19:48:13.812380 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinode.py
+-rw-r--r--   0        0        0     1529 2023-05-06 21:01:52.014567 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py
+-rw-r--r--   0        0        0     1314 2023-05-07 00:29:20.295618 mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py
+-rw-r--r--   0        0        0      519 2022-12-08 19:53:16.276698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-30 21:03:13.691162 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsaddress.py
+-rw-r--r--   0        0        0      639 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsapi.py
+-rw-r--r--   0        0        0     9720 2023-03-17 03:47:56.259994 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsconst.py
+-rw-r--r--   0        0        0     2121 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnshostinfo.py
+-rw-r--r--   0        0        0     9274 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py
+-rw-r--r--   0        0        0    15537 2023-04-30 21:03:11.223140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py
+-rw-r--r--   0        0        0     1862 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnspointer.py
+-rw-r--r--   0        0        0     2250 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsquestion.py
+-rw-r--r--   0        0        0      832 2023-03-16 05:21:20.896073 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py
+-rw-r--r--   0        0        0     6850 2023-04-30 21:03:11.223140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsrecord.py
+-rw-r--r--   0        0        0     3606 2023-04-30 21:03:11.223140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsserver.py
+-rw-r--r--   0        0        0     2719 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsservice.py
+-rw-r--r--   0        0        0     2004 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnstext.py
+-rw-r--r--   0        0        0     3750 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsutil.py
+-rw-r--r--   0        0        0     2807 2023-04-30 21:03:11.207140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsvalidation.py
+-rw-r--r--   0        0        0     1052 2023-03-17 15:51:43.102472 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/exceptions.py
+-rw-r--r--   0        0        0     2615 2023-04-30 21:03:11.223140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsagent.py
+-rw-r--r--   0        0        0     6279 2023-04-30 21:03:11.223140 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py
+-rw-r--r--   0        0        0     2505 2023-03-17 06:36:21.314128 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py
+-rw-r--r--   0        0        0     1294 2023-03-16 22:12:31.133035 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/testmessages.py
+-rw-r--r--   0        0        0        0 2023-03-25 19:42:09.132533 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/__init__.py
+-rw-r--r--   0        0        0      894 2023-03-28 16:14:15.598469 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py
+-rw-r--r--   0        0        0     3767 2023-03-28 16:14:15.598469 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py
+-rw-r--r--   0        0        0     6137 2023-05-08 14:25:39.941564 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py
+-rw-r--r--   0        0        0     7794 2023-03-25 18:55:12.050499 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialagent.py
+-rw-r--r--   0        0        0     4913 2023-04-29 04:47:55.329891 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py
+-rw-r--r--   0        0        0     6058 2023-05-08 14:25:39.941564 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1398 2023-04-29 04:47:55.321890 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py
+-rw-r--r--   0        0        0        0 2023-03-24 06:52:51.435618 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/__init__.py
+-rw-r--r--   0        0        0    70641 2023-03-28 16:14:15.598469 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshagent.py
+-rw-r--r--   0        0        0    12109 2023-04-29 04:47:55.353891 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py
+-rw-r--r--   0        0        0     7540 2023-05-08 14:25:39.937564 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py
+-rw-r--r--   0        0        0     1255 2023-04-29 04:47:55.353891 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshdevice.py
+-rw-r--r--   0        0        0      540 2023-03-20 16:55:58.998382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/__init__.py
+-rw-r--r--   0        0        0      319 2023-03-20 16:55:58.990382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/aliases.py
+-rw-r--r--   0        0        0     2431 2023-03-21 07:47:58.411623 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/content/__init__.py
+-rw-r--r--   0        0        0    15564 2023-03-21 07:49:16.837478 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/content/didllite.py
+-rw-r--r--   0        0        0      557 2023-03-20 16:55:59.002382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/__init__.py
+-rw-r--r--   0        0        0    14091 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py
+-rw-r--r--   0        0        0     1761 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py
+-rw-r--r--   0        0        0    44978 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py
+-rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/dynamic/services/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/embeddeddevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.280698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/rootdevices/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/__init__.py
+-rw-r--r--   0        0        0     3512 2023-04-30 20:52:11.401306 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py
+-rw-r--r--   0        0        0     6222 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    11201 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0    11596 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py
+-rw-r--r--   0        0        0    14933 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py
+-rw-r--r--   0        0        0    20201 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py
+-rw-r--r--   0        0        0    13583 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    16776 2023-04-30 20:52:11.589308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     6120 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py
+-rw-r--r--   0        0        0    12568 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    17020 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4574 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py
+-rw-r--r--   0        0        0      630 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py
+-rw-r--r--   0        0        0     4109 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py
+-rw-r--r--   0        0        0    11330 2023-04-30 20:52:11.049303 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py
+-rw-r--r--   0        0        0    12948 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py
+-rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py
+-rw-r--r--   0        0        0     4161 2023-04-30 20:52:11.589308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py
+-rw-r--r--   0        0        0     5719 2023-04-30 20:52:11.513307 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py
+-rw-r--r--   0        0        0     9453 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py
+-rw-r--r--   0        0        0    11449 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py
+-rw-r--r--   0        0        0    13534 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py
+-rw-r--r--   0        0        0    23744 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py
+-rw-r--r--   0        0        0     4429 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py
+-rw-r--r--   0        0        0     7462 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py
+-rw-r--r--   0        0        0    10870 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py
+-rw-r--r--   0        0        0     7731 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py
+-rw-r--r--   0        0        0     8828 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py
+-rw-r--r--   0        0        0    10006 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py
+-rw-r--r--   0        0        0     2043 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py
+-rw-r--r--   0        0        0     3992 2023-04-30 20:52:10.993303 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py
+-rw-r--r--   0        0        0     4959 2023-04-30 20:52:11.573308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py
+-rw-r--r--   0        0        0     3828 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py
+-rw-r--r--   0        0        0     3166 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     2039 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py
+-rw-r--r--   0        0        0     3577 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py
+-rw-r--r--   0        0        0     3071 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py
+-rw-r--r--   0        0        0     4686 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py
+-rw-r--r--   0        0        0     9951 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py
+-rw-r--r--   0        0        0     1782 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py
+-rw-r--r--   0        0        0     8071 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py
+-rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py
+-rw-r--r--   0        0        0     3931 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py
+-rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py
+-rw-r--r--   0        0        0    10240 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py
+-rw-r--r--   0        0        0     4675 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py
+-rw-r--r--   0        0        0     5801 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py
+-rw-r--r--   0        0        0    11116 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py
+-rw-r--r--   0        0        0     1691 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py
+-rw-r--r--   0        0        0     3288 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py
+-rw-r--r--   0        0        0     2107 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py
+-rw-r--r--   0        0        0     2712 2023-04-30 20:52:11.189304 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py
+-rw-r--r--   0        0        0     4718 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py
+-rw-r--r--   0        0        0     5214 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py
+-rw-r--r--   0        0        0     5733 2023-04-30 20:52:11.321306 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py
+-rw-r--r--   0        0        0     1751 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py
+-rw-r--r--   0        0        0    20947 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py
+-rw-r--r--   0        0        0    22560 2023-04-30 20:52:11.293305 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py
+-rw-r--r--   0        0        0    26952 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py
+-rw-r--r--   0        0        0     7336 2023-04-30 20:52:11.261305 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py
+-rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py
+-rw-r--r--   0        0        0    11158 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py
+-rw-r--r--   0        0        0     9804 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py
+-rw-r--r--   0        0        0    10325 2023-04-30 20:52:11.629308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py
+-rw-r--r--   0        0        0     2199 2023-04-30 20:52:11.157304 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py
+-rw-r--r--   0        0        0     3257 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py
+-rw-r--r--   0        0        0     4234 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py
+-rw-r--r--   0        0        0     7786 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     8132 2023-04-30 20:52:11.597308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py
+-rw-r--r--   0        0        0     6178 2023-04-30 20:52:11.081303 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0     1351 2023-04-30 20:52:11.217305 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    12414 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py
+-rw-r--r--   0        0        0    15214 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py
+-rw-r--r--   0        0        0     5133 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py
+-rw-r--r--   0        0        0     6600 2023-04-30 20:52:11.657309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py
+-rw-r--r--   0        0        0    17131 2023-04-30 20:52:11.601308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py
+-rw-r--r--   0        0        0    30991 2023-04-30 20:52:11.633308 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/__init__.py
+-rw-r--r--   0        0        0      479 2023-03-20 16:55:59.002382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.284698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/dynamic/__init__.py
+-rw-r--r--   0        0        0      247 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:BinaryLight:1.xml
+-rw-r--r--   0        0        0      280 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DigitalSecurityCamera:1.xml
+-rw-r--r--   0        0        0      420 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:DimmableLight:1.xml
+-rw-r--r--   0        0        0     1159 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml
+-rw-r--r--   0        0        0     1865 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml
+-rw-r--r--   0        0        0      459 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:1.xml
+-rw-r--r--   0        0        0      604 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml
+-rw-r--r--   0        0        0      208 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:LANDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:1.xml
+-rw-r--r--   0        0        0      408 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ManageableDevice:2.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml
+-rw-r--r--   0        0        0      999 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml
+-rw-r--r--   0        0        0      580 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml
+-rw-r--r--   0        0        0     1170 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Printer:1.xml
+-rw-r--r--   0        0        0      187 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAClient:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:1.xml
+-rw-r--r--   0        0        0      183 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RADiscoveryAgent:2.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:1.xml
+-rw-r--r--   0        0        0      499 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RAServer:2.xml
+-rw-r--r--   0        0        0      300 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIClientDevice:1.xml
+-rw-r--r--   0        0        0      294 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:RemoteUIServerDevice:1.xml
+-rw-r--r--   0        0        0      561 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:1.xml
+-rw-r--r--   0        0        0      380 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:ScreenDevice:2.xml
+-rw-r--r--   0        0        0      419 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:1.xml
+-rw-r--r--   0        0        0      622 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml
+-rw-r--r--   0        0        0      416 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:1.xml
+-rw-r--r--   0        0        0      936 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml
+-rw-r--r--   0        0        0     1090 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml
+-rw-r--r--   0        0        0     1244 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml
+-rw-r--r--   0        0        0      338 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:1.xml
+-rw-r--r--   0        0        0      340 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANDevice:2.xml
+-rw-r--r--   0        0        0      490 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WLANAccessPointDevice:1.xml
+-rw-r--r--   0        0        0    21478 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml
+-rw-r--r--   0        0        0    22506 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml
+-rw-r--r--   0        0        0    32819 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml
+-rw-r--r--   0        0        0     3894 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml
+-rw-r--r--   0        0        0     5779 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml
+-rw-r--r--   0        0        0    10054 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml
+-rw-r--r--   0        0        0    22061 2022-12-08 19:53:16.288698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml
+-rw-r--r--   0        0        0    27823 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml
+-rw-r--r--   0        0        0     5740 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml
+-rw-r--r--   0        0        0    15507 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml
+-rw-r--r--   0        0        0    22397 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml
+-rw-r--r--   0        0        0     4082 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml
+-rw-r--r--   0        0        0     2151 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml
+-rw-r--r--   0        0        0     5359 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml
+-rw-r--r--   0        0        0    11356 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml
+-rw-r--r--   0        0        0    12959 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml
+-rw-r--r--   0        0        0     7870 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml
+-rw-r--r--   0        0        0     6485 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml
+-rw-r--r--   0        0        0     8455 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml
+-rw-r--r--   0        0        0    14206 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml
+-rw-r--r--   0        0        0    15034 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml
+-rw-r--r--   0        0        0    17600 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml
+-rw-r--r--   0        0        0    27620 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml
+-rw-r--r--   0        0        0     4821 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml
+-rw-r--r--   0        0        0     7808 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml
+-rw-r--r--   0        0        0     8486 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml
+-rw-r--r--   0        0        0     4783 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml
+-rw-r--r--   0        0        0     6607 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml
+-rw-r--r--   0        0        0     8457 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml
+-rw-r--r--   0        0        0     2249 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml
+-rw-r--r--   0        0        0     3447 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml
+-rw-r--r--   0        0        0     5176 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml
+-rw-r--r--   0        0        0     2637 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml
+-rw-r--r--   0        0        0     4564 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml
+-rw-r--r--   0        0        0     3751 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml
+-rw-r--r--   0        0        0     3673 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml
+-rw-r--r--   0        0        0     2461 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml
+-rw-r--r--   0        0        0     4528 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml
+-rw-r--r--   0        0        0     7628 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml
+-rw-r--r--   0        0        0     1045 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml
+-rw-r--r--   0        0        0    15694 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml
+-rw-r--r--   0        0        0     3331 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml
+-rw-r--r--   0        0        0     3234 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml
+-rw-r--r--   0        0        0    12147 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml
+-rw-r--r--   0        0        0    12076 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml
+-rw-r--r--   0        0        0     4682 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml
+-rw-r--r--   0        0        0    13539 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml
+-rw-r--r--   0        0        0    25446 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml
+-rw-r--r--   0        0        0     1919 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml
+-rw-r--r--   0        0        0     3445 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml
+-rw-r--r--   0        0        0     2800 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml
+-rw-r--r--   0        0        0     3264 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml
+-rw-r--r--   0        0        0     4324 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml
+-rw-r--r--   0        0        0     4744 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml
+-rw-r--r--   0        0        0     6642 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml
+-rw-r--r--   0        0        0     2399 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml
+-rw-r--r--   0        0        0    24162 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml
+-rw-r--r--   0        0        0    25624 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml
+-rw-r--r--   0        0        0    29018 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml
+-rw-r--r--   0        0        0    13767 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml
+-rw-r--r--   0        0        0    13651 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml
+-rw-r--r--   0        0        0    13686 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml
+-rw-r--r--   0        0        0    14103 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml
+-rw-r--r--   0        0        0     1285 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml
+-rw-r--r--   0        0        0     2951 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml
+-rw-r--r--   0        0        0     3412 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml
+-rw-r--r--   0        0        0     7592 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml
+-rw-r--r--   0        0        0     8319 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml
+-rw-r--r--   0        0        0     4926 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml
+-rw-r--r--   0        0        0      754 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml
+-rw-r--r--   0        0        0    14359 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml
+-rw-r--r--   0        0        0    19829 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml
+-rw-r--r--   0        0        0     7097 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml
+-rw-r--r--   0        0        0     6730 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml
+-rw-r--r--   0        0        0    18555 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml
+-rw-r--r--   0        0        0    39224 2022-12-08 19:53:16.292698 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml
+-rw-r--r--   0        0        0    16858 2023-04-30 20:52:10.965302 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py
+-rw-r--r--   0        0        0     2631 2023-03-20 16:55:58.994382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/paths.py
+-rw-r--r--   0        0        0      481 2023-03-20 16:55:59.002382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/services/__init__.py
+-rw-r--r--   0        0        0     5518 2023-03-21 07:56:39.142504 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py
+-rw-r--r--   0        0        0    26076 2023-04-30 20:52:11.669309 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py
+-rw-r--r--   0        0        0    11691 2023-04-30 20:52:10.937302 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/soap.py
+-rw-r--r--   0        0        0      943 2023-04-30 20:52:10.853301 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpconstants.py
+-rw-r--r--   0        0        0    55895 2023-04-30 20:52:13.489325 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py
+-rw-r--r--   0        0        0     7480 2023-04-30 21:01:15.502130 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py
+-rw-r--r--   0        0        0     2628 2023-03-21 08:17:25.473613 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnperrors.py
+-rw-r--r--   0        0        0    11109 2023-04-30 20:52:10.881301 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpfactory.py
+-rw-r--r--   0        0        0    21613 2023-03-21 08:16:35.890071 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py
+-rw-r--r--   0        0        0      494 2023-03-20 16:55:59.002382 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/xml/__init__.py
+-rw-r--r--   0        0        0    20710 2023-03-21 08:11:33.022274 mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 mojo_interop-0.0.7/setup.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 mojo_interop-0.0.7/PKG-INFO
```

### Comparing `mojo_interop-0.0.6/LICENSE.txt` & `mojo_interop-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/pyproject.toml` & `mojo_interop-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-interop"
 description = "Automation Mojo Interop Extensions"
-version = "0.0.6"
+version = "0.0.7"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_interop-0.0.6/source/packages/mojo/factories/xmodsfactory.py` & `mojo_interop-0.0.7/source/packages/mojo/factories/xmodsfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclient.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/linux/linuxclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclient.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/osx/osxclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclient.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclient.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclientcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clients/windows/windowsclientcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinode.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinode.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/clusters/raspberrypi/pinodecoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/__init__.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsaddress.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsaddress.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsapi.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsapi.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsconst.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsconst.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnshostinfo.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnshostinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsinboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsoutboundmessage.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnspointer.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnspointer.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsquestion.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsquestion.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsquestionresults.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsrecord.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsrecord.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsserver.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsserver.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsservice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsservice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnstext.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnstext.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsutil.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsutil.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/dnsvalidation.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/dnsvalidation.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/exceptions.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsagent.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsservicecatalog.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/mdnsserviceinfo.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/dns/testmessages.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/dns/testmessages.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipoweragent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/power/dlipower/dlipowercoordinatorcoupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 from mojo.xmods.landscaping.landscape import LandscapeDevice
 from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
-from mojo.xmods.landscaping.precedence import StartupLevel
+from mojo.xmods.landscaping.constants import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
 SUPPORTED_INTEGRATION_CLASS = "network/dlipower"
```

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialagent.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialcoordinatorcoupling.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 __license__ = "MIT"
 
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
 from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
-from mojo.xmods.landscaping.precedence import StartupLevel
+from mojo.xmods.landscaping.constants import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
 SUPPORTED_INTEGRATION_CLASS = "network/tcpserial"
```

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/serial/tcpserialdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshagent.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshagent.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshcoordinatorcoupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.landscaping.coupling.coordinatorcoupling import CoordinatorCoupling
 from mojo.xmods.landscaping.friendlyidentifier import FriendlyIdentifier
 from mojo.xmods.landscaping.landscape import LandscapeDevice
 from mojo.interop.protocols.ssh.sshcoordinator import SshCoordinator
 
-from mojo.xmods.landscaping.precedence import StartupLevel
+from mojo.xmods.landscaping.constants import StartupLevel
 
 # Types imported only for type checking purposes
 if TYPE_CHECKING:
     from mojo.xmods.landscaping.landscape import Landscape
 
 SUPPORTED_INTEGRATION_CLASS = "network/ssh"
```

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/ssh/sshdevice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/ssh/sshdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/__init__.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/aspectsupnp.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/content/didllite.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/content/didllite.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/__init__.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnpdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnpembeddeddevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/devices/upnprootdevice.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/addressbook1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/applicationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/avtransport3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/basicmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/calendar1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/callmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxy1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudproxydevice1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/cloudtransport1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/configurationmanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/connectionmanager3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/contentdirectory4serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/controlvalve1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/deviceprotection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycameramotionimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerasettings1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/digitalsecuritycamerastillimage1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/dimming1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/externalactivity1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/fanspeed1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/feeder1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/housestatus1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_fanoperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_setpointschedule1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/hvac_useroperatingmode1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inboundconnectionconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/inputconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/lanhostconfigmanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/layer3forwarding1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/linkauthentication1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/mediamanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/messaging2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/presence1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printbasic1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/printenhanced1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radaconfig2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radasync2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/radiusclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/rataconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiclient1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/remoteuiserver1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/renderingcontrol3serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scan1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/scheduledrecording2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/softwaremanagement2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/switchpower1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesensor1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/temperaturesetpoint1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancablelinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wancommoninterfaceconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wandsllinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanethernetlinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipconnection2serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanipv6firewallcontrol1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpotslinkconfig1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wanpppconnection1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/extensions/standard/services/UPnP/wlanconfiguration1serviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_System:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:HVAC_ZoneThermostat:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:InternetGatewayDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaRenderer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:MediaServer:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:Scanner:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyClient:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:TelephonyServer:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/embeddeddevices/UPnP/urn:schemas-upnp-org:device:WANConnectionDevice:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AVTransport:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:AddressBook:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ApplicationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:BasicManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Calendar:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CallManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxy:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudProxyDevice:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:CloudTransport:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConfigurationManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ConnectionManager:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ContentDirectory:4.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ControlValve:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DeviceProtection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraMotionImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraSettings:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:DigitalSecurityCameraStillImage:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Dimming:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ExternalActivity:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:FanSpeed:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Feeder:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_FanOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_SetpointSchedule:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HVAC_UserOperatingMode:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:HouseStatus:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InboundConnectionConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:InputConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LANHostConfigManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Layer3Forwarding:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:LinkAuthentication:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:MediaManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Messaging:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Presence:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintBasic:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:PrintEnhanced:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADAConfig:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RADASync:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RATAConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RadiusClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIClient:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RemoteUIServer:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:RenderingControl:3.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:Scan:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:ScheduledRecording:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SoftwareManagement:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:SwitchPower:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSensor:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:TemperatureSetpoint:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCableLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANCommonInterfaceConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANDSLLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANEthernetLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPConnection:2.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANIPv6FirewallControl:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPOTSLinkConfig:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WANPPPConnection:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/standard/services/UPnP/urn:schemas-upnp-org:service:WLANConfiguration:1.xml`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/generator/upnpgenerator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/paths.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/paths.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/services/upnpdefaultvar.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/services/upnpserviceproxy.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/soap.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/soap.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpconstants.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpconstants.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpcoordinator.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpcoordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnperrors.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnperrors.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpfactory.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/upnpprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py` & `mojo_interop-0.0.7/source/packages/mojo/interop/protocols/upnp/xml/upnpdevice1.py`

 * *Files identical despite different names*

### Comparing `mojo_interop-0.0.6/setup.py` & `mojo_interop-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                            'standard/services/UPnP/*']}
 
 install_requires = \
 ['mojo-networking>=0.0.4,<0.1.0', 'mojo-xmodules>=0.0.25,<0.1.0']
 
 setup_kwargs = {
     'name': 'mojo-interop',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Automation Mojo Interop Extensions',
     'long_description': '===============================\nAutomation Mojo Interop Package\n===============================\n\nThis *Automation Mojo Interop Package* contains interop extensions that add interop functionality to\nthe test environment *Landscape* object for a variety of platform clients, clusters, and protocols.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_interop-0.0.6/PKG-INFO` & `mojo_interop-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-interop
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automation Mojo Interop Extensions
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

