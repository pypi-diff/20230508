# Comparing `tmp/tilelog-1.4.1.tar.gz` & `tmp/tilelog-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tilelog-1.4.1.tar", last modified: Wed Oct 26 09:17:53 2022, max compression
+gzip compressed data, was "tilelog-1.5.0.tar", last modified: Mon May  8 06:27:49 2023, max compression
```

## Comparing `tilelog-1.4.1.tar` & `tilelog-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-26 09:17:53.673562 tilelog-1.4.1/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)    35149 2021-03-23 10:40:01.000000 tilelog-1.4.1/LICENSE
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      574 2022-10-26 09:17:53.673562 tilelog-1.4.1/PKG-INFO
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     4220 2022-08-04 04:57:57.000000 tilelog-1.4.1/README.md
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       38 2022-10-26 09:17:53.673562 tilelog-1.4.1/setup.cfg
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      956 2022-10-26 09:17:03.000000 tilelog-1.4.1/setup.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-26 09:17:53.673562 tilelog-1.4.1/tilelog/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     7569 2022-10-26 09:14:24.000000 tilelog-1.4.1/tilelog/__init__.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1997 2022-07-25 04:57:19.000000 tilelog-1.4.1/tilelog/aggregate.py
--rwxr--r--   0 pnorman   (1000) pnorman   (1000)     1304 2022-08-26 22:42:07.000000 tilelog-1.4.1/tilelog/cdn.py
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      233 2022-07-25 04:57:19.000000 tilelog-1.4.1/tilelog/constants.py
-drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2022-10-26 09:17:53.673562 tilelog-1.4.1/tilelog.egg-info/
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      574 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/PKG-INFO
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)      321 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/SOURCES.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/dependency_links.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       40 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/entry_points.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2021-07-03 13:40:41.000000 tilelog-1.4.1/tilelog.egg-info/not-zip-safe
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)       48 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/requires.txt
--rw-r--r--   0 pnorman   (1000) pnorman   (1000)        8 2022-10-26 09:17:53.000000 tilelog-1.4.1/tilelog.egg-info/top_level.txt
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-05-08 06:27:49.398448 tilelog-1.5.0/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)    35149 2021-03-23 10:40:01.000000 tilelog-1.5.0/LICENSE
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      574 2023-05-08 06:27:49.398448 tilelog-1.5.0/PKG-INFO
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     4220 2022-08-04 04:57:57.000000 tilelog-1.5.0/README.md
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       38 2023-05-08 06:27:49.398448 tilelog-1.5.0/setup.cfg
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      956 2023-05-08 05:53:16.000000 tilelog-1.5.0/setup.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-05-08 06:27:49.394448 tilelog-1.5.0/tilelog/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     8005 2023-05-08 06:05:58.000000 tilelog-1.5.0/tilelog/__init__.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)     1987 2023-05-08 06:02:46.000000 tilelog-1.5.0/tilelog/aggregate.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      237 2023-05-08 05:55:12.000000 tilelog-1.5.0/tilelog/constants.py
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      917 2023-05-08 05:58:15.000000 tilelog-1.5.0/tilelog/country.py
+drwxr-xr-x   0 pnorman   (1000) pnorman   (1000)        0 2023-05-08 06:27:49.398448 tilelog-1.5.0/tilelog.egg-info/
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      574 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/PKG-INFO
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)      325 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/SOURCES.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/dependency_links.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       40 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/entry_points.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)        1 2021-07-03 13:40:41.000000 tilelog-1.5.0/tilelog.egg-info/not-zip-safe
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)       48 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/requires.txt
+-rw-r--r--   0 pnorman   (1000) pnorman   (1000)        8 2023-05-08 06:27:49.000000 tilelog-1.5.0/tilelog.egg-info/top_level.txt
```

### Comparing `tilelog-1.4.1/LICENSE` & `tilelog-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tilelog-1.4.1/PKG-INFO` & `tilelog-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilelog
-Version: 1.4.1
+Version: 1.5.0
 Home-page: https://github.com/openstreetmap/tilelog
 Author: Paul Norman
 Author-email: osm@paulnorman.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `tilelog-1.4.1/README.md` & `tilelog-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tilelog-1.4.1/setup.py` & `tilelog-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name='tilelog',
-    version='1.4.1',
+    version='1.5.0',
     author="Paul Norman",
     author_email="osm@paulnorman.ca",
     url="https://github.com/openstreetmap/tilelog",
     packages=find_packages(),
     include_package_data=False,
     zip_safe=False,
     install_requires=[
```

### Comparing `tilelog-1.4.1/tilelog/__init__.py` & `tilelog-1.5.0/tilelog/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,44 +5,53 @@
 import csv
 import datetime
 import lzma
 import re
 
 import tilelog.constants
 import tilelog.aggregate
+import tilelog.country
 
 
 @click.command()
 @click.option('--date', type=click.DateTime(["%Y-%m-%d"]),
               default=(datetime.datetime.utcnow() -
                        datetime.timedelta(days=1)).strftime("%Y-%m-%d"),
               help="Date to generate logs for. Defaults to yesterday.")
 @click.option('--staging',
               default="s3://openstreetmap-fastly-processed-logs/tilelogs/",
               help="AWS s3 location for Athena results")
-@click.option('--generate-success', is_flag=True, default=False, help="Create logs of successful requests in Parquet")
+@click.option('--generate-success', is_flag=True, default=False,
+              help="Create logs of successful requests in Parquet")
 @click.option('--region', default="eu-west-1", help="Region for Athena")
 @click.option('--tile', type=click.File('wb'),
               help="File to output tile usage logs to")
 @click.option('--host', type=click.File('w', encoding='utf-8'),
               help="File to output host usage logs to")
 @click.option('--app', type=click.File('w', encoding='utf-8'),
               help="File to output app usage logs to")
-def cli(date, staging, generate_success, region, tile, host, app):
+@click.option('--country', type=click.File('w', encoding='utf-8'),
+              help="File with country-level statistics")
+def cli(date, staging, generate_success, region, tile, host, app, country):
     click.echo("Generating files for {}".format(date.strftime("%Y-%m-%d")))
     with pyathena.connect(s3_staging_dir=staging, region_name=region,
                           cursor_class=ArrowCursor).cursor() as curs:
+
+        # Aggregation must be run first, because the other tasks depend on it
         if generate_success:
             tilelog.aggregate.create_parquet(curs, date)
+
         if tile is not None:
             tile_logs(curs, date, tile)
         if host is not None:
             host_logs(curs, date, host)
         if app is not None:
             app_logs(curs, date, app)
+        if country is not None:
+            tilelog.country.country_logs(curs, date, country)
 
 
 def tile_logs(curs, date, dest):
     click.echo("Querying for tile usage")
     query = """
 SELECT z, x, y,
         COUNT(*)
@@ -60,30 +69,34 @@
                          "min_distinct": tilelog.constants.MIN_DISTINCT_TILE_REQUESTS,
                          "min_requests": tilelog.constants.MIN_TILE_REQUESTS})
     click.echo("Writing tile usage to file")
     with lzma.open(dest, "w") as file:
         for tile in curs:
             file.write("{}/{}/{} {}\n".format(tile[0], tile[1], tile[2], tile[3]).encode('ascii'))
 
+
 psl = PublicSuffixList()
+
+
 def normalize_host(host):
     if host is None:
         return ""
     # IPs don't have a public/private suffix
-    if re.match("^(\d+\.){3}\d+$", host):
+    if re.match(r"^(\d+\.){3}\d+$", host):
         return host
 
     suffix = psl.privatesuffix(host)
 
     # Something like "localhost", or an invalid host like ".example.com" may return None,
     # so don't try to give just the suffix in those cases
     if suffix is None:
         return host
     return suffix
 
+
 def host_logs(curs, date, dest):
     click.echo("Querying for host usage")
     query = """
 SELECT
 host,
 cast(count(*) as double)/86400 AS tps,
 cast(count(*) FILTER (WHERE cachehit = 'MISS') as double)/86400 AS tps_miss
@@ -111,24 +124,27 @@
         if stripped_hostname not in grouped_hosts:
             grouped_hosts[stripped_hostname] = [host[1], host[2]]
         else:
             # TPS is host[1] and grouped_hosts[][0], so the indexes don't match up
             grouped_hosts[stripped_hostname] = [grouped_hosts[stripped_hostname][0] + host[1],
                                                 grouped_hosts[stripped_hostname][1] + host[2]]
 
-    sorted_hosts = sorted([[host, metrics[0], metrics[1]] for (host,metrics) in grouped_hosts.items() if metrics[0] >= tilelog.constants.MIN_TPS],
-           key=lambda host: host[1], reverse=True) # Sort by TPS
+    sorted_hosts = sorted([[host, metrics[0], metrics[1]]
+                           for (host, metrics) in grouped_hosts.items()
+                           if metrics[0] >= tilelog.constants.MIN_TPS],
+                          key=lambda host: host[1], reverse=True)  # Sort by TPS
     click.echo("Writing host usage to file")
     csvwriter = csv.writer(dest, dialect=csv.unix_dialect,
                            quoting=csv.QUOTE_NONNUMERIC)
     csvwriter.writerows(sorted_hosts)
 
+
 def app_logs(curs, date, dest):
     click.echo("Querying for app usage")
-    query = """
+    query = r"""
 SELECT
 app,
 cast(count(*) as double)/86400 AS tps,
 cast(count(*) filter (WHERE cachehit = 'MISS') as double)/86400 AS tps_miss
 FROM (
     SELECT
     CASE
@@ -164,15 +180,15 @@
         OR referer = '' -- Non-websites
         OR (referer NOT LIKE 'https://%%/%%' AND referer NOT LIKE 'http://%%/%%') -- Referer set, but not a website
     )
 ) AS combined_requests
 GROUP BY app
 HAVING COUNT(*) > %(tps)d*86400
 ORDER BY COUNT(*) DESC
-    """.format(tablename=tilelog.constants.FASTLY_PARQET_LOGS)
+    """.format(tablename=tilelog.constants.FASTLY_PARQET_LOGS)  # noqa: E501
 
     curs.execute(query, {"year": date.year, "month": date.month,
                          "day": date.day, "tps": tilelog.constants.MIN_TPS})
     click.echo("Writing host usage to file")
     csvwriter = csv.writer(dest, dialect=csv.unix_dialect,
                            quoting=csv.QUOTE_NONNUMERIC)
     csvwriter.writerows(curs)
```

### Comparing `tilelog-1.4.1/tilelog/aggregate.py` & `tilelog-1.5.0/tilelog/aggregate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tilelog.constants
 
-TILE_REGEX="""'^GET /(\d{1,2})/(\d{1,6})/(\d{1,6})\.png'"""
+TILE_REGEX = r"""'^GET /(\d{1,2})/(\d{1,6})/(\d{1,6})\.png'"""
 
-SELECT_COLUMNS="""
+SELECT_COLUMNS = """
     time,
     ip,
     CAST(regexp_extract(request, {regex}, 1) AS integer) AS z,
     CAST(regexp_extract(request, {regex}, 2) AS integer) AS x,
     CAST(regexp_extract(request, {regex}, 3) AS integer) AS y,
     regexp_extract(request, ' HTTP/(.+?)$', 1) AS version,
     host,
@@ -27,27 +27,28 @@
     tls,
     render,
     year,
     month,
     day,
     hour""".format(regex=TILE_REGEX)
 
+
 def create_parquet(curs, date):
 
     # Start by checking if any rows are in the table to avoid running twice.
     # This won't catch multiple parallel runs, but will catch running it twice in a row.
     check_query = """
 SELECT * FROM {tablename}
 WHERE year = %(year)d
     AND month = %(month)d
     AND day = %(day)d
 LIMIT 1;
     """.format(tablename=tilelog.constants.FASTLY_PARQET_LOGS)
-    curs.execute(check_query, {"year": date.year, "month": date.month,
-                         "day": date.day})
+    curs.execute(check_query,
+                 {"year": date.year, "month": date.month, "day": date.day})
     # curs.rowcount doesn't work for Athena, so iterate through the row. This does nothing
     # if there are no rows in the table for this day, otherwise, it throws an exception.
     for line in curs:
         raise RuntimeError("aggregation queries have already been run for this day")
 
     insert_query = """
 INSERT INTO {tablename}
@@ -56,9 +57,9 @@
 WHERE status IN (200, 206, 304)
     AND regexp_like(request, {regex})
     AND year = %(year)d
     AND month = %(month)d
     AND day = %(day)d
     """.format(columns=SELECT_COLUMNS, sourcetable=tilelog.constants.FASTLY_LOG_TABLE,
                tablename=tilelog.constants.FASTLY_PARQET_LOGS, regex=TILE_REGEX)
-    curs.execute(insert_query, {"year": date.year, "month": date.month,
-                         "day": date.day})
+    curs.execute(insert_query,
+                 {"year": date.year, "month": date.month, "day": date.day})
```

### Comparing `tilelog-1.4.1/tilelog.egg-info/PKG-INFO` & `tilelog-1.5.0/tilelog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tilelog
-Version: 1.4.1
+Version: 1.5.0
 Home-page: https://github.com/openstreetmap/tilelog
 Author: Paul Norman
 Author-email: osm@paulnorman.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

