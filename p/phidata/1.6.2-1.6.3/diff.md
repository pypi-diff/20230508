# Comparing `tmp/phidata-1.6.2.tar.gz` & `tmp/phidata-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.6.2.tar", last modified: Wed May  3 15:22:22 2023, max compression
+gzip compressed data, was "phidata-1.6.3.tar", last modified: Mon May  8 13:04:37 2023, max compression
```

## Comparing `phidata-1.6.2.tar` & `phidata-1.6.3.tar`

### file list

```diff
@@ -1,511 +1,510 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 15:22:00.000000 phidata-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-03 15:22:22.067049 phidata-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-03 15:22:00.000000 phidata-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.019049 phidata-1.6.2/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.019049 phidata-1.6.2/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.019049 phidata-1.6.2/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.019049 phidata-1.6.2/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/assistant/assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/fastapi/fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.023049 phidata-1.6.2/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/k8s/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/server/app_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.027049 phidata-1.6.2/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18445 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.031049 phidata-1.6.2/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/create/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.035049 phidata-1.6.2/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.039049 phidata-1.6.2/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.043049 phidata-1.6.2/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.047049 phidata-1.6.2/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.051049 phidata-1.6.2/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.055049 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.059049 phidata-1.6.2/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.063049 phidata-1.6.2/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/utils/workspace_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-03 15:22:00.000000 phidata-1.6.2/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.019049 phidata-1.6.2/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-03 15:22:21.000000 phidata-1.6.2/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13473 2023-05-03 15:22:22.000000 phidata-1.6.2/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:22:21.000000 phidata-1.6.2/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 15:22:21.000000 phidata-1.6.2/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:22:21.000000 phidata-1.6.2/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-03 15:22:00.000000 phidata-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:22:22.067049 phidata-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 15:22:00.000000 phidata-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:22:22.067049 phidata-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 15:22:00.000000 phidata-1.6.2/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-05-08 13:04:18.000000 phidata-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 13:04:37.872171 phidata-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-08 13:04:18.000000 phidata-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/assistant/assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18446 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/fastapi/fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.824170 phidata-1.6.3/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/k8s/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.828170 phidata-1.6.3/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18445 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.832170 phidata-1.6.3/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/create/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23286 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16709 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19957 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.836170 phidata-1.6.3/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27957 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.840170 phidata-1.6.3/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22406 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.844170 phidata-1.6.3/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.848170 phidata-1.6.3/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.852170 phidata-1.6.3/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.856170 phidata-1.6.3/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.860170 phidata-1.6.3/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.864170 phidata-1.6.3/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/utils/workspace_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.868171 phidata-1.6.3/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-08 13:04:18.000000 phidata-1.6.3/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.820170 phidata-1.6.3/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 13:04:37.000000 phidata-1.6.3/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 13:04:18.000000 phidata-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:04:37.872171 phidata-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 13:04:18.000000 phidata-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:04:37.872171 phidata-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 13:04:18.000000 phidata-1.6.3/tests/test_placeholder.py
```

### Comparing `phidata-1.6.2/LICENSE` & `phidata-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/PKG-INFO` & `phidata-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.2
+Version: 1.6.3
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.2 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.3 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.2/README.md` & `phidata-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/airflow/operators/empty.py` & `phidata-1.6.3/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_base.py` & `phidata-1.6.3/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_flower.py` & `phidata-1.6.3/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_manager.py` & `phidata-1.6.3/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.6.3/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_webserver.py` & `phidata-1.6.3/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/airflow/airflow_worker.py` & `phidata-1.6.3/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/alertmanager/alertmanager.py` & `phidata-1.6.3/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/amundsen/frontend.py` & `phidata-1.6.3/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/amundsen/metadata.py` & `phidata-1.6.3/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/amundsen/search.py` & `phidata-1.6.3/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/assistant/assistant.py` & `phidata-1.6.3/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/cadvisor/cadvisor.py` & `phidata-1.6.3/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/databox/databox.py` & `phidata-1.6.3/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/db/base_db.py` & `phidata-1.6.3/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/elastic/elastic_app.py` & `phidata-1.6.3/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.6.3/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/fastapi/fastapi.py` & `phidata-1.6.3/phidata/app/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/grafana/grafana.py` & `phidata-1.6.3/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/group.py` & `phidata-1.6.3/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.6.3/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.6.3/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/k8s/app.py` & `phidata-1.6.3/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/k8s/dir.py` & `phidata-1.6.3/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/k8s/url.py` & `phidata-1.6.3/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/mysql/mysql_db.py` & `phidata-1.6.3/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/neo4j/neo4j.py` & `phidata-1.6.3/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.6.3/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/phidata_app.py` & `phidata-1.6.3/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/postgres/postgres_db.py` & `phidata-1.6.3/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/prometheus/prometheus.py` & `phidata-1.6.3/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/redis/redis.py` & `phidata-1.6.3/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/redis/stack.py` & `phidata-1.6.3/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/server/api_server.py` & `phidata-1.6.3/phidata/app/spark/spark_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.server.server_base import (
-    ServerBase,
-    ServerBaseArgs,
+from phidata.app.spark.spark_base import (
+    SparkBase,
+    SparkBaseArgs,
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class ApiServerArgs(ServerBaseArgs):
-    pass
-
-
-class ApiServer(ServerBase):
+class SparkWorker(SparkBase):
     def __init__(
         self,
-        name: str = "api-server",
+        name: str = "spark-worker",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/server",
-        image_tag: str = "latest",
+        image_name: str = "phidata/spark",
+        image_tag: str = "3.3.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "api start",
+        command: Optional[Union[str, List]] = "worker",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
+        # -*- Spark Configuration
+        cores: Optional[int] = None,
+        memory: Optional[str] = None,
+        driver_url: Optional[str] = None,
+        properties_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
@@ -54,26 +55,29 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9090,
+        container_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9090,
+        container_host_port: int = 8080,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/server",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -234,25 +238,32 @@
         extra_crds: Optional[List[Any]] = None,
         # Other args,
         print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
+        if driver_url is None:
+            raise ValueError("driver_url is required for SparkWorker")
+
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
+            cores=cores,
+            memory=memory,
+            driver_url=driver_url,
+            properties_file=properties_file,
             container_name=container_name,
             python_path=python_path,
             add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
```

### Comparing `phidata-1.6.2/phidata/app/server/app_server.py` & `phidata-1.6.3/phidata/app/spark/spark_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.server.server_base import (
-    ServerBase,
-    ServerBaseArgs,
+from phidata.app.spark.spark_base import (
+    SparkBase,
+    SparkBaseArgs,
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class AppServerArgs(ServerBaseArgs):
-    pass
-
-
-class AppServer(ServerBase):
+class SparkDriver(SparkBase):
     def __init__(
         self,
-        name: str = "app-server",
+        name: str = "spark-driver",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/server",
-        image_tag: str = "latest",
+        image_name: str = "phidata/spark",
+        image_tag: str = "3.3.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "app start",
+        command: Optional[Union[str, List]] = "driver",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
+        # -*- Spark Configuration
+        cores: Optional[int] = None,
+        memory: Optional[str] = None,
+        driver_port: int = 7077,
+        properties_file: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
@@ -54,26 +55,29 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9095,
+        container_port: int = 8080,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9095,
+        container_host_port: int = 8080,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/server",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -245,14 +249,18 @@
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
+            cores=cores,
+            memory=memory,
+            driver_port=driver_port,
+            properties_file=properties_file,
             container_name=container_name,
             python_path=python_path,
             add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
```

### Comparing `phidata-1.6.2/phidata/app/server/server_base.py` & `phidata-1.6.3/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/spark/spark_base.py` & `phidata-1.6.3/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/spark/spark_driver.py` & `phidata-1.6.3/phidata/app/server/api_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.spark.spark_base import (
-    SparkBase,
-    SparkBaseArgs,
+from phidata.app.server.server_base import (
+    ServerBase,
+    ServerBaseArgs,
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SparkDriver(SparkBase):
+class ApiServerArgs(ServerBaseArgs):
+    pass
+
+
+class ApiServer(ServerBase):
     def __init__(
         self,
-        name: str = "spark-driver",
+        name: str = "api-server",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/spark",
-        image_tag: str = "3.3.1",
+        image_name: str = "phidata/server",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "driver",
+        command: Optional[Union[str, List]] = "api start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Spark Configuration
-        cores: Optional[int] = None,
-        memory: Optional[str] = None,
-        driver_port: int = 7077,
-        properties_file: Optional[str] = None,
+        # -*- Debug Mode
+        debug_mode: bool = False,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 8080,
+        container_port: int = 80,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 8080,
+        container_host_port: int = 80,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume,
-        # This is the parent directory for the workspace on the container,
-        # i.e. the ws is mounted as a subdir in this dir,
-        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
-        workspace_volume_container_path: str = "/mnt/workspaces",
+        # Path to mount the workspace volume inside the container,
+        workspace_volume_container_path: str = "/usr/local/server",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -164,15 +162,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[ServiceType] = None,
         # The port exposed by the service.,
-        service_port: int = 8000,
+        service_port: int = 80,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -232,16 +230,36 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
+        # -*- AWS configuration,
+        ecs_cluster: Optional[Any] = None,
+        ecs_launch_type: str = "FARGATE",
+        ecs_task_cpu: str = "256",
+        ecs_task_memory: str = "512",
+        ecs_service_count: int = 1,
+        assign_public_ip: bool = True,
+        elb: Optional[Any] = None,
+        aws_subnets: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = True,
+        print_env_on_load: bool = False,
+        skip_create: bool = False,
+        skip_read: bool = False,
+        skip_update: bool = False,
+        recreate_on_update: bool = False,
+        skip_delete: bool = False,
+        wait_for_creation: bool = True,
+        wait_for_update: bool = True,
+        wait_for_deletion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 50,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
         super().__init__(
             name=name,
             version=version,
@@ -249,18 +267,15 @@
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            cores=cores,
-            memory=memory,
-            driver_port=driver_port,
-            properties_file=properties_file,
+            debug_mode=debug_mode,
             container_name=container_name,
             python_path=python_path,
             add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
@@ -342,11 +357,30 @@
             extra_containers=extra_containers,
             extra_init_containers=extra_init_containers,
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
+            ecs_cluster=ecs_cluster,
+            ecs_launch_type=ecs_launch_type,
+            ecs_task_cpu=ecs_task_cpu,
+            ecs_task_memory=ecs_task_memory,
+            ecs_service_count=ecs_service_count,
+            assign_public_ip=assign_public_ip,
+            elb=elb,
+            aws_subnets=aws_subnets,
+            aws_security_groups=aws_security_groups,
             print_env_on_load=print_env_on_load,
+            skip_create=skip_create,
+            skip_read=skip_read,
+            skip_update=skip_update,
+            recreate_on_update=recreate_on_update,
+            skip_delete=skip_delete,
+            wait_for_creation=wait_for_creation,
+            wait_for_update=wait_for_update,
+            wait_for_deletion=wait_for_deletion,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
             use_cache=use_cache,
             **kwargs,
         )
```

### Comparing `phidata-1.6.2/phidata/app/spark/spark_worker.py` & `phidata-1.6.3/phidata/app/streamlit/streamlit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.spark.spark_base import (
-    SparkBase,
-    SparkBaseArgs,
+from phidata.app.server.server_base import (
+    ServerBase,
+    ServerBaseArgs,
     ServiceType,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SparkWorker(SparkBase):
+class StreamlitAppArgs(ServerBaseArgs):
+    pass
+
+
+class StreamlitApp(ServerBase):
     def __init__(
         self,
-        name: str = "spark-worker",
+        name: str = "streamlit-app",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/spark",
-        image_tag: str = "3.3.1",
+        image_name: str = "phidata/streamlit",
+        image_tag: str = "latest",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "worker",
+        command: Optional[Union[str, List]] = "app start",
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Spark Configuration
-        cores: Optional[int] = None,
-        memory: Optional[str] = None,
-        driver_url: Optional[str] = None,
-        properties_file: Optional[str] = None,
+        # -*- Debug Mode
+        debug_mode: bool = False,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
         # Overwrite the PYTHONPATH env var,
         # which is usually set to the workspace_root_container_path,
         python_path: Optional[str] = None,
         # Add to the PYTHONPATH env var. If python_path is set, this is ignored
         # Does not overwrite the PYTHONPATH env var - adds to it.
         add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, str]] = None,
+        env: Optional[Dict[str, Any]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, str]] = None,
+        secrets: Optional[Dict[str, Any]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 8080,
+        container_port: int = 9095,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 8080,
+        container_host_port: int = 9095,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume,
-        # This is the parent directory for the workspace on the container,
-        # i.e. the ws is mounted as a subdir in this dir,
-        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
-        workspace_volume_container_path: str = "/mnt/workspaces",
+        # Path to mount the workspace volume inside the container,
+        workspace_volume_container_path: str = "/usr/local/server",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -164,15 +162,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[ServiceType] = None,
         # The port exposed by the service.,
-        service_port: int = 8000,
+        service_port: int = 9095,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -232,38 +230,52 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
+        # -*- AWS configuration,
+        ecs_cluster: Optional[Any] = None,
+        ecs_launch_type: str = "FARGATE",
+        ecs_task_cpu: str = "256",
+        ecs_task_memory: str = "512",
+        ecs_service_count: int = 1,
+        assign_public_ip: bool = True,
+        elb: Optional[Any] = None,
+        aws_subnets: Optional[List[str]] = None,
+        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = True,
+        print_env_on_load: bool = False,
+        skip_create: bool = False,
+        skip_read: bool = False,
+        skip_update: bool = False,
+        recreate_on_update: bool = False,
+        skip_delete: bool = False,
+        wait_for_creation: bool = True,
+        wait_for_update: bool = True,
+        wait_for_deletion: bool = True,
+        waiter_delay: int = 30,
+        waiter_max_attempts: int = 50,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
         **kwargs,
     ):
-        if driver_url is None:
-            raise ValueError("driver_url is required for SparkWorker")
-
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            cores=cores,
-            memory=memory,
-            driver_url=driver_url,
-            properties_file=properties_file,
+            debug_mode=debug_mode,
             container_name=container_name,
             python_path=python_path,
             add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
@@ -345,11 +357,30 @@
             extra_containers=extra_containers,
             extra_init_containers=extra_init_containers,
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
+            ecs_cluster=ecs_cluster,
+            ecs_launch_type=ecs_launch_type,
+            ecs_task_cpu=ecs_task_cpu,
+            ecs_task_memory=ecs_task_memory,
+            ecs_service_count=ecs_service_count,
+            assign_public_ip=assign_public_ip,
+            elb=elb,
+            aws_subnets=aws_subnets,
+            aws_security_groups=aws_security_groups,
             print_env_on_load=print_env_on_load,
+            skip_create=skip_create,
+            skip_read=skip_read,
+            skip_update=skip_update,
+            recreate_on_update=recreate_on_update,
+            skip_delete=skip_delete,
+            wait_for_creation=wait_for_creation,
+            wait_for_update=wait_for_update,
+            wait_for_deletion=wait_for_deletion,
+            waiter_delay=waiter_delay,
+            waiter_max_attempts=waiter_max_attempts,
             use_cache=use_cache,
             **kwargs,
         )
```

### Comparing `phidata-1.6.2/phidata/app/streamlit/streamlit.py` & `phidata-1.6.3/phidata/app/superset/superset_init.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,128 @@
 from pathlib import Path
 from typing import Optional, Dict, Any, List, Union
 
-from phidata.app.server.server_base import (
-    ServerBase,
-    ServerBaseArgs,
+from phidata.app.superset.superset_base import (
+    SupersetBase,
     ServiceType,
+    DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class StreamlitAppArgs(ServerBaseArgs):
-    pass
-
-
-class StreamlitApp(ServerBase):
+class SupersetInit(SupersetBase):
     def __init__(
         self,
-        name: str = "streamlit-app",
+        name: str = "superset-init",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/streamlit",
-        image_tag: str = "latest",
-        entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "app start",
+        image_name: str = "phidata/superset",
+        image_tag: str = "2.0.1",
+        entrypoint: Optional[Union[str, List]] = "/scripts/init-superset.sh",
+        command: Optional[Union[str, List]] = None,
         # Install python dependencies using a requirements.txt file,
+        # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
-        # -*- Debug Mode
-        debug_mode: bool = False,
+        # -*- Superset Configuration,
+        # Configure Superset db,
+        wait_for_db: bool = False,
+        # Connect to database using a DbApp,
+        db_app: Optional[DbApp] = None,
+        # Provide database connection details manually,
+        # db_user can be provided here or as the,
+        # DATABASE_USER env var in the secrets_file,
+        db_user: Optional[str] = None,
+        # db_password can be provided here or as the,
+        # DATABASE_PASSWORD env var in the secrets_file,
+        db_password: Optional[str] = None,
+        # db_schema can be provided here or as the,
+        # DATABASE_DB env var in the secrets_file,
+        db_schema: Optional[str] = None,
+        # db_host can be provided here or as the,
+        # DATABASE_HOST env var in the secrets_file,
+        db_host: Optional[str] = None,
+        # db_port can be provided here or as the,
+        # DATABASE_PORT env var in the secrets_file,
+        db_port: Optional[int] = None,
+        # db_driver can be provided here or as the,
+        # DATABASE_DIALECT env var in the secrets_file,
+        db_dialect: Optional[str] = None,
+        # Configure superset redis,
+        wait_for_redis: bool = False,
+        # Connect to redis using a PhidataApp,
+        redis_app: Optional[DbApp] = None,
+        # redis_host can be provided here or as the,
+        # REDIS_HOST env var in the secrets_file,
+        redis_host: Optional[str] = None,
+        # redis_port can be provided here or as the,
+        # REDIS_PORT env var in the secrets_file,
+        redis_port: Optional[int] = None,
+        # redis_driver can be provided here or as the,
+        # REDIS_DRIVER env var in the secrets_file,
+        redis_driver: Optional[str] = None,
         # -*- Container Configuration,
         container_name: Optional[str] = None,
-        # Overwrite the PYTHONPATH env var,
-        # which is usually set to the workspace_root_container_path,
+        # Set the SUPERSET_CONFIG_PATH env var,
+        superset_config_path: Optional[str] = None,
+        # Set the FLASK_ENV env var,
+        flask_env: str = "production",
+        # Set the SUPERSET_ENV env var,
+        superset_env: str = "production",
+        # Set the PYTHONPATH env var,
+        # defaults to "/app/pythonpath:/app/docker/pythonpath_dev",
         python_path: Optional[str] = None,
-        # Add to the PYTHONPATH env var. If python_path is set, this is ignored
-        # Does not overwrite the PYTHONPATH env var - adds to it.
-        add_python_path: Optional[str] = None,
         # Add labels to the container,
         container_labels: Optional[Dict[str, Any]] = None,
         # Container env passed to the PhidataApp,
         # Add env variables to container env,
-        env: Optional[Dict[str, Any]] = None,
+        env: Optional[Dict[str, str]] = None,
         # Read env variables from a file in yaml format,
         env_file: Optional[Path] = None,
         # Container secrets,
         # Add secret variables to container env,
-        secrets: Optional[Dict[str, Any]] = None,
+        secrets: Optional[Dict[str, str]] = None,
         # Read secret variables from a file in yaml format,
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # Container ports,
         # Open a container port if open_container_port=True,
-        open_container_port: bool = True,
+        open_container_port: bool = False,
         # Port number on the container,
-        container_port: int = 9095,
+        container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
-        container_host_port: int = 9095,
+        container_host_port: int = 8000,
+        # Open the app port if open_app_port=True,
+        open_app_port: bool = False,
+        # App port number on the container,
+        # Set the SUPERSET_PORT env var,
+        app_port: int = 8088,
+        # Only used by the K8sContainer,
+        app_port_name: str = "app",
+        # Only used by the DockerContainer,
+        app_host_port: int = 8088,
         # Container volumes,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
-        # Path to mount the workspace volume inside the container,
-        workspace_volume_container_path: str = "/usr/local/server",
+        # Path to mount the workspace volume,
+        # This is the parent directory for the workspace on the container,
+        # i.e. the ws is mounted as a subdir in this dir,
+        # eg: if ws name is: idata, workspace_root would be: /mnt/workspaces/idata,
+        workspace_volume_container_path: str = "/mnt/workspaces",
         # How to mount the workspace volume,
         # Option 1: Mount the workspace from the host machine,
         # If None, use the workspace_root_path,
         # Note: This is the default on DockerContainers. We assume that DockerContainers,
         # are running locally on the user's machine so the local workspace_root_path,
         # is mounted to the workspace_volume_container_path,
         workspace_volume_host_path: Optional[str] = None,
@@ -85,14 +132,23 @@
         # Required to create an initial copy of the workspace,
         create_git_sync_init_container: bool = True,
         git_sync_image_name: str = "k8s.gcr.io/git-sync",
         git_sync_image_tag: str = "v3.1.1",
         git_sync_repo: Optional[str] = None,
         git_sync_branch: Optional[str] = None,
         git_sync_wait: int = 1,
+        # Configure resources volume. Only on docker,
+        # Superset resources directory relative to the workspace_root,
+        # This directory contains all the files required by superset.,
+        # eg: docker-bootstrap.sh,
+        # This dir is mounted to the `/app/docker` directory on the container,
+        mount_resources: bool = False,
+        resources_dir: str = "workspace/superset",
+        resources_dir_container_path: str = "/app/docker",
+        resources_volume_name: Optional[str] = None,
         # -*- Docker configuration,
         # Run container in the background and return a Container object.,
         container_detach: bool = True,
         # Enable auto-removal of the container on daemon side when the container’s process exits.,
         container_auto_remove: bool = True,
         # Remove the container when it has finished running. Default: True.,
         container_remove: bool = True,
@@ -160,17 +216,17 @@
         topology_spread_max_skew: Optional[int] = None,
         # How to deal with a pod if it doesn't satisfy the spread constraint.,
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # K8s Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
-        service_type: Optional[ServiceType] = None,
+        service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 9095,
+        service_port: int = 8000,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -181,14 +237,39 @@
         # If ServiceType == ServiceType.LoadBalancer,
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
+        # App Service Configuration,
+        create_app_service: bool = False,
+        # Configure the app service,
+        app_svc_name: Optional[str] = None,
+        app_svc_type: Optional[ServiceType] = None,
+        # The port that will be exposed by the service.,
+        app_svc_port: int = 8088,
+        # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
+        app_node_port: Optional[int] = None,
+        # The app_target_port is the port to access on the pods targeted by the service.,
+        # It can be the port number or port name on the pod.,
+        app_target_port: Optional[Union[str, int]] = None,
+        # Extra ports exposed by the app service,
+        app_svc_ports: Optional[List[Any]] = None,
+        # Add labels to app service,
+        app_svc_labels: Optional[Dict[str, Any]] = None,
+        # Add annotations to app service,
+        app_svc_annotations: Optional[Dict[str, str]] = None,
+        # If ServiceType == LoadBalancer,
+        app_svc_health_check_node_port: Optional[int] = None,
+        app_svc_internal_taffic_policy: Optional[str] = None,
+        app_svc_load_balancer_class: Optional[str] = None,
+        app_svc_load_balancer_ip: Optional[str] = None,
+        app_svc_load_balancer_source_ranges: Optional[List[str]] = None,
+        app_svc_allocate_load_balancer_node_ports: Optional[bool] = None,
         # K8s RBAC Configuration,
         use_rbac: bool = False,
         # Create a Namespace with name ns_name & default values,
         ns_name: Optional[str] = None,
         # or Provide the full Namespace definition,
         # Type: CreateNamespace,
         namespace: Optional[Any] = None,
@@ -230,77 +311,81 @@
         extra_volumes: Optional[List[Any]] = None,
         # Type: CreateStorageClass,
         extra_storage_classes: Optional[List[Any]] = None,
         # Type: CreateCustomObject,
         extra_custom_objects: Optional[List[Any]] = None,
         # Type: CreateCustomResourceDefinition,
         extra_crds: Optional[List[Any]] = None,
-        # -*- AWS configuration,
-        ecs_cluster: Optional[Any] = None,
-        ecs_launch_type: str = "FARGATE",
-        ecs_task_cpu: str = "256",
-        ecs_task_memory: str = "512",
-        ecs_service_count: int = 1,
-        assign_public_ip: bool = True,
-        elb: Optional[Any] = None,
-        aws_subnets: Optional[List[str]] = None,
-        aws_security_groups: Optional[List[str]] = None,
         # Other args,
-        print_env_on_load: bool = False,
-        skip_create: bool = False,
-        skip_read: bool = False,
-        skip_update: bool = False,
-        recreate_on_update: bool = False,
-        skip_delete: bool = False,
-        wait_for_creation: bool = True,
-        wait_for_update: bool = True,
-        wait_for_deletion: bool = True,
-        waiter_delay: int = 30,
-        waiter_max_attempts: int = 50,
+        print_env_on_load: bool = True,
         # If True, skip resource creation if active resources with the same name exist.,
         use_cache: bool = True,
+        # Set SUPERSET_LOAD_EXAMPLES = "yes",
+        load_examples: bool = False,
         **kwargs,
     ):
         super().__init__(
             name=name,
             version=version,
             enabled=enabled,
             image=image,
             image_name=image_name,
             image_tag=image_tag,
             entrypoint=entrypoint,
             command=command,
             install_requirements=install_requirements,
             requirements_file=requirements_file,
-            debug_mode=debug_mode,
+            wait_for_db=wait_for_db,
+            db_app=db_app,
+            db_user=db_user,
+            db_password=db_password,
+            db_schema=db_schema,
+            db_host=db_host,
+            db_port=db_port,
+            db_dialect=db_dialect,
+            wait_for_redis=wait_for_redis,
+            redis_app=redis_app,
+            redis_host=redis_host,
+            redis_port=redis_port,
+            redis_driver=redis_driver,
             container_name=container_name,
+            superset_config_path=superset_config_path,
+            flask_env=flask_env,
+            superset_env=superset_env,
             python_path=python_path,
-            add_python_path=add_python_path,
             container_labels=container_labels,
             env=env,
             env_file=env_file,
             secrets=secrets,
             secrets_file=secrets_file,
             aws_secrets=aws_secrets,
             open_container_port=open_container_port,
             container_port=container_port,
             container_port_name=container_port_name,
             container_host_port=container_host_port,
+            open_app_port=open_app_port,
+            app_port=app_port,
+            app_port_name=app_port_name,
+            app_host_port=app_host_port,
             mount_workspace=mount_workspace,
             workspace_volume_name=workspace_volume_name,
             workspace_volume_type=workspace_volume_type,
             workspace_volume_container_path=workspace_volume_container_path,
             workspace_volume_host_path=workspace_volume_host_path,
             create_git_sync_sidecar=create_git_sync_sidecar,
             create_git_sync_init_container=create_git_sync_init_container,
             git_sync_image_name=git_sync_image_name,
             git_sync_image_tag=git_sync_image_tag,
             git_sync_repo=git_sync_repo,
             git_sync_branch=git_sync_branch,
             git_sync_wait=git_sync_wait,
+            mount_resources=mount_resources,
+            resources_dir=resources_dir,
+            resources_dir_container_path=resources_dir_container_path,
+            resources_volume_name=resources_volume_name,
             container_detach=container_detach,
             container_auto_remove=container_auto_remove,
             container_remove=container_remove,
             container_user=container_user,
             container_stdin_open=container_stdin_open,
             container_tty=container_tty,
             container_healthcheck=container_healthcheck,
@@ -335,14 +420,29 @@
             service_annotations=service_annotations,
             service_health_check_node_port=service_health_check_node_port,
             service_internal_traffic_policy=service_internal_traffic_policy,
             service_load_balancer_class=service_load_balancer_class,
             service_load_balancer_ip=service_load_balancer_ip,
             service_load_balancer_source_ranges=service_load_balancer_source_ranges,
             service_allocate_load_balancer_node_ports=service_allocate_load_balancer_node_ports,
+            create_app_service=create_app_service,
+            app_svc_name=app_svc_name,
+            app_svc_type=app_svc_type,
+            app_svc_port=app_svc_port,
+            app_node_port=app_node_port,
+            app_target_port=app_target_port,
+            app_svc_ports=app_svc_ports,
+            app_svc_labels=app_svc_labels,
+            app_svc_annotations=app_svc_annotations,
+            app_svc_health_check_node_port=app_svc_health_check_node_port,
+            app_svc_internal_taffic_policy=app_svc_internal_taffic_policy,
+            app_svc_load_balancer_class=app_svc_load_balancer_class,
+            app_svc_load_balancer_ip=app_svc_load_balancer_ip,
+            app_svc_load_balancer_source_ranges=app_svc_load_balancer_source_ranges,
+            app_svc_allocate_load_balancer_node_ports=app_svc_allocate_load_balancer_node_ports,
             use_rbac=use_rbac,
             ns_name=ns_name,
             namespace=namespace,
             sa_name=sa_name,
             service_account=service_account,
             cr_name=cr_name,
             cluster_role=cluster_role,
@@ -357,30 +457,12 @@
             extra_containers=extra_containers,
             extra_init_containers=extra_init_containers,
             extra_ports=extra_ports,
             extra_volumes=extra_volumes,
             extra_storage_classes=extra_storage_classes,
             extra_custom_objects=extra_custom_objects,
             extra_crds=extra_crds,
-            ecs_cluster=ecs_cluster,
-            ecs_launch_type=ecs_launch_type,
-            ecs_task_cpu=ecs_task_cpu,
-            ecs_task_memory=ecs_task_memory,
-            ecs_service_count=ecs_service_count,
-            assign_public_ip=assign_public_ip,
-            elb=elb,
-            aws_subnets=aws_subnets,
-            aws_security_groups=aws_security_groups,
             print_env_on_load=print_env_on_load,
-            skip_create=skip_create,
-            skip_read=skip_read,
-            skip_update=skip_update,
-            recreate_on_update=recreate_on_update,
-            skip_delete=skip_delete,
-            wait_for_creation=wait_for_creation,
-            wait_for_update=wait_for_update,
-            wait_for_deletion=wait_for_deletion,
-            waiter_delay=waiter_delay,
-            waiter_max_attempts=waiter_max_attempts,
             use_cache=use_cache,
+            load_examples=load_examples,
             **kwargs,
         )
```

### Comparing `phidata-1.6.2/phidata/app/superset/superset_base.py` & `phidata-1.6.3/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/superset/superset_init.py` & `phidata-1.6.3/phidata/app/superset/superset_webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetInit(SupersetBase):
+class SupersetWebserver(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-init",
+        name: str = "superset-ws",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
-        entrypoint: Optional[Union[str, List]] = "/scripts/init-superset.sh",
-        command: Optional[Union[str, List]] = None,
+        entrypoint: Optional[Union[str, List]] = None,
+        command: Optional[Union[str, List]] = "webserver",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
@@ -97,15 +97,15 @@
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the app port if open_app_port=True,
-        open_app_port: bool = False,
+        open_app_port: bool = True,
         # App port number on the container,
         # Set the SUPERSET_PORT env var,
         app_port: int = 8088,
         # Only used by the K8sContainer,
         app_port_name: str = "app",
         # Only used by the DockerContainer,
         app_host_port: int = 8088,
@@ -238,15 +238,15 @@
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
         # App Service Configuration,
-        create_app_service: bool = False,
+        create_app_service: bool = True,
         # Configure the app service,
         app_svc_name: Optional[str] = None,
         app_svc_type: Optional[ServiceType] = None,
         # The port that will be exposed by the service.,
         app_svc_port: int = 8088,
         # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
         app_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.2/phidata/app/superset/superset_webserver.py` & `phidata-1.6.3/phidata/app/superset/superset_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetWebserver(SupersetBase):
+class SupersetWorker(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-ws",
+        name: str = "superset-worker",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "webserver",
+        command: Optional[Union[str, List]] = "worker",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
@@ -97,15 +97,15 @@
         # Port number on the container,
         container_port: int = 8000,
         # Port name: Only used by the K8sContainer,
         container_port_name: str = "http",
         # Host port: Only used by the DockerContainer,
         container_host_port: int = 8000,
         # Open the app port if open_app_port=True,
-        open_app_port: bool = True,
+        open_app_port: bool = False,
         # App port number on the container,
         # Set the SUPERSET_PORT env var,
         app_port: int = 8088,
         # Only used by the K8sContainer,
         app_port_name: str = "app",
         # Only used by the DockerContainer,
         app_host_port: int = 8088,
@@ -238,15 +238,15 @@
         service_health_check_node_port: Optional[int] = None,
         service_internal_traffic_policy: Optional[str] = None,
         service_load_balancer_class: Optional[str] = None,
         service_load_balancer_ip: Optional[str] = None,
         service_load_balancer_source_ranges: Optional[List[str]] = None,
         service_allocate_load_balancer_node_ports: Optional[bool] = None,
         # App Service Configuration,
-        create_app_service: bool = True,
+        create_app_service: bool = False,
         # Configure the app service,
         app_svc_name: Optional[str] = None,
         app_svc_type: Optional[ServiceType] = None,
         # The port that will be exposed by the service.,
         app_svc_port: int = 8088,
         # The node_port that will be exposed by the service if app_svc_type = ServiceType.NODE_PORT,
         app_node_port: Optional[int] = None,
```

### Comparing `phidata-1.6.2/phidata/app/superset/superset_worker.py` & `phidata-1.6.3/phidata/app/superset/superset_worker_beat.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,27 @@
     DbApp,
     WorkspaceVolumeType,
     ImagePullPolicy,
     RestartPolicy,
 )
 
 
-class SupersetWorker(SupersetBase):
+class SupersetWorkerBeat(SupersetBase):
     def __init__(
         self,
-        name: str = "superset-worker",
+        name: str = "superset-worker-beat",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
         image_name: str = "phidata/superset",
         image_tag: str = "2.0.1",
         entrypoint: Optional[Union[str, List]] = None,
-        command: Optional[Union[str, List]] = "worker",
+        command: Optional[Union[str, List]] = "beat",
         # Install python dependencies using a requirements.txt file,
         # Sets the REQUIREMENTS_LOCAL & REQUIREMENTS_FILE_PATH env var to requirements_file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
         # -*- Superset Configuration,
         # Configure Superset db,
```

### Comparing `phidata-1.6.2/phidata/app/traefik/crds.py` & `phidata-1.6.3/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/traefik/ingress_route.py` & `phidata-1.6.3/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/app/traefik/router.py` & `phidata-1.6.3/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/asset/aws/aws_asset.py` & `phidata-1.6.3/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/asset/data_asset.py` & `phidata-1.6.3/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/asset/local/file.py` & `phidata-1.6.3/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/asset/local/local_asset.py` & `phidata-1.6.3/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/api_client.py` & `phidata-1.6.3/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/athena/query.py` & `phidata-1.6.3/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/config.py` & `phidata-1.6.3/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.6.3/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/create/iam/role.py` & `phidata-1.6.3/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/enums/manager_status.py` & `phidata-1.6.3/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/manager.py` & `phidata-1.6.3/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/acm/certificate.py` & `phidata-1.6.3/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/athena/query.py` & `phidata-1.6.3/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/base.py` & `phidata-1.6.3/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.6.3/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ec2/subnet.py` & `phidata-1.6.3/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ec2/volume.py` & `phidata-1.6.3/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ecs/cluster.py` & `phidata-1.6.3/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ecs/container.py` & `phidata-1.6.3/phidata/aws/resource/ecs/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ecs/service.py` & `phidata-1.6.3/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.6.3/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/ecs/volume.py` & `phidata-1.6.3/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/eks/addon.py` & `phidata-1.6.3/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/eks/cluster.py` & `phidata-1.6.3/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.6.3/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.6.3/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/eks/node_group.py` & `phidata-1.6.3/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.6.3/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.6.3/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/elb/listener.py` & `phidata-1.6.3/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.6.3/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/elb/target_group.py` & `phidata-1.6.3/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/emr/cluster.py` & `phidata-1.6.3/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/glue/crawler.py` & `phidata-1.6.3/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/group.py` & `phidata-1.6.3/phidata/aws/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/iam/group.py` & `phidata-1.6.3/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/iam/policy.py` & `phidata-1.6.3/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/iam/role.py` & `phidata-1.6.3/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.6.3/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/rds/db_instance.py` & `phidata-1.6.3/phidata/aws/resource/rds/db_instance.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.6.3/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/s3/bucket.py` & `phidata-1.6.3/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/secret/manager.py` & `phidata-1.6.3/phidata/aws/resource/secret/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/types.py` & `phidata-1.6.3/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/resource/utils.py` & `phidata-1.6.3/phidata/aws/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/s3/csv_dataset.py` & `phidata-1.6.3/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/s3/dataset.py` & `phidata-1.6.3/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/s3/dataset_base.py` & `phidata-1.6.3/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/s3/object.py` & `phidata-1.6.3/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/aws/worker.py` & `phidata-1.6.3/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/base.py` & `phidata-1.6.3/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/checks/check.py` & `phidata-1.6.3/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/checks/not_empty.py` & `phidata-1.6.3/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/constants.py` & `phidata-1.6.3/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/decorators/timer.py` & `phidata-1.6.3/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/decorators/validate_env.py` & `phidata-1.6.3/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/api_client.py` & `phidata-1.6.3/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/args.py` & `phidata-1.6.3/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/config.py` & `phidata-1.6.3/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/enums.py` & `phidata-1.6.3/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/manager.py` & `phidata-1.6.3/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/base.py` & `phidata-1.6.3/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/container.py` & `phidata-1.6.3/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/group.py` & `phidata-1.6.3/phidata/docker/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/image.py` & `phidata-1.6.3/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/network.py` & `phidata-1.6.3/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/types.py` & `phidata-1.6.3/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/utils.py` & `phidata-1.6.3/phidata/docker/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/resource/volume.py` & `phidata-1.6.3/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/utils/container.py` & `phidata-1.6.3/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/docker/worker.py` & `phidata-1.6.3/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/infra/args.py` & `phidata-1.6.3/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/infra/config.py` & `phidata-1.6.3/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/infra/resource.py` & `phidata-1.6.3/phidata/infra/resource.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/api_client.py` & `phidata-1.6.3/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/args.py` & `phidata-1.6.3/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/config.py` & `phidata-1.6.3/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.3/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.6.3/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/common/port.py` & `phidata-1.6.3/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/container.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/secret.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/service.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/core/v1/volume.py` & `phidata-1.6.3/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.6.3/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/group.py` & `phidata-1.6.3/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/kubeconfig.py` & `phidata-1.6.3/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.6.3/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.3/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.3/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/enums/api_version.py` & `phidata-1.6.3/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/enums/kind.py` & `phidata-1.6.3/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/enums/manager_status.py` & `phidata-1.6.3/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/enums/pv.py` & `phidata-1.6.3/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/manager.py` & `phidata-1.6.3/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.6.3/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.6.3/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/base.py` & `phidata-1.6.3/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/container.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/service.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.6.3/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/group.py` & `phidata-1.6.3/phidata/k8s/resource/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/kubeconfig.py` & `phidata-1.6.3/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.6.3/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.6.3/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.6.3/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.6.3/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.6.3/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/types.py` & `phidata-1.6.3/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/resource/utils.py` & `phidata-1.6.3/phidata/k8s/resource/utils.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/utils/pod.py` & `phidata-1.6.3/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/k8s/worker.py` & `phidata-1.6.3/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/agent.py` & `phidata-1.6.3/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/chain.py` & `phidata-1.6.3/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/connection.py` & `phidata-1.6.3/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/loader.py` & `phidata-1.6.3/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/query.py` & `phidata-1.6.3/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/llm/duckdb/tool.py` & `phidata-1.6.3/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/product/data_product.py` & `phidata-1.6.3/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/local/csv.py` & `phidata-1.6.3/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/local/local_table.py` & `phidata-1.6.3/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/local/parquet.py` & `phidata-1.6.3/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/s3/csv.py` & `phidata-1.6.3/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/s3/parquet.py` & `phidata-1.6.3/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/s3/s3_table.py` & `phidata-1.6.3/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/sql/postgres.py` & `phidata-1.6.3/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/table/sql/sql_table.py` & `phidata-1.6.3/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/aws/athena/run_query.py` & `phidata-1.6.3/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/aws/emr/create_cluster.py` & `phidata-1.6.3/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.6.3/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/aws/glue/start_crawler.py` & `phidata-1.6.3/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/decorator.py` & `phidata-1.6.3/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/download/s3/to_file.py` & `phidata-1.6.3/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/download/url/to_file.py` & `phidata-1.6.3/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/download/url/to_s3.py` & `phidata-1.6.3/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/download/url/to_sql.py` & `phidata-1.6.3/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/plot/sql/query.py` & `phidata-1.6.3/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/python_task.py` & `phidata-1.6.3/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/run/sql/query.py` & `phidata-1.6.3/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/task.py` & `phidata-1.6.3/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/task_relatives.py` & `phidata-1.6.3/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/upload/file/to_s3.py` & `phidata-1.6.3/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/task/upload/file/to_sql.py` & `phidata-1.6.3/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/types/airflow.py` & `phidata-1.6.3/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/types/context.py` & `phidata-1.6.3/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/types/phidata_runtime.py` & `phidata-1.6.3/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/cli_console.py` & `phidata-1.6.3/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/common.py` & `phidata-1.6.3/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/compare.py` & `phidata-1.6.3/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/context.py` & `phidata-1.6.3/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/dttm.py` & `phidata-1.6.3/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/enums.py` & `phidata-1.6.3/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/env_file.py` & `phidata-1.6.3/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/env_var.py` & `phidata-1.6.3/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/filesystem.py` & `phidata-1.6.3/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/log.py` & `phidata-1.6.3/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/prep_infra_config.py` & `phidata-1.6.3/phidata/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/print_table.py` & `phidata-1.6.3/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/utils/workspace_path.py` & `phidata-1.6.3/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/workflow/decorator.py` & `phidata-1.6.3/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/workflow/workflow.py` & `phidata-1.6.3/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/workflow/workflow_relatives.py` & `phidata-1.6.3/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/workspace/config.py` & `phidata-1.6.3/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.6.2/phidata/workspace/settings.py` & `phidata-1.6.3/phidata/workspace/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     #
     dev_airbyte_enabled: bool = False
     dev_airflow_enabled: bool = False
     dev_api_enabled: bool = False
     dev_app_enabled: bool = False
     dev_assistant_enabled: bool = False
     dev_databox_enabled: bool = False
+    dev_db_enabled: bool = False
     dev_grafana_enabled: bool = False
     dev_jupyter_enabled: bool = False
     dev_mysql_enabled: bool = False
     dev_postgres_enabled: bool = False
     dev_prometheus_enabled: bool = False
     dev_redis_enabled: bool = False
     dev_spark_enabled: bool = False
@@ -66,14 +67,15 @@
     #
     stg_airbyte_enabled: bool = False
     stg_airflow_enabled: bool = False
     stg_api_enabled: bool = False
     stg_app_enabled: bool = False
     stg_assistant_enabled: bool = False
     stg_databox_enabled: bool = False
+    stg_db_enabled: bool = False
     stg_grafana_enabled: bool = False
     stg_jupyter_enabled: bool = False
     stg_mysql_enabled: bool = False
     stg_postgres_enabled: bool = False
     stg_prometheus_enabled: bool = False
     stg_redis_enabled: bool = False
     stg_spark_enabled: bool = False
@@ -97,14 +99,15 @@
     #
     prd_airbyte_enabled: bool = False
     prd_airflow_enabled: bool = False
     prd_api_enabled: bool = False
     prd_app_enabled: bool = False
     prd_assistant_enabled: bool = False
     prd_databox_enabled: bool = False
+    prd_db_enabled: bool = False
     prd_grafana_enabled: bool = False
     prd_jupyter_enabled: bool = False
     prd_mysql_enabled: bool = False
     prd_postgres_enabled: bool = False
     prd_prometheus_enabled: bool = False
     prd_redis_enabled: bool = False
     prd_spark_enabled: bool = False
```

### Comparing `phidata-1.6.2/phidata.egg-info/PKG-INFO` & `phidata-1.6.3/phidata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.6.2
+Version: 1.6.3
 Summary: Building blocks for Data Engineering
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://www.phidata.com
 Project-URL: documentation, https://www.docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.6.2 Summary: Building blocks for
+Metadata-Version: 2.1 Name: phidata Version: 1.6.3 Summary: Building blocks for
 Data Engineering Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://www.phidata.com Project-URL:
 documentation, https://www.docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
                      Building Blocks for Data Engineering
```

### Comparing `phidata-1.6.2/phidata.egg-info/SOURCES.txt` & `phidata-1.6.3/phidata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 phidata/app/prometheus/__init__.py
 phidata/app/prometheus/prometheus.py
 phidata/app/redis/__init__.py
 phidata/app/redis/redis.py
 phidata/app/redis/stack.py
 phidata/app/server/__init__.py
 phidata/app/server/api_server.py
-phidata/app/server/app_server.py
 phidata/app/server/server_base.py
 phidata/app/spark/__init__.py
 phidata/app/spark/spark_base.py
 phidata/app/spark/spark_driver.py
 phidata/app/spark/spark_worker.py
 phidata/app/streamlit/__init__.py
 phidata/app/streamlit/streamlit.py
```

### Comparing `phidata-1.6.2/pyproject.toml` & `phidata-1.6.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "phidata"
-version = "1.6.2"
+version = "1.6.3"
 description = "Building blocks for Data Engineering"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3",
-  "phiterm==1.6.2",
+  "phiterm==1.6.3",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
@@ -54,16 +54,14 @@
   "git",
   "setuptools",
   "boto3",
   "boto3.*",
   "botocore",
   "botocore.*",
   "duckdb.*",
-  "typer",
-  "tiingo",
   "docker.*",
   "airflow.*",
   "pandas.*",
   "pyarrow.*",
   "kubernetes.*",
   "langchain.*",
   "sqlalchemy.*",
```

