# Comparing `tmp/compose_chart_export-0.0.16-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.16rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13196 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-06 09:53 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-06 09:53 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14200 b- defN 23-May-06 09:53 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-06 09:53 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-06 09:53 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9380 b- defN 23-May-06 09:53 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-06 09:53 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-06 09:53 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/RECORD
-13 files, 37738 bytes uncompressed, 11140 bytes compressed:  70.5%
+Zip file size: 13247 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-08 16:57 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-08 16:57 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14200 b- defN 23-May-08 16:57 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-08 16:57 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-08 16:57 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9543 b- defN 23-May-08 16:57 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-08 16:57 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-08 16:57 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      586 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1214 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/RECORD
+13 files, 37919 bytes uncompressed, 11161 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.16.dist-info/METADATA
+Filename: compose_chart_export-0.0.16rc1.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.16.dist-info/WHEEL
+Filename: compose_chart_export-0.0.16rc1.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.16.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.16.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.16rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.16.dist-info/RECORD
+Filename: compose_chart_export-0.0.16rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/compose_export.py

```diff
@@ -72,14 +72,17 @@
     return labels.get("chart_path", "")
 
 
 def parse_service_account_name(labels: dict[str, str]):
     return labels.get("chart_service_account_name", "")
 
 
+def parse_chart_name(labels: dict[str, str]) -> str:
+    return labels.get("chart_name", "")
+
 class ExtraContainer(BaseModel):
     name: kubernetes_label_regex
     env: dict[str, str]
     command: list[str]
 
 
 def parse_service_name_extra_containers(
@@ -92,15 +95,15 @@
         if info.labels.get("extra_container") == "true":
             container_name = each_service_name.replace("_", "-")
             extra_containers.append(
                 ExtraContainer(
                     name=container_name, env=info.default_env, command=info.command
                 )
             )
-        elif info.labels.get("chart_name"):
+        elif parse_chart_name(info.labels):
             service_names_with_chart_name.append(each_service_name)
         else:
             service_names.append(each_service_name)
     if service_names_with_chart_name:
         service_names = service_names_with_chart_name
     if not service_names:
         raise ValueError(f"No main service name found in {compose_path}")
@@ -132,25 +135,26 @@
     semver.parse_version_info(updated_version)
     return updated_version
 
 
 def export_from_compose(
     compose_path: PathLike,
     chart_version: str,
-    chart_name: str,
+    chart_name: str = "",
     image_url: str = "unset",
     on_exported: Callable[[Path], None] | None = None,
     use_chart_name_as_container_name: bool = True,
 ):
     chart_version = ensure_chart_version_valid(chart_version)
     compose_path = Path(compose_path)
     service_name, extra_containers = parse_service_name_extra_containers(compose_path)
     info = read_compose_info(compose_path, service_name)
     env = info.default_env
     compose_labels = info.labels
+    chart_name = chart_name or parse_chart_name(compose_labels)
     prefix_ports = parse_container_ports(compose_labels, info.host_container_ports)
     container_name = (
         chart_name.replace("_", "-")
         if use_chart_name_as_container_name
         else service_name.replace("_", "-")
     )
     with TemporaryDirectory() as path:
```

## Comparing `compose_chart_export-0.0.16.dist-info/METADATA` & `compose_chart_export-0.0.16rc1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.16
+Version: 0.0.16rc1
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Requires-Dist: docker-compose-parser (==0.0.16)
 Requires-Dist: model-lib (==0.0.16)
```

## Comparing `compose_chart_export-0.0.16.dist-info/RECORD` & `compose_chart_export-0.0.16rc1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
 compose_chart_export/chart_file_templates.py,sha256=bG35ma5Un9_18GpPiB5MYdKtvbZOQ-4zzEn7oCv0rSs,14200
 compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
 compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
-compose_chart_export/compose_export.py,sha256=w0ionkwWLTGOz9Lf2MIZVTRrUAjj7_pzmhJOxU80ZZw,9380
+compose_chart_export/compose_export.py,sha256=w7MblSmri-sPAJd6yNjghJQw7WhAbCZJe0w1P2XM4G0,9543
 compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.16.dist-info/METADATA,sha256=R7x_HyXXnAuqa8WEXGr8vKbBkUtQg_dj6tM-Jhc-5c0,583
-compose_chart_export-0.0.16.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.16.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.16.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.16.dist-info/RECORD,,
+compose_chart_export-0.0.16rc1.dist-info/METADATA,sha256=s4jS3b-jskSAUvfGfcpmagdMdiEkx4m7Y6FVfro1EhY,586
+compose_chart_export-0.0.16rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.16rc1.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.16rc1.dist-info/RECORD,,
```

