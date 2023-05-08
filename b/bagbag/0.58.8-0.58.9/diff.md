# Comparing `tmp/bagbag-0.58.8.tar.gz` & `tmp/bagbag-0.58.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.58.8.tar", max compression
+gzip compressed data, was "bagbag-0.58.9.tar", max compression
```

## Comparing `bagbag-0.58.8.tar` & `bagbag-0.58.9.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.58.8/LICENSE
--rw-r--r--   0        0        0    16310 2023-05-03 13:30:21.697775 bagbag-0.58.8/README.md
--rw-r--r--   0        0        0     2152 2023-05-05 05:56:43.422110 bagbag-0.58.8/pyproject.toml
--rw-r--r--   0        0        0      456 2022-12-18 14:46:48.344905 bagbag-0.58.8/src/bagbag/Base64.py
--rw-r--r--   0        0        0     5749 2023-04-18 10:31:59.025703 bagbag-0.58.8/src/bagbag/Cmd.py
--rw-r--r--   0        0        0     2530 2023-04-28 07:15:37.583071 bagbag-0.58.8/src/bagbag/Cryptoo.py
--rw-r--r--   0        0        0     4558 2023-04-27 09:57:17.336471 bagbag-0.58.8/src/bagbag/File.py
--rw-r--r--   0        0        0      951 2023-04-06 11:26:46.488789 bagbag-0.58.8/src/bagbag/Funcs/CutSentence.py
--rw-r--r--   0        0        0    16724 2022-10-11 13:26:11.473001 bagbag-0.58.8/src/bagbag/Funcs/CutSentenceStopWords.py
--rw-r--r--   0        0        0     6790 2023-02-21 10:25:15.382302 bagbag-0.58.8/src/bagbag/Funcs/FakeIdentity.py
--rw-r--r--   0        0        0      515 2023-03-15 05:06:17.699339 bagbag-0.58.8/src/bagbag/Funcs/FileType.py
--rw-r--r--   0        0        0      783 2022-10-16 15:29:21.224299 bagbag-0.58.8/src/bagbag/Funcs/Format.py
--rw-r--r--   0        0        0      825 2022-08-25 08:45:04.248840 bagbag-0.58.8/src/bagbag/Funcs/GetPublicIP.py
--rw-r--r--   0        0        0      253 2022-08-06 09:50:15.275766 bagbag-0.58.8/src/bagbag/Funcs/IPAddressConvert.py
--rw-r--r--   0        0        0      185 2022-12-20 12:28:30.619497 bagbag-0.58.8/src/bagbag/Funcs/Markdown.py
--rw-r--r--   0        0        0     1107 2023-04-06 11:12:42.351012 bagbag-0.58.8/src/bagbag/Funcs/Ping.py
--rw-r--r--   0        0        0     1687 2022-12-25 11:45:41.361813 bagbag-0.58.8/src/bagbag/Funcs/ResizeImage.py
--rw-r--r--   0        0        0       70 2022-10-01 18:51:28.539798 bagbag-0.58.8/src/bagbag/Funcs/UUID.py
--rw-r--r--   0        0        0     1415 2023-02-13 06:34:05.155815 bagbag-0.58.8/src/bagbag/Funcs/Wget.py
--rw-r--r--   0        0        0      389 2023-03-15 05:07:00.007727 bagbag-0.58.8/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-26 07:07:50.732472 bagbag-0.58.8/src/bagbag/Hash.py
--rw-r--r--   0        0        0    13466 2023-04-24 16:25:51.632962 bagbag-0.58.8/src/bagbag/Http.py
--rw-r--r--   0        0        0     1628 2023-01-12 10:33:44.123536 bagbag-0.58.8/src/bagbag/Json.py
--rw-r--r--   0        0        0    10860 2022-12-22 06:05:36.078005 bagbag-0.58.8/src/bagbag/Lg.py
--rw-r--r--   0        0        0     2055 2022-08-18 13:37:24.221488 bagbag-0.58.8/src/bagbag/Math.py
--rw-r--r--   0        0        0     1665 2023-04-14 07:49:40.462303 bagbag-0.58.8/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     3050 2023-03-23 13:34:08.290027 bagbag-0.58.8/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     1022 2023-01-26 18:08:40.527831 bagbag-0.58.8/src/bagbag/Process.py
--rw-r--r--   0        0        0      962 2022-11-30 19:42:40.659521 bagbag-0.58.8/src/bagbag/Python.py
--rw-r--r--   0        0        0      611 2022-10-07 15:25:00.730045 bagbag-0.58.8/src/bagbag/Random.py
--rw-r--r--   0        0        0     4951 2023-04-25 15:43:10.177547 bagbag-0.58.8/src/bagbag/Socket/TCP.py
--rw-r--r--   0        0        0       17 2022-08-05 14:47:59.523595 bagbag-0.58.8/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0    15867 2023-04-24 15:52:44.638080 bagbag-0.58.8/src/bagbag/String.py
--rw-r--r--   0        0        0      439 2022-08-10 11:11:23.471024 bagbag-0.58.8/src/bagbag/Thread.py
--rw-r--r--   0        0        0     4686 2023-04-06 11:26:37.528262 bagbag-0.58.8/src/bagbag/Time.py
--rw-r--r--   0        0        0     2396 2022-09-16 08:58:48.233364 bagbag-0.58.8/src/bagbag/Tools/Argparser.py
--rw-r--r--   0        0        0     2572 2023-04-10 05:27:14.813130 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py
--rw-r--r--   0        0        0      918 2023-02-14 12:53:32.011975 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py
--rw-r--r--   0        0        0       68 2023-04-09 15:54:13.555282 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0       36 2023-02-20 11:29:39.344076 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      272 2023-02-20 11:33:21.209236 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0       53 2023-02-06 12:12:49.206521 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    23137 2023-04-06 11:30:14.742190 bagbag-0.58.8/src/bagbag/Tools/BlockChain/Tron/tron.py
--rw-r--r--   0        0        0       65 2023-02-20 11:35:34.074298 bagbag-0.58.8/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3041 2023-02-13 06:23:00.196283 bagbag-0.58.8/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     3833 2023-04-25 13:07:57.003030 bagbag-0.58.8/src/bagbag/Tools/Chan.py
--rw-r--r--   0        0        0    32184 2023-05-05 05:53:40.244510 bagbag-0.58.8/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3274 2022-09-15 08:56:37.350792 bagbag-0.58.8/src/bagbag/Tools/Crontab.py
--rw-r--r--   0        0        0    33457 2023-03-29 10:41:45.581869 bagbag-0.58.8/src/bagbag/Tools/Database.py
--rw-r--r--   0        0        0     5342 2023-02-15 08:29:18.848798 bagbag-0.58.8/src/bagbag/Tools/DistributedLock.py
--rw-r--r--   0        0        0     4700 2023-01-19 11:17:18.748095 bagbag-0.58.8/src/bagbag/Tools/Elasticsearch.py
--rw-r--r--   0        0        0     4441 2023-01-17 15:18:13.958863 bagbag-0.58.8/src/bagbag/Tools/Github.py
--rw-r--r--   0        0        0     1398 2023-03-17 07:42:12.672824 bagbag-0.58.8/src/bagbag/Tools/JavaScript.py
--rw-r--r--   0        0        0     2201 2023-03-08 07:11:22.568544 bagbag-0.58.8/src/bagbag/Tools/Kafka.py
--rw-r--r--   0        0        0     1975 2023-05-04 17:08:07.122161 bagbag-0.58.8/src/bagbag/Tools/Lock.py
--rw-r--r--   0        0        0     6734 2023-01-16 07:23:53.117189 bagbag-0.58.8/src/bagbag/Tools/MatrixBot.py
--rw-r--r--   0        0        0      413 2022-12-27 07:28:58.688307 bagbag-0.58.8/src/bagbag/Tools/Nslookup.py
--rw-r--r--   0        0        0     2430 2023-05-03 13:29:38.917729 bagbag-0.58.8/src/bagbag/Tools/OCR.py
--rw-r--r--   0        0        0     2763 2023-02-12 16:33:24.414810 bagbag-0.58.8/src/bagbag/Tools/ProgressBar.py
--rw-r--r--   0        0        0     1607 2023-02-02 12:01:54.298178 bagbag-0.58.8/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3281 2023-02-13 05:16:20.084875 bagbag-0.58.8/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0       75 2023-01-08 14:37:29.001741 bagbag-0.58.8/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4670 2023-02-02 11:59:41.614890 bagbag-0.58.8/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2669 2022-12-25 18:30:26.203387 bagbag-0.58.8/src/bagbag/Tools/Queue.py
--rw-r--r--   0        0        0     2364 2022-12-21 11:16:06.096822 bagbag-0.58.8/src/bagbag/Tools/RSS/Feed.py
--rw-r--r--   0        0        0      608 2022-12-20 13:54:34.868627 bagbag-0.58.8/src/bagbag/Tools/RSS/Opml.py
--rw-r--r--   0        0        0       63 2022-12-20 13:51:52.113940 bagbag-0.58.8/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3734 2023-02-01 12:01:16.040605 bagbag-0.58.8/src/bagbag/Tools/Ratelimit.py
--rw-r--r--   0        0        0    18528 2023-03-08 07:40:25.704818 bagbag-0.58.8/src/bagbag/Tools/Redis.py
--rw-r--r--   0        0        0     5584 2023-03-14 17:28:24.607245 bagbag-0.58.8/src/bagbag/Tools/SSH.py
--rw-r--r--   0        0        0    32081 2023-03-22 05:32:28.072104 bagbag-0.58.8/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    24493 2023-04-27 09:55:24.505212 bagbag-0.58.8/src/bagbag/Tools/Telegram.py
--rw-r--r--   0        0        0    14070 2022-10-11 17:50:44.936863 bagbag-0.58.8/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     3205 2023-04-26 11:42:55.114246 bagbag-0.58.8/src/bagbag/Tools/TelegramBot.py
--rw-r--r--   0        0        0     5034 2023-04-03 05:37:03.126681 bagbag-0.58.8/src/bagbag/Tools/TelegramBotOfficial.py
--rw-r--r--   0        0        0      142 2023-02-03 16:58:05.049775 bagbag-0.58.8/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     4174 2023-01-20 21:55:20.155790 bagbag-0.58.8/src/bagbag/Tools/Translater.py
--rw-r--r--   0        0        0     9625 2023-03-14 10:07:44.832848 bagbag-0.58.8/src/bagbag/Tools/Twitter/Elevated.py
--rw-r--r--   0        0        0     2026 2023-01-19 08:07:09.796818 bagbag-0.58.8/src/bagbag/Tools/Twitter/Essential.py
--rw-r--r--   0        0        0      115 2023-02-10 11:22:25.584307 bagbag-0.58.8/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3069 2023-01-10 07:22:39.926298 bagbag-0.58.8/src/bagbag/Tools/URL.py
--rw-r--r--   0        0        0      706 2022-09-22 12:55:34.535377 bagbag-0.58.8/src/bagbag/Tools/WaitGroup.py
--rw-r--r--   0        0        0     8073 2023-04-12 13:00:33.539301 bagbag-0.58.8/src/bagbag/Tools/WebCrawler.py
--rw-r--r--   0        0        0     5519 2023-04-26 09:49:53.097526 bagbag-0.58.8/src/bagbag/Tools/WebServer.py
--rw-r--r--   0        0        0     1649 2022-09-29 08:11:47.066310 bagbag-0.58.8/src/bagbag/Tools/XPath.py
--rw-r--r--   0        0        0     3141 2023-02-17 12:39:22.967883 bagbag-0.58.8/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     1298 2023-05-03 13:23:08.445668 bagbag-0.58.8/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0      297 2022-08-07 06:00:20.038297 bagbag-0.58.8/src/bagbag/Tools/orator/__init__.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.038583 bagbag-0.58.8/src/bagbag/Tools/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2022-08-07 06:00:20.038727 bagbag-0.58.8/src/bagbag/Tools/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2022-08-07 06:00:20.038865 bagbag-0.58.8/src/bagbag/Tools/orator/commands/command.py
--rw-r--r--   0        0        0      330 2022-08-07 06:00:20.039098 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2022-08-07 06:00:20.039235 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2022-08-07 06:00:20.039365 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2022-08-07 06:00:20.039505 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2022-08-07 06:00:20.039641 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2022-08-07 06:00:20.039774 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2022-08-07 06:00:20.039842 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2022-08-07 06:00:20.039917 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2022-08-07 06:00:20.040021 bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2022-08-07 06:00:20.040169 bagbag-0.58.8/src/bagbag/Tools/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2022-08-07 06:00:20.040266 bagbag-0.58.8/src/bagbag/Tools/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2022-08-07 06:00:20.040350 bagbag-0.58.8/src/bagbag/Tools/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2022-08-07 06:00:20.040493 bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2022-08-07 06:00:20.040578 bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2022-08-07 06:00:20.040660 bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2022-08-07 06:00:20.040748 bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2022-08-07 06:00:20.040920 bagbag-0.58.8/src/bagbag/Tools/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2022-08-07 06:00:20.041031 bagbag-0.58.8/src/bagbag/Tools/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2022-08-07 06:00:20.041124 bagbag-0.58.8/src/bagbag/Tools/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2022-08-07 06:00:20.041207 bagbag-0.58.8/src/bagbag/Tools/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2022-08-07 06:00:20.041284 bagbag-0.58.8/src/bagbag/Tools/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2022-08-07 06:00:20.041364 bagbag-0.58.8/src/bagbag/Tools/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2022-08-07 06:00:20.041439 bagbag-0.58.8/src/bagbag/Tools/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2022-08-07 06:00:20.041571 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2022-08-07 06:00:20.041658 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2022-08-07 09:41:15.514461 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2022-08-08 19:39:59.546483 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2022-08-07 06:00:20.041888 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2022-08-08 19:41:02.356677 bagbag-0.58.8/src/bagbag/Tools/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2022-08-07 06:00:20.042031 bagbag-0.58.8/src/bagbag/Tools/orator/database_manager.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.042156 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2022-08-07 06:00:20.042224 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2022-08-07 06:00:20.042293 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2022-08-07 06:00:20.042368 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2022-08-07 06:00:20.042446 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2022-08-07 06:00:20.042563 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2022-08-07 06:00:20.042633 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2022-08-07 06:00:20.042698 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2022-08-07 06:00:20.042768 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2022-08-07 06:00:20.042837 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2022-08-07 06:00:20.042961 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.043084 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2022-08-07 06:00:20.043158 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2022-08-07 06:00:20.043230 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.043299 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2022-08-07 06:00:20.043366 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2022-08-07 06:00:20.043436 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2022-08-07 06:00:20.043505 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2022-08-07 06:00:20.043582 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2022-08-07 06:00:20.043657 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2022-08-07 06:00:20.043740 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2022-08-07 06:00:20.043817 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2022-08-07 06:00:20.043891 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2022-08-07 06:00:20.043965 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2022-08-07 06:00:20.044039 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2022-08-07 06:00:20.044104 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2022-08-07 06:00:20.044199 bagbag-0.58.8/src/bagbag/Tools/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2022-08-07 06:00:20.044295 bagbag-0.58.8/src/bagbag/Tools/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2022-08-07 06:00:20.044403 bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2022-08-07 06:00:20.044462 bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2022-08-07 06:00:20.044523 bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2022-08-07 06:00:20.044585 bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2022-08-07 06:00:20.044641 bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2022-08-07 06:00:20.044755 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2022-08-07 06:00:20.044822 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2022-08-07 06:00:20.044893 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2022-08-07 06:00:20.044962 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2022-08-07 06:00:20.045025 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2022-08-07 06:00:20.045084 bagbag-0.58.8/src/bagbag/Tools/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2022-08-07 06:00:20.045189 bagbag-0.58.8/src/bagbag/Tools/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2022-08-07 06:00:20.045255 bagbag-0.58.8/src/bagbag/Tools/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2022-08-07 06:00:20.045316 bagbag-0.58.8/src/bagbag/Tools/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2022-08-07 06:00:20.045377 bagbag-0.58.8/src/bagbag/Tools/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2022-08-07 06:00:20.045436 bagbag-0.58.8/src/bagbag/Tools/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2022-08-07 06:00:20.045540 bagbag-0.58.8/src/bagbag/Tools/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2022-08-07 06:00:20.045606 bagbag-0.58.8/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2022-08-07 06:00:20.045826 bagbag-0.58.8/src/bagbag/Tools/orator/orm/model.py
--rw-r--r--   0        0        0      371 2022-08-07 06:00:20.045999 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2022-08-07 06:00:20.046068 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2022-08-07 06:08:32.255340 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2022-08-07 06:00:20.046219 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2022-08-07 06:00:20.046291 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2022-08-07 06:00:20.046375 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2022-08-07 06:00:20.046441 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2022-08-07 06:00:20.046507 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2022-08-07 06:00:20.046569 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2022-08-07 06:00:20.046631 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2022-08-07 06:00:20.046687 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2022-08-07 06:00:20.046748 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2022-08-07 06:00:20.046819 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2022-08-07 06:00:20.046886 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2022-08-07 06:00:20.046948 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2022-08-07 06:00:20.047011 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2022-08-07 06:00:20.047082 bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2022-08-07 06:00:20.047192 bagbag-0.58.8/src/bagbag/Tools/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2022-08-07 06:00:20.047249 bagbag-0.58.8/src/bagbag/Tools/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2022-08-07 06:00:20.047310 bagbag-0.58.8/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2022-08-07 06:00:20.047371 bagbag-0.58.8/src/bagbag/Tools/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2022-08-07 06:00:20.047490 bagbag-0.58.8/src/bagbag/Tools/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2022-08-07 06:00:20.047576 bagbag-0.58.8/src/bagbag/Tools/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2022-08-07 06:00:20.047639 bagbag-0.58.8/src/bagbag/Tools/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2022-08-07 06:00:20.047708 bagbag-0.58.8/src/bagbag/Tools/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2022-08-07 06:00:20.047810 bagbag-0.58.8/src/bagbag/Tools/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-02-12 15:39:50.939251 bagbag-0.58.8/src/bagbag/Tools/orator/query/builder.py
--rw-r--r--   0        0        0      230 2022-08-07 06:00:20.047933 bagbag-0.58.8/src/bagbag/Tools/orator/query/expression.py
--rw-r--r--   0        0        0      202 2022-08-07 06:00:20.048024 bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2022-08-07 06:00:20.048082 bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2022-08-07 06:00:20.048144 bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2022-08-07 06:00:20.048201 bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2022-08-07 06:00:20.048271 bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2022-08-07 06:00:20.048331 bagbag-0.58.8/src/bagbag/Tools/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2022-08-07 06:00:20.048431 bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2022-08-07 06:00:20.048489 bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2022-08-07 06:00:20.048547 bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2022-08-07 06:00:20.048615 bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2022-08-07 06:00:20.048676 bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2022-08-07 06:00:20.048774 bagbag-0.58.8/src/bagbag/Tools/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2022-08-07 06:00:20.048840 bagbag-0.58.8/src/bagbag/Tools/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2022-08-07 06:00:20.048903 bagbag-0.58.8/src/bagbag/Tools/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2022-08-07 06:00:20.048999 bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2022-08-07 06:00:20.049052 bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2022-08-07 06:00:20.049109 bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2022-08-07 06:00:20.049180 bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2022-08-07 06:00:20.049247 bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2022-08-07 06:00:20.049305 bagbag-0.58.8/src/bagbag/Tools/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2022-08-07 06:00:20.049367 bagbag-0.58.8/src/bagbag/Tools/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2022-08-07 06:00:20.049468 bagbag-0.58.8/src/bagbag/Tools/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.049522 bagbag-0.58.8/src/bagbag/Tools/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2022-08-07 06:00:20.049577 bagbag-0.58.8/src/bagbag/Tools/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2022-08-07 06:00:20.049675 bagbag-0.58.8/src/bagbag/Tools/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2022-08-07 06:00:20.049735 bagbag-0.58.8/src/bagbag/Tools/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2022-08-07 06:00:20.049798 bagbag-0.58.8/src/bagbag/Tools/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2022-08-07 06:00:20.049852 bagbag-0.58.8/src/bagbag/Tools/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2022-08-07 06:00:20.049949 bagbag-0.58.8/src/bagbag/Tools/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2022-08-07 06:00:20.050007 bagbag-0.58.8/src/bagbag/Tools/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2022-08-07 06:00:20.050061 bagbag-0.58.8/src/bagbag/Tools/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2022-08-07 06:00:20.050118 bagbag-0.58.8/src/bagbag/Tools/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2022-08-07 06:00:20.050175 bagbag-0.58.8/src/bagbag/Tools/orator/utils/url.py
--rw-r--r--   0        0        0     3335 2023-04-06 11:06:08.005936 bagbag-0.58.8/src/bagbag/__init__.py
--rw-r--r--   0        0        0    19046 1970-01-01 00:00:00.000000 bagbag-0.58.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.58.9/LICENSE
+-rw-r--r--   0        0        0    16310 2023-05-03 13:30:21.697775 bagbag-0.58.9/README.md
+-rw-r--r--   0        0        0     2152 2023-05-05 17:15:04.292498 bagbag-0.58.9/pyproject.toml
+-rw-r--r--   0        0        0      456 2022-12-18 14:46:48.344905 bagbag-0.58.9/src/bagbag/Base64.py
+-rw-r--r--   0        0        0     5749 2023-04-18 10:31:59.025703 bagbag-0.58.9/src/bagbag/Cmd.py
+-rw-r--r--   0        0        0     2530 2023-04-28 07:15:37.583071 bagbag-0.58.9/src/bagbag/Cryptoo.py
+-rw-r--r--   0        0        0     4558 2023-04-27 09:57:17.336471 bagbag-0.58.9/src/bagbag/File.py
+-rw-r--r--   0        0        0      951 2023-04-06 11:26:46.488789 bagbag-0.58.9/src/bagbag/Funcs/CutSentence.py
+-rw-r--r--   0        0        0    16724 2022-10-11 13:26:11.473001 bagbag-0.58.9/src/bagbag/Funcs/CutSentenceStopWords.py
+-rw-r--r--   0        0        0     6790 2023-02-21 10:25:15.382302 bagbag-0.58.9/src/bagbag/Funcs/FakeIdentity.py
+-rw-r--r--   0        0        0      515 2023-03-15 05:06:17.699339 bagbag-0.58.9/src/bagbag/Funcs/FileType.py
+-rw-r--r--   0        0        0      783 2022-10-16 15:29:21.224299 bagbag-0.58.9/src/bagbag/Funcs/Format.py
+-rw-r--r--   0        0        0      825 2022-08-25 08:45:04.248840 bagbag-0.58.9/src/bagbag/Funcs/GetPublicIP.py
+-rw-r--r--   0        0        0      253 2022-08-06 09:50:15.275766 bagbag-0.58.9/src/bagbag/Funcs/IPAddressConvert.py
+-rw-r--r--   0        0        0      185 2022-12-20 12:28:30.619497 bagbag-0.58.9/src/bagbag/Funcs/Markdown.py
+-rw-r--r--   0        0        0     1107 2023-04-06 11:12:42.351012 bagbag-0.58.9/src/bagbag/Funcs/Ping.py
+-rw-r--r--   0        0        0     1687 2022-12-25 11:45:41.361813 bagbag-0.58.9/src/bagbag/Funcs/ResizeImage.py
+-rw-r--r--   0        0        0       70 2022-10-01 18:51:28.539798 bagbag-0.58.9/src/bagbag/Funcs/UUID.py
+-rw-r--r--   0        0        0     1415 2023-02-13 06:34:05.155815 bagbag-0.58.9/src/bagbag/Funcs/Wget.py
+-rw-r--r--   0        0        0      389 2023-03-15 05:07:00.007727 bagbag-0.58.9/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0     1431 2023-04-26 07:07:50.732472 bagbag-0.58.9/src/bagbag/Hash.py
+-rw-r--r--   0        0        0    13466 2023-04-24 16:25:51.632962 bagbag-0.58.9/src/bagbag/Http.py
+-rw-r--r--   0        0        0     1628 2023-01-12 10:33:44.123536 bagbag-0.58.9/src/bagbag/Json.py
+-rw-r--r--   0        0        0    10860 2022-12-22 06:05:36.078005 bagbag-0.58.9/src/bagbag/Lg.py
+-rw-r--r--   0        0        0     2055 2022-08-18 13:37:24.221488 bagbag-0.58.9/src/bagbag/Math.py
+-rw-r--r--   0        0        0     1665 2023-04-14 07:49:40.462303 bagbag-0.58.9/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     3050 2023-03-23 13:34:08.290027 bagbag-0.58.9/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     1022 2023-01-26 18:08:40.527831 bagbag-0.58.9/src/bagbag/Process.py
+-rw-r--r--   0        0        0      962 2022-11-30 19:42:40.659521 bagbag-0.58.9/src/bagbag/Python.py
+-rw-r--r--   0        0        0      611 2022-10-07 15:25:00.730045 bagbag-0.58.9/src/bagbag/Random.py
+-rw-r--r--   0        0        0     4951 2023-04-25 15:43:10.177547 bagbag-0.58.9/src/bagbag/Socket/TCP.py
+-rw-r--r--   0        0        0       17 2022-08-05 14:47:59.523595 bagbag-0.58.9/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0    15867 2023-04-24 15:52:44.638080 bagbag-0.58.9/src/bagbag/String.py
+-rw-r--r--   0        0        0      439 2022-08-10 11:11:23.471024 bagbag-0.58.9/src/bagbag/Thread.py
+-rw-r--r--   0        0        0     4686 2023-04-06 11:26:37.528262 bagbag-0.58.9/src/bagbag/Time.py
+-rw-r--r--   0        0        0     2396 2022-09-16 08:58:48.233364 bagbag-0.58.9/src/bagbag/Tools/Argparser.py
+-rw-r--r--   0        0        0     2572 2023-04-10 05:27:14.813130 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py
+-rw-r--r--   0        0        0      918 2023-02-14 12:53:32.011975 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py
+-rw-r--r--   0        0        0       68 2023-04-09 15:54:13.555282 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0       36 2023-02-20 11:29:39.344076 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      272 2023-02-20 11:33:21.209236 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0       53 2023-02-06 12:12:49.206521 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    23137 2023-04-06 11:30:14.742190 bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/tron.py
+-rw-r--r--   0        0        0       65 2023-02-20 11:35:34.074298 bagbag-0.58.9/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3041 2023-02-13 06:23:00.196283 bagbag-0.58.9/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     3833 2023-04-25 13:07:57.003030 bagbag-0.58.9/src/bagbag/Tools/Chan.py
+-rw-r--r--   0        0        0    32840 2023-05-05 14:45:08.189272 bagbag-0.58.9/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3274 2022-09-15 08:56:37.350792 bagbag-0.58.9/src/bagbag/Tools/Crontab.py
+-rw-r--r--   0        0        0    33457 2023-03-29 10:41:45.581869 bagbag-0.58.9/src/bagbag/Tools/Database.py
+-rw-r--r--   0        0        0     5342 2023-02-15 08:29:18.848798 bagbag-0.58.9/src/bagbag/Tools/DistributedLock.py
+-rw-r--r--   0        0        0     4700 2023-01-19 11:17:18.748095 bagbag-0.58.9/src/bagbag/Tools/Elasticsearch.py
+-rw-r--r--   0        0        0     4441 2023-01-17 15:18:13.958863 bagbag-0.58.9/src/bagbag/Tools/Github.py
+-rw-r--r--   0        0        0     1398 2023-03-17 07:42:12.672824 bagbag-0.58.9/src/bagbag/Tools/JavaScript.py
+-rw-r--r--   0        0        0     2201 2023-03-08 07:11:22.568544 bagbag-0.58.9/src/bagbag/Tools/Kafka.py
+-rw-r--r--   0        0        0     1975 2023-05-04 17:08:07.122161 bagbag-0.58.9/src/bagbag/Tools/Lock.py
+-rw-r--r--   0        0        0     6734 2023-01-16 07:23:53.117189 bagbag-0.58.9/src/bagbag/Tools/MatrixBot.py
+-rw-r--r--   0        0        0      413 2022-12-27 07:28:58.688307 bagbag-0.58.9/src/bagbag/Tools/Nslookup.py
+-rw-r--r--   0        0        0     2430 2023-05-03 13:29:38.917729 bagbag-0.58.9/src/bagbag/Tools/OCR.py
+-rw-r--r--   0        0        0     2763 2023-02-12 16:33:24.414810 bagbag-0.58.9/src/bagbag/Tools/ProgressBar.py
+-rw-r--r--   0        0        0     1607 2023-02-02 12:01:54.298178 bagbag-0.58.9/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3281 2023-02-13 05:16:20.084875 bagbag-0.58.9/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0       75 2023-01-08 14:37:29.001741 bagbag-0.58.9/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4670 2023-02-02 11:59:41.614890 bagbag-0.58.9/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2669 2022-12-25 18:30:26.203387 bagbag-0.58.9/src/bagbag/Tools/Queue.py
+-rw-r--r--   0        0        0     2364 2022-12-21 11:16:06.096822 bagbag-0.58.9/src/bagbag/Tools/RSS/Feed.py
+-rw-r--r--   0        0        0      608 2022-12-20 13:54:34.868627 bagbag-0.58.9/src/bagbag/Tools/RSS/Opml.py
+-rw-r--r--   0        0        0       63 2022-12-20 13:51:52.113940 bagbag-0.58.9/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3734 2023-02-01 12:01:16.040605 bagbag-0.58.9/src/bagbag/Tools/Ratelimit.py
+-rw-r--r--   0        0        0    18528 2023-03-08 07:40:25.704818 bagbag-0.58.9/src/bagbag/Tools/Redis.py
+-rw-r--r--   0        0        0     5584 2023-03-14 17:28:24.607245 bagbag-0.58.9/src/bagbag/Tools/SSH.py
+-rw-r--r--   0        0        0    32178 2023-05-05 17:14:55.298931 bagbag-0.58.9/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    24493 2023-04-27 09:55:24.505212 bagbag-0.58.9/src/bagbag/Tools/Telegram.py
+-rw-r--r--   0        0        0    14070 2022-10-11 17:50:44.936863 bagbag-0.58.9/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     3205 2023-04-26 11:42:55.114246 bagbag-0.58.9/src/bagbag/Tools/TelegramBot.py
+-rw-r--r--   0        0        0     5034 2023-04-03 05:37:03.126681 bagbag-0.58.9/src/bagbag/Tools/TelegramBotOfficial.py
+-rw-r--r--   0        0        0      142 2023-02-03 16:58:05.049775 bagbag-0.58.9/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     4174 2023-01-20 21:55:20.155790 bagbag-0.58.9/src/bagbag/Tools/Translater.py
+-rw-r--r--   0        0        0     9625 2023-03-14 10:07:44.832848 bagbag-0.58.9/src/bagbag/Tools/Twitter/Elevated.py
+-rw-r--r--   0        0        0     2026 2023-01-19 08:07:09.796818 bagbag-0.58.9/src/bagbag/Tools/Twitter/Essential.py
+-rw-r--r--   0        0        0      115 2023-02-10 11:22:25.584307 bagbag-0.58.9/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0     3069 2023-01-10 07:22:39.926298 bagbag-0.58.9/src/bagbag/Tools/URL.py
+-rw-r--r--   0        0        0      706 2022-09-22 12:55:34.535377 bagbag-0.58.9/src/bagbag/Tools/WaitGroup.py
+-rw-r--r--   0        0        0     8073 2023-04-12 13:00:33.539301 bagbag-0.58.9/src/bagbag/Tools/WebCrawler.py
+-rw-r--r--   0        0        0     5519 2023-04-26 09:49:53.097526 bagbag-0.58.9/src/bagbag/Tools/WebServer.py
+-rw-r--r--   0        0        0     1649 2022-09-29 08:11:47.066310 bagbag-0.58.9/src/bagbag/Tools/XPath.py
+-rw-r--r--   0        0        0     3141 2023-02-17 12:39:22.967883 bagbag-0.58.9/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     1298 2023-05-03 13:23:08.445668 bagbag-0.58.9/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0      297 2022-08-07 06:00:20.038297 bagbag-0.58.9/src/bagbag/Tools/orator/__init__.py
+-rw-r--r--   0        0        0       24 2022-08-07 06:00:20.038583 bagbag-0.58.9/src/bagbag/Tools/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2022-08-07 06:00:20.038727 bagbag-0.58.9/src/bagbag/Tools/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2022-08-07 06:00:20.038865 bagbag-0.58.9/src/bagbag/Tools/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2022-08-07 06:00:20.039098 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2022-08-07 06:00:20.039235 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2022-08-07 06:00:20.039365 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2022-08-07 06:00:20.039505 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2022-08-07 06:00:20.039641 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2022-08-07 06:00:20.039774 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2022-08-07 06:00:20.039842 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2022-08-07 06:00:20.039917 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2022-08-07 06:00:20.040021 bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2022-08-07 06:00:20.040169 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2022-08-07 06:00:20.040266 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2022-08-07 06:00:20.040350 bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2022-08-07 06:00:20.040493 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2022-08-07 06:00:20.040578 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2022-08-07 06:00:20.040660 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2022-08-07 06:00:20.040748 bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2022-08-07 06:00:20.040920 bagbag-0.58.9/src/bagbag/Tools/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2022-08-07 06:00:20.041031 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2022-08-07 06:00:20.041124 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2022-08-07 06:00:20.041207 bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2022-08-07 06:00:20.041284 bagbag-0.58.9/src/bagbag/Tools/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2022-08-07 06:00:20.041364 bagbag-0.58.9/src/bagbag/Tools/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2022-08-07 06:00:20.041439 bagbag-0.58.9/src/bagbag/Tools/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2022-08-07 06:00:20.041571 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2022-08-07 06:00:20.041658 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2022-08-07 09:41:15.514461 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2022-08-08 19:39:59.546483 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2022-08-07 06:00:20.041888 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2022-08-08 19:41:02.356677 bagbag-0.58.9/src/bagbag/Tools/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2022-08-07 06:00:20.042031 bagbag-0.58.9/src/bagbag/Tools/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2022-08-07 06:00:20.042156 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2022-08-07 06:00:20.042224 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2022-08-07 06:00:20.042293 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2022-08-07 06:00:20.042368 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2022-08-07 06:00:20.042446 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2022-08-07 06:00:20.042563 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2022-08-07 06:00:20.042633 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2022-08-07 06:00:20.042698 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2022-08-07 06:00:20.042768 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2022-08-07 06:00:20.042837 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2022-08-07 06:00:20.042961 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2022-08-07 06:00:20.043084 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2022-08-07 06:00:20.043158 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2022-08-07 06:00:20.043230 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.043299 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2022-08-07 06:00:20.043366 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2022-08-07 06:00:20.043436 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2022-08-07 06:00:20.043505 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2022-08-07 06:00:20.043582 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2022-08-07 06:00:20.043657 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2022-08-07 06:00:20.043740 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2022-08-07 06:00:20.043817 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2022-08-07 06:00:20.043891 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2022-08-07 06:00:20.043965 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2022-08-07 06:00:20.044039 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2022-08-07 06:00:20.044104 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2022-08-07 06:00:20.044199 bagbag-0.58.9/src/bagbag/Tools/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2022-08-07 06:00:20.044295 bagbag-0.58.9/src/bagbag/Tools/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2022-08-07 06:00:20.044403 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2022-08-07 06:00:20.044462 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2022-08-07 06:00:20.044523 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2022-08-07 06:00:20.044585 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2022-08-07 06:00:20.044641 bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2022-08-07 06:00:20.044755 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2022-08-07 06:00:20.044822 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2022-08-07 06:00:20.044893 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2022-08-07 06:00:20.044962 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2022-08-07 06:00:20.045025 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2022-08-07 06:00:20.045084 bagbag-0.58.9/src/bagbag/Tools/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2022-08-07 06:00:20.045189 bagbag-0.58.9/src/bagbag/Tools/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2022-08-07 06:00:20.045255 bagbag-0.58.9/src/bagbag/Tools/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2022-08-07 06:00:20.045316 bagbag-0.58.9/src/bagbag/Tools/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2022-08-07 06:00:20.045377 bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2022-08-07 06:00:20.045436 bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2022-08-07 06:00:20.045540 bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2022-08-07 06:00:20.045606 bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2022-08-07 06:00:20.045826 bagbag-0.58.9/src/bagbag/Tools/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2022-08-07 06:00:20.045999 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2022-08-07 06:00:20.046068 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2022-08-07 06:08:32.255340 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2022-08-07 06:00:20.046219 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2022-08-07 06:00:20.046291 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2022-08-07 06:00:20.046375 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2022-08-07 06:00:20.046441 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2022-08-07 06:00:20.046507 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2022-08-07 06:00:20.046569 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2022-08-07 06:00:20.046631 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2022-08-07 06:00:20.046687 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2022-08-07 06:00:20.046748 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2022-08-07 06:00:20.046819 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2022-08-07 06:00:20.046886 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2022-08-07 06:00:20.046948 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2022-08-07 06:00:20.047011 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2022-08-07 06:00:20.047082 bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2022-08-07 06:00:20.047192 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2022-08-07 06:00:20.047249 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2022-08-07 06:00:20.047310 bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2022-08-07 06:00:20.047371 bagbag-0.58.9/src/bagbag/Tools/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2022-08-07 06:00:20.047490 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2022-08-07 06:00:20.047576 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2022-08-07 06:00:20.047639 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2022-08-07 06:00:20.047708 bagbag-0.58.9/src/bagbag/Tools/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2022-08-07 06:00:20.047810 bagbag-0.58.9/src/bagbag/Tools/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-02-12 15:39:50.939251 bagbag-0.58.9/src/bagbag/Tools/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2022-08-07 06:00:20.047933 bagbag-0.58.9/src/bagbag/Tools/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2022-08-07 06:00:20.048024 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2022-08-07 06:00:20.048082 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2022-08-07 06:00:20.048144 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2022-08-07 06:00:20.048201 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2022-08-07 06:00:20.048271 bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2022-08-07 06:00:20.048331 bagbag-0.58.9/src/bagbag/Tools/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2022-08-07 06:00:20.048431 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2022-08-07 06:00:20.048489 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2022-08-07 06:00:20.048547 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2022-08-07 06:00:20.048615 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2022-08-07 06:00:20.048676 bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2022-08-07 06:00:20.048774 bagbag-0.58.9/src/bagbag/Tools/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2022-08-07 06:00:20.048840 bagbag-0.58.9/src/bagbag/Tools/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2022-08-07 06:00:20.048903 bagbag-0.58.9/src/bagbag/Tools/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2022-08-07 06:00:20.048999 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2022-08-07 06:00:20.049052 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2022-08-07 06:00:20.049109 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2022-08-07 06:00:20.049180 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2022-08-07 06:00:20.049247 bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2022-08-07 06:00:20.049305 bagbag-0.58.9/src/bagbag/Tools/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2022-08-07 06:00:20.049367 bagbag-0.58.9/src/bagbag/Tools/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2022-08-07 06:00:20.049468 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2022-08-07 06:00:20.049522 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2022-08-07 06:00:20.049577 bagbag-0.58.9/src/bagbag/Tools/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2022-08-07 06:00:20.049675 bagbag-0.58.9/src/bagbag/Tools/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2022-08-07 06:00:20.049735 bagbag-0.58.9/src/bagbag/Tools/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2022-08-07 06:00:20.049798 bagbag-0.58.9/src/bagbag/Tools/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2022-08-07 06:00:20.049852 bagbag-0.58.9/src/bagbag/Tools/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2022-08-07 06:00:20.049949 bagbag-0.58.9/src/bagbag/Tools/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2022-08-07 06:00:20.050007 bagbag-0.58.9/src/bagbag/Tools/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2022-08-07 06:00:20.050061 bagbag-0.58.9/src/bagbag/Tools/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2022-08-07 06:00:20.050118 bagbag-0.58.9/src/bagbag/Tools/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2022-08-07 06:00:20.050175 bagbag-0.58.9/src/bagbag/Tools/orator/utils/url.py
+-rw-r--r--   0        0        0     3335 2023-04-06 11:06:08.005936 bagbag-0.58.9/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    19046 1970-01-01 00:00:00.000000 bagbag-0.58.9/PKG-INFO
```

### Comparing `bagbag-0.58.8/LICENSE` & `bagbag-0.58.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/README.md` & `bagbag-0.58.9/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/pyproject.toml` & `bagbag-0.58.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.58.8"
+version = "0.58.9"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
```

### Comparing `bagbag-0.58.8/src/bagbag/Cmd.py` & `bagbag-0.58.9/src/bagbag/Cmd.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Cryptoo.py` & `bagbag-0.58.9/src/bagbag/Cryptoo.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/File.py` & `bagbag-0.58.9/src/bagbag/File.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/CutSentence.py` & `bagbag-0.58.9/src/bagbag/Funcs/CutSentence.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/CutSentenceStopWords.py` & `bagbag-0.58.9/src/bagbag/Funcs/CutSentenceStopWords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/FakeIdentity.py` & `bagbag-0.58.9/src/bagbag/Funcs/FakeIdentity.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/FileType.py` & `bagbag-0.58.9/src/bagbag/Funcs/FileType.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/Format.py` & `bagbag-0.58.9/src/bagbag/Funcs/Format.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/GetPublicIP.py` & `bagbag-0.58.9/src/bagbag/Funcs/GetPublicIP.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/Ping.py` & `bagbag-0.58.9/src/bagbag/Funcs/Ping.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/ResizeImage.py` & `bagbag-0.58.9/src/bagbag/Funcs/ResizeImage.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Funcs/Wget.py` & `bagbag-0.58.9/src/bagbag/Funcs/Wget.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Hash.py` & `bagbag-0.58.9/src/bagbag/Hash.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Http.py` & `bagbag-0.58.9/src/bagbag/Http.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Json.py` & `bagbag-0.58.9/src/bagbag/Json.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Lg.py` & `bagbag-0.58.9/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Math.py` & `bagbag-0.58.9/src/bagbag/Math.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Os/Path/__init__.py` & `bagbag-0.58.9/src/bagbag/Os/Path/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Os/__init__.py` & `bagbag-0.58.9/src/bagbag/Os/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Process.py` & `bagbag-0.58.9/src/bagbag/Process.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Python.py` & `bagbag-0.58.9/src/bagbag/Python.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Random.py` & `bagbag-0.58.9/src/bagbag/Random.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Socket/TCP.py` & `bagbag-0.58.9/src/bagbag/Socket/TCP.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/String.py` & `bagbag-0.58.9/src/bagbag/String.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Time.py` & `bagbag-0.58.9/src/bagbag/Time.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Argparser.py` & `bagbag-0.58.9/src/bagbag/Tools/Argparser.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py` & `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/CoinsPrice.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py` & `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Binance/OfficalAccountVertify.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/BlockChain/Tron/tron.py` & `bagbag-0.58.9/src/bagbag/Tools/BlockChain/Tron/tron.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/CSV.py` & `bagbag-0.58.9/src/bagbag/Tools/CSV.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Chan.py` & `bagbag-0.58.9/src/bagbag/Tools/Chan.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.58.9/src/bagbag/Tools/ComputerVision.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             confidence = self.confidences[i]
             cv2.rectangle(frame.frame, (round(x), round(y)), (round(x+w), round(y+h)), color, 1)
             # print('%s: %.2f%%' % (label, confidence*100))
             # print(x+25, y+30)
             cv2.putText(frame.frame, '%s: %.2f%%' % (label, confidence*100),
                         (round(x)+5, round(y)+15),
                         cv2.FONT_HERSHEY_DUPLEX,
-                        0.5, color, 1) 
+                        0.5, color, 0.5) 
     
         return frame 
 
     def drawByAPIServer(self, frame:cvStreamFrame, filterAbove:int=0, filterName:list=[]) -> cvStreamFrame:
         frame = copy.deepcopy(frame)
 
         global colorsapiserver
@@ -666,69 +666,84 @@
             colorsyolo = np.random.uniform(0, 255, size=(len(classesyolo), 3))
 
             netyolo = cv2.dnn.readNet(weights, config)
     
     def SetAPIServerForObjectDetect(self, server:str, model:str="yolo"):
         self.objectDetectModel = f"APIServer|{server}|{model}"
         
-    def Close(self):
+    def Close(self, destroyAllWindows:bool=True):
         self.closed = True
         try:
             if self.stype == "c":
-                Lg.Trace("关闭socket")
+                Lg.Trace("关闭stream")
                 self.stream.release()
             elif self.stype == "n":
-                Lg.Trace("关闭stream")
+                Lg.Trace("关闭socket")
                 self.stream.Close()
         except Exception as e:
             Lg.Trace("关闭有异常:", e)
             pass 
-        try:
-            Lg.Trace("销毁所有窗口")
-            cv2.destroyAllWindows()
-        except Exception as e:
-            Lg.Trace("销毁有异常:", e)
-            pass
+    
+        if destroyAllWindows:
+            try:
+                Lg.Trace("销毁所有窗口")
+                cv2.destroyAllWindows()
+            except Exception as e:
+                Lg.Trace("销毁有异常:", e)
+                pass
+        Lg.Trace("关闭完成")
 
     def openStream(self):
         if type(self.source) == str and self.source.startswith("socket://"):
+            Lg.Trace("打开网络接口")
             self.stype = "n"
             _ = String(self.source).RegexFind("socket://(.+?):(.+)")
             # print(_[0])
             self.stream = Socket.TCP.Connect(_[0][1], int(_[0][2])).PacketConnection()
         else:
             self.stream = cv2.VideoCapture(self.source)
             self.stype = "c"
+        Lg.Trace("开启stream完成, 模式:", self.stype)
 
     def run(self):
         self.openStream()
 
         frameCountSec = 0
         lastSec = Time.Now()
         while True:
             if self.stype == "c":
                 (grabbed, frame) = self.stream.read()
 
                 if not grabbed:
                     Lg.Trace("没有抓到帧")
-                    self.Close()
+                    try:
+                        Lg.Trace("关闭stream")
+                        self.stream.release()
+                    except Exception as e:
+                        Lg.Trace("关闭有异常:", e)
+                        pass 
                     time.sleep(1)
                     Lg.Trace("重新尝试")
                     self.openStream()
                     time.sleep(1)
                     continue 
                 
             elif self.stype == "n":
                 # print(2)
                 try:
                     self.stream.Send("d")
                     imgdata = self.stream.Recv()
                 except Exception as e:
                     Lg.Trace("从socket抓帧报错了:", e)
-                    self.Close()
+                    try:
+                        Lg.Trace("关闭socket")
+                        self.stream.Close()
+                    except Exception as e:
+                        Lg.Trace("关闭有异常:", e)
+                        pass 
                     time.sleep(1)
                     Lg.Trace("重新尝试")
                     self.openStream()
                     time.sleep(1)
                     continue 
                 
                 nparr = np.fromstring(imgdata, np.uint8)
```

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Crontab.py` & `bagbag-0.58.9/src/bagbag/Tools/Crontab.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Database.py` & `bagbag-0.58.9/src/bagbag/Tools/Database.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/DistributedLock.py` & `bagbag-0.58.9/src/bagbag/Tools/DistributedLock.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Elasticsearch.py` & `bagbag-0.58.9/src/bagbag/Tools/Elasticsearch.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Github.py` & `bagbag-0.58.9/src/bagbag/Tools/Github.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/JavaScript.py` & `bagbag-0.58.9/src/bagbag/Tools/JavaScript.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Kafka.py` & `bagbag-0.58.9/src/bagbag/Tools/Kafka.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Lock.py` & `bagbag-0.58.9/src/bagbag/Tools/Lock.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/MatrixBot.py` & `bagbag-0.58.9/src/bagbag/Tools/MatrixBot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/OCR.py` & `bagbag-0.58.9/src/bagbag/Tools/OCR.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/ProgressBar.py` & `bagbag-0.58.9/src/bagbag/Tools/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.58.9/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.58.9/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.58.9/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Queue.py` & `bagbag-0.58.9/src/bagbag/Tools/Queue.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/RSS/Feed.py` & `bagbag-0.58.9/src/bagbag/Tools/RSS/Feed.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/RSS/Opml.py` & `bagbag-0.58.9/src/bagbag/Tools/RSS/Opml.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Ratelimit.py` & `bagbag-0.58.9/src/bagbag/Tools/Ratelimit.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Redis.py` & `bagbag-0.58.9/src/bagbag/Tools/Redis.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/SSH.py` & `bagbag-0.58.9/src/bagbag/Tools/SSH.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Selenium.py` & `bagbag-0.58.9/src/bagbag/Tools/Selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,17 @@
                     time.sleep(1)
                 else:
                     raise e 
 
         # import ipdb
         # ipdb.set_trace()
     
+    def Exists(self, xpath:str) -> bool:
+        return self.Find(xpath, timeout=0) != None
+    
     def StatusCode(self) -> int:
         self.driver.stat
     
     def ResizeWindow(self, width:int, height:int):
         """
         :param width: The width of the window in pixels
         :type width: int
```

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Telegram.py` & `bagbag-0.58.9/src/bagbag/Tools/Telegram.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.58.9/src/bagbag/Tools/TelegramAsync.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/TelegramBot.py` & `bagbag-0.58.9/src/bagbag/Tools/TelegramBot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/TelegramBotOfficial.py` & `bagbag-0.58.9/src/bagbag/Tools/TelegramBotOfficial.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Translater.py` & `bagbag-0.58.9/src/bagbag/Tools/Translater.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Twitter/Elevated.py` & `bagbag-0.58.9/src/bagbag/Tools/Twitter/Elevated.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Twitter/Essential.py` & `bagbag-0.58.9/src/bagbag/Tools/Twitter/Essential.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/URL.py` & `bagbag-0.58.9/src/bagbag/Tools/URL.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/WaitGroup.py` & `bagbag-0.58.9/src/bagbag/Tools/WaitGroup.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/WebCrawler.py` & `bagbag-0.58.9/src/bagbag/Tools/WebCrawler.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/WebServer.py` & `bagbag-0.58.9/src/bagbag/Tools/WebServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/XPath.py` & `bagbag-0.58.9/src/bagbag/Tools/XPath.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/Xlsx.py` & `bagbag-0.58.9/src/bagbag/Tools/Xlsx.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/__init__.py` & `bagbag-0.58.9/src/bagbag/Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/application.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/install_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/make_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/migrate_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/refresh_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/reset_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/rollback_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/migrations/status_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/models/make_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/make_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/commands/seeds/seed_command.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connections/connection.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connections/connection_interface.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connections/mysql_connection.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connections/postgres_connection.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connections/sqlite_connection.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connectors/connection_factory.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connectors/connector.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connectors/mysql_connector.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connectors/postgres_connector.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/connectors/sqlite_connector.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/database_manager.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/abstract_asset.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/column.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/column_diff.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/comparator.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/exceptions/__init__.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/index.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/platform.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/schema_manager.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/table.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/dbal/table_diff.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/events/__init__.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/connectors.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/exceptions/orm.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/migrations/database_migration_repository.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/migrations/migration_creator.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/migrations/migrator.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/migrations/stubs.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/builder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/collection.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/factory.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/factory_builder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/model.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/belongs_to.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_many_through.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_one.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_one.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_pivot.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_to.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/morph_to_many.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/pivot.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/relation.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/result.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/relations/wrapper.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/orm/utils.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/pagination/base.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/pagination/length_aware_paginator.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/pagination/paginator.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/builder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/join_clause.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/mysql_processor.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/postgres_processor.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/query/processors/processor.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/blueprint.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/builder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/mysql_builder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/schema/schema.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/seeds/seeder.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/support/fluent.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/support/grammar.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/utils/__init__.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/utils/command_formatter.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/utils/helpers.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/utils/qmarker.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/Tools/orator/utils/url.py` & `bagbag-0.58.9/src/bagbag/Tools/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/src/bagbag/__init__.py` & `bagbag-0.58.9/src/bagbag/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.58.8/PKG-INFO` & `bagbag-0.58.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.58.8
+Version: 0.58.9
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

