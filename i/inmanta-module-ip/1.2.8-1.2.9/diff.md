# Comparing `tmp/inmanta_module_ip-1.2.8-py3-none-any.whl.zip` & `tmp/inmanta_module_ip-1.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6082 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     3967 b- defN 22-Apr-25 06:53 inmanta_plugins/ip/__init__.py
--rw-rw-r--  2.0 unx      359 b- defN 22-Apr-25 06:56 inmanta_plugins/ip/setup.cfg
--rw-rw-r--  2.0 unx     3408 b- defN 22-Apr-25 06:53 inmanta_plugins/ip/model/_init.cf
--rw-rw-r--  2.0 unx     4328 b- defN 22-Apr-25 06:53 inmanta_plugins/ip/model/services.cf
--rw-rw-r--  2.0 unx      130 b- defN 22-Apr-25 06:53 inmanta_plugins/ip/templates/host_uri.j2
--rw-rw-r--  2.0 unx      288 b- defN 22-Apr-25 06:56 inmanta_module_ip-1.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-25 06:56 inmanta_module_ip-1.2.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Apr-25 06:56 inmanta_module_ip-1.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      787 b- defN 22-Apr-25 06:56 inmanta_module_ip-1.2.8.dist-info/RECORD
-9 files, 13375 bytes uncompressed, 4706 bytes compressed:  64.8%
+Zip file size: 6245 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     4647 b- defN 22-May-20 02:09 inmanta_plugins/ip/__init__.py
+-rw-rw-r--  2.0 unx      359 b- defN 22-May-20 02:09 inmanta_plugins/ip/setup.cfg
+-rw-rw-r--  2.0 unx     3408 b- defN 22-May-20 02:09 inmanta_plugins/ip/model/_init.cf
+-rw-rw-r--  2.0 unx     4328 b- defN 22-May-20 02:09 inmanta_plugins/ip/model/services.cf
+-rw-rw-r--  2.0 unx      130 b- defN 22-May-20 02:09 inmanta_plugins/ip/templates/host_uri.j2
+-rw-rw-r--  2.0 unx      244 b- defN 22-May-20 02:09 inmanta_module_ip-1.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 22-May-20 02:09 inmanta_module_ip-1.2.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 22-May-20 02:09 inmanta_module_ip-1.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      787 b- defN 22-May-20 02:09 inmanta_module_ip-1.2.9.dist-info/RECORD
+9 files, 14011 bytes uncompressed, 4869 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: inmanta_plugins/ip/model/services.cf
 Comment: 
 
 Filename: inmanta_plugins/ip/templates/host_uri.j2
 Comment: 
 
-Filename: inmanta_module_ip-1.2.8.dist-info/METADATA
+Filename: inmanta_module_ip-1.2.9.dist-info/METADATA
 Comment: 
 
-Filename: inmanta_module_ip-1.2.8.dist-info/WHEEL
+Filename: inmanta_module_ip-1.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: inmanta_module_ip-1.2.8.dist-info/top_level.txt
+Filename: inmanta_module_ip-1.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: inmanta_module_ip-1.2.8.dist-info/RECORD
+Filename: inmanta_module_ip-1.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inmanta_plugins/ip/__init__.py

```diff
@@ -66,14 +66,32 @@
 def net_to_nm(network_addr: "string") -> "string":
     net = netaddr.IPNetwork(network_addr)
     return str(net.netmask)
 
 
 @plugin
 def ipnet(addr: "ip::cidr_v10", what: "string") -> "string":
+    """
+    Return the ip, prefixlen, netmask or network address of the CIDR
+
+    :param addr: CIDR
+    :param what: The required result:
+
+     - ip: The IP address of `addr` object.
+     - prefixlen: The prefix length of `addr` object.
+     - netmask: The subnet mask of `addr` object.
+     - network: The network address of `addr` object.
+
+    For instance:
+
+        | std::print(ipnet("192.168.1.100/24", "ip"))         -->  192.168.1.100
+        | std::print(ipnet("192.168.1.100/24", "prefixlen"))  -->  24
+        | std::print(ipnet("192.168.1.100/24", "netmask"))    -->  255.255.255.0
+        | std::print(ipnet("192.168.1.100/24", "network"))    -->  192.168.1.0
+    """
     net = netaddr.IPNetwork(addr)
     if what == "ip":
         return str(net.ip)
 
     elif what == "prefixlen":
         return str(net.prefixlen)
```

## inmanta_plugins/ip/setup.cfg

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = inmanta-module-ip
 freeze_recursive = False
 freeze_operator = ~=
-version = 1.2.8
+version = 1.2.9
 license = Apache 2.0
 
 [options]
 install_requires = inmanta-module-ip
 	inmanta-module-net
 	inmanta-module-std
 	netaddr~=0.8.0
```

## Comparing `inmanta_module_ip-1.2.8.dist-info/RECORD` & `inmanta_module_ip-1.2.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-inmanta_plugins/ip/__init__.py,sha256=jzHpYbxQ3nlHhLisXAslnVhqj6V6pF-e1FnBtA0icXY,3967
-inmanta_plugins/ip/setup.cfg,sha256=Updr-i81AnmNAOrHB6m-sNp4NE_A0ElUPYbyc9OmFfQ,359
+inmanta_plugins/ip/__init__.py,sha256=QYlSWpqzzww-4TPSn2HdDsJAueCb_ca7aIhsr07xG-U,4647
+inmanta_plugins/ip/setup.cfg,sha256=PV8lAmabpfl16WolBTBHrXOqhkIphFwBiemYEysseFU,359
 inmanta_plugins/ip/model/_init.cf,sha256=GcddJRwxkt99otPl67yFDUM_Xu1QTwRrrOYHuO0t9Lo,3408
 inmanta_plugins/ip/model/services.cf,sha256=aJeNEYi_OVj6mljpZSuk9KX6W8DlORjXTlHbwKI201Q,4328
 inmanta_plugins/ip/templates/host_uri.j2,sha256=JSCdyz2Y4TXJQAgzXziWmhG_FvK-Z3r_rN1LD2dUt_k,130
-inmanta_module_ip-1.2.8.dist-info/METADATA,sha256=3ICsMdYiOxL5I2k9X2rvpM8EaNQAumnJX9toI5Dwk9A,288
-inmanta_module_ip-1.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-inmanta_module_ip-1.2.8.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
-inmanta_module_ip-1.2.8.dist-info/RECORD,,
+inmanta_module_ip-1.2.9.dist-info/METADATA,sha256=J1WNyL6Qjz7oZb0wggKGH1BXocNgt2bhuSUb-gn0Ta0,244
+inmanta_module_ip-1.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+inmanta_module_ip-1.2.9.dist-info/top_level.txt,sha256=rb9c6eWQS8KFuSa3ktEcXpk-oSsCL9ZCVAgv7S0Eg_w,16
+inmanta_module_ip-1.2.9.dist-info/RECORD,,
```

