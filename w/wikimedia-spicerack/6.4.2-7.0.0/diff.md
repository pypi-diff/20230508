# Comparing `tmp/wikimedia-spicerack-6.4.2.tar.gz` & `tmp/wikimedia-spicerack-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimedia-spicerack-6.4.2.tar", last modified: Mon Apr 17 16:46:52 2023, max compression
+gzip compressed data, was "wikimedia-spicerack-7.0.0.tar", last modified: Mon May  8 16:46:43 2023, max compression
```

## Comparing `wikimedia-spicerack-6.4.2.tar` & `wikimedia-spicerack-7.0.0.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.518626 wikimedia-spicerack-6.4.2/
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/.git-blame-ignore-revs
--rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/.mailmap
--rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)   104056 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-04-17 16:46:52.519043 wikimedia-spicerack-6.4.2/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.255108 wikimedia-spicerack-6.4.2/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.256811 wikimedia-spicerack-6.4.2/doc/examples/
--rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/examples/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.332229 wikimedia-spicerack-6.4.2/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.334326 wikimedia-spicerack-6.4.2/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/_static/theme_overrides.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.795046 wikimedia-spicerack-6.4.2/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.administrative.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.alerting.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.alertmanager.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.apt.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.confctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.debmonitor.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.dhcp.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.dnsdisc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.elasticsearch_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.ganeti.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.icinga.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.ipmi.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.k8s.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.kafka.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mediawiki.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mysql.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mysql_legacy.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.netbox.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.peeringdb.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.puppet.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.redfish.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.redis_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.remote.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.reposync.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.service.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.toolforge.etcdctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.toolforge.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.typing.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     6670 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/configuration.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/development.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/docutils.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     9468 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/pyproject.toml
--rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-04-17 16:46:52.624861 wikimedia-spicerack-6.4.2/setup.cfg
--rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/setup.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.379719 wikimedia-spicerack-6.4.2/spicerack/
--rw-r--r--   0 riccardo   (501) staff       (20)    27361 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3900 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_log.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_menu.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_module_api.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3869 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13849 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.2/spicerack/redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27921 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.386947 wikimedia-spicerack-6.4.2/spicerack/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.562800 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.566876 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/
--rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/schema.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.569476 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config/valid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_bad_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_empty_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_wrong_overrides.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:48.993912 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.622925 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.803489 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
--rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
--rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
--rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.828194 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/
--rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.899697 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.919420 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
--rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.159012 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
--rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.164216 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.255261 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
--rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
--rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
--rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
--rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
--rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
--rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
--rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.259270 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/root.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.263743 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/debmonitor/
--rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/debmonitor/config.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.266512 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/discovery/
--rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/discovery/authdns.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.267939 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/elasticsearch/
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/elasticsearch/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.000014 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.271368 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
--rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.297131 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.377228 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/
--rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.386252 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
--rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_extender.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.410001 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/404.json
--rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/bogus.json
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/info.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/instance.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.671811 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/
--rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_downtimed.json
--rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_invalid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_missing.json
--rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_valid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.749223 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/kafka/
--rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/kafka/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.758503 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/netbox/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/netbox/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.804776 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/
--rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/asn.json
--rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/ixlan.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.807678 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/phabricator/valid.conf
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.810737 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/redis_cluster/
--rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/redis_cluster/cluster.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.815176 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/config_installer.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.817549 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/reposync/
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/reposync/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.838797 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/
--rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/service.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.378280 wikimedia-spicerack-6.4.2/spicerack/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4574 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__log.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5416 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18840 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15541 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14385 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_init.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    22477 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.380167 wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/test_etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.433410 wikimedia-spicerack-6.4.2/spicerack/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/toolforge/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/toolforge/etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/typing.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.440156 wikimedia-spicerack-6.4.2/utils/
--rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/utils/check-style.sh
--rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/utils/format-code.sh
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.517573 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/entry_points.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.688488 wikimedia-spicerack-7.0.0/
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/.git-blame-ignore-revs
+-rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/.mailmap
+-rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)   105356 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.0.0/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-08 16:46:43.688860 wikimedia-spicerack-7.0.0/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.880379 wikimedia-spicerack-7.0.0/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.881397 wikimedia-spicerack-7.0.0/doc/examples/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/examples/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.899994 wikimedia-spicerack-7.0.0/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.906083 wikimedia-spicerack-7.0.0/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/_static/theme_overrides.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.070043 wikimedia-spicerack-7.0.0/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.administrative.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.alerting.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.alertmanager.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.apt.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.confctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.debmonitor.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.dhcp.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.dnsdisc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.elasticsearch_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.ganeti.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.icinga.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.ipmi.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.k8s.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.kafka.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mediawiki.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mysql.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.mysql_legacy.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.netbox.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.peeringdb.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.puppet.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.redfish.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.redis_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.remote.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.reposync.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.service.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.toolforge.etcdctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.toolforge.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/api/spicerack.typing.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/configuration.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/doc/source/development.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/docutils.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.0.0/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     9572 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/pyproject.toml
+-rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-05-08 16:46:43.697942 wikimedia-spicerack-7.0.0/setup.cfg
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/setup.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.272551 wikimedia-spicerack-7.0.0/spicerack/
+-rw-r--r--   0 riccardo   (501) staff       (20)    27623 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/_log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_menu.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/_module_api.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3949 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10442 2023-05-04 08:02:07.000000 wikimedia-spicerack-7.0.0/spicerack/dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13883 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.0.0/spicerack/redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27921 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.298973 wikimedia-spicerack-7.0.0/spicerack/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.313471 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.317026 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/
+-rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/schema.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.318224 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config/valid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.812885 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.337922 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.367670 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.377674 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.384063 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.406166 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.444137 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.445600 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.448918 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.452151 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.454216 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/debmonitor/
+-rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/debmonitor/config.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.455480 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/discovery/
+-rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/discovery/authdns.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.461750 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/elasticsearch/
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/elasticsearch/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:42.819426 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.474676 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
+-rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.477553 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.482027 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/
+-rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.484877 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.508703 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/404.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/bogus.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/info.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/instance.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.525046 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/
+-rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_downtimed.json
+-rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_invalid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_missing.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_valid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.526160 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/kafka/
+-rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/kafka/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.527086 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/netbox/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/netbox/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.529189 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/
+-rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/asn.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/ixlan.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.530154 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/phabricator/valid.conf
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.531094 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/redis_cluster/
+-rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.533049 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/remote/config_installer.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.534033 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/reposync/
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/reposync/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.534964 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/service.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.639110 wikimedia-spicerack-7.0.0/spicerack/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5648 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18840 2023-05-04 08:02:07.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15575 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14445 2023-05-08 16:29:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_init.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    22477 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.651438 wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/test_etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.0.0/spicerack/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.661640 wikimedia-spicerack-7.0.0/spicerack/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.0.0/spicerack/toolforge/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/toolforge/etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.0.0/spicerack/typing.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.0.0/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.675764 wikimedia-spicerack-7.0.0/utils/
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/utils/check-style.sh
+-rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.0.0/utils/format-code.sh
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-08 16:46:43.687783 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/entry_points.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-05-08 16:46:42.000000 wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/top_level.txt
```

### Comparing `wikimedia-spicerack-6.4.2/.mailmap` & `wikimedia-spicerack-7.0.0/.mailmap`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/CHANGELOG.rst` & `wikimedia-spicerack-7.0.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,43 @@
 Spicerack Changelog
 -------------------
 
+`v7.0.0`_ (2023-05-08)
+^^^^^^^^^^^^^^^^^^^^^^
+
+API breaking changes
+""""""""""""""""""""
+
+* spicerack: refactor IRC logging:
+
+  * Rename the existing ``irc_logger`` to ``sal_logger`` as it logs to IRC with the ``!log`` and hence to SAL.
+  * Add a new ``irc_logger`` property to log to IRC on the ``#wikimedia-operations`` channel without the ``!log``
+    prefix to just log to IRC and not SAL.
+
+Bug fixes
+"""""""""
+
+* doc: do not load UI fix when building the manpage.
+
+`v6.4.3`_ (2023-05-08)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+* ganeti: enable ``--no-wait-for-sync`` by default for the virtual machine creation command.
+
+Bug fixes
+"""""""""
+
+* decorators: fix ``dry_run`` detection that had a bug in the case of a function with a ``dry_run`` argument with a
+  default value. The default value was used also in the presence of a an explicit value set by the caller (`T335855`_).
+* doc: fix search in documentation as ``jQuery`` is not automatically loaded by the rtd theme.
+* doc: Remove extra preceding space in intro example.
+
 `v6.4.2`_ (2023-04-17)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Minor improvements
 """"""""""""""""""
 
 * kafka: remove setting to avoid checking the hostname in TLS certs as all clusters in production are now running
@@ -2452,14 +2485,15 @@
 .. _`T315537`: https://phabricator.wikimedia.org/T315537
 .. _`T319277`: https://phabricator.wikimedia.org/T319277
 .. _`T319401`: https://phabricator.wikimedia.org/T319401
 .. _`T320696`: https://phabricator.wikimedia.org/T320696
 .. _`T325168`: https://phabricator.wikimedia.org/T325168
 .. _`T329773`: https://phabricator.wikimedia.org/T329773
 .. _`T330318`: https://phabricator.wikimedia.org/T330318
+.. _`T335855`: https://phabricator.wikimedia.org/T335855
 
 .. _`v0.0.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.1
 .. _`v0.0.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.2
 .. _`v0.0.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.3
 .. _`v0.0.4`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.4
 .. _`v0.0.5`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.5
 .. _`v0.0.6`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v0.0.6
@@ -2550,7 +2584,9 @@
 .. _`v6.2.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.0
 .. _`v6.2.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.1
 .. _`v6.2.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.2
 .. _`v6.3.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.3.0
 .. _`v6.4.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.0
 .. _`v6.4.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.1
 .. _`v6.4.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.2
+.. _`v6.4.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.3
+.. _`v7.0.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.0.0
```

### Comparing `wikimedia-spicerack-6.4.2/LICENSE` & `wikimedia-spicerack-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/PKG-INFO` & `wikimedia-spicerack-7.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 6.4.2
+Version: 7.0.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-6.4.2/doc/Makefile` & `wikimedia-spicerack-7.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/examples/config.yaml` & `wikimedia-spicerack-7.0.0/doc/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/source/api/index.rst` & `wikimedia-spicerack-7.0.0/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/source/conf.py` & `wikimedia-spicerack-7.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use pathlib's resolve() to make it absolute, like shown here.
 #
+import os
 import sys
 from datetime import date
 from pathlib import Path
 
 import sphinx_rtd_theme
 from pkg_resources import get_distribution
 
@@ -37,14 +38,16 @@
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
     "sphinx_autodoc_typehints",
     "sphinxarg.ext",
 ]
+if not os.environ.get("PYBUILD_NAME", ""):
+    extensions.append("sphinxcontrib.jquery")
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `wikimedia-spicerack-6.4.2/doc/source/configuration.rst` & `wikimedia-spicerack-7.0.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/source/development.rst` & `wikimedia-spicerack-7.0.0/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/source/installation.rst` & `wikimedia-spicerack-7.0.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/doc/source/introduction.rst` & `wikimedia-spicerack-7.0.0/doc/source/introduction.rst`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,18 @@
 ^^^^^^^
 
 The logging is already pre-setup by the ``cookbook`` entry point script that initialize the root logger, so that each
 cookbook can just initialize its own :py:mod:`logging` instance and log.
 
 A special logger to send notification to the ``#wikimedia-operations`` IRC channel with the ``!log`` prefix is also
 available through the ``spicerack`` argument, passed to the cookbook's ``run()`` function for the module API or
-available in the cookbook class as ``self.spicerack`` for the class API, in its ``irc_logger`` property.
+available in the cookbook class as ``self.spicerack`` for the class API, in its ``sal_logger`` property. An additional
+``irc_logger`` logger is also available to just write to the ``#wikimedia-operations`` IRC channel.
 
-The ``irc_logger`` logs to both IRC and the nomal log outputs of Spicerack. If the dry-run mode is set it does not log
+Both IRC loggers log to both IRC and the nomal log outputs of Spicerack. If the dry-run mode is set it does not log
 to IRC.
 
 Log files
 """""""""
 
 The log files can be found in ``/var/log/spicerack/${PATH_OF_THE_COOKBOOK}`` on the host where the cookbooks are run.
 All normal log messages are sent to two separate files, of which one always logs at ``DEBUG`` level even if
@@ -195,23 +196,23 @@
 Example
 """""""
 
 ::
 
    import logging
 
-    logger = logging.getLogger(__name__)
+   logger = logging.getLogger(__name__)
 
-    logger.info('message')  # this goes to stdout in the operator shell and is logged in both files.
-    logger.debug('message') # this goes to stdout in the operator shell only if -v/--verbose is set and is logged only
-                            # in the extended file.
-
-    def run(args, spicerack):
-        spicerack.irc_logger.info('message')  # This sends a message to the #wikimedia-operation IRC channel with:
-                                              # !log user@host message
+   logger.info('message')  # this goes to stdout in the operator shell and is logged in both files.
+   logger.debug('message') # this goes to stdout in the operator shell only if -v/--verbose is set and is logged only
+                           # in the extended file.
+
+   def run(args, spicerack):
+       spicerack.irc_logger.info('message')  # This sends a message to the #wikimedia-operation IRC channel with:
+                                             # !log user@host message
 
 Spicerack library
 ^^^^^^^^^^^^^^^^^
 
 All the available modules in the Spicerack package are exposed to the cookbooks through the ``spicerack`` instance
 injected in the cookbook. It offers helper methods to obtain initialized instances of all the available libraries.
 This instance exposes also some of the global CLI arguments parsed by the ``cookbook`` entry point script such as
```

### Comparing `wikimedia-spicerack-6.4.2/prospector.yaml` & `wikimedia-spicerack-7.0.0/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/setup.cfg` & `wikimedia-spicerack-7.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/setup.py` & `wikimedia-spicerack-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/__init__.py` & `wikimedia-spicerack-7.0.0/spicerack/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from wmflib.actions import ActionsDict
 from wmflib.config import load_ini_config, load_yaml_config
 from wmflib.dns import Dns
 from wmflib.interactive import get_username
 from wmflib.phabricator import Phabricator, create_phabricator
 from wmflib.prometheus import Prometheus, Thanos
 
-from spicerack._log import irc_logger
+from spicerack._log import irc_logger, sal_logger
 from spicerack.administrative import Reason
 from spicerack.alerting import AlertingHosts
 from spicerack.alertmanager import Alertmanager, AlertmanagerHosts
 from spicerack.apt import AptGetHosts
 from spicerack.confctl import Confctl, ConftoolEntity
 from spicerack.debmonitor import Debmonitor
 from spicerack.dhcp import DHCP
@@ -116,14 +116,15 @@
         self._debmonitor_config = debmonitor_config
         self._spicerack_config_dir = Path(spicerack_config_dir)
         self._get_cookbook_callback = get_cookbook_callback
 
         self._username = get_username()
         self._current_hostname = gethostname()
         self._irc_logger = irc_logger
+        self._sal_logger = sal_logger
         self._confctl: Optional[Confctl] = None
         self._service_catalog: Optional[Catalog] = None
         self._management_password: str = ""
         self._actions = ActionsDict()
         self._authdns_servers: dict[str, str] = {}
 
         self._extender = None
@@ -186,18 +187,23 @@
         if not self._http_proxy:
             return None
 
         return {"http": self._http_proxy, "https": self._http_proxy}
 
     @property
     def irc_logger(self) -> Logger:
-        """Returns the logger instance to write to IRC logging to SAL."""
+        """Returns the logger instance to write to IRC in the #wikimedia-operations channel."""
         return self._irc_logger
 
     @property
+    def sal_logger(self) -> Logger:
+        """Returns the logger instance to write to IRC in the #wikimedia-operations and logging to SAL."""
+        return self._sal_logger
+
+    @property
     def actions(self) -> ActionsDict:
         """Returns a dictionary to log and record cookbook actions."""
         return self._actions
 
     @property
     def icinga_master_host(self) -> RemoteHosts:
         """Returns the instance to execute commands on the Icinga master host."""
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/_cookbook.py` & `wikimedia-spicerack-7.0.0/spicerack/_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/_log.py` & `wikimedia-spicerack-7.0.0/spicerack/_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Log module."""
 import logging
 from pathlib import Path
 from typing import Optional
 
-from wmflib.irc import SALSocketHandler
+from wmflib.irc import SALSocketHandler, SocketHandler
 
 root_logger = logging.getLogger()
 irc_logger = logging.getLogger("spicerack_irc_announce")
+sal_logger = logging.getLogger("spicerack_sal_announce")
 
 
 class FilterOutCumin(logging.Filter):
     """A logging output filter to filter out Cumin's logs."""
 
     def filter(self, record: logging.LogRecord) -> bool:
         """Filter out Cumin's log messages.
@@ -83,16 +84,18 @@
 
     root_logger.addHandler(handler)
     root_logger.addHandler(handler_extended)
     root_logger.addHandler(output_handler)
     root_logger.setLevel(logging.DEBUG)
 
     if not dry_run and host is not None and port > 0:
-        irc_logger.addHandler(SALSocketHandler(host, port, user))
+        irc_logger.addHandler(SocketHandler(host, port, user))
         irc_logger.setLevel(logging.INFO)
+        sal_logger.addHandler(SALSocketHandler(host, port, user))
+        sal_logger.setLevel(logging.INFO)
 
     # Silence external noisy loggers
     logging.getLogger("urllib3").setLevel(logging.WARNING)
     logging.getLogger("requests").setLevel(logging.WARNING)
 
     # Elasticsearch lib is very noisy about HTTP level errors
     # ideally, we'd want to keep it at WARNING level for logs
@@ -104,19 +107,19 @@
 def log_task_start(message: str) -> None:
     """Log the start of a task both on the logs and IRC.
 
     Arguments:
         message: the message to be logged.
 
     """
-    irc_logger.info("START - %s", message)
+    sal_logger.info("START - %s", message)
 
 
 def log_task_end(status: str, message: str) -> None:
     """Log the start of a task both on the logs and IRC.
 
     Arguments:
         status: the final status of the task.
         message: the message to be logged.
 
     """
-    irc_logger.info("END (%s) - %s", status, message)
+    sal_logger.info("END (%s) - %s", status, message)
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/_menu.py` & `wikimedia-spicerack-7.0.0/spicerack/_menu.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/_module_api.py` & `wikimedia-spicerack-7.0.0/spicerack/_module_api.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/administrative.py` & `wikimedia-spicerack-7.0.0/spicerack/administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/alerting.py` & `wikimedia-spicerack-7.0.0/spicerack/alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/alertmanager.py` & `wikimedia-spicerack-7.0.0/spicerack/alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/apt.py` & `wikimedia-spicerack-7.0.0/spicerack/apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/confctl.py` & `wikimedia-spicerack-7.0.0/spicerack/confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/cookbook.py` & `wikimedia-spicerack-7.0.0/spicerack/cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/debmonitor.py` & `wikimedia-spicerack-7.0.0/spicerack/debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/decorators.py` & `wikimedia-spicerack-7.0.0/spicerack/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,21 +37,21 @@
     if has_self and (
         getattr(args[0], "_dry_run", False)  # Has self._dry_run
         or getattr(getattr(args[0], "_remote_hosts", False), "_dry_run", False)  # Has self._remote_hosts
     ):
         reduce_tries = True
 
     # When the decorated object is a function or method
-    signature_params = inspect.signature(func).parameters
-    if kwargs.get("dry_run", False) or (  # Has an explicit dry_run parameter that was set in by the caller
-        # Has a dry_run parameter with a default value
-        "dry_run" in signature_params
-        and signature_params["dry_run"].default is True
-    ):
-        reduce_tries = True
+    if "dry_run" in kwargs:  # Has an explicit dry_run parameter that was set in by the caller, use this one
+        if kwargs["dry_run"] is True:
+            reduce_tries = True
+    else:  # Check if has a dry_run parameter with a default value
+        signature_params = inspect.signature(func).parameters
+        if "dry_run" in signature_params and signature_params["dry_run"].default is True:
+            reduce_tries = True
 
     if reduce_tries:
         logger.warning("Reduce tries from %d to 1 in DRY-RUN mode", params.tries)
         params.tries = 1
 
 
 def set_tries(params: RetryParams, _func: Callable, _params: tuple, kwargs: dict) -> None:
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/dhcp.py` & `wikimedia-spicerack-7.0.0/spicerack/dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/dnsdisc.py` & `wikimedia-spicerack-7.0.0/spicerack/dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/elasticsearch_cluster.py` & `wikimedia-spicerack-7.0.0/spicerack/elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/exceptions.py` & `wikimedia-spicerack-7.0.0/spicerack/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/ganeti.py` & `wikimedia-spicerack-7.0.0/spicerack/ganeti.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
             "gnt-instance add"
             " -t drbd"
             " -I hail"
             f" --net 0:link={link}"
             " --hypervisor-parameters=kvm:boot_order=network"
             " -o debootstrap+default"
             " --no-install"
+            " --no-wait-for-sync"
             f" -g {group}"
             f" -B vcpus={vcpus},memory={memory}g"
             f" --disk 0:size={disk}g"
             f" {self._instance}"
         )
 
         logger.info(
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/icinga.py` & `wikimedia-spicerack-7.0.0/spicerack/icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/interactive.py` & `wikimedia-spicerack-7.0.0/spicerack/interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/ipmi.py` & `wikimedia-spicerack-7.0.0/spicerack/ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/k8s.py` & `wikimedia-spicerack-7.0.0/spicerack/k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/kafka.py` & `wikimedia-spicerack-7.0.0/spicerack/kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/mediawiki.py` & `wikimedia-spicerack-7.0.0/spicerack/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/mysql.py` & `wikimedia-spicerack-7.0.0/spicerack/mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/mysql_legacy.py` & `wikimedia-spicerack-7.0.0/spicerack/mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/netbox.py` & `wikimedia-spicerack-7.0.0/spicerack/netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/peeringdb.py` & `wikimedia-spicerack-7.0.0/spicerack/peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/puppet.py` & `wikimedia-spicerack-7.0.0/spicerack/puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/redfish.py` & `wikimedia-spicerack-7.0.0/spicerack/redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/redis_cluster.py` & `wikimedia-spicerack-7.0.0/spicerack/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/remote.py` & `wikimedia-spicerack-7.0.0/spicerack/remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/reposync.py` & `wikimedia-spicerack-7.0.0/spicerack/reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/service.py` & `wikimedia-spicerack-7.0.0/spicerack/service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/__init__.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/schema.yaml` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/confctl/schema.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_extender.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/info.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/info.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/instance.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/ganeti/instance.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_failed_services.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/asn.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/asn.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/ixlan.json` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/peeringdb/ixlan.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/service.yaml` & `wikimedia-spicerack-7.0.0/spicerack/tests/fixtures/service/service.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/sphinx_checker.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__cookbook.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__log.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test__log.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for logfile in tmp_dir.iterdir():
         with open(tmp_dir / logfile, "r") as f:
             assert match in f.read()
 
 
 def _reset_logging_module():
     """Reset the logging module removing all handlers and filters."""
-    for log_logger in (log.root_logger, log.irc_logger):
+    for log_logger in (log.root_logger, log.irc_logger, log.sal_logger):
         list(map(log_logger.removeHandler, log_logger.handlers))
         list(map(log_logger.removeFilter, log_logger.filters))
 
 
 def test_cumin_filter_pass():
     """The FilterOutCumin filter() method should let a normal log record pass."""
     log_filter = log.FilterOutCumin()
@@ -48,22 +48,26 @@
     assert message in caplog.text
     _assert_match_in_tmpdir(message, tmpdir.strpath)
     _reset_logging_module()
 
 
 @mock.patch("wmflib.irc.socket")
 def test_setup_logging_with_irc(mocked_socket, tmpdir, caplog):
-    """Calling setup_logging() with host and port should also setup the IRC logger."""
+    """Calling setup_logging() with host and port should also setup the IRC loggers."""
     log.setup_logging(Path(tmpdir.strpath), "task", "user", host="host", port=123, dry_run=False)
-    message = str(uuid.uuid4())
-    log.irc_logger.info(message)
+    irc_message = str(uuid.uuid4())
+    sal_message = str(uuid.uuid4())
+    log.irc_logger.info(irc_message)
+    log.sal_logger.info(sal_message)
 
     assert mock.call.socket().connect(("host", 123)) in mocked_socket.mock_calls
-    assert message in caplog.text
-    _assert_match_in_tmpdir(message, tmpdir.strpath)
+    assert irc_message in caplog.text
+    assert sal_message in caplog.text
+    _assert_match_in_tmpdir(irc_message, tmpdir.strpath)
+    _assert_match_in_tmpdir(sal_message, tmpdir.strpath)
     _reset_logging_module()
 
 
 def test_setup_logging_dry_run(capsys, tmpdir, caplog):
     """Calling setup_logging() when in dry run mode should setup all the handlers and the stdout with DEBUG level."""
     log.setup_logging(Path(tmpdir.strpath), "task", "user", dry_run=True)
     message = str(uuid.uuid4())
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_administrative.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alerting.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alertmanager.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_apt.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_confctl.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_debmonitor.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_decorators.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,35 @@
 
     sleep_call_count = 2
     if dry_run:
         sleep_call_count = 0
     assert mocked_sleep.call_count == sleep_call_count
 
 
+@pytest.mark.parametrize("dry_run", (True, False, None))
 @mock.patch("wmflib.decorators.time.sleep", return_value=None)
-def test_retry_pass_no_args_dry_run_func(mocked_sleep):
+def test_retry_pass_no_args_dry_run_func(mocked_sleep, dry_run):
     """Using @retry with no arguments should use the default values but set tries to 1 if in DRY-RUN."""
 
     @retry
-    def a_func(dry_run=True):
+    def a_func(*, dry_run=True):
         print(dry_run)
         raise SpicerackError
 
+    kwargs = {}
+    if dry_run is not None:
+        kwargs["dry_run"] = dry_run
+
     with pytest.raises(SpicerackError):
-        a_func()
+        a_func(**kwargs)
 
-    assert not mocked_sleep.called
+    if dry_run is False:
+        assert mocked_sleep.called
+    else:
+        assert not mocked_sleep.called
 
 
 @pytest.mark.parametrize(
     "exc, calls, sleep_calls",
     (
         (SpicerackError, [SpicerackError("error")] * 3, [3.0, 9.0]),
         (Exception, [Exception("error")], []),
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dhcp.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dnsdisc.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_elasticsearch_cluster.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ganeti.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ganeti.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,16 @@
         ]
         self.remote.query.return_value.run_sync.return_value = iter(results)
 
         instance.add(group="row_A", vcpus=2, memory=3, disk=4, link="private")
 
         self.remote.query.return_value.run_sync.assert_called_once_with(
             "gnt-instance add -t drbd -I hail --net 0:link=private --hypervisor-parameters=kvm:boot_order=network "
-            "-o debootstrap+default --no-install -g row_A -B vcpus=2,memory=3g --disk 0:size=4g test.example.com",
+            "-o debootstrap+default --no-install --no-wait-for-sync -g row_A -B vcpus=2,memory=3g --disk 0:size=4g "
+            "test.example.com",
             print_output=True,
         )
 
     @pytest.mark.parametrize(
         "kwargs, exc_message",
         (
             (
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_icinga.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_init.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     assert spicerack.username == "user1"
     assert spicerack.config_dir == get_fixture_path()
     assert spicerack.http_proxy == proxy
     assert spicerack.requests_proxies == {"http": proxy, "https": proxy}
     assert spicerack.authdns_servers == {"authdns1001.example.org": "10.0.0.1", "authdns2001.example.org": "10.0.0.2"}
     assert list(spicerack.authdns_active_hosts.hosts) == ["authdns1001.example.org", "authdns2001.example.org"]
     assert isinstance(spicerack.irc_logger, logging.Logger)
+    assert isinstance(spicerack.sal_logger, logging.Logger)
     assert isinstance(spicerack.actions, ActionsDict)
     assert isinstance(spicerack.remote(), Remote)
     assert isinstance(spicerack.remote(installer=True), Remote)
     assert isinstance(spicerack.confctl("discovery"), ConftoolEntity)
     assert isinstance(spicerack.confctl("mwconfig"), ConftoolEntity)
     assert isinstance(spicerack.dns(), Dns)
     assert isinstance(spicerack.discovery("discovery-record"), Discovery)
```

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_interactive.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ipmi.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_k8s.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_kafka.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mediawiki.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql_legacy.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_netbox.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_peeringdb.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_puppet.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redfish.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redis_cluster.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_remote.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_reposync.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_service.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/test_etcdctl.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/unit/toolforge/test_etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/tests/vulture_whitelist.py` & `wikimedia-spicerack-7.0.0/spicerack/tests/vulture_whitelist.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/spicerack/toolforge/etcdctl.py` & `wikimedia-spicerack-7.0.0/spicerack/toolforge/etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/tox.ini` & `wikimedia-spicerack-7.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/utils/check-style.sh` & `wikimedia-spicerack-7.0.0/utils/check-style.sh`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/PKG-INFO` & `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 6.4.2
+Version: 7.0.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/SOURCES.txt` & `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/requires.txt` & `wikimedia-spicerack-7.0.0/wikimedia_spicerack.egg-info/requires.txt`

 * *Files identical despite different names*

